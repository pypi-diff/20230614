# Comparing `tmp/ml-starter-0.0.57.tar.gz` & `tmp/ml-starter-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.57.tar", last modified: Wed Jun 14 02:41:41 2023, max compression
+gzip compressed data, was "ml-starter-0.0.58.tar", last modified: Wed Jun 14 05:29:27 2023, max compression
```

## Comparing `ml-starter-0.0.57.tar` & `ml-starter-0.0.58.tar`

### file list

```diff
@@ -1,166 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 02:41:29.000000 ml-starter-0.0.57/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 02:41:29.000000 ml-starter-0.0.57/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 02:41:41.115714 ml-starter-0.0.57/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-14 02:41:29.000000 ml-starter-0.0.57/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.099714 ml-starter-0.0.57/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.099714 ml-starter-0.0.57/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.111714 ml-starter-0.0.57/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.111714 ml-starter-0.0.57/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-14 02:41:29.000000 ml-starter-0.0.57/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 02:41:29.000000 ml-starter-0.0.57/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 02:41:29.000000 ml-starter-0.0.57/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-14 02:41:29.000000 ml-starter-0.0.57/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 02:41:41.115714 ml-starter-0.0.57/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 02:41:29.000000 ml-starter-0.0.57/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 05:29:13.000000 ml-starter-0.0.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 05:29:13.000000 ml-starter-0.0.58/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 05:29:27.063916 ml-starter-0.0.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-14 05:29:13.000000 ml-starter-0.0.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.027913 ml-starter-0.0.58/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.031913 ml-starter-0.0.58/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.031913 ml-starter-0.0.58/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.035914 ml-starter-0.0.58/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.035914 ml-starter-0.0.58/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.035914 ml-starter-0.0.58/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.039914 ml-starter-0.0.58/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.043914 ml-starter-0.0.58/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.047915 ml-starter-0.0.58/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.047915 ml-starter-0.0.58/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.051915 ml-starter-0.0.58/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.051915 ml-starter-0.0.58/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.051915 ml-starter-0.0.58/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.055915 ml-starter-0.0.58/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.055915 ml-starter-0.0.58/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.055915 ml-starter-0.0.58/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.059916 ml-starter-0.0.58/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 05:29:26.000000 ml-starter-0.0.58/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-14 05:29:27.000000 ml-starter-0.0.58/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:29:26.000000 ml-starter-0.0.58/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 05:29:26.000000 ml-starter-0.0.58/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 05:29:26.000000 ml-starter-0.0.58/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-14 05:29:13.000000 ml-starter-0.0.58/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 05:29:13.000000 ml-starter-0.0.58/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 05:29:13.000000 ml-starter-0.0.58/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-14 05:29:13.000000 ml-starter-0.0.58/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 05:29:27.067916 ml-starter-0.0.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 05:29:13.000000 ml-starter-0.0.58/setup.py
```

### Comparing `ml-starter-0.0.57/LICENSE` & `ml-starter-0.0.58/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/PKG-INFO` & `ml-starter-0.0.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.57
+Version: 0.0.58
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.57/README.md` & `ml-starter-0.0.58/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/api.py` & `ml-starter-0.0.58/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/core/common_types.py` & `ml-starter-0.0.58/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/core/config.py` & `ml-starter-0.0.58/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/core/env.py` & `ml-starter-0.0.58/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/core/registry.py` & `ml-starter-0.0.58/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/core/state.py` & `ml-starter-0.0.58/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/launchers/base.py` & `ml-starter-0.0.58/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/launchers/mp.py` & `ml-starter-0.0.58/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/launchers/slurm.py` & `ml-starter-0.0.58/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/launchers/torchrun.py` & `ml-starter-0.0.58/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/loggers/base.py` & `ml-starter-0.0.58/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/loggers/meter.py` & `ml-starter-0.0.58/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/loggers/multi.py` & `ml-starter-0.0.58/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/loggers/stdout.py` & `ml-starter-0.0.58/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/loggers/tensorboard.py` & `ml-starter-0.0.58/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/lr_schedulers/base.py` & `ml-starter-0.0.58/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/lr_schedulers/constant.py` & `ml-starter-0.0.58/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.58/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.58/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/lr_schedulers/linear.py` & `ml-starter-0.0.58/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.58/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.58/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/models/activations.py` & `ml-starter-0.0.58/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/models/base.py` & `ml-starter-0.0.58/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/models/embeddings.py` & `ml-starter-0.0.58/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/models/init.py` & `ml-starter-0.0.58/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/models/kmeans.py` & `ml-starter-0.0.58/ml/models/kmeans.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,78 @@
 """Defines a distributed K-Means module.
 
 This is used to apply K-Means clusters to a tensor. This module can be used
 with cluster centers found via Scikit-Learn, Faiss, or other libraries.
 """
 
+import logging
+from typing import Callable
+
 import numpy as np
 import torch
 from torch import Tensor, nn
 
+logger = logging.getLogger(__name__)
+
+
+def _vanilla_kmeans(x: Tensor, centers: Tensor, centers_norm: Tensor) -> Tensor:
+    # Equivalent code:
+    # dist = torch.norm(x[..., None, :] - centers, p=2, dim=-1)
+    # return dist.argmin(dim=-1)
+    x_norm = (x**2).sum(-1)
+    dist = x_norm[..., None] - (2 * (x @ centers.transpose(0, 1))) + centers_norm
+    # Absolute value is required here because sometimes the distance
+    # can be negative due to numerical instability.
+    return dist.abs().argmin(dim=-1)
+
+
+def kmeans_fn(use_triton: bool) -> Callable[[Tensor, Tensor, Tensor], Tensor]:
+    if torch.cuda.is_available() and use_triton:
+        try:
+            from ml.utils.triton.kmeans import kmeans as triton_kmeans_fn
+
+            return triton_kmeans_fn
+
+        except ImportError:
+            logger.warning("Triton is not installed. Using vanilla Lion update function.")
+
+    return _vanilla_kmeans
+
 
 class KMeans(nn.Module):
     __constants__ = ["n_clusters", "n_features"]
 
     centers: Tensor
+    centers_norm: Tensor
 
-    def __init__(self, centers: Tensor | np.ndarray) -> None:
+    def __init__(self, centers: Tensor | np.ndarray, *, use_triton_if_available: bool = True) -> None:
         super().__init__()
 
         n_clusters, n_features = centers.shape
         self.n_clusters = n_clusters
         self.n_features = n_features
         self.register_buffer("centers", torch.empty(n_clusters, n_features))
+        self.register_buffer("centers_norm", torch.empty(n_clusters))
         self.load_centers(centers)
+        self.kmeans_fn = kmeans_fn(use_triton_if_available)
 
     def load_centers(self, centers: Tensor | np.ndarray) -> None:
         if isinstance(centers, np.ndarray):
             centers = torch.from_numpy(centers)
         assert centers.shape == self.centers.shape, f"Expected shape {self.centers.shape}, got {centers.shape}"
         self.centers.copy_(centers.to(self.centers))
+        self.centers_norm.copy_((self.centers**2).sum(-1))
 
     def forward(self, x: Tensor) -> Tensor:
         """Applies K-Means to get cluster IDs.
 
         We compute ``(x - centers) ^ 2`` by rewriting as
         ``x ^ 2 - 2 * x * centers + centers ^ 2`` which avoids expanding the
         tensor when doing the norm.
 
         Args:
             x: The input tensor, with shape ``(*, n_features)``
 
         Returns:
             The cluster IDs, with shape ``(*)``
         """
-        # Equivalent code:
-        # dist = torch.norm(x[..., None, :] - self.centers, p=2, dim=-1)
-        # return dist.argmin(dim=-1)
-        x_norm, centers_norm = (x**2).sum(-1), (self.centers**2).sum(-1)
-        dist = x_norm[..., None] - (2 * (x @ self.centers.transpose(0, 1))) + centers_norm[..., None]
-        # Absolute value is required here because sometimes the distance
-        # can be negative due to numerical instability.
-        return dist.abs().argmin(dim=-1)
+        return self.kmeans_fn(x, self.centers, self.centers_norm)
```

### Comparing `ml-starter-0.0.57/ml/models/lora.py` & `ml-starter-0.0.58/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/models/norms.py` & `ml-starter-0.0.58/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/models/parallel.py` & `ml-starter-0.0.58/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/optimizers/adam.py` & `ml-starter-0.0.58/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/optimizers/adamw.py` & `ml-starter-0.0.58/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/optimizers/adan.py` & `ml-starter-0.0.58/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/optimizers/base.py` & `ml-starter-0.0.58/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/optimizers/common.py` & `ml-starter-0.0.58/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/optimizers/lion.py` & `ml-starter-0.0.58/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/optimizers/sgd.py` & `ml-starter-0.0.58/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/optimizers/shampoo.py` & `ml-starter-0.0.58/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/scripts/cli.py` & `ml-starter-0.0.58/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/scripts/stage.py` & `ml-starter-0.0.58/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/scripts/train.py` & `ml-starter-0.0.58/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/base.py` & `ml-starter-0.0.58/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.58/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.58/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/collate.py` & `ml-starter-0.0.58/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.58/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.58/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.58/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.58/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.58/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/utils.py` & `ml-starter-0.0.58/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.58/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/environments/base.py` & `ml-starter-0.0.58/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/environments/utils.py` & `ml-starter-0.0.58/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/environments/worker.py` & `ml-starter-0.0.58/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/losses/reduce.py` & `ml-starter-0.0.58/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/rl/base.py` & `ml-starter-0.0.58/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/rl/replay.py` & `ml-starter-0.0.58/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/tasks/sl/base.py` & `ml-starter-0.0.58/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/base.py` & `ml-starter-0.0.58/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/learning.py` & `ml-starter-0.0.58/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/compile.py` & `ml-starter-0.0.58/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.58/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.58/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.58/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.58/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.58/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.58/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.58/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.58/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.58/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/rl.py` & `ml-starter-0.0.58/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/trainers/sl.py` & `ml-starter-0.0.58/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/argparse.py` & `ml-starter-0.0.58/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/atomic.py` & `ml-starter-0.0.58/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/audio.py` & `ml-starter-0.0.58/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/augmentation.py` & `ml-starter-0.0.58/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/caching.py` & `ml-starter-0.0.58/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/checkpoint.py` & `ml-starter-0.0.58/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/cli.py` & `ml-starter-0.0.58/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/colors.py` & `ml-starter-0.0.58/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/config.py` & `ml-starter-0.0.58/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/data.py` & `ml-starter-0.0.58/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/datetime.py` & `ml-starter-0.0.58/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/device/auto.py` & `ml-starter-0.0.58/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/device/base.py` & `ml-starter-0.0.58/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/device/cpu.py` & `ml-starter-0.0.58/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/device/gpu.py` & `ml-starter-0.0.58/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/device/metal.py` & `ml-starter-0.0.58/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/distributed.py` & `ml-starter-0.0.58/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/image.py` & `ml-starter-0.0.58/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/large_models.py` & `ml-starter-0.0.58/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/logging.py` & `ml-starter-0.0.58/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/meter.py` & `ml-starter-0.0.58/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/parallel.py` & `ml-starter-0.0.58/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/staging.py` & `ml-starter-0.0.58/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/timer.py` & `ml-starter-0.0.58/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/tokens.py` & `ml-starter-0.0.58/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/torch_distributed.py` & `ml-starter-0.0.58/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml/utils/triton/lion.py` & `ml-starter-0.0.58/ml/utils/triton/lion.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     lr,
     wd,
     beta1,
     beta2,
     n_elements,
     BLOCK_SIZE: tl.constexpr,
 ):
-    b_idx = tl.program_id(axis=0)
+    b_idx = tl.program_id(0)
 
     block_start = b_idx * BLOCK_SIZE
     offsets = block_start + tl.arange(0, BLOCK_SIZE)
 
     mask = offsets < n_elements
 
     offset_p_ptr = p_ptr + offsets
```

### Comparing `ml-starter-0.0.57/ml/utils/video.py` & `ml-starter-0.0.58/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.58/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.57
+Version: 0.0.58
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.57/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.58/ml_starter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -131,13 +131,14 @@
 ml/utils/device/__init__.py
 ml/utils/device/auto.py
 ml/utils/device/base.py
 ml/utils/device/cpu.py
 ml/utils/device/gpu.py
 ml/utils/device/metal.py
 ml/utils/triton/__init__.py
+ml/utils/triton/kmeans.py
 ml/utils/triton/lion.py
 ml_starter.egg-info/PKG-INFO
 ml_starter.egg-info/SOURCES.txt
 ml_starter.egg-info/dependency_links.txt
 ml_starter.egg-info/requires.txt
 ml_starter.egg-info/top_level.txt
```

### Comparing `ml-starter-0.0.57/pyproject.toml` & `ml-starter-0.0.58/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.57/setup.py` & `ml-starter-0.0.58/setup.py`

 * *Files identical despite different names*

