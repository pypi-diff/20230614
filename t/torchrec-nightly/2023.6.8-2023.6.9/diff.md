# Comparing `tmp/torchrec_nightly-2023.6.8-py39-none-any.whl.zip` & `tmp/torchrec_nightly-2023.6.9-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,145 +1,145 @@
-Zip file size: 351028 bytes, number of entries: 143
--rw-r--r--  2.0 unx      811 b- defN 23-Jun-08 11:18 torchrec/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 23-Jun-08 11:18 torchrec/streamable.py
--rw-r--r--  2.0 unx      854 b- defN 23-Jun-08 11:18 torchrec/types.py
--rw-r--r--  2.0 unx     1153 b- defN 23-Jun-08 11:18 torchrec/datasets/__init__.py
--rw-r--r--  2.0 unx    41469 b- defN 23-Jun-08 11:18 torchrec/datasets/criteo.py
--rw-r--r--  2.0 unx     4548 b- defN 23-Jun-08 11:18 torchrec/datasets/movielens.py
--rw-r--r--  2.0 unx     6539 b- defN 23-Jun-08 11:18 torchrec/datasets/random.py
--rw-r--r--  2.0 unx    10909 b- defN 23-Jun-08 11:18 torchrec/datasets/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/datasets/scripts/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Jun-08 11:18 torchrec/datasets/scripts/contiguous_preproc_criteo.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jun-08 11:18 torchrec/datasets/scripts/npy_preproc_criteo.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jun-08 11:18 torchrec/datasets/scripts/shuffle_preproc_criteo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/datasets/test_utils/__init__.py
--rw-r--r--  2.0 unx     5308 b- defN 23-Jun-08 11:18 torchrec/datasets/test_utils/criteo_test_utils.py
--rw-r--r--  2.0 unx     1912 b- defN 23-Jun-08 11:18 torchrec/distributed/__init__.py
--rw-r--r--  2.0 unx    37053 b- defN 23-Jun-08 11:18 torchrec/distributed/batched_embedding_kernel.py
--rw-r--r--  2.0 unx     2069 b- defN 23-Jun-08 11:18 torchrec/distributed/collective_utils.py
--rw-r--r--  2.0 unx     4988 b- defN 23-Jun-08 11:18 torchrec/distributed/comm.py
--rw-r--r--  2.0 unx    55918 b- defN 23-Jun-08 11:18 torchrec/distributed/comm_ops.py
--rw-r--r--  2.0 unx    35580 b- defN 23-Jun-08 11:18 torchrec/distributed/dist_data.py
--rw-r--r--  2.0 unx    31599 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding.py
--rw-r--r--  2.0 unx     3872 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_kernel.py
--rw-r--r--  2.0 unx    28994 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_lookup.py
--rw-r--r--  2.0 unx    18564 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_sharding.py
--rw-r--r--  2.0 unx    37089 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_tower_sharding.py
--rw-r--r--  2.0 unx    15030 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_types.py
--rw-r--r--  2.0 unx    35078 b- defN 23-Jun-08 11:18 torchrec/distributed/embeddingbag.py
--rw-r--r--  2.0 unx     7373 b- defN 23-Jun-08 11:18 torchrec/distributed/fbgemm_qcomm_codec.py
--rw-r--r--  2.0 unx     5542 b- defN 23-Jun-08 11:18 torchrec/distributed/fp_embeddingbag.py
--rw-r--r--  2.0 unx     5273 b- defN 23-Jun-08 11:18 torchrec/distributed/fused_embedding.py
--rw-r--r--  2.0 unx     5110 b- defN 23-Jun-08 11:18 torchrec/distributed/fused_embeddingbag.py
--rw-r--r--  2.0 unx     1709 b- defN 23-Jun-08 11:18 torchrec/distributed/fused_params.py
--rw-r--r--  2.0 unx     3807 b- defN 23-Jun-08 11:18 torchrec/distributed/grouped_position_weighted.py
--rw-r--r--  2.0 unx    19786 b- defN 23-Jun-08 11:18 torchrec/distributed/model_parallel.py
--rw-r--r--  2.0 unx    13729 b- defN 23-Jun-08 11:18 torchrec/distributed/quant_embedding.py
--rw-r--r--  2.0 unx    13343 b- defN 23-Jun-08 11:18 torchrec/distributed/quant_embedding_kernel.py
--rw-r--r--  2.0 unx    10931 b- defN 23-Jun-08 11:18 torchrec/distributed/quant_embeddingbag.py
--rw-r--r--  2.0 unx     9261 b- defN 23-Jun-08 11:18 torchrec/distributed/shard.py
--rw-r--r--  2.0 unx    19411 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding_plan.py
--rw-r--r--  2.0 unx    34059 b- defN 23-Jun-08 11:18 torchrec/distributed/train_pipeline.py
--rw-r--r--  2.0 unx    24927 b- defN 23-Jun-08 11:18 torchrec/distributed/types.py
--rw-r--r--  2.0 unx    11873 b- defN 23-Jun-08 11:18 torchrec/distributed/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/distributed/composable/__init__.py
--rw-r--r--  2.0 unx     3207 b- defN 23-Jun-08 11:18 torchrec/distributed/composable/table_batched_embedding_slice.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/__init__.py
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/constants.py
--rw-r--r--  2.0 unx    10318 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/enumerators.py
--rw-r--r--  2.0 unx    12642 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/partitioners.py
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/perf_models.py
--rw-r--r--  2.0 unx    13288 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/planners.py
--rw-r--r--  2.0 unx    11134 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/proposers.py
--rw-r--r--  2.0 unx    40395 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/shard_estimators.py
--rw-r--r--  2.0 unx    23617 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/stats.py
--rw-r--r--  2.0 unx     9125 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/storage_reservations.py
--rw-r--r--  2.0 unx    13899 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/types.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/__init__.py
--rw-r--r--  2.0 unx     2539 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/cw_sequence_sharding.py
--rw-r--r--  2.0 unx     9519 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/cw_sharding.py
--rw-r--r--  2.0 unx     2802 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/dp_sequence_sharding.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/dp_sharding.py
--rw-r--r--  2.0 unx     5041 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/rw_sequence_sharding.py
--rw-r--r--  2.0 unx    12850 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/rw_sharding.py
--rw-r--r--  2.0 unx     3114 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/sequence_sharding.py
--rw-r--r--  2.0 unx     7692 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/tw_sequence_sharding.py
--rw-r--r--  2.0 unx    16315 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/tw_sharding.py
--rw-r--r--  2.0 unx     1284 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/twcw_sharding.py
--rw-r--r--  2.0 unx    19898 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/twrw_sharding.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/__init__.py
--rw-r--r--  2.0 unx    10213 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/infer_utils.py
--rw-r--r--  2.0 unx     4868 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/multi_process.py
--rw-r--r--  2.0 unx    34246 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/test_model.py
--rw-r--r--  2.0 unx    11193 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/test_model_parallel.py
--rw-r--r--  2.0 unx    25190 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/test_model_parallel_base.py
--rw-r--r--  2.0 unx    15367 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/test_sharding.py
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-08 11:18 torchrec/fx/__init__.py
--rw-r--r--  2.0 unx     6477 b- defN 23-Jun-08 11:18 torchrec/fx/tracer.py
--rw-r--r--  2.0 unx     4401 b- defN 23-Jun-08 11:18 torchrec/fx/utils.py
--rw-r--r--  2.0 unx     1223 b- defN 23-Jun-08 11:18 torchrec/inference/__init__.py
--rw-r--r--  2.0 unx     3614 b- defN 23-Jun-08 11:18 torchrec/inference/client.py
--rw-r--r--  2.0 unx     3957 b- defN 23-Jun-08 11:18 torchrec/inference/model_packager.py
--rw-r--r--  2.0 unx     8068 b- defN 23-Jun-08 11:18 torchrec/inference/modules.py
--rw-r--r--  2.0 unx     3797 b- defN 23-Jun-08 11:18 torchrec/inference/state_dict_transform.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/metrics/__init__.py
--rw-r--r--  2.0 unx     4168 b- defN 23-Jun-08 11:18 torchrec/metrics/accuracy.py
--rw-r--r--  2.0 unx    12549 b- defN 23-Jun-08 11:18 torchrec/metrics/auc.py
--rw-r--r--  2.0 unx     3703 b- defN 23-Jun-08 11:18 torchrec/metrics/calibration.py
--rw-r--r--  2.0 unx     3465 b- defN 23-Jun-08 11:18 torchrec/metrics/ctr.py
--rw-r--r--  2.0 unx     3836 b- defN 23-Jun-08 11:18 torchrec/metrics/mae.py
--rw-r--r--  2.0 unx    17909 b- defN 23-Jun-08 11:18 torchrec/metrics/metric_module.py
--rw-r--r--  2.0 unx     6778 b- defN 23-Jun-08 11:18 torchrec/metrics/metrics_config.py
--rw-r--r--  2.0 unx     3695 b- defN 23-Jun-08 11:18 torchrec/metrics/metrics_namespace.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Jun-08 11:18 torchrec/metrics/model_utils.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Jun-08 11:18 torchrec/metrics/mse.py
--rw-r--r--  2.0 unx     5605 b- defN 23-Jun-08 11:18 torchrec/metrics/multiclass_recall.py
--rw-r--r--  2.0 unx     6811 b- defN 23-Jun-08 11:18 torchrec/metrics/ne.py
--rw-r--r--  2.0 unx    31495 b- defN 23-Jun-08 11:18 torchrec/metrics/rec_metric.py
--rw-r--r--  2.0 unx    10490 b- defN 23-Jun-08 11:18 torchrec/metrics/recall_session.py
--rw-r--r--  2.0 unx     6057 b- defN 23-Jun-08 11:18 torchrec/metrics/throughput.py
--rw-r--r--  2.0 unx    10622 b- defN 23-Jun-08 11:18 torchrec/metrics/tower_qps.py
--rw-r--r--  2.0 unx     2867 b- defN 23-Jun-08 11:18 torchrec/metrics/weighted_avg.py
--rw-r--r--  2.0 unx    16441 b- defN 23-Jun-08 11:18 torchrec/metrics/test_utils/__init__.py
--rw-r--r--  2.0 unx      913 b- defN 23-Jun-08 11:18 torchrec/models/__init__.py
--rw-r--r--  2.0 unx    11410 b- defN 23-Jun-08 11:18 torchrec/models/deepfm.py
--rw-r--r--  2.0 unx    30000 b- defN 23-Jun-08 11:18 torchrec/models/dlrm.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/models/experimental/__init__.py
--rw-r--r--  2.0 unx     9825 b- defN 23-Jun-08 11:18 torchrec/models/experimental/test_transformerdlrm.py
--rw-r--r--  2.0 unx     7434 b- defN 23-Jun-08 11:18 torchrec/models/experimental/transformerdlrm.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Jun-08 11:18 torchrec/modules/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 23-Jun-08 11:18 torchrec/modules/activation.py
--rw-r--r--  2.0 unx    15163 b- defN 23-Jun-08 11:18 torchrec/modules/crossnet.py
--rw-r--r--  2.0 unx     8415 b- defN 23-Jun-08 11:18 torchrec/modules/deepfm.py
--rw-r--r--  2.0 unx     5537 b- defN 23-Jun-08 11:18 torchrec/modules/embedding_configs.py
--rw-r--r--  2.0 unx    14021 b- defN 23-Jun-08 11:18 torchrec/modules/embedding_modules.py
--rw-r--r--  2.0 unx     4858 b- defN 23-Jun-08 11:18 torchrec/modules/embedding_tower.py
--rw-r--r--  2.0 unx    12360 b- defN 23-Jun-08 11:18 torchrec/modules/feature_processor.py
--rw-r--r--  2.0 unx     2169 b- defN 23-Jun-08 11:18 torchrec/modules/feature_processor_.py
--rw-r--r--  2.0 unx     3855 b- defN 23-Jun-08 11:18 torchrec/modules/fp_embedding_modules.py
--rw-r--r--  2.0 unx    31193 b- defN 23-Jun-08 11:18 torchrec/modules/fused_embedding_modules.py
--rw-r--r--  2.0 unx    10696 b- defN 23-Jun-08 11:18 torchrec/modules/lazy_extension.py
--rw-r--r--  2.0 unx     6309 b- defN 23-Jun-08 11:18 torchrec/modules/mlp.py
--rw-r--r--  2.0 unx     4022 b- defN 23-Jun-08 11:18 torchrec/modules/utils.py
--rw-r--r--  2.0 unx     1639 b- defN 23-Jun-08 11:18 torchrec/optim/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-Jun-08 11:18 torchrec/optim/apply_optimizer_in_backward.py
--rw-r--r--  2.0 unx     1569 b- defN 23-Jun-08 11:18 torchrec/optim/clipping.py
--rw-r--r--  2.0 unx     1353 b- defN 23-Jun-08 11:18 torchrec/optim/fused.py
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-08 11:18 torchrec/optim/keyed.py
--rw-r--r--  2.0 unx     4420 b- defN 23-Jun-08 11:18 torchrec/optim/optimizers.py
--rw-r--r--  2.0 unx     7405 b- defN 23-Jun-08 11:18 torchrec/optim/rowwise_adagrad.py
--rw-r--r--  2.0 unx     4865 b- defN 23-Jun-08 11:18 torchrec/optim/warmup.py
--rw-r--r--  2.0 unx      560 b- defN 23-Jun-08 11:18 torchrec/optim/test_utils/__init__.py
--rw-r--r--  2.0 unx     1140 b- defN 23-Jun-08 11:18 torchrec/quant/__init__.py
--rw-r--r--  2.0 unx    22933 b- defN 23-Jun-08 11:18 torchrec/quant/embedding_modules.py
--rw-r--r--  2.0 unx     4100 b- defN 23-Jun-08 11:18 torchrec/quant/utils.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Jun-08 11:18 torchrec/sparse/__init__.py
--rw-r--r--  2.0 unx    55583 b- defN 23-Jun-08 11:18 torchrec/sparse/jagged_tensor.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jun-08 11:18 torchrec/sparse/test_utils/__init__.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Jun-08 11:18 torchrec/test_utils/__init__.py
--rw-r--r--  2.0 unx     1530 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     5011 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    13347 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/RECORD
-143 files, 1428724 bytes uncompressed, 329674 bytes compressed:  76.9%
+Zip file size: 353905 bytes, number of entries: 143
+-rw-r--r--  2.0 unx      811 b- defN 23-Jun-09 11:18 torchrec/__init__.py
+-rw-r--r--  2.0 unx     1638 b- defN 23-Jun-09 11:18 torchrec/streamable.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Jun-09 11:18 torchrec/types.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Jun-09 11:18 torchrec/datasets/__init__.py
+-rw-r--r--  2.0 unx    41469 b- defN 23-Jun-09 11:18 torchrec/datasets/criteo.py
+-rw-r--r--  2.0 unx     4548 b- defN 23-Jun-09 11:18 torchrec/datasets/movielens.py
+-rw-r--r--  2.0 unx     6539 b- defN 23-Jun-09 11:18 torchrec/datasets/random.py
+-rw-r--r--  2.0 unx    10909 b- defN 23-Jun-09 11:18 torchrec/datasets/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/datasets/scripts/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Jun-09 11:18 torchrec/datasets/scripts/contiguous_preproc_criteo.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jun-09 11:18 torchrec/datasets/scripts/npy_preproc_criteo.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jun-09 11:18 torchrec/datasets/scripts/shuffle_preproc_criteo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/datasets/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5308 b- defN 23-Jun-09 11:18 torchrec/datasets/test_utils/criteo_test_utils.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-Jun-09 11:18 torchrec/distributed/__init__.py
+-rw-r--r--  2.0 unx    37411 b- defN 23-Jun-09 11:18 torchrec/distributed/batched_embedding_kernel.py
+-rw-r--r--  2.0 unx     2069 b- defN 23-Jun-09 11:18 torchrec/distributed/collective_utils.py
+-rw-r--r--  2.0 unx     4988 b- defN 23-Jun-09 11:18 torchrec/distributed/comm.py
+-rw-r--r--  2.0 unx    55918 b- defN 23-Jun-09 11:18 torchrec/distributed/comm_ops.py
+-rw-r--r--  2.0 unx    35580 b- defN 23-Jun-09 11:18 torchrec/distributed/dist_data.py
+-rw-r--r--  2.0 unx    32013 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding.py
+-rw-r--r--  2.0 unx     4947 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_kernel.py
+-rw-r--r--  2.0 unx    29176 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_lookup.py
+-rw-r--r--  2.0 unx    20599 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_sharding.py
+-rw-r--r--  2.0 unx    37089 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_tower_sharding.py
+-rw-r--r--  2.0 unx    15030 b- defN 23-Jun-09 11:18 torchrec/distributed/embedding_types.py
+-rw-r--r--  2.0 unx    35218 b- defN 23-Jun-09 11:18 torchrec/distributed/embeddingbag.py
+-rw-r--r--  2.0 unx     7373 b- defN 23-Jun-09 11:18 torchrec/distributed/fbgemm_qcomm_codec.py
+-rw-r--r--  2.0 unx     6137 b- defN 23-Jun-09 11:18 torchrec/distributed/fp_embeddingbag.py
+-rw-r--r--  2.0 unx     5243 b- defN 23-Jun-09 11:18 torchrec/distributed/fused_embedding.py
+-rw-r--r--  2.0 unx     5110 b- defN 23-Jun-09 11:18 torchrec/distributed/fused_embeddingbag.py
+-rw-r--r--  2.0 unx     2271 b- defN 23-Jun-09 11:18 torchrec/distributed/fused_params.py
+-rw-r--r--  2.0 unx     3807 b- defN 23-Jun-09 11:18 torchrec/distributed/grouped_position_weighted.py
+-rw-r--r--  2.0 unx    19786 b- defN 23-Jun-09 11:18 torchrec/distributed/model_parallel.py
+-rw-r--r--  2.0 unx    14686 b- defN 23-Jun-09 11:18 torchrec/distributed/quant_embedding.py
+-rw-r--r--  2.0 unx    14976 b- defN 23-Jun-09 11:18 torchrec/distributed/quant_embedding_kernel.py
+-rw-r--r--  2.0 unx    11770 b- defN 23-Jun-09 11:18 torchrec/distributed/quant_embeddingbag.py
+-rw-r--r--  2.0 unx     9261 b- defN 23-Jun-09 11:18 torchrec/distributed/shard.py
+-rw-r--r--  2.0 unx    19411 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding_plan.py
+-rw-r--r--  2.0 unx    36724 b- defN 23-Jun-09 11:18 torchrec/distributed/train_pipeline.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Jun-09 11:18 torchrec/distributed/types.py
+-rw-r--r--  2.0 unx    11873 b- defN 23-Jun-09 11:18 torchrec/distributed/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/distributed/composable/__init__.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-Jun-09 11:18 torchrec/distributed/composable/table_batched_embedding_slice.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/__init__.py
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/constants.py
+-rw-r--r--  2.0 unx    10318 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/enumerators.py
+-rw-r--r--  2.0 unx    12642 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/partitioners.py
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/perf_models.py
+-rw-r--r--  2.0 unx    13288 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/planners.py
+-rw-r--r--  2.0 unx    11236 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/proposers.py
+-rw-r--r--  2.0 unx    40395 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/shard_estimators.py
+-rw-r--r--  2.0 unx    23617 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/stats.py
+-rw-r--r--  2.0 unx     9125 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/storage_reservations.py
+-rw-r--r--  2.0 unx    13899 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/types.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Jun-09 11:18 torchrec/distributed/planner/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/__init__.py
+-rw-r--r--  2.0 unx     2539 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/cw_sequence_sharding.py
+-rw-r--r--  2.0 unx     9519 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/cw_sharding.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/dp_sequence_sharding.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/dp_sharding.py
+-rw-r--r--  2.0 unx     5041 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/rw_sequence_sharding.py
+-rw-r--r--  2.0 unx    12850 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/rw_sharding.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/sequence_sharding.py
+-rw-r--r--  2.0 unx     7692 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/tw_sequence_sharding.py
+-rw-r--r--  2.0 unx    16315 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/tw_sharding.py
+-rw-r--r--  2.0 unx     1284 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/twcw_sharding.py
+-rw-r--r--  2.0 unx    19898 b- defN 23-Jun-09 11:18 torchrec/distributed/sharding/twrw_sharding.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/__init__.py
+-rw-r--r--  2.0 unx    10453 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/infer_utils.py
+-rw-r--r--  2.0 unx     4868 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/multi_process.py
+-rw-r--r--  2.0 unx    34246 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/test_model.py
+-rw-r--r--  2.0 unx    11193 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/test_model_parallel.py
+-rw-r--r--  2.0 unx    25308 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/test_model_parallel_base.py
+-rw-r--r--  2.0 unx    15367 b- defN 23-Jun-09 11:18 torchrec/distributed/test_utils/test_sharding.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-09 11:18 torchrec/fx/__init__.py
+-rw-r--r--  2.0 unx     6477 b- defN 23-Jun-09 11:18 torchrec/fx/tracer.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-Jun-09 11:18 torchrec/fx/utils.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Jun-09 11:18 torchrec/inference/__init__.py
+-rw-r--r--  2.0 unx     3614 b- defN 23-Jun-09 11:18 torchrec/inference/client.py
+-rw-r--r--  2.0 unx     3957 b- defN 23-Jun-09 11:18 torchrec/inference/model_packager.py
+-rw-r--r--  2.0 unx     8068 b- defN 23-Jun-09 11:18 torchrec/inference/modules.py
+-rw-r--r--  2.0 unx     3797 b- defN 23-Jun-09 11:18 torchrec/inference/state_dict_transform.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/metrics/__init__.py
+-rw-r--r--  2.0 unx     4168 b- defN 23-Jun-09 11:18 torchrec/metrics/accuracy.py
+-rw-r--r--  2.0 unx    12549 b- defN 23-Jun-09 11:18 torchrec/metrics/auc.py
+-rw-r--r--  2.0 unx     3703 b- defN 23-Jun-09 11:18 torchrec/metrics/calibration.py
+-rw-r--r--  2.0 unx     3465 b- defN 23-Jun-09 11:18 torchrec/metrics/ctr.py
+-rw-r--r--  2.0 unx     3836 b- defN 23-Jun-09 11:18 torchrec/metrics/mae.py
+-rw-r--r--  2.0 unx    17909 b- defN 23-Jun-09 11:18 torchrec/metrics/metric_module.py
+-rw-r--r--  2.0 unx     6778 b- defN 23-Jun-09 11:18 torchrec/metrics/metrics_config.py
+-rw-r--r--  2.0 unx     3695 b- defN 23-Jun-09 11:18 torchrec/metrics/metrics_namespace.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-Jun-09 11:18 torchrec/metrics/model_utils.py
+-rw-r--r--  2.0 unx     4631 b- defN 23-Jun-09 11:18 torchrec/metrics/mse.py
+-rw-r--r--  2.0 unx     5605 b- defN 23-Jun-09 11:18 torchrec/metrics/multiclass_recall.py
+-rw-r--r--  2.0 unx     6811 b- defN 23-Jun-09 11:18 torchrec/metrics/ne.py
+-rw-r--r--  2.0 unx    33554 b- defN 23-Jun-09 11:18 torchrec/metrics/rec_metric.py
+-rw-r--r--  2.0 unx    10490 b- defN 23-Jun-09 11:18 torchrec/metrics/recall_session.py
+-rw-r--r--  2.0 unx     6057 b- defN 23-Jun-09 11:18 torchrec/metrics/throughput.py
+-rw-r--r--  2.0 unx    11160 b- defN 23-Jun-09 11:18 torchrec/metrics/tower_qps.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Jun-09 11:18 torchrec/metrics/weighted_avg.py
+-rw-r--r--  2.0 unx    16441 b- defN 23-Jun-09 11:18 torchrec/metrics/test_utils/__init__.py
+-rw-r--r--  2.0 unx      913 b- defN 23-Jun-09 11:18 torchrec/models/__init__.py
+-rw-r--r--  2.0 unx    11410 b- defN 23-Jun-09 11:18 torchrec/models/deepfm.py
+-rw-r--r--  2.0 unx    30000 b- defN 23-Jun-09 11:18 torchrec/models/dlrm.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 11:18 torchrec/models/experimental/__init__.py
+-rw-r--r--  2.0 unx     9825 b- defN 23-Jun-09 11:18 torchrec/models/experimental/test_transformerdlrm.py
+-rw-r--r--  2.0 unx     7434 b- defN 23-Jun-09 11:18 torchrec/models/experimental/transformerdlrm.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-Jun-09 11:18 torchrec/modules/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jun-09 11:18 torchrec/modules/activation.py
+-rw-r--r--  2.0 unx    15163 b- defN 23-Jun-09 11:18 torchrec/modules/crossnet.py
+-rw-r--r--  2.0 unx     8415 b- defN 23-Jun-09 11:18 torchrec/modules/deepfm.py
+-rw-r--r--  2.0 unx     5537 b- defN 23-Jun-09 11:18 torchrec/modules/embedding_configs.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-Jun-09 11:18 torchrec/modules/embedding_modules.py
+-rw-r--r--  2.0 unx     4858 b- defN 23-Jun-09 11:18 torchrec/modules/embedding_tower.py
+-rw-r--r--  2.0 unx    12360 b- defN 23-Jun-09 11:18 torchrec/modules/feature_processor.py
+-rw-r--r--  2.0 unx     4830 b- defN 23-Jun-09 11:18 torchrec/modules/feature_processor_.py
+-rw-r--r--  2.0 unx     4403 b- defN 23-Jun-09 11:18 torchrec/modules/fp_embedding_modules.py
+-rw-r--r--  2.0 unx    31453 b- defN 23-Jun-09 11:18 torchrec/modules/fused_embedding_modules.py
+-rw-r--r--  2.0 unx    10894 b- defN 23-Jun-09 11:18 torchrec/modules/lazy_extension.py
+-rw-r--r--  2.0 unx     6309 b- defN 23-Jun-09 11:18 torchrec/modules/mlp.py
+-rw-r--r--  2.0 unx     4022 b- defN 23-Jun-09 11:18 torchrec/modules/utils.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-Jun-09 11:18 torchrec/optim/__init__.py
+-rw-r--r--  2.0 unx     2012 b- defN 23-Jun-09 11:18 torchrec/optim/apply_optimizer_in_backward.py
+-rw-r--r--  2.0 unx     1569 b- defN 23-Jun-09 11:18 torchrec/optim/clipping.py
+-rw-r--r--  2.0 unx     1353 b- defN 23-Jun-09 11:18 torchrec/optim/fused.py
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-09 11:18 torchrec/optim/keyed.py
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jun-09 11:18 torchrec/optim/optimizers.py
+-rw-r--r--  2.0 unx     7405 b- defN 23-Jun-09 11:18 torchrec/optim/rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4865 b- defN 23-Jun-09 11:18 torchrec/optim/warmup.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Jun-09 11:18 torchrec/optim/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1140 b- defN 23-Jun-09 11:18 torchrec/quant/__init__.py
+-rw-r--r--  2.0 unx    25656 b- defN 23-Jun-09 11:18 torchrec/quant/embedding_modules.py
+-rw-r--r--  2.0 unx     4296 b- defN 23-Jun-09 11:18 torchrec/quant/utils.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Jun-09 11:18 torchrec/sparse/__init__.py
+-rw-r--r--  2.0 unx    55583 b- defN 23-Jun-09 11:18 torchrec/sparse/jagged_tensor.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Jun-09 11:18 torchrec/sparse/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-09 11:18 torchrec/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1530 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5011 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    13347 b- defN 23-Jun-09 11:22 torchrec_nightly-2023.6.9.dist-info/RECORD
+143 files, 1449792 bytes uncompressed, 332551 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -408,23 +408,23 @@
 
 Filename: torchrec/sparse/test_utils/__init__.py
 Comment: 
 
 Filename: torchrec/test_utils/__init__.py
 Comment: 
 
-Filename: torchrec_nightly-2023.6.8.dist-info/LICENSE
+Filename: torchrec_nightly-2023.6.9.dist-info/LICENSE
 Comment: 
 
-Filename: torchrec_nightly-2023.6.8.dist-info/METADATA
+Filename: torchrec_nightly-2023.6.9.dist-info/METADATA
 Comment: 
 
-Filename: torchrec_nightly-2023.6.8.dist-info/WHEEL
+Filename: torchrec_nightly-2023.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: torchrec_nightly-2023.6.8.dist-info/top_level.txt
+Filename: torchrec_nightly-2023.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: torchrec_nightly-2023.6.8.dist-info/RECORD
+Filename: torchrec_nightly-2023.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchrec/distributed/batched_embedding_kernel.py

```diff
@@ -5,15 +5,26 @@
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import abc
 import copy
 import itertools
 from dataclasses import dataclass
-from typing import Any, cast, Dict, Iterator, List, Optional, Tuple, Union
+from typing import (
+    Any,
+    cast,
+    Dict,
+    Generic,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import torch
 import torch.distributed as dist
 from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     IntNBitTableBatchedEmbeddingBagsCodegen,
 )
 from fbgemm_gpu.split_table_batched_embeddings_ops_training import (
@@ -423,15 +434,18 @@
             end_offset=offset + table_count * rows * dim,
             num_embeddings=-1,
             embedding_dim=dim,
         )
         yield (table_name, weight)
 
 
-class BaseBatchedEmbedding(BaseEmbedding):
+SplitWeightType = TypeVar("SplitWeightType")
+
+
+class BaseBatchedEmbedding(BaseEmbedding, Generic[SplitWeightType]):
     def __init__(
         self,
         config: GroupedEmbeddingConfig,
         pg: Optional[dist.ProcessGroup] = None,
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
@@ -465,16 +479,16 @@
         for (rows, emb_dim, weight_init_min, weight_init_max, param) in zip(
             self._local_rows,
             self._local_cols,
             self._weight_init_mins,
             self._weight_init_maxs,
             self.split_embedding_weights(),
         ):
-            assert param.shape == (rows, emb_dim)
-            param.data.uniform_(
+            assert param.shape == (rows, emb_dim)  # pyre-ignore[16]
+            param.data.uniform_(  # pyre-ignore[16]
                 weight_init_min,
                 weight_init_max,
             )
 
     def forward(self, features: KeyedJaggedTensor) -> torch.Tensor:
         return self.emb_module(
             indices=features.values().long(),
@@ -487,21 +501,22 @@
         destination: Optional[Dict[str, Any]] = None,
         prefix: str = "",
         keep_vars: bool = False,
     ) -> Dict[str, Any]:
         self.flush()
         return get_state_dict(
             self._config.embedding_tables,
+            # pyre-ignore
             self.split_embedding_weights(),
             self._pg,
             destination,
             prefix,
         )
 
-    def split_embedding_weights(self) -> List[torch.Tensor]:
+    def split_embedding_weights(self) -> List[SplitWeightType]:
         return self.emb_module.split_embedding_weights()
 
     @property
     @abc.abstractmethod
     def emb_module(
         self,
     ) -> Union[
@@ -539,15 +554,15 @@
         For a single table with multiple shards (i.e CW) these are combined into one table/weight.
         Used in composability.
         """
         for name, param in self._param_per_table.items():
             yield name, param
 
 
-class BatchedFusedEmbedding(BaseBatchedEmbedding, FusedOptimizerModule):
+class BatchedFusedEmbedding(BaseBatchedEmbedding[torch.Tensor], FusedOptimizerModule):
     def __init__(
         self,
         config: GroupedEmbeddingConfig,
         pg: Optional[dist.ProcessGroup] = None,
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__(config, pg, device)
@@ -630,15 +645,15 @@
             param._in_backward_optimizers = [EmptyFusedOptimizer()]
             yield name, param
 
     def flush(self) -> None:
         self._emb_module.flush()
 
 
-class BatchedDenseEmbedding(BaseBatchedEmbedding):
+class BatchedDenseEmbedding(BaseBatchedEmbedding[torch.Tensor]):
     def __init__(
         self,
         config: GroupedEmbeddingConfig,
         pg: Optional[dist.ProcessGroup] = None,
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__(config, pg, device)
@@ -680,15 +695,15 @@
             [config.name for config in self._config.embedding_tables]
         )
         yield append_prefix(prefix, f"{combined_key}.weight"), cast(
             nn.Parameter, self._emb_module.weights
         )
 
 
-class BaseBatchedEmbeddingBag(BaseEmbedding):
+class BaseBatchedEmbeddingBag(BaseEmbedding, Generic[SplitWeightType]):
     def __init__(
         self,
         config: GroupedEmbeddingConfig,
         pg: Optional[dist.ProcessGroup] = None,
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__()
@@ -726,16 +741,16 @@
         for (rows, emb_dim, weight_init_min, weight_init_max, param) in zip(
             self._local_rows,
             self._local_cols,
             self._weight_init_mins,
             self._weight_init_maxs,
             self.split_embedding_weights(),
         ):
-            assert param.shape == (rows, emb_dim)
-            param.data.uniform_(
+            assert param.shape == (rows, emb_dim)  # pyre-ignore[16]
+            param.data.uniform_(  # pyre-ignore[16]
                 weight_init_min,
                 weight_init_max,
             )
 
     def forward(self, features: KeyedJaggedTensor) -> torch.Tensor:
         weights = features.weights_or_none()
         if weights is not None and not torch.is_floating_point(weights):
@@ -752,21 +767,22 @@
         destination: Optional[Dict[str, Any]] = None,
         prefix: str = "",
         keep_vars: bool = False,
     ) -> Dict[str, Any]:
         self.flush()
         return get_state_dict(
             self._config.embedding_tables,
+            # pyre-ignore
             self.split_embedding_weights(),
             self._pg,
             destination,
             prefix,
         )
 
-    def split_embedding_weights(self) -> List[torch.Tensor]:
+    def split_embedding_weights(self) -> List[SplitWeightType]:
         return self.emb_module.split_embedding_weights()
 
     @property
     @abc.abstractmethod
     def emb_module(
         self,
     ) -> Union[
@@ -804,15 +820,17 @@
         For a single table with multiple shards (i.e CW) these are combined into one table/weight.
         Used in composability.
         """
         for name, param in self._param_per_table.items():
             yield name, param
 
 
-class BatchedFusedEmbeddingBag(BaseBatchedEmbeddingBag, FusedOptimizerModule):
+class BatchedFusedEmbeddingBag(
+    BaseBatchedEmbeddingBag[torch.Tensor], FusedOptimizerModule
+):
     def __init__(
         self,
         config: GroupedEmbeddingConfig,
         pg: Optional[dist.ProcessGroup] = None,
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__(config, pg, device)
@@ -898,15 +916,15 @@
             param._in_backward_optimizers = [EmptyFusedOptimizer()]
             yield name, param
 
     def flush(self) -> None:
         self._emb_module.flush()
 
 
-class BatchedDenseEmbeddingBag(BaseBatchedEmbeddingBag):
+class BatchedDenseEmbeddingBag(BaseBatchedEmbeddingBag[torch.Tensor]):
     def __init__(
         self,
         config: GroupedEmbeddingConfig,
         pg: Optional[dist.ProcessGroup] = None,
         device: Optional[torch.device] = None,
     ) -> None:
         super().__init__(config, pg, device)
```

## torchrec/distributed/embedding.py

```diff
@@ -499,14 +499,16 @@
                     table_name = key[: -len(".weight")]
                     self._model_parallel_name_to_local_shards[table_name].extend(
                         v.local_shards()
                     )
             for (
                 table_name,
                 tbe_slice,
+                # pyre-fixme[16]: Item `Tensor` of `Union[Tensor, Module]` has no
+                #  attribute `named_parameters_by_table`.
             ) in lookup.named_parameters_by_table():
                 self.embeddings[table_name].register_parameter("weight", tbe_slice)
         for (
             table_name,
             local_shards,
         ) in self._model_parallel_name_to_local_shards.items():
             # for shards that don't exist on this rank, register with empty tensor
@@ -702,14 +704,16 @@
         for odist, embeddings, sharding_ctx in zip(
             self._output_dists,
             output,
             ctx.sharding_contexts,
         ):
             awaitables_per_sharding.append(odist(embeddings, sharding_ctx))
             features_before_all2all_per_sharding.append(
+                # pyre-fixme[6]: For 1st argument expected `KeyedJaggedTensor` but
+                #  got `Optional[KeyedJaggedTensor]`.
                 sharding_ctx.features_before_input_dist
             )
         return EmbeddingCollectionAwaitable(
             awaitables_per_sharding=awaitables_per_sharding,
             features_per_sharding=features_before_all2all_per_sharding,
             embedding_names_per_sharding=self._embedding_names_per_sharding,
             need_indices=self._need_indices,
@@ -732,14 +736,16 @@
                 -1, features.stride()
             )
             embedding_dim = self._embedding_dim_for_sharding_type(sharding_type)
             awaitables_per_sharding.append(
                 odist(lookup(features).view(-1, embedding_dim), sharding_ctx)
             )
             features_before_all2all_per_sharding.append(
+                # pyre-fixme[6]: For 1st argument expected `KeyedJaggedTensor` but
+                #  got `Optional[KeyedJaggedTensor]`.
                 sharding_ctx.features_before_input_dist
             )
         return EmbeddingCollectionAwaitable(
             awaitables_per_sharding=awaitables_per_sharding,
             features_per_sharding=features_before_all2all_per_sharding,
             embedding_names_per_sharding=self._embedding_names_per_sharding,
             need_indices=self._need_indices,
```

## torchrec/distributed/embedding_kernel.py

```diff
@@ -4,15 +4,15 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import abc
 import logging
 from collections import defaultdict, OrderedDict
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import torch
 import torch.distributed as dist
 from torch import nn
 from torchrec.distributed.embedding_types import (
     EmbeddingComputeKernel,
     GroupedEmbeddingConfig,
@@ -50,14 +50,15 @@
 
 def get_state_dict(
     embedding_tables: List[ShardedEmbeddingTable],
     params: Union[
         nn.ModuleList,
         List[Union[nn.Module, torch.Tensor]],
         List[torch.Tensor],
+        List[Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]],
     ],
     pg: Optional[dist.ProcessGroup] = None,
     destination: Optional[Dict[str, Any]] = None,
     prefix: str = "",
 ) -> Dict[str, Any]:
     if destination is None:
         destination = OrderedDict()
@@ -72,35 +73,56 @@
     key_to_global_metadata: Dict[str, ShardedTensorMetadata] = {}
 
     def get_key_from_embedding_table(embedding_table: ShardedEmbeddingTable) -> str:
         return prefix + f"{embedding_table.name}.weight"
 
     for embedding_table, param in zip(embedding_tables, params):
         key = get_key_from_embedding_table(embedding_table)
-        assert embedding_table.local_rows == param.size(0)
-        if embedding_table.compute_kernel not in [
+        is_quant = embedding_table.compute_kernel in [
             EmbeddingComputeKernel.QUANT,
             EmbeddingComputeKernel.QUANT_UVM,
             EmbeddingComputeKernel.QUANT_UVM_CACHING,
-        ]:
-            assert embedding_table.local_cols == param.size(1)
-        # for inference there is no pg, all tensors are local
+        ]
+        qscale = None
+        qbias = None
+        if is_quant:
+            # For QUANT* param is Tuple[torch.Tensor, Optional[torch.Tensor]] where first argument is the weight table, the second is optional quantization extra information, depending on quantization type. e.g. for fbgemm rowwise quantization this is scale and shift for each row.
+            assert isinstance(param, tuple)
+            qscale = param[1]
+            qbias = param[2]
+            param = param[0]
+
+        assert embedding_table.local_rows == param.size(0)  # pyre-ignore[16]
+
+        if qscale is not None:
+            assert embedding_table.local_cols == param.size(1)  # pyre-ignore[16]
+
         if embedding_table.global_metadata is not None and pg is not None:
             # set additional field of sharded tensor based on local tensor properties
-            embedding_table.global_metadata.tensor_properties.dtype = param.dtype
+            embedding_table.global_metadata.tensor_properties.dtype = (
+                param.dtype  # pyre-ignore[16]
+            )
             embedding_table.global_metadata.tensor_properties.requires_grad = (
-                param.requires_grad
+                param.requires_grad  # pyre-ignore[16]
             )
             key_to_global_metadata[key] = embedding_table.global_metadata
 
             key_to_local_shards[key].append(
+                # pyre-fixme[6]: For 1st argument expected `Tensor` but got
+                #  `Union[Module, Tensor]`.
+                # pyre-fixme[6]: For 2nd argument expected `ShardMetadata` but got
+                #  `Optional[ShardMetadata]`.
                 Shard(param, embedding_table.local_metadata)
             )
         else:
             destination[key] = param
+            if qscale is not None:
+                destination[f"{key}_qscale"] = qscale
+            if qbias is not None:
+                destination[f"{key}_qbias"] = qbias
 
     if pg is not None:
         # Populate the remaining destinations that have a global metadata
         for key in key_to_local_shards:
             global_metadata = key_to_global_metadata[key]
             destination[
                 key
```

## torchrec/distributed/embedding_lookup.py

```diff
@@ -444,15 +444,17 @@
         fused_params: Optional[Dict[str, Any]] = None,
     ) -> None:
         # TODO rename to _create_embedding_kernel
         def _create_lookup(
             config: GroupedEmbeddingConfig,
             device: Optional[torch.device] = None,
             fused_params: Optional[Dict[str, Any]] = None,
-        ) -> BaseBatchedEmbedding:
+        ) -> BaseBatchedEmbedding[
+            Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]
+        ]:
             return QuantBatchedEmbedding(
                 config=config,
                 device=device,
                 fused_params=fused_params,
             )
 
         super().__init__()
@@ -561,15 +563,17 @@
         fused_params: Optional[Dict[str, Any]] = None,
     ) -> None:
         # TODO rename to _create_embedding_kernel
         def _create_lookup(
             config: GroupedEmbeddingConfig,
             device: Optional[torch.device] = None,
             fused_params: Optional[Dict[str, Any]] = None,
-        ) -> BaseBatchedEmbeddingBag:
+        ) -> BaseBatchedEmbeddingBag[
+            Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]
+        ]:
             return QuantBatchedEmbeddingBag(
                 config=config,
                 device=device,
                 fused_params=fused_params,
             )
 
         super().__init__()
```

## torchrec/distributed/embedding_sharding.py

```diff
@@ -358,30 +358,60 @@
             splits_list = self._splits_awaitable.wait()
             splits_per_awaitable = _split(splits_list, self._lengths)
         else:
             splits_per_awaitable = [[] for _ in range(len(self._lengths))]
         tensors_awaitables = []
         for splits, awaitable in zip(splits_per_awaitable, self._awaitables):
             if not splits:  # NoWait
+                # pyre-fixme[16]: Item `KJTSplitsAllToAllMeta` of
+                #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                #  KJTSplitsAllToAllMeta]` has no attribute `wait`.
                 tensors_awaitables.append(awaitable.wait())
                 continue
             output_splits = splits[:-1]
             batch_size_per_rank = splits[-1]
             tensors_awaitables.append(
                 KJTAllToAllTensorsAwaitable(
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `pg`.
                     pg=awaitable.pg,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `input`.
                     input=awaitable.input,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `splits`.
                     splits=awaitable.splits,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `input_splits`.
                     input_splits=awaitable.input_splits,
                     output_splits=output_splits,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `input_tensors`.
                     input_tensors=awaitable.input_tensors,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `labels`.
                     labels=awaitable.labels,
                     batch_size_per_rank=batch_size_per_rank,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `keys`.
                     keys=awaitable.keys,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `device`.
                     device=awaitable.device,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `stagger`.
                     stagger=awaitable.stagger,
                 )
             )
         output = []
         awaitables_per_output = _split(tensors_awaitables, self._output_lengths)
         for awaitables, ctx in zip(awaitables_per_output, self._contexts):
             _set_sharding_context(awaitables, ctx)
```

## torchrec/distributed/embeddingbag.py

```diff
@@ -499,14 +499,16 @@
                     table_name = key[: -len(".weight")]
                     self._model_parallel_name_to_local_shards[table_name].extend(
                         v.local_shards()
                     )
             for (
                 table_name,
                 tbe_slice,
+                # pyre-fixme[16]: Item `Tensor` of `Union[Tensor, Module]` has no
+                #  attribute `named_parameters_by_table`.
             ) in lookup.named_parameters_by_table():
                 self.embedding_bags[table_name].register_parameter("weight", tbe_slice)
         for (
             table_name,
             local_shards,
         ) in self._model_parallel_name_to_local_shards.items():
             # for shards that don't exist on this rank, register with empty tensor
```

## torchrec/distributed/fp_embeddingbag.py

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Dict, Iterator, List, Optional, Type
+from typing import Dict, Iterator, List, Optional, Type, Union
 
 import torch
+from torch import nn
 
 from torchrec.distributed.embedding_types import (
     BaseEmbeddingSharder,
     KJTList,
     ShardedEmbeddingModule,
 )
 from torchrec.distributed.embeddingbag import (
@@ -24,14 +25,15 @@
     LazyAwaitable,
     ParameterSharding,
     QuantizedCommCodecs,
     ShardingEnv,
     ShardingType,
 )
 from torchrec.distributed.utils import append_prefix
+from torchrec.modules.feature_processor_ import FeatureProcessorsCollection
 from torchrec.modules.fp_embedding_modules import (
     apply_feature_processors_to_kjt,
     FeatureProcessedEmbeddingBagCollection,
 )
 from torchrec.sparse.jagged_tensor import KeyedJaggedTensor, KeyedTensor
 
 
@@ -58,61 +60,64 @@
                 module._embedding_bag_collection,
                 table_name_to_parameter_sharding,
                 env=env,
                 device=device,
             )
         )
 
-        self._feature_processors = torch.nn.ModuleDict(
-            {key: fp.to(device) for key, fp in module._feature_processors.items()}
-        )
+        self._feature_processors: Union[nn.ModuleDict, FeatureProcessorsCollection]
+        if isinstance(module._feature_processors, FeatureProcessorsCollection):
+            self._feature_processors = module._feature_processors.to(device)
+        else:
+            self._feature_processors = torch.nn.ModuleDict(
+                {key: fp.to(device) for key, fp in module._feature_processors.items()}
+            )
 
     # pyre-ignore
     def input_dist(
         self, ctx: EmbeddingBagCollectionContext, features: KeyedJaggedTensor
     ) -> Awaitable[Awaitable[KJTList]]:
         return self._embedding_bag_collection.input_dist(ctx, features)
 
+    def apply_feature_processors_to_kjt_list(self, dist_input: KJTList) -> KJTList:
+        if isinstance(self._feature_processors, FeatureProcessorsCollection):
+            return KJTList(
+                [self._feature_processors(features) for features in dist_input]
+            )
+        else:
+            return KJTList(
+                [
+                    apply_feature_processors_to_kjt(
+                        features,
+                        self._feature_processors,
+                    )
+                    for features in dist_input
+                ]
+            )
+
     def compute(
         self,
         ctx: EmbeddingBagCollectionContext,
         dist_input: KJTList,
     ) -> List[torch.Tensor]:
 
-        fp_features = KJTList(
-            [
-                apply_feature_processors_to_kjt(
-                    features,
-                    self._feature_processors,
-                )
-                for features in dist_input
-            ]
-        )
-
+        fp_features = self.apply_feature_processors_to_kjt_list(dist_input)
         return self._embedding_bag_collection.compute(ctx, fp_features)
 
     def output_dist(
         self,
         ctx: EmbeddingBagCollectionContext,
         output: List[torch.Tensor],
     ) -> LazyAwaitable[KeyedTensor]:
         return self._embedding_bag_collection.output_dist(ctx, output)
 
     def compute_and_output_dist(
         self, ctx: EmbeddingBagCollectionContext, input: KJTList
     ) -> LazyAwaitable[KeyedTensor]:
-        fp_features = KJTList(
-            [
-                apply_feature_processors_to_kjt(
-                    features,
-                    self._feature_processors,
-                )
-                for features in input
-            ]
-        )
+        fp_features = self.apply_feature_processors_to_kjt_list(input)
         return self._embedding_bag_collection.compute_and_output_dist(ctx, fp_features)
 
     def create_context(self) -> EmbeddingBagCollectionContext:
         return self._embedding_bag_collection.create_context()
 
     def sharded_parameter_names(self, prefix: str = "") -> Iterator[str]:
         for fqn, _ in self.named_parameters():
```

## torchrec/distributed/fused_embedding.py

```diff
@@ -67,15 +67,14 @@
                     module=lookup,
                     device_ids=[device],
                     process_group=env.process_group,
                     gradient_as_bucket_view=True,
                     broadcast_buffers=False,
                     static_graph=True,
                 )
-                # pyre-ignore
                 self._lookups[index]._register_fused_optim(
                     optimizer_type, **optimizer_kwargs
                 )
                 # TODO - We need a way to get this optimizer back (and add to optims) so it
                 # can be checkpointed.
                 # We need to ensure that a checkpoint from DDP and a checkpoint from a
                 # model parallel version are compatible.
```

## torchrec/distributed/fused_params.py

```diff
@@ -11,14 +11,17 @@
 
 from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     IntNBitTableBatchedEmbeddingBagsCodegen,
 )
 from torchrec.distributed.embedding_types import GroupedEmbeddingConfig
 
 FUSED_PARAM_REGISTER_TBE_BOOL: str = "__register_tbes_in_named_modules"
+FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS: str = (
+    "__register_quant_state_dict_split_scale_bias"
+)
 
 
 class TBEToRegisterMixIn:
     def get_tbes_to_register(
         self,
     ) -> Dict[IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig]:
         raise NotImplementedError
@@ -38,18 +41,30 @@
     return (
         fused_params
         and FUSED_PARAM_REGISTER_TBE_BOOL in fused_params
         and fused_params[FUSED_PARAM_REGISTER_TBE_BOOL]
     )
 
 
+def is_fused_param_quant_state_dict_split_scale_bias(
+    fused_params: Optional[Dict[str, Any]]
+) -> bool:
+    return (
+        fused_params
+        and FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS in fused_params
+        and fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS]
+    )
+
+
 def tbe_fused_params(
     fused_params: Optional[Dict[str, Any]]
 ) -> Optional[Dict[str, Any]]:
     if not fused_params:
         return None
 
     fused_params_for_tbe = dict(fused_params)
     if FUSED_PARAM_REGISTER_TBE_BOOL in fused_params_for_tbe:
         fused_params_for_tbe.pop(FUSED_PARAM_REGISTER_TBE_BOOL)
+    if FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS in fused_params_for_tbe:
+        fused_params_for_tbe.pop(FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS)
 
     return fused_params_for_tbe
```

## torchrec/distributed/quant_embedding.py

```diff
@@ -25,14 +25,15 @@
     GroupedEmbeddingConfig,
     KJTList,
     ListOfKJTList,
     ShardedEmbeddingModule,
     ShardingType,
 )
 from torchrec.distributed.fused_params import (
+    FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
     get_tbes_to_register_from_iterable,
     is_fused_param_register_tbe,
 )
 from torchrec.distributed.sharding.sequence_sharding import InferSequenceShardingContext
 from torchrec.distributed.sharding.tw_sequence_sharding import (
     InferTwSequenceEmbeddingSharding,
 )
@@ -40,14 +41,15 @@
 from torchrec.modules.embedding_configs import (
     data_type_to_sparse_type,
     dtype_to_data_type,
     EmbeddingConfig,
 )
 from torchrec.quant.embedding_modules import (
     EmbeddingCollection as QuantEmbeddingCollection,
+    MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
 )
 from torchrec.sparse.jagged_tensor import JaggedTensor, KeyedJaggedTensor
 from torchrec.streamable import Multistreamable
 
 torch.fx.wrap("len")
 
 try:
@@ -206,28 +208,38 @@
             self.embeddings[table.name] = torch.nn.Module()
 
         for _sharding_type, lookup in zip(
             self._sharding_type_to_sharding.keys(), self._lookups
         ):
             lookup_state_dict = lookup.state_dict()
             for key in lookup_state_dict:
-                if not key.endswith(".weight"):
+                if key.endswith(".weight"):
+                    table_name = key[: -len(".weight")]
+                    # Register as buffer because this is an inference model, and can potentially use uint8 types.
+                    self.embeddings[table_name].register_buffer(
+                        "weight", lookup_state_dict[key]
+                    )
+                elif key.endswith(".weight_qscale"):
+                    table_name = key[: -len(".weight_qscale")]
+                    self.embeddings[table_name].register_buffer(
+                        "weight_qscale", lookup_state_dict[key]
+                    )
+                elif key.endswith(".weight_qbias"):
+                    table_name = key[: -len(".weight_qbias")]
+                    self.embeddings[table_name].register_buffer(
+                        "weight_qbias", lookup_state_dict[key]
+                    )
+                else:
                     continue
-                table_name = key[: -len(".weight")]
-                # Register as buffer because this is an inference model, and can potentially use uint8 types.
-                self.embeddings[table_name].register_buffer(
-                    "weight", lookup_state_dict[key]
-                )
 
         # Optional registration of TBEs for model post processing utilities
         if is_fused_param_register_tbe(fused_params):
             tbes: Dict[
                 IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig
             ] = get_tbes_to_register_from_iterable(self._lookups)
-
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(tbes.keys())
 
     def _create_input_dist(
         self,
         input_feature_names: List[str],
         device: torch.device,
         input_dist_device: Optional[torch.device] = None,
@@ -329,14 +341,16 @@
         features_per_sharding: List[List[KeyedJaggedTensor]] = []
         for odist, embeddings, sharding_ctx in zip(
             self._output_dists,
             output,
             ctx.sharding_contexts,
         ):
             emb_per_sharding.append(odist.forward(embeddings, sharding_ctx))
+            # pyre-fixme[6]: For 1st argument expected `List[KeyedJaggedTensor]` but
+            #  got `Optional[KJTList]`.
             features_per_sharding.append(sharding_ctx.features)
 
         return output_jt_dict(
             emb_per_sharding, features_per_sharding, self._need_indices
         )
 
     # pyre-ignore
@@ -380,12 +394,15 @@
         env: ShardingEnv,
         device: Optional[torch.device] = None,
     ) -> ShardedQuantEmbeddingCollection:
         fused_params = self.fused_params if self.fused_params else {}
         fused_params["output_dtype"] = data_type_to_sparse_type(
             dtype_to_data_type(module.output_dtype())
         )
+        fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS] = getattr(
+            module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+        )
         return ShardedQuantEmbeddingCollection(module, params, env, fused_params)
 
     @property
     def module_type(self) -> Type[QuantEmbeddingCollection]:
         return QuantEmbeddingCollection
```

## torchrec/distributed/quant_embedding_kernel.py

```diff
@@ -26,14 +26,15 @@
 )
 from torchrec.distributed.embedding_kernel import BaseEmbedding
 from torchrec.distributed.embedding_types import (
     compute_kernel_to_embedding_location,
     GroupedEmbeddingConfig,
 )
 from torchrec.distributed.fused_params import (
+    is_fused_param_quant_state_dict_split_scale_bias,
     is_fused_param_register_tbe,
     tbe_fused_params,
     TBEToRegisterMixIn,
 )
 from torchrec.distributed.utils import append_prefix
 from torchrec.modules.embedding_configs import (
     DATA_TYPE_NUM_BITS,
@@ -109,15 +110,20 @@
         quant_weight = quantized_weights[:, :-4]
         scale_shift = quantized_weights[:, -4:]
 
         quant_weight_list.append((quant_weight, scale_shift))
     return quant_weight_list
 
 
-class QuantBatchedEmbeddingBag(BaseBatchedEmbeddingBag, TBEToRegisterMixIn):
+class QuantBatchedEmbeddingBag(
+    BaseBatchedEmbeddingBag[
+        Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]
+    ],
+    TBEToRegisterMixIn,
+):
     def __init__(
         self,
         config: GroupedEmbeddingConfig,
         pg: Optional[dist.ProcessGroup] = None,
         device: Optional[torch.device] = None,
         fused_params: Optional[Dict[str, Any]] = None,
     ) -> None:
@@ -129,29 +135,30 @@
                 managed.append(
                     compute_kernel_to_embedding_location(table.compute_kernel)
                 )
             else:
                 managed.append(EmbeddingLocation.HOST)
         self._config: GroupedEmbeddingConfig = config
         self._emb_module_registered: bool = is_fused_param_register_tbe(fused_params)
+        self._quant_state_dict_split_scale_bias: bool = (
+            is_fused_param_quant_state_dict_split_scale_bias(fused_params)
+        )
         self._emb_module: IntNBitTableBatchedEmbeddingBagsCodegen = IntNBitTableBatchedEmbeddingBagsCodegen(
             embedding_specs=[
                 (
                     table.name,
                     local_rows,
-                    # TODO(ivankobzarev):
-                    # _copy_config makes local_cols be aligned with TBE specific alignment and local_cols become not equal to table.embedding_dim, while logical size is table.embedding_dim.
-                    # Using logical size table.embedding_dim here for now.
-                    # This Needed to be changed to local_cols to support CW sharding in future when logical cols number != table.embedding_dim.
-                    table.embedding_dim,
+                    local_cols
+                    if self._quant_state_dict_split_scale_bias
+                    else table.embedding_dim,
                     data_type_to_sparse_type(config.data_type),
                     location,
                 )
-                for local_rows, table, location in zip(
-                    self._local_rows, config.embedding_tables, managed
+                for local_rows, local_cols, table, location in zip(
+                    self._local_rows, self._local_cols, config.embedding_tables, managed
                 )
             ],
             device=device,
             pooling_mode=self._pooling,
             feature_table_map=self._feature_table_map,
             row_alignment=16,
             uvm_host_mapped=True,  # Use cudaHostAlloc for UVM CACHING to fix imbalance numa memory issue
@@ -194,25 +201,38 @@
 
     def named_buffers(
         self, prefix: str = "", recurse: bool = True, remove_duplicate: bool = True
     ) -> Iterator[Tuple[str, torch.Tensor]]:
         assert (
             remove_duplicate
         ), "remove_duplicate=False not supported in QuantBatchedEmbeddingBag.named_split_embedding_weights"
-        for config, weight in zip(
+        for config, (weight, weight_qscale, weight_qbias) in zip(
             self._config.embedding_tables,
-            self.emb_module.split_embedding_weights(),
+            self.emb_module.split_embedding_weights_with_scale_bias(
+                split_scale_bias_mode=2
+                if self._quant_state_dict_split_scale_bias
+                else 0
+            ),
         ):
-            yield append_prefix(prefix, f"{config.name}.weight"), weight[0]
+            yield append_prefix(prefix, f"{config.name}.weight"), weight
+            if self._quant_state_dict_split_scale_bias:
+                yield append_prefix(
+                    prefix, f"{config.name}.weight_qscale"
+                ), weight_qscale
+                yield append_prefix(prefix, f"{config.name}.weight_qbias"), weight_qbias
 
-    def split_embedding_weights(self) -> List[torch.Tensor]:
+    def split_embedding_weights(
+        self,
+    ) -> List[Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]]:
         return [
-            weight
-            for weight, _ in self.emb_module.split_embedding_weights(
-                split_scale_shifts=False
+            (weight, qscale, qbias)
+            for weight, qscale, qbias in self.emb_module.split_embedding_weights_with_scale_bias(
+                split_scale_bias_mode=2
+                if self._quant_state_dict_split_scale_bias
+                else 0
             )
         ]
 
     @classmethod
     def from_float(cls, module: BaseEmbedding) -> "QuantBatchedEmbeddingBag":
         assert hasattr(
             module, "qconfig"
@@ -236,15 +256,20 @@
         # pyre-ignore
         quant_weight_list = _quantize_weight(state_dict, data_type)
         ret.emb_module.assign_embedding_weights(quant_weight_list)
 
         return ret
 
 
-class QuantBatchedEmbedding(BaseBatchedEmbedding, TBEToRegisterMixIn):
+class QuantBatchedEmbedding(
+    BaseBatchedEmbedding[
+        Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]
+    ],
+    TBEToRegisterMixIn,
+):
     def __init__(
         self,
         config: GroupedEmbeddingConfig,
         pg: Optional[dist.ProcessGroup] = None,
         device: Optional[torch.device] = None,
         fused_params: Optional[Dict[str, Any]] = None,
     ) -> None:
@@ -256,25 +281,30 @@
                 managed.append(
                     compute_kernel_to_embedding_location(table.compute_kernel)
                 )
             else:
                 managed.append(EmbeddingLocation.HOST)
         self._config: GroupedEmbeddingConfig = config
         self._emb_module_registered: bool = is_fused_param_register_tbe(fused_params)
+        self._quant_state_dict_split_scale_bias: bool = (
+            is_fused_param_quant_state_dict_split_scale_bias(fused_params)
+        )
         self._emb_module: IntNBitTableBatchedEmbeddingBagsCodegen = IntNBitTableBatchedEmbeddingBagsCodegen(
             embedding_specs=[
                 (
                     table.name,
                     local_rows,
-                    table.embedding_dim,
+                    local_cols
+                    if self._quant_state_dict_split_scale_bias
+                    else table.embedding_dim,
                     data_type_to_sparse_type(config.data_type),
                     location,
                 )
-                for local_rows, table, location in zip(
-                    self._local_rows, config.embedding_tables, managed
+                for local_rows, local_cols, table, location in zip(
+                    self._local_rows, self._local_cols, config.embedding_tables, managed
                 )
             ],
             device=device,
             pooling_mode=PoolingMode.NONE,
             feature_table_map=self._feature_table_map,
             row_alignment=16,
             uvm_host_mapped=True,  # Use cudaHostAlloc for UVM CACHING to fix imbalance numa memory issue
@@ -290,19 +320,23 @@
         return self._emb_module
 
     def get_tbes_to_register(
         self,
     ) -> Dict[IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig]:
         return {self._emb_module: self._config}
 
-    def split_embedding_weights(self) -> List[torch.Tensor]:
+    def split_embedding_weights(
+        self,
+    ) -> List[Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]]:
         return [
-            weight
-            for weight, _ in self.emb_module.split_embedding_weights(
-                split_scale_shifts=False
+            (weight, qscale, qbias)
+            for weight, qscale, qbias in self.emb_module.split_embedding_weights_with_scale_bias(
+                split_scale_bias_mode=2
+                if self._quant_state_dict_split_scale_bias
+                else 0
             )
         ]
 
     def forward(self, features: KeyedJaggedTensor) -> torch.Tensor:
         if self._emb_module_registered:
             return self.emb_module(
                 indices=features.values().int(),
@@ -313,19 +347,28 @@
                 indices=features.values().int(),
                 offsets=features.offsets().int(),
             )
 
     def named_buffers(
         self, prefix: str = "", recurse: bool = True, remove_duplicate: bool = True
     ) -> Iterator[Tuple[str, torch.Tensor]]:
-        for config, weight in zip(
+        for config, (weight, weight_qscale, weight_qbias) in zip(
             self._config.embedding_tables,
-            self.emb_module.split_embedding_weights(),
+            self.emb_module.split_embedding_weights_with_scale_bias(
+                split_scale_bias_mode=2
+                if self._quant_state_dict_split_scale_bias
+                else 0
+            ),
         ):
-            yield append_prefix(prefix, f"{config.name}.weight"), weight[0]
+            yield append_prefix(prefix, f"{config.name}.weight"), weight
+            if self._quant_state_dict_split_scale_bias:
+                yield append_prefix(
+                    prefix, f"{config.name}.weight_qscale"
+                ), weight_qscale
+                yield append_prefix(prefix, f"{config.name}.weight_qbias"), weight_qbias
 
     @classmethod
     def from_float(cls, module: BaseEmbedding) -> "QuantBatchedEmbedding":
         assert hasattr(
             module, "qconfig"
         ), "BaseEmbedding input float module must have qconfig defined"
```

## torchrec/distributed/quant_embeddingbag.py

```diff
@@ -25,14 +25,15 @@
     ShardedEmbeddingModule,
 )
 from torchrec.distributed.embeddingbag import (
     construct_output_kt,
     create_sharding_infos_by_sharding,
 )
 from torchrec.distributed.fused_params import (
+    FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
     get_tbes_to_register_from_iterable,
     is_fused_param_register_tbe,
 )
 from torchrec.distributed.sharding.tw_sharding import InferTwEmbeddingSharding
 from torchrec.distributed.types import (
     NullShardedModuleContext,
     NullShardingContext,
@@ -44,14 +45,15 @@
     data_type_to_sparse_type,
     dtype_to_data_type,
     EmbeddingBagConfig,
 )
 from torchrec.modules.embedding_modules import EmbeddingBagCollectionInterface
 from torchrec.quant.embedding_modules import (
     EmbeddingBagCollection as QuantEmbeddingBagCollection,
+    MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
 )
 from torchrec.sparse.jagged_tensor import KeyedJaggedTensor, KeyedTensor
 
 torch.fx.wrap("len")
 
 
 def create_infer_embedding_bag_sharding(
@@ -132,21 +134,32 @@
             self.embedding_bags[table.name] = torch.nn.Module()
 
         for _sharding_type, lookup in zip(
             self._sharding_type_to_sharding.keys(), self._lookups
         ):
             lookup_state_dict = lookup.state_dict()
             for key in lookup_state_dict:
-                if not key.endswith(".weight"):
+                if key.endswith(".weight"):
+                    table_name = key[: -len(".weight")]
+                    # Register as buffer because this is an inference model, and can potentially use uint8 types.
+                    self.embedding_bags[table_name].register_buffer(
+                        "weight", lookup_state_dict[key]
+                    )
+                elif key.endswith("weight_qscale"):
+                    table_name = key[: -len(".weight_qscale")]
+                    self.embedding_bags[table_name].register_buffer(
+                        "weight_qscale", lookup_state_dict[key]
+                    )
+                elif key.endswith("weight_qbias"):
+                    table_name = key[: -len(".weight_qbias")]
+                    self.embedding_bags[table_name].register_buffer(
+                        "weight_qbias", lookup_state_dict[key]
+                    )
+                else:
                     continue
-                table_name = key[: -len(".weight")]
-                # Register as buffer because this is an inference model, and can potentially use uint8 types.
-                self.embedding_bags[table_name].register_buffer(
-                    "weight", lookup_state_dict[key]
-                )
 
         # Optional registration of TBEs for model post processing utilities
         if is_fused_param_register_tbe(fused_params):
             tbes: Dict[
                 IntNBitTableBatchedEmbeddingBagsCodegen, GroupedEmbeddingConfig
             ] = get_tbes_to_register_from_iterable(self._lookups)
 
@@ -287,12 +300,15 @@
         env: ShardingEnv,
         device: Optional[torch.device] = None,
     ) -> ShardedQuantEmbeddingBagCollection:
         fused_params = self.fused_params if self.fused_params else {}
         fused_params["output_dtype"] = data_type_to_sparse_type(
             dtype_to_data_type(module.output_dtype())
         )
+        fused_params[FUSED_PARAM_QUANT_STATE_DICT_SPLIT_SCALE_BIAS] = getattr(
+            module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+        )
         return ShardedQuantEmbeddingBagCollection(module, params, env, fused_params)
 
     @property
     def module_type(self) -> Type[QuantEmbeddingBagCollection]:
         return QuantEmbeddingBagCollection
```

## torchrec/distributed/train_pipeline.py

```diff
@@ -296,30 +296,60 @@
             splits_list = self._splits_awaitable.wait()
             splits_per_awaitable = _split(splits_list, self._lengths)
         else:
             splits_per_awaitable = [[] for _ in range(len(self._lengths))]
         tensors_awaitables = []
         for splits, awaitable in zip(splits_per_awaitable, self._awaitables):
             if not splits:  # NoWait
+                # pyre-fixme[16]: Item `KJTSplitsAllToAllMeta` of
+                #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                #  KJTSplitsAllToAllMeta]` has no attribute `wait`.
                 tensors_awaitables.append(awaitable.wait())
                 continue
             output_splits = splits[:-1]
             batch_size_per_rank = splits[-1]
             tensors_awaitables.append(
                 KJTAllToAllTensorsAwaitable(
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `pg`.
                     pg=awaitable.pg,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `input`.
                     input=awaitable.input,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `splits`.
                     splits=awaitable.splits,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `input_splits`.
                     input_splits=awaitable.input_splits,
                     output_splits=output_splits,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `input_tensors`.
                     input_tensors=awaitable.input_tensors,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `labels`.
                     labels=awaitable.labels,
                     batch_size_per_rank=batch_size_per_rank,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `keys`.
                     keys=awaitable.keys,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `device`.
                     device=awaitable.device,
+                    # pyre-fixme[16]: Item `Awaitable` of
+                    #  `Union[Awaitable[Awaitable[KeyedJaggedTensor]],
+                    #  KJTSplitsAllToAllMeta]` has no attribute `stagger`.
                     stagger=awaitable.stagger,
                 )
             )
         output = []
         awaitables_per_output = _split(tensors_awaitables, self._output_lengths)
         for awaitables, ctx in zip(awaitables_per_output, self._contexts):
             _set_sharding_context(awaitables, ctx)
@@ -582,23 +612,31 @@
                 arg = child_node.args[0]
             elif (
                 child_node.op == "call_function"
                 and child_node.target.__module__ == "builtins"
                 # pyre-ignore[16]
                 and child_node.target.__name__ == "getattr"
             ):
+                # pyre-fixme[6]: For 2nd argument expected `str` but got
+                #  `Union[None, Dict[str, typing.Any], List[typing.Any], Node, bool,
+                #  complex, float, int, range, slice, str, device, dtype, layout,
+                #  memory_format, Tensor, typing.Tuple[typing.Any, ...]]`.
                 arg_info.input_attrs.insert(0, child_node.args[1])
                 arg_info.is_getitems.insert(0, False)
                 arg = child_node.args[0]
             elif (
                 child_node.op == "call_function"
                 and child_node.target.__module__ == "_operator"
                 # pyre-ignore[16]
                 and child_node.target.__name__ == "getitem"
             ):
+                # pyre-fixme[6]: For 2nd argument expected `str` but got
+                #  `Union[None, Dict[str, typing.Any], List[typing.Any], Node, bool,
+                #  complex, float, int, range, slice, str, device, dtype, layout,
+                #  memory_format, Tensor, typing.Tuple[typing.Any, ...]]`.
                 arg_info.input_attrs.insert(0, child_node.args[1])
                 arg_info.is_getitems.insert(0, True)
                 arg = child_node.args[0]
             else:
                 break
     return arg_info_list, num_found
```

## torchrec/distributed/planner/proposers.py

```diff
@@ -216,14 +216,16 @@
                 f"Max proposals allowed: {self._max_proposals}\n"
             )
             return
         sharding_options_by_fqn_indices = [
             range(len(sharding_options))
             for sharding_options in self._sharding_options_by_fqn.values()
         ]
+        # pyre-fixme[8]: Attribute has type `List[List[int]]`; used as
+        #  `List[Tuple[int]]`.
         self._proposals = list(itertools.product(*sharding_options_by_fqn_indices))
 
     def _reset(self) -> None:
         self._sharding_options_by_fqn = {}
         self._proposal_index = 0
         self._proposals = []
```

## torchrec/distributed/test_utils/infer_utils.py

```diff
@@ -4,15 +4,15 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 #!/usr/bin/env python3
 
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import torch
 import torchrec
 from torch import quantization as quant
 from torchrec import EmbeddingCollection, EmbeddingConfig, KeyedJaggedTensor
 from torchrec.distributed.embedding_types import ModuleSharder
 from torchrec.distributed.fused_params import FUSED_PARAM_REGISTER_TBE_BOOL
@@ -34,15 +34,16 @@
     data_type_to_sparse_type,
     dtype_to_data_type,
     EmbeddingBagConfig,
 )
 from torchrec.modules.embedding_modules import EmbeddingBagCollection
 from torchrec.quant.embedding_modules import (
     EmbeddingCollection as QuantEmbeddingCollection,
-    MODULE_ATTR_REGISTER_TBES_BOOL,
+    quant_prep_enable_quant_state_dict_split_scale_bias_for_types,
+    quant_prep_enable_register_tbes,
 )
 
 
 @dataclass
 class TestModelInfo:
     sparse_device: torch.device
     dense_device: torch.device
@@ -141,21 +142,26 @@
 
 
 def quantize(
     module: torch.nn.Module,
     inplace: bool,
     output_type: torch.dtype = torch.float,
     register_tbes: bool = False,
+    quant_state_dict_split_scale_bias: bool = False,
 ) -> torch.nn.Module:
+    module_types: List[Type[torch.nn.Module]] = [
+        torchrec.modules.embedding_modules.EmbeddingBagCollection,
+        torchrec.modules.embedding_modules.EmbeddingCollection,
+    ]
     if register_tbes:
-        for m in module.modules():
-            if isinstance(
-                m, torchrec.modules.embedding_modules.EmbeddingBagCollection
-            ) or isinstance(m, torchrec.modules.embedding_modules.EmbeddingCollection):
-                setattr(m, MODULE_ATTR_REGISTER_TBES_BOOL, True)
+        quant_prep_enable_register_tbes(module, module_types)
+    if quant_state_dict_split_scale_bias:
+        quant_prep_enable_quant_state_dict_split_scale_bias_for_types(
+            module, module_types
+        )
 
     qconfig = quant.QConfig(
         activation=quant.PlaceholderObserver.with_args(dtype=output_type),
         weight=quant.PlaceholderObserver.with_args(dtype=torch.qint8),
     )
     return quant.quantize_dynamic(
         module,
```

## torchrec/distributed/test_utils/test_model_parallel_base.py

```diff
@@ -4,15 +4,15 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import os
 import unittest
 from collections import defaultdict
-from typing import Callable, cast, Dict, List, Optional, OrderedDict, Tuple
+from typing import Any, Callable, cast, Dict, List, Optional, OrderedDict, Tuple
 
 import numpy as np
 
 import torch
 import torch.nn as nn
 from fbgemm_gpu.split_embedding_configs import EmbOptimType
 from hypothesis import given, settings, strategies as st, Verbosity
@@ -84,14 +84,15 @@
         self,
         world_size: int,
         model_class: TestSparseNNBase,
         embedding_groups: Dict[str, List[str]],
         tables: List[EmbeddingTableConfig],
         sharders: List[ModuleSharder[nn.Module]],
         quantize_callable: Callable[[nn.Module], nn.Module],
+        quantize_callable_kwargs: Dict[str, Any],
         dedup_features_names: Optional[List[str]] = None,
         dedup_tables: Optional[List[EmbeddingTableConfig]] = None,
         weighted_tables: Optional[List[EmbeddingTableConfig]] = None,
         constraints: Optional[Dict[str, ParameterConstraints]] = None,
         generate: ModelInputCallable = ModelInput.generate,
     ) -> None:
         default_rank = 0
@@ -108,15 +109,15 @@
             embedding_groups=embedding_groups,
             world_size=1,  # generate only one copy of feature for inference
             num_float_features=16,
             dense_device=cuda_device,
             sparse_device=cuda_device,
             generate=generate,
         )
-        global_model = quantize_callable(global_model)
+        global_model = quantize_callable(global_model, **quantize_callable_kwargs)
         local_input = _inputs[0][1][default_rank].to(cuda_device)
 
         # Shard model.
         if dedup_features_names:
             local_model = model_class(
                 tables=cast(
                     List[BaseEmbeddingConfig],
@@ -137,25 +138,25 @@
                 ),
                 weighted_tables=cast(List[BaseEmbeddingConfig], weighted_tables),
                 embedding_groups=embedding_groups,
                 dense_device=cuda_device,
                 sparse_device=torch.device("meta"),
                 num_float_features=16,
             )
-        local_model = quantize_callable(local_model)
+        local_model = quantize_callable(local_model, **quantize_callable_kwargs)
 
         planner = EmbeddingShardingPlanner(
             topology=Topology(world_size, "cuda"),
             constraints=constraints,
         )
         plan: ShardingPlan = planner.plan(local_model, sharders)
 
         # Generate a sharded model on a default rank.
         local_model = DistributedModelParallel(
-            local_model,
+            module=local_model,
             env=ShardingEnv.from_local(world_size, default_rank),
             plan=plan,
             sharders=sharders,
             init_data_parallel=False,
         )
 
         # materialize inference sharded model on one device for dense part
```

## torchrec/metrics/rec_metric.py

```diff
@@ -555,30 +555,60 @@
                         weights=weights,
                         **kwargs,
                     )
             else:
                 for task, metric_ in zip(self._tasks, self._metrics_computations):
                     if task.name not in predictions:
                         continue
+                    # pyre-fixme[6]: For 1st argument expected `Union[None,
+                    #  List[typing.Any], int, slice, Tensor, typing.Tuple[typing.Any,
+                    #  ...]]` but got `str`.
                     if torch.numel(predictions[task.name]) == 0:
+                        # pyre-fixme[6]: For 1st argument expected `Union[None,
+                        #  List[typing.Any], int, slice, Tensor,
+                        #  typing.Tuple[typing.Any, ...]]` but got `str`.
                         assert torch.numel(labels[task.name]) == 0
+                        # pyre-fixme[6]: For 1st argument expected `Union[None,
+                        #  List[typing.Any], int, slice, Tensor,
+                        #  typing.Tuple[typing.Any, ...]]` but got `str`.
                         assert weights is None or torch.numel(weights[task.name]) == 0
                         continue
                     task_predictions = (
+                        # pyre-fixme[6]: For 1st argument expected `Union[None,
+                        #  List[typing.Any], int, slice, Tensor,
+                        #  typing.Tuple[typing.Any, ...]]` but got `str`.
                         predictions[task.name].view(1, -1)
+                        # pyre-fixme[6]: For 1st argument expected `Union[None,
+                        #  List[typing.Any], int, slice, Tensor,
+                        #  typing.Tuple[typing.Any, ...]]` but got `str`.
                         if predictions[task.name].dim() == labels[task.name].dim()
                         # predictions[task.name].dim() == labels[task.name].dim() + 1 for multiclass models
+                        # pyre-fixme[6]: For 1st argument expected `Union[None,
+                        #  List[typing.Any], int, slice, Tensor,
+                        #  typing.Tuple[typing.Any, ...]]` but got `str`.
                         else predictions[task.name].view(
-                            1, -1, predictions[task.name].size()[-1]
+                            1,
+                            -1,
+                            predictions[
+                                task.name  # pyre-fixme[6]: For 1st argument expected `Union[None,
+                                #  List[typing.Any], int, slice, Tensor,
+                                #  typing.Tuple[typing.Any, ...]]` but got `str`.
+                            ].size()[-1],
                         )
                     )
+                    # pyre-fixme[6]: For 1st argument expected `Union[None,
+                    #  List[typing.Any], int, slice, Tensor, typing.Tuple[typing.Any,
+                    #  ...]]` but got `str`.
                     task_labels = labels[task.name].view(1, -1)
                     if weights is None:
                         task_weights = self._create_default_weights(task_predictions)
                     else:
+                        # pyre-fixme[6]: For 1st argument expected `Union[None,
+                        #  List[typing.Any], int, slice, Tensor,
+                        #  typing.Tuple[typing.Any, ...]]` but got `str`.
                         task_weights = weights[task.name].view(1, -1)
                     if self._should_validate_update:
                         # has_valid_weights is a tensor with only 1 value corresponding to
                         # whether the weights are valid, i.e. are set to non-zero values for
                         # the task in this update.
                         # If has_valid_update[0] is False, we just ignore this update.
                         has_valid_weights = self._check_nonempty_weights(task_weights)
```

## torchrec/metrics/tower_qps.py

```diff
@@ -256,23 +256,31 @@
                     self._metrics_computations[0].update(
                         predictions=None, labels=labels, weights=None
                     )
             else:
                 for task, metric_ in zip(self._tasks, self._metrics_computations):
                     if task.name not in labels:
                         continue
+                    # pyre-fixme[6]: For 1st argument expected `Union[None,
+                    #  List[typing.Any], int, slice, Tensor, typing.Tuple[typing.Any,
+                    #  ...]]` but got `str`.
                     task_labels = labels[task.name].view(1, -1)
                     if self._should_validate_update:
                         has_valid_weights = torch.ones(
                             1, dtype=torch.bool, device=metric_.has_valid_update.device
                         )
                         if weights is not None and task.name in weights:
                             has_valid_weights = torch.gt(
                                 torch.count_nonzero(
-                                    weights[task.name].view(1, -1), dim=-1
+                                    # pyre-fixme[6]: For 1st argument expected
+                                    #  `Union[None, List[typing.Any], int, slice,
+                                    #  Tensor, typing.Tuple[typing.Any, ...]]` but got
+                                    #  `str`.
+                                    weights[task.name].view(1, -1),
+                                    dim=-1,
                                 ),
                                 0,
                             )
                         if has_valid_weights[0]:
                             metric_.has_valid_update.logical_or_(has_valid_weights)
                         else:
                             continue
```

## torchrec/modules/feature_processor_.py

```diff
@@ -4,19 +4,20 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 #!/usr/bin/env python3
 
 import abc
+from typing import Dict, Optional
 
 import torch
 
 from torch import nn
-from torchrec.sparse.jagged_tensor import JaggedTensor
+from torchrec.sparse.jagged_tensor import JaggedTensor, KeyedJaggedTensor
 
 
 class FeatureProcessor(nn.Module):
     """
     Abstract base class for feature processor.
 
     Args:
@@ -82,7 +83,93 @@
         weighted_features = JaggedTensor(
             values=features.values(),
             lengths=features.lengths(),
             offsets=features.offsets(),
             weights=torch.gather(self.position_weight, dim=0, index=seq),
         )
         return weighted_features
+
+
+class FeatureProcessorsCollection(nn.Module):
+    """
+    Abstract base class for feature processor.
+
+    Args:
+        features (KeyedJaggedTensor]): feature representation
+
+    Returns:
+        KeyedJaggedTensor: modified KJT
+
+
+    Example::
+        kjt = JaggedTensor(...)
+        grouped_fp = FeatureProcessorsCollection(...)
+        fp_kjt = grouped_fp(kjt)
+    """
+
+    @abc.abstractmethod
+    def forward(
+        self,
+        features: KeyedJaggedTensor,
+    ) -> KeyedJaggedTensor:
+        """
+        Args:
+        features (JaggedTensor]): feature representation
+
+        Returns:
+            JaggedTensor: modified JT
+        """
+        pass
+
+
+class PositionWeightedModuleCollection(FeatureProcessorsCollection):
+    def __init__(
+        self, max_feature_lengths: Dict[str, int], device: Optional[torch.device] = None
+    ) -> None:
+        super().__init__()
+        self.max_feature_lengths = max_feature_lengths
+        for length in self.max_feature_lengths.values():
+            if length <= 0:
+                raise
+        self.position_weights: nn.ParameterDict = nn.ParameterDict()
+        for key, length in max_feature_lengths.items():
+            self.position_weights[key] = nn.Parameter(
+                torch.empty([length], device=device).fill_(1.0)
+            )
+        self.register_buffer(
+            "_dummy_weights",
+            torch.tensor(
+                max(self.max_feature_lengths.values()),
+                device=device,
+            ).fill_(1.0),
+        )
+
+    def forward(self, features: KeyedJaggedTensor) -> KeyedJaggedTensor:
+        if len(features.keys()) == 0:
+            return features
+
+        cat_seq = torch.ops.fbgemm.offsets_range(
+            features.offsets().long(), torch.numel(features.values())
+        )
+
+        seqs = torch.split(cat_seq, features.length_per_key())
+        weights_list = []
+        for key, seq in zip(features.keys(), seqs):
+            if key in self.max_feature_lengths:
+                weights_list.append(
+                    torch.gather(self.position_weights[key], dim=0, index=seq)
+                )
+            else:
+                weights_list.append(
+                    self._dummy_weights[: self.max_feature_lengths[key]]
+                )
+        weights = torch.cat(weights_list)
+
+        return KeyedJaggedTensor(
+            keys=features.keys(),
+            values=features.values(),
+            weights=weights,
+            lengths=features.lengths(),
+            offsets=features.offsets(),
+            stride=features.stride(),
+            length_per_key=features.length_per_key(),
+        )
```

## torchrec/modules/fp_embedding_modules.py

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Dict
+from typing import Dict, Union
 
 import torch
 import torch.nn as nn
 from torchrec.modules.embedding_modules import EmbeddingBagCollection
-from torchrec.modules.feature_processor_ import FeatureProcessor
+from torchrec.modules.feature_processor_ import (
+    FeatureProcessor,
+    FeatureProcessorsCollection,
+)
 from torchrec.sparse.jagged_tensor import KeyedJaggedTensor, KeyedTensor
 
 
 @torch.fx.wrap
 def apply_feature_processors_to_kjt(
     features: KeyedJaggedTensor,
     feature_processors: nn.ModuleDict,
@@ -79,31 +82,37 @@
             "feature_2": torch.Tensor(...)
         }
     """
 
     def __init__(
         self,
         embedding_bag_collection: EmbeddingBagCollection,
-        feature_processors: Dict[str, FeatureProcessor],
+        feature_processors: Union[
+            Dict[str, FeatureProcessor], FeatureProcessorsCollection
+        ],
     ) -> None:
         super().__init__()
         self._embedding_bag_collection = embedding_bag_collection
-        self._feature_processors = nn.ModuleDict(feature_processors)
+        self._feature_processors: Union[nn.ModuleDict, FeatureProcessorsCollection]
 
-        assert set(
-            sum(
-                [
-                    config.feature_names
-                    for config in self._embedding_bag_collection.embedding_bag_configs()
-                ],
-                [],
-            )
-        ) == set(
-            feature_processors.keys()
-        ), "Passed in feature processors do not match feature names of embedding bag"
+        if isinstance(feature_processors, FeatureProcessorsCollection):
+            self._feature_processors = feature_processors
+        else:
+            self._feature_processors = nn.ModuleDict(feature_processors)
+            assert set(
+                sum(
+                    [
+                        config.feature_names
+                        for config in self._embedding_bag_collection.embedding_bag_configs()
+                    ],
+                    [],
+                )
+            ) == set(
+                feature_processors.keys()
+            ), "Passed in feature processors do not match feature names of embedding bag"
 
         assert (
             embedding_bag_collection.is_weighted()
         ), "EmbeddingBagCollection must accept weighted inputs for feature processor"
 
     def forward(
         self,
@@ -113,11 +122,14 @@
         Args:
             features (KeyedJaggedTensor): KJT of form [F X B X L].
 
         Returns:
             KeyedTensor
         """
 
-        fp_features = apply_feature_processors_to_kjt(
-            features, self._feature_processors
-        )
+        if isinstance(self._feature_processors, FeatureProcessorsCollection):
+            fp_features = self._feature_processors(features)
+        else:
+            fp_features = apply_feature_processors_to_kjt(
+                features, self._feature_processors
+            )
         return self._embedding_bag_collection(fp_features)
```

## torchrec/modules/fused_embedding_modules.py

```diff
@@ -433,15 +433,17 @@
         # representation. This provides consistency between this class and the EmbeddingBagCollection's
         # nn.Module API calls (state_dict, named_modules, etc)
         self.embedding_bags: nn.ModuleDict = nn.ModuleDict()
         for (_key, tables), emb_module in zip(
             self._key_to_tables.items(), self._emb_modules
         ):
             for embedding_config, weight in zip(
-                tables, emb_module.split_embedding_weights()
+                tables,
+                emb_module.split_embedding_weights(),  # pyre-fixme[29]: `Union[nn.modules.module.Module,
+                #  torch._tensor.Tensor]` is not a function.
             ):
                 self.embedding_bags[embedding_config.name] = torch.nn.Module()
                 self.embedding_bags[embedding_config.name].register_parameter(
                     "weight", torch.nn.Parameter(weight)
                 )
 
     def forward(self, features: KeyedJaggedTensor) -> KeyedTensor:
@@ -679,15 +681,17 @@
         # representation. This provides consistency between this class and the EmbeddingBagCollection's
         # nn.Module API calls (state_dict, named_modules, etc)
         self.embeddings: nn.ModuleDict = nn.ModuleDict()
         for (_key, tables), emb_module in zip(
             self._key_to_tables.items(), self._emb_modules
         ):
             for embedding_config, weight in zip(
-                tables, emb_module.split_embedding_weights()
+                tables,
+                emb_module.split_embedding_weights(),  # pyre-fixme[29]: `Union[nn.modules.module.Module,
+                #  torch._tensor.Tensor]` is not a function.
             ):
                 self.embeddings[embedding_config.name] = torch.nn.Module()
                 self.embeddings[embedding_config.name].register_parameter(
                     "weight", torch.nn.Parameter(weight)
                 )
 
     def forward(self, features: KeyedJaggedTensor) -> Dict[str, JaggedTensor]:
```

## torchrec/modules/lazy_extension.py

```diff
@@ -161,14 +161,16 @@
         # If the module is already initialized, call `super().apply(fn)` to
         # run the usual apply logic.
         # pyre-ignore[16]
         return super().apply(fn)
 
     # fmt: off
     # pyre-ignore[2, 47]
+    # pyre-fixme[14]: `_infer_parameters` overrides method defined in
+    #  `LazyModuleMixin` inconsistently.
     def _infer_parameters(self: _LazyExtensionProtocol, module, input, kwargs) -> None:
         r"""Infers the size and initializes the parameters according to the
         provided input batch.
         Given a module that contains parameters that were declared inferrable
         using :class:`torch.nn.parameter.ParameterMode.Infer`, runs a forward pass
         in the complete module using the provided input to initialize all the parameters
         as needed.
@@ -252,8 +254,9 @@
                 # pyre-ignore[16]
                 self._maybe_warn_non_full_backward_hook(input, result, grad_fn)
 
         return result
     # fmt: on
 
     # pyre-ignore[4]
+    # pyre-fixme[15]: `__call__` overrides attribute defined in `type` inconsistently.
     __call__: Callable[..., Any] = _call_impl
```

## torchrec/quant/embedding_modules.py

```diff
@@ -4,15 +4,15 @@
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import copy
 import itertools
 from collections import defaultdict
-from typing import Dict, List, Optional, Tuple
+from typing import Callable, Dict, List, Optional, Tuple, Type
 
 import torch
 import torch.nn as nn
 from fbgemm_gpu.split_table_batched_embeddings_ops_inference import (
     EmbeddingLocation,
     IntNBitTableBatchedEmbeddingBagsCodegen,
     PoolingMode,
@@ -49,14 +49,54 @@
 try:
     import fbgemm_gpu  # @manual  # noqa
 except ImportError:
     pass
 
 MODULE_ATTR_REGISTER_TBES_BOOL: str = "__register_tbes_in_named_modules"
 
+MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS: str = (
+    "__quant_state_dict_split_scale_bias"
+)
+
+
+def for_each_module_of_type_do(
+    module: nn.Module,
+    module_types: List[Type[torch.nn.Module]],
+    op: Callable[[torch.nn.Module], None],
+) -> None:
+    for m in module.modules():
+        if any([isinstance(m, t) for t in module_types]):
+            op(m)
+
+
+def quant_prep_enable_quant_state_dict_split_scale_bias(module: nn.Module) -> None:
+    setattr(module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, True)
+
+
+def quant_prep_enable_quant_state_dict_split_scale_bias_for_types(
+    module: nn.Module, module_types: List[Type[torch.nn.Module]]
+) -> None:
+
+    for_each_module_of_type_do(
+        module,
+        module_types,
+        lambda m: setattr(m, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, True),
+    )
+
+
+def quant_prep_enable_register_tbes(
+    module: nn.Module, module_types: List[Type[torch.nn.Module]]
+) -> None:
+
+    for_each_module_of_type_do(
+        module,
+        module_types,
+        lambda m: setattr(m, MODULE_ATTR_REGISTER_TBES_BOOL, True),
+    )
+
 
 def quantize_state_dict(
     module: nn.Module,
     table_name_to_quantized_weights: Dict[str, Tuple[Tensor, Tensor]],
     data_type: DataType,
 ) -> torch.device:
     device = torch.device("cpu")
@@ -183,14 +223,15 @@
         is_weighted: bool,
         device: torch.device,
         output_dtype: torch.dtype = torch.float,
         table_name_to_quantized_weights: Optional[
             Dict[str, Tuple[Tensor, Tensor]]
         ] = None,
         register_tbes: bool = False,
+        quant_state_dict_split_scale_bias: bool = False,
     ) -> None:
         super().__init__()
         self._is_weighted = is_weighted
         self._embedding_bag_configs: List[EmbeddingBagConfig] = tables
         self._key_to_tables: Dict[
             Tuple[PoolingType, DataType], List[EmbeddingBagConfig]
         ] = defaultdict(list)
@@ -264,25 +305,41 @@
         # We map over the parameters from FBGEMM backed kernels to the canonical nn.EmbeddingBag
         # representation. This provides consistency between this class and the EmbeddingBagCollection
         # nn.Module API calls (state_dict, named_modules, etc)
         self.embedding_bags: nn.ModuleDict = nn.ModuleDict()
         for (_key, tables), emb_module in zip(
             self._key_to_tables.items(), self._emb_modules
         ):
-            for embedding_config, (weight, _) in zip(
-                tables, emb_module.split_embedding_weights(split_scale_shifts=False)
+            for embedding_config, (weight, qscale, qbias) in zip(
+                tables,
+                emb_module.split_embedding_weights_with_scale_bias(  # pyre-ignore[29]
+                    split_scale_bias_mode=2 if quant_state_dict_split_scale_bias else 0
+                ),
             ):
                 self.embedding_bags[embedding_config.name] = torch.nn.Module()
                 # register as a buffer so it's exposed in state_dict.
                 # TODO: register as param instead of buffer
                 # however, since this is only needed for inference, we do not need to expose it as part of parameters.
                 # Additionally, we cannot expose uint8 weights as parameters due to autograd restrictions.
                 self.embedding_bags[embedding_config.name].register_buffer(
                     "weight", weight
                 )
+                if quant_state_dict_split_scale_bias:
+                    self.embedding_bags[embedding_config.name].register_buffer(
+                        "weight_qscale", qscale
+                    )
+                    self.embedding_bags[embedding_config.name].register_buffer(
+                        "weight_qbias", qbias
+                    )
+
+        setattr(
+            self,
+            MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
+            quant_state_dict_split_scale_bias,
+        )
         self.register_tbes = register_tbes
         if register_tbes:
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(self._emb_modules)
 
     def forward(
         self,
         features: KeyedJaggedTensor,
@@ -370,14 +427,17 @@
             embedding_bag_configs,
             module.is_weighted(),
             device=device,
             # pyre-ignore [16]
             output_dtype=module.qconfig.activation().dtype,
             table_name_to_quantized_weights=table_name_to_quantized_weights,
             register_tbes=getattr(module, MODULE_ATTR_REGISTER_TBES_BOOL, False),
+            quant_state_dict_split_scale_bias=getattr(
+                module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+            ),
         )
 
     def embedding_bag_configs(
         self,
     ) -> List[EmbeddingBagConfig]:
         return self._embedding_bag_configs
 
@@ -453,14 +513,15 @@
         device: torch.device,
         need_indices: bool = False,
         output_dtype: torch.dtype = torch.float,
         table_name_to_quantized_weights: Optional[
             Dict[str, Tuple[Tensor, Tensor]]
         ] = None,
         register_tbes: bool = False,
+        quant_state_dict_split_scale_bias: bool = False,
     ) -> None:
         super().__init__()
         self._emb_modules: List[IntNBitTableBatchedEmbeddingBagsCodegen] = []
         self.embeddings: nn.ModuleDict = nn.ModuleDict()
 
         self._embedding_configs = tables
         self._embedding_dim: int = -1
@@ -510,23 +571,37 @@
 
             self._emb_modules.append(emb_module)
             self.embeddings[config.name] = torch.nn.Module()
             # register as a buffer so it's exposed in state_dict.
             # TODO: register as param instead of buffer
             # however, since this is only needed for inference, we do not need to expose it as part of parameters.
             # Additionally, we cannot expose uint8 weights as parameters due to autograd restrictions.
-            weights_list = emb_module.split_embedding_weights(split_scale_shifts=False)
+            weights_list = emb_module.split_embedding_weights_with_scale_bias(
+                split_scale_bias_mode=2 if quant_state_dict_split_scale_bias else 0
+            )
             self.embeddings[config.name].register_buffer("weight", weights_list[0][0])
+            if quant_state_dict_split_scale_bias:
+                self.embeddings[config.name].register_buffer(
+                    "weight_qscale", weights_list[0][1]
+                )
+                self.embeddings[config.name].register_buffer(
+                    "weight_qbias", weights_list[0][2]
+                )
 
             if not config.feature_names:
                 config.feature_names = [config.name]
 
         self._embedding_names_by_table: List[List[str]] = get_embedding_names_by_table(
             tables
         )
+        setattr(
+            self,
+            MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS,
+            quant_state_dict_split_scale_bias,
+        )
         self.register_tbes = register_tbes
         if register_tbes:
             self.tbes: torch.nn.ModuleList = torch.nn.ModuleList(self._emb_modules)
 
     def forward(
         self,
         features: KeyedJaggedTensor,
@@ -583,14 +658,17 @@
         return cls(
             tables,
             device=device,
             need_indices=module.need_indices(),
             # pyre-ignore
             output_dtype=module.qconfig.activation().dtype,
             table_name_to_quantized_weights=table_name_to_quantized_weights,
+            quant_state_dict_split_scale_bias=getattr(
+                module, MODULE_ATTR_QUANT_STATE_DICT_SPLIT_SCALE_BIAS, False
+            ),
         )
 
     def _get_name(self) -> str:
         return "QuantizedEmbeddingCollection"
 
     def need_indices(self) -> bool:
         return self._need_indices
```

## torchrec/quant/utils.py

```diff
@@ -29,22 +29,25 @@
         for emb_configs, emb_module in zip(
             quant_ebc._key_to_tables, quant_ebc._emb_modules
         ):
             table_names = []
             for config in emb_configs:
                 table_names.append(config.name)
             joined_table_names = ",".join(table_names)
+            # pyre-fixme[16]: `Module` has no attribute `_fx_path`.
             emb_module._fx_path = f"emb_module.{joined_table_names}"
     elif isinstance(quant_ebc, ShardedQuantEmbeddingBagCollection):
         for i, (emb_module, emb_dist_module) in enumerate(
             zip(quant_ebc._lookups, quant_ebc._output_dists)
         ):
             embedding_fx_path = f"embedding_lookup.sharding_{i}"
             emb_module._fx_path = embedding_fx_path
             emb_dist_module._fx_path = f"embedding_dist.{i}"
+            # pyre-fixme[6]: For 1st argument expected `Iterable[Variable[_T]]` but
+            #  got `Union[Module, Tensor]`.
             for rank, rank_module in enumerate(emb_module._embedding_lookups_per_rank):
                 rank_fx_path = f"{embedding_fx_path}.rank_{rank}"
                 rank_module._fx_path = rank_fx_path
                 for group, group_module in enumerate(rank_module._emb_modules):
                     group_module._fx_path = f"{rank_fx_path}.group_{group}"
                     group_module._emb_module._fx_path = (
                         f"{rank_fx_path}.group_{group}.tbe"
```

## Comparing `torchrec_nightly-2023.6.8.dist-info/LICENSE` & `torchrec_nightly-2023.6.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchrec_nightly-2023.6.8.dist-info/METADATA` & `torchrec_nightly-2023.6.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrec-nightly
-Version: 2023.6.8
+Version: 2023.6.9
 Summary: Pytorch domain library for recommendation systems
 Home-page: https://github.com/pytorch/torchrec
 Author: TorchRec Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: pytorch,recommendation systems,sharding
 Classifier: Development Status :: 4 - Beta
```

## Comparing `torchrec_nightly-2023.6.8.dist-info/RECORD` & `torchrec_nightly-2023.6.9.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -9,50 +9,50 @@
 torchrec/datasets/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/datasets/scripts/contiguous_preproc_criteo.py,sha256=8jjtDiQScJH6R4FfKLgJ3fm-FzfnJxyfbV52zj3SM_8,2448
 torchrec/datasets/scripts/npy_preproc_criteo.py,sha256=QOyHZpPGL6HtPrVijk7qTALvnDqgecWPEZxKB_eVA94,2847
 torchrec/datasets/scripts/shuffle_preproc_criteo.py,sha256=PC1t5EkJkG6qu3ioewAVZM-Bnzo01HKMUH92IprFth0,3077
 torchrec/datasets/test_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/datasets/test_utils/criteo_test_utils.py,sha256=Ob2fJniGOsfbWNF_Gy2RJhrGAVnLAFPSlUTJOp2kay4,5308
 torchrec/distributed/__init__.py,sha256=VCy8GKOM-1dejxUWNSA3gozG3HQ4x5-Y9c9-WFbAMGg,1912
-torchrec/distributed/batched_embedding_kernel.py,sha256=_LWPI3zO_rObQgg0J0f-iojtpmazMfDfgHHg63hr_tE,37053
+torchrec/distributed/batched_embedding_kernel.py,sha256=wNLqxMtbcBasLfm7OBA77QfPfswrFkzy96wYaIfz7ZQ,37411
 torchrec/distributed/collective_utils.py,sha256=r7Aawq-KSVC-HjjEd6U8k0vNnRMx_-8_sAhYdElGaJw,2069
 torchrec/distributed/comm.py,sha256=21Std9n_HJCF3Nsw9O4yQQOJuL2DUVzZzoRhH3M6my8,4988
 torchrec/distributed/comm_ops.py,sha256=C63THNJOnJWkfRYGuNw5opFyKsdlpZs9_23u-DHSrAQ,55918
 torchrec/distributed/dist_data.py,sha256=pWuAzn98i5O4lNHmv2wMGa4gksYEh_DOJT4rzRp_nYg,35580
-torchrec/distributed/embedding.py,sha256=U59gMHspqHedq1X4yb3DTLFTTxGn0YPjKd-CTDOu25g,31599
-torchrec/distributed/embedding_kernel.py,sha256=SNpvTbW1V4HtjSmAzPPa5imrUzSOe7zuQDkK3GFudHc,3872
-torchrec/distributed/embedding_lookup.py,sha256=1D7xO_ljztKkIIZJ7iziCI5mF65-S-l9hZ4Z6RAc1rY,28994
-torchrec/distributed/embedding_sharding.py,sha256=Kp8zJRIuBo_3XswENCCym9vnVId28Zh0HMoVqmcEoJI,18564
+torchrec/distributed/embedding.py,sha256=xbzsxuqclElhNIN7lQxF-i06Cx4jBw4R8M6j-fUz4tg,32013
+torchrec/distributed/embedding_kernel.py,sha256=9OA5PDofQZ-ZRORNR4Ca1pJoEZk5Oj2gE6axYwcXIds,4947
+torchrec/distributed/embedding_lookup.py,sha256=Cyl1osqBbk1wpQlcHjSYp-9nsOJ-l_9A55x9VuAMg4U,29176
+torchrec/distributed/embedding_sharding.py,sha256=jhbxU4mCMCCLE3NnV3bLHvzJKRgTiL-rPJPbqutl3WQ,20599
 torchrec/distributed/embedding_tower_sharding.py,sha256=ypr4JbTZUh_35dYUoKWoOSJNEVG3c6gV9g5gt-fs6lQ,37089
 torchrec/distributed/embedding_types.py,sha256=QbDVqeT2wb1RpnGZxrFtFdHYDsOHKW7SH8fLWmN_d0E,15030
-torchrec/distributed/embeddingbag.py,sha256=JffPXLKq_K0HAeSe8R3W3PrQuKowtdPTyHHez3qgdBs,35078
+torchrec/distributed/embeddingbag.py,sha256=ILPW9XGRYGVPFwKGNU8DF5zk0Oj70-duRz2JUdxxlMo,35218
 torchrec/distributed/fbgemm_qcomm_codec.py,sha256=StYltKC6Eq6SE_YiX6GsVW3ZF0VyqTcGHXuCYmPAFlU,7373
-torchrec/distributed/fp_embeddingbag.py,sha256=tbwvTzBZXCBo_SSlyd7JnQOW6qWx1jdjmdeqnAnOaWM,5542
-torchrec/distributed/fused_embedding.py,sha256=uIgeaoEPujTgkcq8S2OPRYBe03J4TUF04uOOy_iRsMk,5273
+torchrec/distributed/fp_embeddingbag.py,sha256=sC7ZIECzJtwn5LNRrUzf0OH7phI3kQHqQ6wBPaGGvPQ,6137
+torchrec/distributed/fused_embedding.py,sha256=1VJeW5Dl7EFMvyOfhBvDKZlp39GYucBo8vNFJY2alFI,5243
 torchrec/distributed/fused_embeddingbag.py,sha256=7DIMc5sHdsDAgqCnNomcPo6V4aIH1wlkzyshHeJB3pc,5110
-torchrec/distributed/fused_params.py,sha256=THLZYo_6mErDx2DGMB3Fi_VFPpLKCrq6Amvg8CckjsA,1709
+torchrec/distributed/fused_params.py,sha256=YEbH5KUphcSWkwLi-JzXUR9SRDm2OykFxP46CJj6nTM,2271
 torchrec/distributed/grouped_position_weighted.py,sha256=q-QE0U306BiPkXIAlJGIQ80EUDZj-FXTbWwjz3EyvLI,3807
 torchrec/distributed/model_parallel.py,sha256=YzXWgCmmeA_ccHtqfzeDM5ZTnnFUXfYCtocx1pKHV7Q,19786
-torchrec/distributed/quant_embedding.py,sha256=tbUP4_-iVvfAZlJ7gCf5ZJb6snH35EFLeJrZhATUZD8,13729
-torchrec/distributed/quant_embedding_kernel.py,sha256=FNEKKje7yvnOI28ODg5POQy2pmeKWNmPvf193JF8iEw,13343
-torchrec/distributed/quant_embeddingbag.py,sha256=MxFdFDn4HAJ9PRc3ko_6q4O0KuWkh3_Y1BHajX0E9aY,10931
+torchrec/distributed/quant_embedding.py,sha256=cyawhiEPlefP3pAAJB8A0uegGnlUj41OOYIlRt8qNBc,14686
+torchrec/distributed/quant_embedding_kernel.py,sha256=3WRKuTrKi8dJvhfAsb_vYDp3aqOc2YOrKPeMhZ7MDJk,14976
+torchrec/distributed/quant_embeddingbag.py,sha256=f_yZU9nKlmdzpJNHpugfmAbyIkTYZGiY_H1NzDExRno,11770
 torchrec/distributed/shard.py,sha256=4Dr5ixWCoMEFEuL5WN4fL2gIdl9wmSUjZWsiF-kdCdQ,9261
 torchrec/distributed/sharding_plan.py,sha256=vVQhmXy2w4FmXyuJa1t6PyfaqEEVSxoLZ5ChWlc7TbU,19411
-torchrec/distributed/train_pipeline.py,sha256=0twZDc4PIt2Sz6q2DEvyaz6P6jHb7-fmj_bTiA7ir7E,34059
+torchrec/distributed/train_pipeline.py,sha256=pQ_bIP5dI70_ypkE2OWcv_pVwKa1nNjdT6oBZaTunpI,36724
 torchrec/distributed/types.py,sha256=tNd_B5PXjaOqPmUXxSZLXB3a71sjU8LBtSY9kuGxe7I,24927
 torchrec/distributed/utils.py,sha256=PbVfo9_QBugfSOvwmySdjXlhWOAYSl9eGpYYH0d0SqI,11873
 torchrec/distributed/composable/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/distributed/composable/table_batched_embedding_slice.py,sha256=x439M8TTXQtzoihan1OKKbmGYkqJlAxxTHCDz5295RY,3207
 torchrec/distributed/planner/__init__.py,sha256=UWnxb-SuE211uJGdwtSkKRVADT3plQozB2l6fvs6Ve0,1025
 torchrec/distributed/planner/constants.py,sha256=MkeVqYO2QGg57i6fs29lZb2dScaaR9mdQVsee4NxyFc,3135
 torchrec/distributed/planner/enumerators.py,sha256=hZzhnfMrOz65lBoddxTKBb01hm43R_5tdpysJFSzCLE,10318
 torchrec/distributed/planner/partitioners.py,sha256=k-rzm6oMZ_sLpGHT8yAu2tIMkMumhJMvAFeY0cdNirk,12642
 torchrec/distributed/planner/perf_models.py,sha256=vYIjVr0NG6sZItfxVuRWF7AS8lGGtbRn66O0flNJpoU,835
 torchrec/distributed/planner/planners.py,sha256=LjMOoQTu_IlwlG-wl03H39c886oxBgfEQMKsouYI1pM,13288
-torchrec/distributed/planner/proposers.py,sha256=s8nDZcZWiGmaFVHr8J3wmuoUYFGpe6n1NPLtprOqSgk,11134
+torchrec/distributed/planner/proposers.py,sha256=tfhI0DavpRYfY4UN5diXBMl8fWHIEm8wNco5R6yBIGI,11236
 torchrec/distributed/planner/shard_estimators.py,sha256=JTdL0OI0kpFbkxdCZN9qK46PN6v2kv2mIMdXLIZMsOE,40395
 torchrec/distributed/planner/stats.py,sha256=oIhRnFQybUdx-2NEH3ZBhyx0nqtiR4VkQKnS7YLW6CY,23617
 torchrec/distributed/planner/storage_reservations.py,sha256=rPqeD03f3mg8yoSqy9CZfOmxVMUGrCz98nPqwvxhApc,9125
 torchrec/distributed/planner/types.py,sha256=JG39UMXzWQ7_G38aG2qo3h601s2UsII_OPyHJ068kOM,13899
 torchrec/distributed/planner/utils.py,sha256=YwOUrqb-D6HaVtWCRFz9RWhBdMRBqjMaYYhoQgyOkQg,1119
 torchrec/distributed/sharding/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/distributed/sharding/cw_sequence_sharding.py,sha256=o8RZAs2zivNP8MZ5QUWF0alw7KwWZnJVG9iKHM4EJdE,2539
@@ -63,19 +63,19 @@
 torchrec/distributed/sharding/rw_sharding.py,sha256=k3ym1GGjdQeRnLeUheZm5o9D8co_U4dUQgHrF771XUQ,12850
 torchrec/distributed/sharding/sequence_sharding.py,sha256=LBUW1PvAV9WNwf-m-x9bYIcU96PL75mPE_uQK9dLAOU,3114
 torchrec/distributed/sharding/tw_sequence_sharding.py,sha256=SR_G_rniSZx_DBnrWW14HEMoeqwRnMPN3LdQlnptLL8,7692
 torchrec/distributed/sharding/tw_sharding.py,sha256=JtI2GW9YR-eg1VuQDwDa6qaR6sOgBAzGx3Y3XkEOBZM,16315
 torchrec/distributed/sharding/twcw_sharding.py,sha256=LyOowcADWmRdkRn-eEW6QB0b0xYi0vM-Ubrr6N2zwwA,1284
 torchrec/distributed/sharding/twrw_sharding.py,sha256=k69AX5oKj3ep38tM_RI_NkwyZ4z_U8kVQpLtDjRYPKI,19898
 torchrec/distributed/test_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torchrec/distributed/test_utils/infer_utils.py,sha256=v3OLVjfmy612aSSDPpFeu8m7K9omDAO9JFWQ08NHcZI,10213
+torchrec/distributed/test_utils/infer_utils.py,sha256=r2HdvqgADtAbP5-S5FCANaO734GF68hdCtB1vJ7Lgfs,10453
 torchrec/distributed/test_utils/multi_process.py,sha256=6AxYe2cO44EGdw-Lt5YNwqmWZW8Ldu7bVGTluIIOFbA,4868
 torchrec/distributed/test_utils/test_model.py,sha256=ACqCdD3bcxX74JihIg7jTcLvBsV8U-Bvwvy9-Pbj7nI,34246
 torchrec/distributed/test_utils/test_model_parallel.py,sha256=oN_fl-QOaAarrZwnr7q5Lz4f9xiqxxof9Bk_4PM13hM,11193
-torchrec/distributed/test_utils/test_model_parallel_base.py,sha256=gny2CZ7n4GUzIwAAKw6Iuq0lgd7LL5mhwKKR_gvG9uE,25190
+torchrec/distributed/test_utils/test_model_parallel_base.py,sha256=I7q2IIZLN79RdqYCrg6hr_yBysZr2VO4AlESYsCtq5g,25308
 torchrec/distributed/test_utils/test_sharding.py,sha256=DlB6N5-qlRp-xQfEEFElDkNffnEX6LO4vOrDCGp8VkQ,15367
 torchrec/fx/__init__.py,sha256=TxNjllMWlB_rpDy4SNSA_e-xbZbhxGGTb9AxpZGcaFk,422
 torchrec/fx/tracer.py,sha256=iXfWWgPNdFlRs89RbA18Nel0Tl9z8UprRWPfTQbLx5k,6477
 torchrec/fx/utils.py,sha256=N50AfwlUhyS9r1Sv21fSbqRxiOk4KRX0MX9sDjCaQcA,4401
 torchrec/inference/__init__.py,sha256=vi2C_o1Bvsp6hS3_uVZTL7kShgxw5qFZp248Svee2Og,1223
 torchrec/inference/client.py,sha256=jS6ldQxBRY3Bp_LwDLUNSlPt2VYMc-Hsd4iKKoHfDVU,3614
 torchrec/inference/model_packager.py,sha256=HxOEbnqXB2K4uUB9dBBJAL49ZYJME4xTFyVzKjpsjy4,3957
@@ -90,18 +90,18 @@
 torchrec/metrics/metric_module.py,sha256=8XXa5DJ5eYrS1Pat34_FZ3E9OKUj--8i80nCqXqtJsg,17909
 torchrec/metrics/metrics_config.py,sha256=tL9etUu4FsA_Dr9kUKCf3zIixK6VbIgVi4UoBTZ1GnM,6778
 torchrec/metrics/metrics_namespace.py,sha256=fodij0OglzAGOWNEefuPw0UL1cYfQZAAedCjTErDV6M,3695
 torchrec/metrics/model_utils.py,sha256=WNMsAKK9b5OVPWeuRrNDZ2HjwKuAw3gjNG3OdE99EXw,3904
 torchrec/metrics/mse.py,sha256=tkK3yBV8Uu9Z8Mw_3c1k4kYAhp1jUQkFEJxc0l2LtWU,4631
 torchrec/metrics/multiclass_recall.py,sha256=7NqjkA4IUy4Db90du3hVt8cJxoWS18PBaOourHETkEs,5605
 torchrec/metrics/ne.py,sha256=wXEb9Eh5Mn3D_uuAIaUb3CvJ1eDs06ahVxaWOjR4CtU,6811
-torchrec/metrics/rec_metric.py,sha256=Oq6SRk_TVOXba3qgKbNc7X2ExsiaHNA00J_ZhhkYpHY,31495
+torchrec/metrics/rec_metric.py,sha256=j1ias-rsD1nlCx_iR1Wmvw0BLoe9DHgjHfzAwd5Uvjs,33554
 torchrec/metrics/recall_session.py,sha256=24aDBSi8V5XXSnwpqCR5bWcm2CWslBBZ9_a0LQ6VGeg,10490
 torchrec/metrics/throughput.py,sha256=A_WqccFNgu4XpBZzZxnGxAT84Xp2ld43qQM6R1zaqik,6057
-torchrec/metrics/tower_qps.py,sha256=YC-EzaU2hbAQ3VZ1GJDHjWNKLD8fEvyyM5A5WerjwZU,10622
+torchrec/metrics/tower_qps.py,sha256=PXTBsLGjEEbQV5q2kGQriRq8GCneNkhBKTFAgNXzc-0,11160
 torchrec/metrics/weighted_avg.py,sha256=dX-qwha2__F-p-R5u27152OwlGRS6Xfnbt1DEIBw8NQ,2867
 torchrec/metrics/test_utils/__init__.py,sha256=p_uep7Hg7_aY3rOg8CxtS-REopQ4ywQq075KFoso1Lw,16441
 torchrec/models/__init__.py,sha256=iYpG-yLxFaa3ZdN-UU9PWNIdgm9EXoEj_QzJ2OLKGJQ,913
 torchrec/models/deepfm.py,sha256=-SxFKF-kHKFEzC0XIsLigQh673-B_Lu6xFlZPkR5t2g,11410
 torchrec/models/dlrm.py,sha256=37v6MOb8P06DtXfDDqokvSKSDyhDVGFEPsRoBSRtCTY,30000
 torchrec/models/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/models/experimental/test_transformerdlrm.py,sha256=pxdu5k-EdTdYX5RblAe1A97GuiHAUmm6oJwfG_qX8Vw,9825
@@ -110,34 +110,34 @@
 torchrec/modules/activation.py,sha256=o3rGyy40bmmsplyxQy3dDMe8kITRERLJQF7oa5VTKfE,1456
 torchrec/modules/crossnet.py,sha256=hiE375Y0atKsyWYK3GLPtx5VzqkaoNl79r9HsxtMBVA,15163
 torchrec/modules/deepfm.py,sha256=05ZM2sB1YMVliZwrLHvtMYf3eWGguLFopaZwGZK16bs,8415
 torchrec/modules/embedding_configs.py,sha256=97g9ui8baC7RdqzB6EPxgkLvGaiX_-r24igTSlXyfcs,5537
 torchrec/modules/embedding_modules.py,sha256=ezRcQ2BqgEEdDF-86Aeribm44YHtaA21NrgOvfr_KYM,14021
 torchrec/modules/embedding_tower.py,sha256=rHiMEUUMoMZUxIPKBE2HyI7I5uNthGQsZIxH038TmoI,4858
 torchrec/modules/feature_processor.py,sha256=UqDELZQ7cRpAQb_6LyxwVByJDdM5NPDfAyEk4qYQmKM,12360
-torchrec/modules/feature_processor_.py,sha256=P4gttrqiWmdmMB7sceB8D0Nn-oKTn4LzXpocK7voCd8,2169
-torchrec/modules/fp_embedding_modules.py,sha256=9E8VGvUfZPZKxJpYKz5nLqVc_VUBlUj21KBXMp6sKO4,3855
-torchrec/modules/fused_embedding_modules.py,sha256=a0mRx3JGTGtMoEwagOhJyW5DTI85iagUT7l6WN0YJOE,31193
-torchrec/modules/lazy_extension.py,sha256=0yOchNRZsOT3A2n5DN5wZhYHjIZkc0F6z_xWX_ULGp0,10696
+torchrec/modules/feature_processor_.py,sha256=Cvhuim-U8t84jL_h5EEAM7Yiwo1SOoSLHA5Gtkf4Hfc,4830
+torchrec/modules/fp_embedding_modules.py,sha256=AdUxhEODvE-h0FbqQoD0o-haLBgMRhXl2O0gvcstxI0,4403
+torchrec/modules/fused_embedding_modules.py,sha256=FsScroCb_IN8WhI_CjM0IkPgQrlrv7aU0XPm7dtsNkM,31453
+torchrec/modules/lazy_extension.py,sha256=iYkjlFGzpI1dbVZ7ofTN1OIA7FI-IlNgM57v3EymPE0,10894
 torchrec/modules/mlp.py,sha256=lV3vCEmNLI1kDtF4eGlCaGvtG3FQ8UEMs4Hcc6Nf3pM,6309
 torchrec/modules/utils.py,sha256=Ohx144TmZCEHbv3oEUsBf8e4DkGjmyPf98N4mA8kCxo,4022
 torchrec/optim/__init__.py,sha256=4-nuv6JsmuWBtzyUvCKJ0b9-m7oFi8QB2b3krFF0KgQ,1639
 torchrec/optim/apply_optimizer_in_backward.py,sha256=0wjamGai9i0rXvIf4GNYNhCz7NtkH_9expuepk1qcbI,2012
 torchrec/optim/clipping.py,sha256=sDotlb8Sf4D7-lbBxhzRDFHoiO_DVx34F1J8vOEWq8I,1569
 torchrec/optim/fused.py,sha256=J4u2PWaHD65PIEdg0wTWoK_riZCoSKAVKYPGuZtfKLY,1353
 torchrec/optim/keyed.py,sha256=5QASHSkw2oYwu3OVHU5JJ2mm5tQaSCOQ3z_vBVRLPtk,16069
 torchrec/optim/optimizers.py,sha256=tmf-ww_47F_tu04ufffVCczM2AOMR5yTNh_8S-gJl-8,4420
 torchrec/optim/rowwise_adagrad.py,sha256=jHpCZDFWRrXbwlKiwROg2dl0qK1lG2uXMJkTtbZ_uSg,7405
 torchrec/optim/warmup.py,sha256=QaMcWU-jMZbDOfRHEH_x9r7EsjtI_LRgOGAmEgzJWSQ,4865
 torchrec/optim/test_utils/__init__.py,sha256=mkNZr5iNV3kseuamPBnnAeknjbv4ELPFMGyJ1lWiJGU,560
 torchrec/quant/__init__.py,sha256=A6NIA6ztq6iP1JTLRLNzlgnCcd-LaN8efnxGub3Ii4A,1140
-torchrec/quant/embedding_modules.py,sha256=RLuYVywThBXgLEZeHrH2F1sGEA1XydzBg4S9v2rivgY,22933
-torchrec/quant/utils.py,sha256=PkgXn7wnnBIqJ5JAidJMvpAVre1YL8oiYGiPuV_gU2c,4100
+torchrec/quant/embedding_modules.py,sha256=EKWK6_AkLSSj3Hc-capmN2_VXY52s0pfuNqyDvjPX5M,25656
+torchrec/quant/utils.py,sha256=ab7J2QfHjeB7UF1BRh20KygcJR5ZHKwRMImgyCZOagE,4296
 torchrec/sparse/__init__.py,sha256=dLqSye4Jo6obnNNTUKdPDxPQb9sL2U4weemSn-DjpYk,1163
 torchrec/sparse/jagged_tensor.py,sha256=3874Ka-1XE6nsvHIVu8iGM6l3nNlSF7PQW-fM5rnl4c,55583
 torchrec/sparse/test_utils/__init__.py,sha256=BLxfGKJvwjjCiQM64O5wGAA_Cea0sG-buw9lTDWuqug,1430
 torchrec/test_utils/__init__.py,sha256=JncJcXS4N3gI7-fsizQ2-qiWM6MhIrpvskF_9gDf0Go,5661
-torchrec_nightly-2023.6.8.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
-torchrec_nightly-2023.6.8.dist-info/METADATA,sha256=BwIzJWdT-QmzyTfPYoxkWS7MlNvibruyLtEneEF3c-s,5011
-torchrec_nightly-2023.6.8.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
-torchrec_nightly-2023.6.8.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
-torchrec_nightly-2023.6.8.dist-info/RECORD,,
+torchrec_nightly-2023.6.9.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
+torchrec_nightly-2023.6.9.dist-info/METADATA,sha256=mRb6bQBNu8fDMGkIss2u0G4F8zWTV4sjjEH7LX0f13Q,5011
+torchrec_nightly-2023.6.9.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
+torchrec_nightly-2023.6.9.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
+torchrec_nightly-2023.6.9.dist-info/RECORD,,
```

