# Comparing `tmp/ml-starter-0.0.58.tar.gz` & `tmp/ml-starter-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.58.tar", last modified: Wed Jun 14 05:29:27 2023, max compression
+gzip compressed data, was "ml-starter-0.0.59.tar", last modified: Wed Jun 14 06:53:13 2023, max compression
```

## Comparing `ml-starter-0.0.58.tar` & `ml-starter-0.0.59.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 05:29:13.000000 ml-starter-0.0.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 05:29:13.000000 ml-starter-0.0.58/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 05:29:27.063916 ml-starter-0.0.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-14 05:29:13.000000 ml-starter-0.0.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.027913 ml-starter-0.0.58/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.031913 ml-starter-0.0.58/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.031913 ml-starter-0.0.58/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.035914 ml-starter-0.0.58/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.035914 ml-starter-0.0.58/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.035914 ml-starter-0.0.58/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.039914 ml-starter-0.0.58/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.043914 ml-starter-0.0.58/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.047915 ml-starter-0.0.58/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.047915 ml-starter-0.0.58/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.051915 ml-starter-0.0.58/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.051915 ml-starter-0.0.58/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.051915 ml-starter-0.0.58/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.055915 ml-starter-0.0.58/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.055915 ml-starter-0.0.58/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.055915 ml-starter-0.0.58/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.059916 ml-starter-0.0.58/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-14 05:29:13.000000 ml-starter-0.0.58/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 05:29:27.063916 ml-starter-0.0.58/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 05:29:26.000000 ml-starter-0.0.58/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-14 05:29:27.000000 ml-starter-0.0.58/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 05:29:26.000000 ml-starter-0.0.58/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 05:29:26.000000 ml-starter-0.0.58/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 05:29:26.000000 ml-starter-0.0.58/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-14 05:29:13.000000 ml-starter-0.0.58/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 05:29:13.000000 ml-starter-0.0.58/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 05:29:13.000000 ml-starter-0.0.58/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-14 05:29:13.000000 ml-starter-0.0.58/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 05:29:27.067916 ml-starter-0.0.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 05:29:13.000000 ml-starter-0.0.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.606784 ml-starter-0.0.59/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 06:53:00.000000 ml-starter-0.0.59/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 06:53:00.000000 ml-starter-0.0.59/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 06:53:13.606784 ml-starter-0.0.59/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-14 06:53:00.000000 ml-starter-0.0.59/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.578784 ml-starter-0.0.59/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.578784 ml-starter-0.0.59/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.578784 ml-starter-0.0.59/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.582784 ml-starter-0.0.59/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.582784 ml-starter-0.0.59/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.582784 ml-starter-0.0.59/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.586784 ml-starter-0.0.59/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.586784 ml-starter-0.0.59/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.590784 ml-starter-0.0.59/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.590784 ml-starter-0.0.59/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.590784 ml-starter-0.0.59/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.590784 ml-starter-0.0.59/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.594784 ml-starter-0.0.59/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.594784 ml-starter-0.0.59/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.594784 ml-starter-0.0.59/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.594784 ml-starter-0.0.59/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.598784 ml-starter-0.0.59/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.602784 ml-starter-0.0.59/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.602784 ml-starter-0.0.59/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.606784 ml-starter-0.0.59/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-14 06:53:00.000000 ml-starter-0.0.59/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:53:13.606784 ml-starter-0.0.59/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 06:53:13.000000 ml-starter-0.0.59/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-14 06:53:00.000000 ml-starter-0.0.59/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 06:53:00.000000 ml-starter-0.0.59/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 06:53:00.000000 ml-starter-0.0.59/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-14 06:53:00.000000 ml-starter-0.0.59/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 06:53:13.606784 ml-starter-0.0.59/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 06:53:00.000000 ml-starter-0.0.59/setup.py
```

### Comparing `ml-starter-0.0.58/LICENSE` & `ml-starter-0.0.59/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/PKG-INFO` & `ml-starter-0.0.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.58
+Version: 0.0.59
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.58/README.md` & `ml-starter-0.0.59/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/api.py` & `ml-starter-0.0.59/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/core/common_types.py` & `ml-starter-0.0.59/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/core/config.py` & `ml-starter-0.0.59/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/core/env.py` & `ml-starter-0.0.59/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/core/registry.py` & `ml-starter-0.0.59/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/core/state.py` & `ml-starter-0.0.59/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/launchers/base.py` & `ml-starter-0.0.59/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/launchers/mp.py` & `ml-starter-0.0.59/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/launchers/slurm.py` & `ml-starter-0.0.59/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/launchers/torchrun.py` & `ml-starter-0.0.59/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/loggers/base.py` & `ml-starter-0.0.59/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/loggers/meter.py` & `ml-starter-0.0.59/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/loggers/multi.py` & `ml-starter-0.0.59/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/loggers/stdout.py` & `ml-starter-0.0.59/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/loggers/tensorboard.py` & `ml-starter-0.0.59/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/lr_schedulers/base.py` & `ml-starter-0.0.59/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/lr_schedulers/constant.py` & `ml-starter-0.0.59/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.59/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.59/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/lr_schedulers/linear.py` & `ml-starter-0.0.59/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.59/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.59/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/models/activations.py` & `ml-starter-0.0.59/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/models/base.py` & `ml-starter-0.0.59/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/models/embeddings.py` & `ml-starter-0.0.59/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/models/init.py` & `ml-starter-0.0.59/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/models/kmeans.py` & `ml-starter-0.0.59/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/models/lora.py` & `ml-starter-0.0.59/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/models/norms.py` & `ml-starter-0.0.59/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/models/parallel.py` & `ml-starter-0.0.59/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/optimizers/adam.py` & `ml-starter-0.0.59/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/optimizers/adamw.py` & `ml-starter-0.0.59/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/optimizers/adan.py` & `ml-starter-0.0.59/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/optimizers/base.py` & `ml-starter-0.0.59/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/optimizers/common.py` & `ml-starter-0.0.59/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/optimizers/lion.py` & `ml-starter-0.0.59/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/optimizers/sgd.py` & `ml-starter-0.0.59/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/optimizers/shampoo.py` & `ml-starter-0.0.59/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/scripts/cli.py` & `ml-starter-0.0.59/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/scripts/stage.py` & `ml-starter-0.0.59/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/scripts/train.py` & `ml-starter-0.0.59/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/base.py` & `ml-starter-0.0.59/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.59/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.59/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/collate.py` & `ml-starter-0.0.59/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.59/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.59/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.59/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.59/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.59/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/utils.py` & `ml-starter-0.0.59/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.59/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/environments/base.py` & `ml-starter-0.0.59/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/environments/utils.py` & `ml-starter-0.0.59/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/environments/worker.py` & `ml-starter-0.0.59/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/losses/reduce.py` & `ml-starter-0.0.59/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/rl/base.py` & `ml-starter-0.0.59/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/rl/replay.py` & `ml-starter-0.0.59/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/tasks/sl/base.py` & `ml-starter-0.0.59/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/base.py` & `ml-starter-0.0.59/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/learning.py` & `ml-starter-0.0.59/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/compile.py` & `ml-starter-0.0.59/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.59/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.59/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.59/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.59/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.59/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.59/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.59/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.59/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.59/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/rl.py` & `ml-starter-0.0.59/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/trainers/sl.py` & `ml-starter-0.0.59/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/argparse.py` & `ml-starter-0.0.59/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/atomic.py` & `ml-starter-0.0.59/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/audio.py` & `ml-starter-0.0.59/ml/utils/audio.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,91 +6,117 @@
 .. code-blocks:: python
 
     from ml.utils.audio import read_audio, write_audio
 
 This just uses FFMPEG so it should be rasonably quick.
 """
 
+import fractions
 import shutil
 import warnings
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Iterator, Literal
 
 import av
 import numpy as np
+import soundfile as sf
 import torch
 import torchaudio.functional as A
 from torch import Tensor
 
 from ml.utils.numpy import as_numpy_array
 
 
 @dataclass
 class AudioProps:
     sample_rate: int
     channels: int
-    duration: float
+    num_frames: int
 
     @classmethod
-    def from_file_av(cls, fpath: str | Path) -> "AudioProps":
-        container = av.open(str(fpath))
-        stream = container.streams.audio[0]
-
+    def from_file_sf(cls, fpath: str | Path) -> "AudioProps":
+        info = sf.info(str(fpath))
         return cls(
-            sample_rate=stream.rate,
-            channels=stream.channels,
-            duration=stream.duration,
+            sample_rate=info.samplerate,
+            channels=info.channels,
+            num_frames=info.frames,
         )
 
     @classmethod
+    def from_file_av(cls, fpath: str | Path) -> "AudioProps":
+        with av.open(str(fpath)) as container:
+            stream = container.streams.audio[0]
+
+            return cls(
+                sample_rate=stream.rate,
+                channels=stream.channels,
+                num_frames=stream.duration,
+            )
+
+    @classmethod
     def from_file_ffmpeg(cls, fpath: str | Path) -> "AudioProps":
         try:
             import ffmpeg
         except ImportError as e:
             raise ImportError("Please install matplotlib to use this function: `pip install ffmpeg-python`") from e
 
         probe = ffmpeg.probe(str(fpath))
 
         for stream in probe["streams"]:
             if stream["codec_type"] == "audio":
                 return cls(
                     sample_rate=int(stream["sample_rate"]),
                     channels=int(stream["channels"]),
-                    duration=float(stream["duration"]),
+                    num_frames=int(stream["duration_ts"]),
                 )
 
         raise ValueError(f"Could not find audio stream in {fpath}")
 
 
 def _cleanup_wav_chunk(wav: np.ndarray, channels: int | None = None) -> np.ndarray:
     if wav.ndim == 1:
         wav = wav.reshape(-1, 1 if channels is None else channels).T
     return wav
 
 
+def read_audio_sf(in_file: str | Path, *, blocksize: int = 16_000) -> Iterator[np.ndarray]:
+    """Function that reads an audio file to a stream of numpy arrays using SoundFile.
+
+    Args:
+        in_file: Path to the input file.
+        blocksize: Number of samples to read at a time.
+
+    Yields:
+        Audio chunks as numpy arrays, with shape (n_channels, n_samples).
+    """
+    with sf.SoundFile(str(in_file)) as f:
+        for frame in f.blocks(blocksize=blocksize):
+            yield _cleanup_wav_chunk(frame.T)
+
+
 def read_audio_av(in_file: str | Path) -> Iterator[np.ndarray]:
     """Function that reads an audio file to a stream of numpy arrays using PyAV.
 
     Args:
         in_file: Path to the input file.
 
     Yields:
         Audio chunks as numpy arrays, with shape (n_channels, n_samples).
     """
     props = AudioProps.from_file_av(in_file)
 
-    container = av.open(str(in_file))
-    stream = container.streams.audio[0]
+    with av.open(str(in_file)) as container:
+        stream = container.streams.audio[0]
 
-    for frame in container.decode(stream):
-        frame_np = frame.to_ndarray().reshape(-1, props.channels).T
-        if frame_np.dtype == np.int16:
-            frame_np = frame_np.astype(np.float32) / 2**15
-        yield frame_np
+        for frame in container.decode(stream):
+            frame_np = frame.to_ndarray().reshape(-1, props.channels).T
+            if frame_np.dtype == np.int16:
+                frame_np = frame_np.astype(np.float32) / 2**15
+            yield frame_np
 
 
 def read_audio_ffmpeg(in_file: str | Path, *, chunk_size: int = 16_000) -> Iterator[np.ndarray]:
     """Function that reads an audio file to a stream of numpy arrays using FFMPEG.
 
     Args:
         in_file: Path to the input file.
@@ -116,46 +142,72 @@
             break
         yield np.frombuffer(chunk, dtype=np.float32).reshape(props.channels, -1)
 
     stream.stdout.close()
     stream.wait()
 
 
+def write_audio_sf(itr: Iterator[np.ndarray | Tensor], out_file: str | Path, sampling_rate: int) -> None:
+    """Function that writes a stream of audio to a file using SoundFile.
+
+    Args:
+        itr: Iterator of audio chunks, with shape (n_channels, n_samples).
+        out_file: Path to the output file.
+        sampling_rate: Sampling rate of the audio.
+    """
+    first_chunk = _cleanup_wav_chunk(as_numpy_array(next(itr)))
+    assert (channels := first_chunk.shape[0]) in (1, 2), f"Expected 1 or 2 channels, got {channels}"
+    with sf.SoundFile(str(out_file), mode="w", samplerate=sampling_rate, channels=channels) as f:
+        f.write(first_chunk.T)
+        for chunk in itr:
+            f.write(chunk.T)
+
+
 def write_audio_av(itr: Iterator[np.ndarray | Tensor], out_file: str | Path, sampling_rate: int) -> None:
     """Function that writes a stream of audio to a file using PyAV.
 
     Args:
         itr: Iterator of audio chunks, with shape (n_channels, n_samples).
         out_file: Path to the output file.
         sampling_rate: Sampling rate of the audio.
     """
-    container = av.open(str(out_file), mode="w")
-    stream = container.add_stream("pcm_f32le", rate=sampling_rate)
+    with av.open(str(out_file), mode="w") as container:
+        stream = container.add_stream("pcm_f32le", rate=sampling_rate)
 
-    is_first_frame = True
-    is_mono = True
-    for frame in itr:
-        frame_np_float = _cleanup_wav_chunk(as_numpy_array(frame))
-        assert frame_np_float.ndim == 2, f"Expected 2D array, got {frame_np_float.shape}D"
+        is_first_frame = True
+        is_mono = True
+        for frame in itr:
+            frame_np_float = _cleanup_wav_chunk(as_numpy_array(frame))
+            assert frame_np_float.ndim == 2, f"Expected 2D array, got {frame_np_float.shape}D"
+
+            if is_first_frame:
+                assert (channels := frame_np_float.shape[0]) in (1, 2), f"Expected 1 or 2 channels, got {channels}"
+                is_mono = channels == 1
+                stream.channels = channels
+                stream.layout = "mono" if is_mono else "stereo"
+                stream.time_base = fractions.Fraction(1, sampling_rate)
+                is_first_frame = False
+
+            out_fmt = "s16" if is_mono else "s16p"
+
+            frame_np = (frame_np_float * 2**15).astype(np.int16)
+            # frame_np = frame_np_float.astype(np.float32)
+
+            frame_np = frame_np.reshape(-1, stream.channels).T.copy(order="C")
+
+            frame_av = av.AudioFrame.from_ndarray(frame_np, layout=stream.layout.name, format=out_fmt)
+            frame_av.rate = sampling_rate
+            frame_av.time_base = stream.time_base
+            frame_av.pts = None
 
-        if is_first_frame:
-            assert (channels := frame_np_float.shape[0]) in (1, 2), f"Expected 1 or 2 channels, got {channels}"
-            is_mono = channels == 1
-            stream.channels = channels
-            stream.layout = "mono" if is_mono else "stereo"
-            is_first_frame = False
-
-        frame_np = (frame_np_float * 2**15).astype(np.int16)
-        output_fmt = "s16" if is_mono else "s16p"
-        frame_av = av.AudioFrame.from_ndarray(frame_np, format=output_fmt)
-        frame_av.rate = sampling_rate
-        frame_av.time_base = stream.time_base
-        container.mux(stream.encode(frame_av))
+            for packet in stream.encode(frame_av):
+                container.mux(packet)
 
-    container.close()
+        for packet in stream.encode():
+            container.mux(packet)
 
 
 def write_audio_ffmpeg(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     sampling_rate: int,
 ) -> None:
@@ -191,22 +243,25 @@
     stream.wait()
 
 
 Reader = Literal["ffmpeg", "av", "sf"]
 Writer = Literal["ffmpeg", "av", "sf"]
 
 
-def get_audio_props(in_file: str | Path, *, reader: Reader = "av") -> AudioProps:
+def get_audio_props(in_file: str | Path, *, reader: Reader = "sf") -> AudioProps:
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in this system.")
             reader = "av"
         else:
             return AudioProps.from_file_ffmpeg(in_file)
 
+    if reader == "sf":
+        return AudioProps.from_file_sf(in_file)
+
     if reader == "av":
         return AudioProps.from_file_av(in_file)
 
     raise ValueError(f"Unknown reader {reader}")
 
 
 def _resample_audio(
@@ -240,68 +295,76 @@
 
 
 def read_audio(
     in_file: str | Path,
     *,
     chunk_length: int | None = None,
     sampling_rate: int | None = None,
-    reader: Reader = "av",
+    reader: Reader = "sf",
 ) -> Iterator[np.ndarray]:
     """Function that reads a stream of audio from a file.
 
     The output audio is in ``float32`` format.
 
     Args:
         in_file: Path to the input file.
         chunk_length: Size of the chunks to read. If ``None``, will iterate
             whatever chunk size the underlying reader uses. Otherwise, samples
             will be rechunked to the desired size.
         sampling_rate: Sampling rate to resample the audio to. If ``None``,
             will use the sampling rate of the input audio.
-        reader: Reader to use. Can be either ``ffmpeg`` or ``av``.
+        reader: Reader to use. Can be either ``sf``, ``ffmpeg`` or ``av``.
 
     Returns:
         Iterator over numpy arrays, with shape ``(n_channels, n_samples)``.
     """
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in this system.")
             reader = "av"
         else:
             sr = None if sampling_rate is None else (AudioProps.from_file_ffmpeg(in_file).sample_rate, sampling_rate)
             return _resample_audio(read_audio_ffmpeg(in_file), chunk_length=chunk_length, sampling_rate=sr)
 
+    if reader == "sf":
+        sr = None if sampling_rate is None else (AudioProps.from_file_sf(in_file).sample_rate, sampling_rate)
+        return _resample_audio(read_audio_sf(in_file), chunk_length=chunk_length, sampling_rate=sr)
+
     if reader == "av":
         sr = None if sampling_rate is None else (AudioProps.from_file_av(in_file).sample_rate, sampling_rate)
         return _resample_audio(read_audio_av(in_file), chunk_length=chunk_length, sampling_rate=sr)
 
     raise ValueError(f"Unknown reader {reader}")
 
 
 def write_audio(
     itr: Iterator[np.ndarray | Tensor],
     out_file: str | Path,
     sample_rate: int,
     *,
-    writer: Writer = "av",
+    writer: Writer = "sf",
 ) -> None:
     """Function that writes a stream of audio to a file.
 
     Args:
         itr: Iterator of audio chunks.
         out_file: Path to the output file.
         sample_rate: Sample rate of the audio.
-        writer: Writer to use. Can be either `ffmpeg` or `av`.
+        writer: Writer to use. Can be either ``sf``, ``ffmpeg``, ``av``.
     """
     if writer == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in this system.")
             writer = "av"
         else:
             write_audio_ffmpeg(itr, out_file, sample_rate)
             return
 
+    if writer == "sf":
+        write_audio_sf(itr, out_file, sample_rate)
+        return
+
     if writer == "av":
         write_audio_av(itr, out_file, sample_rate)
         return
 
     raise ValueError(f"Unknown writer {writer}")
```

### Comparing `ml-starter-0.0.58/ml/utils/augmentation.py` & `ml-starter-0.0.59/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/caching.py` & `ml-starter-0.0.59/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/checkpoint.py` & `ml-starter-0.0.59/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/cli.py` & `ml-starter-0.0.59/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/colors.py` & `ml-starter-0.0.59/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/config.py` & `ml-starter-0.0.59/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/data.py` & `ml-starter-0.0.59/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/datetime.py` & `ml-starter-0.0.59/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/device/auto.py` & `ml-starter-0.0.59/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/device/base.py` & `ml-starter-0.0.59/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/device/cpu.py` & `ml-starter-0.0.59/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/device/gpu.py` & `ml-starter-0.0.59/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/device/metal.py` & `ml-starter-0.0.59/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/distributed.py` & `ml-starter-0.0.59/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/image.py` & `ml-starter-0.0.59/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/large_models.py` & `ml-starter-0.0.59/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/logging.py` & `ml-starter-0.0.59/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/meter.py` & `ml-starter-0.0.59/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/parallel.py` & `ml-starter-0.0.59/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/staging.py` & `ml-starter-0.0.59/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/timer.py` & `ml-starter-0.0.59/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/tokens.py` & `ml-starter-0.0.59/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/torch_distributed.py` & `ml-starter-0.0.59/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/triton/kmeans.py` & `ml-starter-0.0.59/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/triton/lion.py` & `ml-starter-0.0.59/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml/utils/video.py` & `ml-starter-0.0.59/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.59/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.58
+Version: 0.0.59
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.58/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.59/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/pyproject.toml` & `ml-starter-0.0.59/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.58/setup.py` & `ml-starter-0.0.59/setup.py`

 * *Files identical despite different names*

