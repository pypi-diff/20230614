# Comparing `tmp/ml-starter-0.0.56.tar.gz` & `tmp/ml-starter-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.56.tar", last modified: Tue Jun 13 21:27:21 2023, max compression
+gzip compressed data, was "ml-starter-0.0.57.tar", last modified: Wed Jun 14 02:41:41 2023, max compression
```

## Comparing `ml-starter-0.0.56.tar` & `ml-starter-0.0.57.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 21:27:03.000000 ml-starter-0.0.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 21:27:03.000000 ml-starter-0.0.56/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 21:27:21.133587 ml-starter-0.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-13 21:27:03.000000 ml-starter-0.0.56/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.105587 ml-starter-0.0.56/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.105587 ml-starter-0.0.56/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.109587 ml-starter-0.0.56/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.109587 ml-starter-0.0.56/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.109587 ml-starter-0.0.56/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.109587 ml-starter-0.0.56/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.113587 ml-starter-0.0.56/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.117587 ml-starter-0.0.56/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.117587 ml-starter-0.0.56/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.117587 ml-starter-0.0.56/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.121587 ml-starter-0.0.56/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.125587 ml-starter-0.0.56/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-06-13 21:27:03.000000 ml-starter-0.0.56/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:27:21.133587 ml-starter-0.0.56/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 21:27:21.000000 ml-starter-0.0.56/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 21:27:03.000000 ml-starter-0.0.56/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 21:27:03.000000 ml-starter-0.0.56/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 21:27:03.000000 ml-starter-0.0.56/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 21:27:03.000000 ml-starter-0.0.56/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-13 21:27:21.137587 ml-starter-0.0.56/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-13 21:27:03.000000 ml-starter-0.0.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-14 02:41:29.000000 ml-starter-0.0.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 02:41:29.000000 ml-starter-0.0.57/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 02:41:41.115714 ml-starter-0.0.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-14 02:41:29.000000 ml-starter-0.0.57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.099714 ml-starter-0.0.57/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.099714 ml-starter-0.0.57/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25216 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44680 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.103714 ml-starter-0.0.57/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47547 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.107715 ml-starter-0.0.57/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.111714 ml-starter-0.0.57/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.111714 ml-starter-0.0.57/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-06-14 02:41:29.000000 ml-starter-0.0.57/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:41:41.115714 ml-starter-0.0.57/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 02:41:41.000000 ml-starter-0.0.57/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-14 02:41:29.000000 ml-starter-0.0.57/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 02:41:29.000000 ml-starter-0.0.57/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 02:41:29.000000 ml-starter-0.0.57/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-14 02:41:29.000000 ml-starter-0.0.57/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-14 02:41:41.115714 ml-starter-0.0.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-14 02:41:29.000000 ml-starter-0.0.57/setup.py
```

### Comparing `ml-starter-0.0.56/LICENSE` & `ml-starter-0.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/PKG-INFO` & `ml-starter-0.0.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.56
+Version: 0.0.57
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.56/README.md` & `ml-starter-0.0.57/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/api.py` & `ml-starter-0.0.57/ml/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
     "init_empty_weights",
     "init_parallelism",
     "InitializationType",
     "instantiate_config",
     "is_debugging",
     "is_distributed",
     "is_master",
+    "KMeans",
     "launch_subprocesses",
     "LearnedPositionalEmbeddings",
     "load_model_and_task",
     "lora",
     "LoraConv1d",
     "LoraConv2d",
     "LoraConvTranspose1d",
@@ -207,14 +208,15 @@
     LearnedPositionalEmbeddings,
     RotaryEmbeddings,
     SinusoidalEmbeddings,
     cast_embedding_kind,
     get_positional_embeddings,
 )
 from ml.models.init import InitializationType, cast_init_type, init_
+from ml.models.kmeans import KMeans
 from ml.models.lora import (
     LoraConv1d,
     LoraConv2d,
     LoraConvTranspose1d,
     LoraConvTranspose2d,
     LoraEmbedding,
     LoraGRU,
```

### Comparing `ml-starter-0.0.56/ml/core/common_types.py` & `ml-starter-0.0.57/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/core/config.py` & `ml-starter-0.0.57/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/core/env.py` & `ml-starter-0.0.57/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/core/registry.py` & `ml-starter-0.0.57/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/core/state.py` & `ml-starter-0.0.57/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/launchers/base.py` & `ml-starter-0.0.57/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/launchers/mp.py` & `ml-starter-0.0.57/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/launchers/slurm.py` & `ml-starter-0.0.57/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/launchers/torchrun.py` & `ml-starter-0.0.57/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/loggers/base.py` & `ml-starter-0.0.57/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/loggers/meter.py` & `ml-starter-0.0.57/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/loggers/multi.py` & `ml-starter-0.0.57/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/loggers/stdout.py` & `ml-starter-0.0.57/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/loggers/tensorboard.py` & `ml-starter-0.0.57/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/lr_schedulers/base.py` & `ml-starter-0.0.57/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/lr_schedulers/constant.py` & `ml-starter-0.0.57/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.57/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.57/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/lr_schedulers/linear.py` & `ml-starter-0.0.57/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.57/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.57/ml/lr_schedulers/scripts/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ml.core.state import State
 from ml.utils.argparse import add_args, from_args
 
 
 def main() -> None:
     """Plots a learning rate schedule."""
     try:
-        import matplotlib.pyplot as plt
+        import matplotlib.pyplot as plt  # type: ignore[import]
     except ImportError as e:
         raise ImportError("Please install matplotlib to use this script: `pip install matplotlib`") from e
 
     # Gets the plotting-specific arguments.
     parser = argparse.ArgumentParser(description="Plots a learning rate schedule")
     parser.add_argument("lr_scheduler", help="Which scheduler to plot")
     parser.add_argument("save_path", help="Where to save the plot")
```

### Comparing `ml-starter-0.0.56/ml/models/activations.py` & `ml-starter-0.0.57/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/models/base.py` & `ml-starter-0.0.57/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/models/embeddings.py` & `ml-starter-0.0.57/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/models/init.py` & `ml-starter-0.0.57/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/models/lora.py` & `ml-starter-0.0.57/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/models/norms.py` & `ml-starter-0.0.57/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/models/parallel.py` & `ml-starter-0.0.57/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/optimizers/adam.py` & `ml-starter-0.0.57/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/optimizers/adamw.py` & `ml-starter-0.0.57/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/optimizers/adan.py` & `ml-starter-0.0.57/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/optimizers/base.py` & `ml-starter-0.0.57/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/optimizers/common.py` & `ml-starter-0.0.57/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/optimizers/lion.py` & `ml-starter-0.0.57/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/optimizers/sgd.py` & `ml-starter-0.0.57/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/optimizers/shampoo.py` & `ml-starter-0.0.57/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/scripts/cli.py` & `ml-starter-0.0.57/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/scripts/stage.py` & `ml-starter-0.0.57/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/scripts/train.py` & `ml-starter-0.0.57/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/base.py` & `ml-starter-0.0.57/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.57/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.57/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/collate.py` & `ml-starter-0.0.57/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.57/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.57/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.57/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.57/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.57/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/utils.py` & `ml-starter-0.0.57/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.57/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/environments/base.py` & `ml-starter-0.0.57/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/environments/utils.py` & `ml-starter-0.0.57/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/environments/worker.py` & `ml-starter-0.0.57/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/losses/reduce.py` & `ml-starter-0.0.57/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/rl/base.py` & `ml-starter-0.0.57/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/rl/replay.py` & `ml-starter-0.0.57/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/tasks/sl/base.py` & `ml-starter-0.0.57/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/base.py` & `ml-starter-0.0.57/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/learning.py` & `ml-starter-0.0.57/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/compile.py` & `ml-starter-0.0.57/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.57/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.57/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.57/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.57/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.57/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.57/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.57/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.57/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.57/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/rl.py` & `ml-starter-0.0.57/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/trainers/sl.py` & `ml-starter-0.0.57/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/argparse.py` & `ml-starter-0.0.57/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/atomic.py` & `ml-starter-0.0.57/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/audio.py` & `ml-starter-0.0.57/ml/utils/audio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="import"
 """Defines utilites for saving and loading audio streams.
 
 The main API for using this module is:
 
 .. code-blocks:: python
 
     from ml.utils.audio import read_audio, write_audio
@@ -78,15 +79,18 @@
     """
     props = AudioProps.from_file_av(in_file)
 
     container = av.open(str(in_file))
     stream = container.streams.audio[0]
 
     for frame in container.decode(stream):
-        yield frame.to_ndarray().reshape(-1, props.channels).T
+        frame_np = frame.to_ndarray().reshape(-1, props.channels).T
+        if frame_np.dtype == np.int16:
+            frame_np = frame_np.astype(np.float32) / 2**15
+        yield frame_np
 
 
 def read_audio_ffmpeg(in_file: str | Path, *, chunk_size: int = 16_000) -> Iterator[np.ndarray]:
     """Function that reads an audio file to a stream of numpy arrays using FFMPEG.
 
     Args:
         in_file: Path to the input file.
@@ -240,27 +244,27 @@
     *,
     chunk_length: int | None = None,
     sampling_rate: int | None = None,
     reader: Reader = "av",
 ) -> Iterator[np.ndarray]:
     """Function that reads a stream of audio from a file.
 
-    The audio is expected to be in the range (-1, 1).
+    The output audio is in ``float32`` format.
 
     Args:
         in_file: Path to the input file.
-        chunk_length: Size of the chunks to read. If `None`, will iterate
+        chunk_length: Size of the chunks to read. If ``None``, will iterate
             whatever chunk size the underlying reader uses. Otherwise, samples
             will be rechunked to the desired size.
-        sampling_rate: Sampling rate to resample the audio to. If `None`, will
-            use the sampling rate of the input audio.
-        reader: Reader to use. Can be either `ffmpeg` or `av`.
+        sampling_rate: Sampling rate to resample the audio to. If ``None``,
+            will use the sampling rate of the input audio.
+        reader: Reader to use. Can be either ``ffmpeg`` or ``av``.
 
     Returns:
-        Iterator over numpy arrays, with shape (n_channels, n_samples).
+        Iterator over numpy arrays, with shape ``(n_channels, n_samples)``.
     """
     if reader == "ffmpeg":
         if not shutil.which("ffmpeg"):
             warnings.warn("FFMPEG is not available in this system.")
             reader = "av"
         else:
             sr = None if sampling_rate is None else (AudioProps.from_file_ffmpeg(in_file).sample_rate, sampling_rate)
```

### Comparing `ml-starter-0.0.56/ml/utils/augmentation.py` & `ml-starter-0.0.57/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/caching.py` & `ml-starter-0.0.57/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/checkpoint.py` & `ml-starter-0.0.57/ml/utils/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 from ml.trainers.base import BaseTrainer
 from ml.utils.data import check_md5, check_sha256
 from ml.utils.device.auto import AutoDevice
 from ml.utils.timer import Timer
 
 logger = logging.getLogger(__name__)
 
-USER_AGENT = "ml-starter"
-
 T = TypeVar("T")
 
 
 def instantiate_config(config: str | Path | DictConfig | dict) -> Objects:
     """Builds the objects from the raw config.
 
     Args:
```

### Comparing `ml-starter-0.0.56/ml/utils/cli.py` & `ml-starter-0.0.57/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/colors.py` & `ml-starter-0.0.57/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/config.py` & `ml-starter-0.0.57/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/data.py` & `ml-starter-0.0.57/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/datetime.py` & `ml-starter-0.0.57/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/device/auto.py` & `ml-starter-0.0.57/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/device/base.py` & `ml-starter-0.0.57/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/device/cpu.py` & `ml-starter-0.0.57/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/device/gpu.py` & `ml-starter-0.0.57/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/device/metal.py` & `ml-starter-0.0.57/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/distributed.py` & `ml-starter-0.0.57/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/image.py` & `ml-starter-0.0.57/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/large_models.py` & `ml-starter-0.0.57/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/logging.py` & `ml-starter-0.0.57/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/meter.py` & `ml-starter-0.0.57/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/parallel.py` & `ml-starter-0.0.57/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/staging.py` & `ml-starter-0.0.57/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/timer.py` & `ml-starter-0.0.57/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/tokens.py` & `ml-starter-0.0.57/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/torch_distributed.py` & `ml-starter-0.0.57/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/ml/utils/triton/lion.py` & `ml-starter-0.0.57/ml/utils/triton/lion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="import"
 # ruff: noqa: ANN001, ANN201, ANN202, N803, N806
 """Implements a Triton kernel for the Lion optimizer."""
 
 from typing import Any
 
 import triton
 import triton.language as tl
```

### Comparing `ml-starter-0.0.56/ml/utils/video.py` & `ml-starter-0.0.57/ml/utils/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# mypy: disable-error-code="import"
 """Defines utilites for saving and loading video streams.
 
 The main API for using this module is:
 
 .. code-block:: python
 
     from ml.utils.video import read_video, write_video
```

### Comparing `ml-starter-0.0.56/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.57/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.56
+Version: 0.0.57
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.56/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.57/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.56/pyproject.toml` & `ml-starter-0.0.57/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -38,20 +38,16 @@
 # For TorchScript stuff.
 disable_error_code = ["attr-defined"]
 
 [[tool.mypy.overrides]]
 
 module = [
     "av.*",
-    "cv2.*",
-    "ffmpeg.*",
-    "matplotlib.*",
     "torchaudio.*",
     "torchvision.*",
-    "triton.*",
 ]
 
 ignore_missing_imports = true
 
 [tool.isort]
 
 profile = "black"
```

### Comparing `ml-starter-0.0.56/setup.py` & `ml-starter-0.0.57/setup.py`

 * *Files identical despite different names*

