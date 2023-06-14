# Comparing `tmp/secretflow-0.8.2b3-cp38-cp38-manylinux2014_x86_64.whl.zip` & `tmp/secretflow-0.8.3b0-cp38-cp38-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,297 +1,343 @@
-Zip file size: 1288179 bytes, number of entries: 295
--rw-r--r--  2.0 unx     1321 b- defN 23-May-15 12:09 secretflow/__init__.py
--rw-r--r--  2.0 unx     3229 b- defN 23-May-15 12:09 secretflow/cli.py
--rw-r--r--  2.0 unx      607 b- defN 23-May-15 12:09 secretflow/version.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/component/__init__.py
--rw-r--r--  2.0 unx    21958 b- defN 23-May-15 12:09 secretflow/component/component.py
--rw-r--r--  2.0 unx     2235 b- defN 23-May-15 12:09 secretflow/component/entry.py
--rw-r--r--  2.0 unx     7339 b- defN 23-May-15 12:09 secretflow/component/node_reader.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/component/ml/__init__.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/component/ml/linear/__init__.py
--rw-r--r--  2.0 unx     7573 b- defN 23-May-15 12:09 secretflow/component/ml/linear/ss_sgd.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/component/preprocessing/__init__.py
--rw-r--r--  2.0 unx     3938 b- defN 23-May-15 12:09 secretflow/component/preprocessing/train_test_split.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/component/psi/__init__.py
--rw-r--r--  2.0 unx     5605 b- defN 23-May-15 12:09 secretflow/component/psi/two_party_balanced.py
--rw-r--r--  2.0 unx      754 b- defN 23-May-15 12:09 secretflow/data/__init__.py
--rw-r--r--  2.0 unx    14806 b- defN 23-May-15 12:09 secretflow/data/base.py
--rw-r--r--  2.0 unx     1108 b- defN 23-May-15 12:09 secretflow/data/math_utils.py
--rw-r--r--  2.0 unx    24878 b- defN 23-May-15 12:09 secretflow/data/ndarray.py
--rw-r--r--  2.0 unx     5420 b- defN 23-May-15 12:09 secretflow/data/split.py
--rw-r--r--  2.0 unx      716 b- defN 23-May-15 12:09 secretflow/data/horizontal/__init__.py
--rw-r--r--  2.0 unx    15042 b- defN 23-May-15 12:09 secretflow/data/horizontal/dataframe.py
--rw-r--r--  2.0 unx     2557 b- defN 23-May-15 12:09 secretflow/data/horizontal/io.py
--rw-r--r--  2.0 unx     1555 b- defN 23-May-15 12:09 secretflow/data/horizontal/sampler.py
--rw-r--r--  2.0 unx      627 b- defN 23-May-15 12:09 secretflow/data/io/__init__.py
--rw-r--r--  2.0 unx     2112 b- defN 23-May-15 12:09 secretflow/data/io/oss.py
--rw-r--r--  2.0 unx     2501 b- defN 23-May-15 12:09 secretflow/data/io/util.py
--rw-r--r--  2.0 unx      691 b- defN 23-May-15 12:09 secretflow/data/mix/__init__.py
--rw-r--r--  2.0 unx    15054 b- defN 23-May-15 12:09 secretflow/data/mix/dataframe.py
--rw-r--r--  2.0 unx      716 b- defN 23-May-15 12:09 secretflow/data/vertical/__init__.py
--rw-r--r--  2.0 unx    22944 b- defN 23-May-15 12:09 secretflow/data/vertical/dataframe.py
--rw-r--r--  2.0 unx     6972 b- defN 23-May-15 12:09 secretflow/data/vertical/io.py
--rw-r--r--  2.0 unx      745 b- defN 23-May-15 12:09 secretflow/device/__init__.py
--rw-r--r--  2.0 unx    21823 b- defN 23-May-15 12:09 secretflow/device/driver.py
--rw-r--r--  2.0 unx     2981 b- defN 23-May-15 12:09 secretflow/device/global_state.py
--rw-r--r--  2.0 unx    10795 b- defN 23-May-15 12:09 secretflow/device/link.py
--rw-r--r--  2.0 unx     8100 b- defN 23-May-15 12:09 secretflow/device/proxy.py
--rw-r--r--  2.0 unx      939 b- defN 23-May-15 12:09 secretflow/device/device/__init__.py
--rw-r--r--  2.0 unx      889 b- defN 23-May-15 12:09 secretflow/device/device/_utils.py
--rw-r--r--  2.0 unx     2264 b- defN 23-May-15 12:09 secretflow/device/device/base.py
--rw-r--r--  2.0 unx    22932 b- defN 23-May-15 12:09 secretflow/device/device/heu.py
--rw-r--r--  2.0 unx     6096 b- defN 23-May-15 12:09 secretflow/device/device/heu_object.py
--rw-r--r--  2.0 unx     4693 b- defN 23-May-15 12:09 secretflow/device/device/pyu.py
--rw-r--r--  2.0 unx     3589 b- defN 23-May-15 12:09 secretflow/device/device/register.py
--rw-r--r--  2.0 unx    67451 b- defN 23-May-15 12:09 secretflow/device/device/spu.py
--rw-r--r--  2.0 unx     7667 b- defN 23-May-15 12:09 secretflow/device/device/teeu.py
--rw-r--r--  2.0 unx     2410 b- defN 23-May-15 12:09 secretflow/device/device/type_traits.py
--rw-r--r--  2.0 unx      638 b- defN 23-May-15 12:09 secretflow/device/kernels/__init__.py
--rw-r--r--  2.0 unx     5716 b- defN 23-May-15 12:09 secretflow/device/kernels/heu.py
--rw-r--r--  2.0 unx     6842 b- defN 23-May-15 12:09 secretflow/device/kernels/pyu.py
--rw-r--r--  2.0 unx    16767 b- defN 23-May-15 12:09 secretflow/device/kernels/spu.py
--rw-r--r--  2.0 unx      923 b- defN 23-May-15 12:09 secretflow/device/kernels/teeu.py
--rw-r--r--  2.0 unx      784 b- defN 23-May-15 12:09 secretflow/distributed/__init__.py
--rw-r--r--  2.0 unx     6373 b- defN 23-May-15 12:09 secretflow/distributed/primitive.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/kuscia/__init__.py
--rw-r--r--  2.0 unx     3722 b- defN 23-May-15 12:09 secretflow/kuscia/entry.py
--rw-r--r--  2.0 unx     5912 b- defN 23-May-15 12:09 secretflow/kuscia/task_config.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/__init__.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/boost/__init__.py
--rw-r--r--  2.0 unx      654 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/__init__.py
--rw-r--r--  2.0 unx     9580 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/homo_booster.py
--rw-r--r--  2.0 unx     7462 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/homo_booster_worker.py
--rw-r--r--  2.0 unx    11166 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/homo_decision_tree.py
--rw-r--r--  2.0 unx     3043 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_param.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/boost_core/__init__.py
--rw-r--r--  2.0 unx     4365 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/boost_core/callback.py
--rw-r--r--  2.0 unx     7200 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/boost_core/core.py
--rw-r--r--  2.0 unx     9292 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/boost_core/training.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_core/__init__.py
--rw-r--r--  2.0 unx     4429 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_core/criterion.py
--rw-r--r--  2.0 unx    18577 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_core/decision_tree.py
--rw-r--r--  2.0 unx     9371 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_core/feature_histogram.py
--rw-r--r--  2.0 unx     2535 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_core/feature_importance.py
--rw-r--r--  2.0 unx     4218 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_core/loss_function.py
--rw-r--r--  2.0 unx     2060 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_core/node.py
--rw-r--r--  2.0 unx     9846 b- defN 23-May-15 12:09 secretflow/ml/boost/homo_boost/tree_core/splitter.py
--rw-r--r--  2.0 unx      712 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/__init__.py
--rw-r--r--  2.0 unx     7826 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/model.py
--rw-r--r--  2.0 unx    19839 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/sgb.py
--rw-r--r--  2.0 unx      584 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/__init__.py
--rw-r--r--  2.0 unx      584 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/cache/__init__.py
--rw-r--r--  2.0 unx     2561 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/cache/level_cache.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/distributed_tree/__init__.py
--rw-r--r--  2.0 unx     3817 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/distributed_tree/distributed_tree.py
--rw-r--r--  2.0 unx     2767 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/distributed_tree/split_tree.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/label_holder/__init__.py
--rw-r--r--  2.0 unx     9416 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/label_holder/label_holder.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/preprocessing/__init__.py
--rw-r--r--  2.0 unx     1238 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/preprocessing/params.py
--rw-r--r--  2.0 unx     3355 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/preprocessing/preprocessing.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/boost.py
--rw-r--r--  2.0 unx     1724 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/bucket_sum.py
--rw-r--r--  2.0 unx      988 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/grad.py
--rw-r--r--  2.0 unx     2807 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/node_select.py
--rw-r--r--  2.0 unx     1466 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/pred.py
--rw-r--r--  2.0 unx      765 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/random.py
--rw-r--r--  2.0 unx      584 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/split_tree_trainer/__init__.py
--rw-r--r--  2.0 unx     4714 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/split_tree_trainer/order_map_context.py
--rw-r--r--  2.0 unx     2631 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/split_tree_trainer/shuffler.py
--rw-r--r--  2.0 unx     4166 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/split_tree_trainer/split_tree_trainer.py
--rw-r--r--  2.0 unx     5057 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/core/split_tree_trainer/splitter.py
--rw-r--r--  2.0 unx      644 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/__init__.py
--rw-r--r--  2.0 unx     4366 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/factory.py
--rw-r--r--  2.0 unx      683 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/booster/__init__.py
--rw-r--r--  2.0 unx     4272 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/booster/global_ordermap_booster.py
--rw-r--r--  2.0 unx      935 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/__init__.py
--rw-r--r--  2.0 unx     2073 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/component.py
--rw-r--r--  2.0 unx      676 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/__init__.py
--rw-r--r--  2.0 unx     4658 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/bucket_sum_calculator.py
--rw-r--r--  2.0 unx      661 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/cache/__init__.py
--rw-r--r--  2.0 unx     2051 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/cache/level_wise_cache.py
--rw-r--r--  2.0 unx      666 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/__init__.py
--rw-r--r--  2.0 unx     2503 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/data_preprocessor.py
--rw-r--r--  2.0 unx      669 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/__init__.py
--rw-r--r--  2.0 unx     4833 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/gradient_encryptor.py
--rw-r--r--  2.0 unx      651 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/__init__.py
--rw-r--r--  2.0 unx     1633 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/leaf_actor.py
--rw-r--r--  2.0 unx     2588 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/leaf_manager.py
--rw-r--r--  2.0 unx      654 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/loss_computer/__init__.py
--rw-r--r--  2.0 unx     2326 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/loss_computer/loss_computer.py
--rw-r--r--  2.0 unx      654 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/model_builder/__init__.py
--rw-r--r--  2.0 unx     2655 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/model_builder/model_builder.py
--rw-r--r--  2.0 unx      654 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/node_selector/__init__.py
--rw-r--r--  2.0 unx     4494 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/node_selector/node_selector.py
--rw-r--r--  2.0 unx      664 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/order_map_manager/__init__.py
--rw-r--r--  2.0 unx     4121 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/order_map_manager/order_map_actor.py
--rw-r--r--  2.0 unx     4280 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/order_map_manager/order_map_manager.py
--rw-r--r--  2.0 unx      638 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/sampler/__init__.py
--rw-r--r--  2.0 unx     7180 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/sampler/sampler.py
--rw-r--r--  2.0 unx      641 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/shuffler/__init__.py
--rw-r--r--  2.0 unx     2468 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/shuffler/shuffler.py
--rw-r--r--  2.0 unx     1721 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/shuffler/worker_shuffler.py
--rw-r--r--  2.0 unx      651 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/split_finder/__init__.py
--rw-r--r--  2.0 unx     3265 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/split_finder/split_finder.py
--rw-r--r--  2.0 unx      667 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_actor.py
--rw-r--r--  2.0 unx     6550 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_builder.py
--rw-r--r--  2.0 unx      147 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/tree_trainer/__init__.py
--rw-r--r--  2.0 unx    10486 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/tree_trainer/level_wise_tree_trainer.py
--rw-r--r--  2.0 unx     1142 b- defN 23-May-15 12:09 secretflow/ml/boost/sgb_v/factory/components/tree_trainer/tree_trainer.py
--rw-r--r--  2.0 unx      661 b- defN 23-May-15 12:09 secretflow/ml/boost/ss_xgb_v/__init__.py
--rw-r--r--  2.0 unx    19885 b- defN 23-May-15 12:09 secretflow/ml/boost/ss_xgb_v/model.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-15 12:09 secretflow/ml/boost/ss_xgb_v/core/__init__.py
--rw-r--r--  2.0 unx     8801 b- defN 23-May-15 12:09 secretflow/ml/boost/ss_xgb_v/core/node_split.py
--rw-r--r--  2.0 unx     9885 b- defN 23-May-15 12:09 secretflow/ml/boost/ss_xgb_v/core/tree_worker.py
--rw-r--r--  2.0 unx     1513 b- defN 23-May-15 12:09 secretflow/ml/boost/ss_xgb_v/core/utils.py
--rw-r--r--  2.0 unx      980 b- defN 23-May-15 12:09 secretflow/ml/boost/ss_xgb_v/core/xgb_tree.py
--rw-r--r--  2.0 unx     1013 b- defN 23-May-15 12:09 secretflow/ml/linear/__init__.py
--rw-r--r--  2.0 unx    11993 b- defN 23-May-15 12:09 secretflow/ml/linear/fl_lr_mix.py
--rw-r--r--  2.0 unx    19143 b- defN 23-May-15 12:09 secretflow/ml/linear/fl_lr_v.py
--rw-r--r--  2.0 unx     3129 b- defN 23-May-15 12:09 secretflow/ml/linear/linear_model.py
--rw-r--r--  2.0 unx      673 b- defN 23-May-15 12:09 secretflow/ml/linear/hess_sgd/__init__.py
--rw-r--r--  2.0 unx    13354 b- defN 23-May-15 12:09 secretflow/ml/linear/hess_sgd/model.py
--rw-r--r--  2.0 unx      639 b- defN 23-May-15 12:09 secretflow/ml/linear/ss_glm/__init__.py
--rw-r--r--  2.0 unx    23754 b- defN 23-May-15 12:09 secretflow/ml/linear/ss_glm/model.py
--rw-r--r--  2.0 unx      233 b- defN 23-May-15 12:09 secretflow/ml/linear/ss_glm/core/__init__.py
--rw-r--r--  2.0 unx     5287 b- defN 23-May-15 12:09 secretflow/ml/linear/ss_glm/core/distribution.py
--rw-r--r--  2.0 unx     2950 b- defN 23-May-15 12:09 secretflow/ml/linear/ss_glm/core/link.py
--rw-r--r--  2.0 unx      653 b- defN 23-May-15 12:09 secretflow/ml/linear/ss_sgd/__init__.py
--rw-r--r--  2.0 unx    21895 b- defN 23-May-15 12:09 secretflow/ml/linear/ss_sgd/model.py
--rw-r--r--  2.0 unx      698 b- defN 23-May-15 12:09 secretflow/ml/nn/__init__.py
--rw-r--r--  2.0 unx     8064 b- defN 23-May-15 12:09 secretflow/ml/nn/metrics.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/applications/__init__.py
--rw-r--r--  2.0 unx     5261 b- defN 23-May-15 12:09 secretflow/ml/nn/applications/sl_deep_fm.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/__init__.py
--rw-r--r--  2.0 unx     1743 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/compress.py
--rw-r--r--  2.0 unx    30837 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/fl_model.py
--rw-r--r--  2.0 unx     2152 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/strategy_dispatcher.py
--rw-r--r--  2.0 unx     3279 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/utils.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/__init__.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/__init__.py
--rw-r--r--  2.0 unx    12678 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/fl_base.py
--rw-r--r--  2.0 unx     4369 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/sampler.py
--rw-r--r--  2.0 unx      904 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/strategy/__init__.py
--rw-r--r--  2.0 unx     4073 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_g.py
--rw-r--r--  2.0 unx     4105 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_u.py
--rw-r--r--  2.0 unx     3834 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_w.py
--rw-r--r--  2.0 unx     4677 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_prox.py
--rw-r--r--  2.0 unx     5579 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_scr.py
--rw-r--r--  2.0 unx     5453 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_stc.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/__init__.py
--rw-r--r--  2.0 unx    13406 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/fl_base.py
--rw-r--r--  2.0 unx     3606 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/sampler.py
--rw-r--r--  2.0 unx     2710 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/utils.py
--rw-r--r--  2.0 unx      904 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/strategy/__init__.py
--rw-r--r--  2.0 unx     3482 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_g.py
--rw-r--r--  2.0 unx     3324 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_u.py
--rw-r--r--  2.0 unx     3381 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_w.py
--rw-r--r--  2.0 unx     3838 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/strategy/fed_prox.py
--rw-r--r--  2.0 unx     5266 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/strategy/fed_scr.py
--rw-r--r--  2.0 unx     5275 b- defN 23-May-15 12:09 secretflow/ml/nn/fl/backend/torch/strategy/fed_stc.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/__init__.py
--rw-r--r--  2.0 unx    28640 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/sl_model.py
--rw-r--r--  2.0 unx     2395 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/strategy_dispatcher.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/backend/__init__.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/backend/tensorflow/__init__.py
--rw-r--r--  2.0 unx    34424 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/backend/tensorflow/sl_base.py
--rw-r--r--  2.0 unx     4487 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/backend/tensorflow/utils.py
--rw-r--r--  2.0 unx      753 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/backend/tensorflow/strategy/__init__.py
--rw-r--r--  2.0 unx     6773 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/backend/tensorflow/strategy/split_async.py
--rw-r--r--  2.0 unx     5162 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/backend/tensorflow/strategy/split_state_async.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/ml/nn/sl/backend/torch/__init__.py
--rw-r--r--  2.0 unx      923 b- defN 23-May-15 12:09 secretflow/preprocessing/__init__.py
--rw-r--r--  2.0 unx     1231 b- defN 23-May-15 12:09 secretflow/preprocessing/base.py
--rw-r--r--  2.0 unx    11845 b- defN 23-May-15 12:09 secretflow/preprocessing/discretization.py
--rw-r--r--  2.0 unx    13154 b- defN 23-May-15 12:09 secretflow/preprocessing/encoder.py
--rw-r--r--  2.0 unx    14116 b- defN 23-May-15 12:09 secretflow/preprocessing/scaler.py
--rw-r--r--  2.0 unx     5162 b- defN 23-May-15 12:09 secretflow/preprocessing/transformer.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/__init__.py
--rw-r--r--  2.0 unx     7218 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/homo_binning.py
--rw-r--r--  2.0 unx    11274 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/homo_binning_base.py
--rw-r--r--  2.0 unx    10841 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/vert_woe_binning.py
--rw-r--r--  2.0 unx    22492 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/vert_woe_binning_pyu.py
--rw-r--r--  2.0 unx     3503 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/vert_woe_substitution.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/kernels/__init__.py
--rw-r--r--  2.0 unx     2524 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/kernels/base_binning.py
--rw-r--r--  2.0 unx     5291 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/kernels/quantile_binning.py
--rw-r--r--  2.0 unx     6517 b- defN 23-May-15 12:09 secretflow/preprocessing/binning/kernels/quantile_summaries.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/protos/__init__.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/protos/component/__init__.py
--rw-r--r--  2.0 unx    18614 b- defN 23-May-15 12:09 secretflow/protos/component/cluster_pb2.py
--rw-r--r--  2.0 unx    48160 b- defN 23-May-15 12:09 secretflow/protos/component/comp_def_pb2.py
--rw-r--r--  2.0 unx    12421 b- defN 23-May-15 12:09 secretflow/protos/component/data_def_pb2.py
--rw-r--r--  2.0 unx    11115 b- defN 23-May-15 12:09 secretflow/protos/component/evaluation_pb2.py
--rw-r--r--  2.0 unx    29124 b- defN 23-May-15 12:09 secretflow/protos/component/node_def_pb2.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/protos/kuscia/__init__.py
--rw-r--r--  2.0 unx    11123 b- defN 23-May-15 12:09 secretflow/protos/kuscia/kuscia_task_pb2.py
--rw-r--r--  2.0 unx      941 b- defN 23-May-15 12:09 secretflow/security/__init__.py
--rw-r--r--  2.0 unx    11579 b- defN 23-May-15 12:09 secretflow/security/diffie_hellman.py
--rw-r--r--  2.0 unx      946 b- defN 23-May-15 12:09 secretflow/security/aggregation/__init__.py
--rw-r--r--  2.0 unx     1039 b- defN 23-May-15 12:09 secretflow/security/aggregation/_utils.py
--rw-r--r--  2.0 unx     1072 b- defN 23-May-15 12:09 secretflow/security/aggregation/aggregator.py
--rw-r--r--  2.0 unx     4473 b- defN 23-May-15 12:09 secretflow/security/aggregation/plain_aggregator.py
--rw-r--r--  2.0 unx    12148 b- defN 23-May-15 12:09 secretflow/security/aggregation/secure_aggregator.py
--rw-r--r--  2.0 unx     5009 b- defN 23-May-15 12:09 secretflow/security/aggregation/sparse_plain_aggregator.py
--rw-r--r--  2.0 unx     4179 b- defN 23-May-15 12:09 secretflow/security/aggregation/spu_aggregator.py
--rw-r--r--  2.0 unx      858 b- defN 23-May-15 12:09 secretflow/security/compare/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 23-May-15 12:09 secretflow/security/compare/comparator.py
--rw-r--r--  2.0 unx     2220 b- defN 23-May-15 12:09 secretflow/security/compare/device_comparator.py
--rw-r--r--  2.0 unx     1871 b- defN 23-May-15 12:09 secretflow/security/compare/plain_comparator.py
--rw-r--r--  2.0 unx     1762 b- defN 23-May-15 12:09 secretflow/security/compare/spu_comparator.py
--rw-r--r--  2.0 unx      933 b- defN 23-May-15 12:09 secretflow/security/privacy/__init__.py
--rw-r--r--  2.0 unx  2221784 b- defN 23-May-15 12:12 secretflow/security/privacy/_lib.cpython-38-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     2749 b- defN 23-May-15 12:09 secretflow/security/privacy/strategy.py
--rw-r--r--  2.0 unx     1875 b- defN 23-May-15 12:09 secretflow/security/privacy/strategy_fl.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/security/privacy/accounting/__init__.py
--rw-r--r--  2.0 unx     2508 b- defN 23-May-15 12:09 secretflow/security/privacy/accounting/gdp_accountant.py
--rw-r--r--  2.0 unx     3670 b- defN 23-May-15 12:09 secretflow/security/privacy/accounting/log_utils.py
--rw-r--r--  2.0 unx     5702 b- defN 23-May-15 12:09 secretflow/security/privacy/accounting/rdp_accountant.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/security/privacy/mechanism/__init__.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/security/privacy/mechanism/tensorflow/__init__.py
--rw-r--r--  2.0 unx     6127 b- defN 23-May-15 12:09 secretflow/security/privacy/mechanism/tensorflow/layers.py
--rw-r--r--  2.0 unx     5251 b- defN 23-May-15 12:09 secretflow/security/privacy/mechanism/tensorflow/mechanism_fl.py
--rw-r--r--  2.0 unx     1159 b- defN 23-May-15 12:09 secretflow/stats/__init__.py
--rw-r--r--  2.0 unx     4042 b- defN 23-May-15 12:09 secretflow/stats/biclassification_eval.py
--rw-r--r--  2.0 unx     2386 b- defN 23-May-15 12:09 secretflow/stats/psi_eval.py
--rw-r--r--  2.0 unx     2751 b- defN 23-May-15 12:09 secretflow/stats/pva_eval.py
--rw-r--r--  2.0 unx     2995 b- defN 23-May-15 12:09 secretflow/stats/regression_eval.py
--rw-r--r--  2.0 unx     4421 b- defN 23-May-15 12:09 secretflow/stats/score_card.py
--rw-r--r--  2.0 unx     2421 b- defN 23-May-15 12:09 secretflow/stats/ss_pearsonr_v.py
--rw-r--r--  2.0 unx     7265 b- defN 23-May-15 12:09 secretflow/stats/ss_pvalue_v.py
--rw-r--r--  2.0 unx     3631 b- defN 23-May-15 12:09 secretflow/stats/ss_vif_v.py
--rw-r--r--  2.0 unx     3262 b- defN 23-May-15 12:09 secretflow/stats/table_statistics.py
--rw-r--r--  2.0 unx      726 b- defN 23-May-15 12:09 secretflow/stats/core/__init__.py
--rw-r--r--  2.0 unx    20039 b- defN 23-May-15 12:09 secretflow/stats/core/biclassification_eval_core.py
--rw-r--r--  2.0 unx     2802 b- defN 23-May-15 12:09 secretflow/stats/core/psi_core.py
--rw-r--r--  2.0 unx     1665 b- defN 23-May-15 12:09 secretflow/stats/core/pva_core.py
--rw-r--r--  2.0 unx     1776 b- defN 23-May-15 12:09 secretflow/stats/core/utils.py
--rw-r--r--  2.0 unx      662 b- defN 23-May-15 12:09 secretflow/utils/__init__.py
--rw-r--r--  2.0 unx    13370 b- defN 23-May-15 12:09 secretflow/utils/cloudpickle.py
--rw-r--r--  2.0 unx    11236 b- defN 23-May-15 12:09 secretflow/utils/compressor.py
--rw-r--r--  2.0 unx     1084 b- defN 23-May-15 12:09 secretflow/utils/errors.py
--rw-r--r--  2.0 unx      870 b- defN 23-May-15 12:09 secretflow/utils/hash.py
--rw-r--r--  2.0 unx      978 b- defN 23-May-15 12:09 secretflow/utils/io.py
--rw-r--r--  2.0 unx      964 b- defN 23-May-15 12:09 secretflow/utils/logging.py
--rw-r--r--  2.0 unx     2842 b- defN 23-May-15 12:09 secretflow/utils/ndarray_bigint.py
--rw-r--r--  2.0 unx     2489 b- defN 23-May-15 12:09 secretflow/utils/ndarray_encoding.py
--rw-r--r--  2.0 unx      803 b- defN 23-May-15 12:09 secretflow/utils/random.py
--rw-r--r--  2.0 unx     1330 b- defN 23-May-15 12:09 secretflow/utils/ray_compatibility.py
--rw-r--r--  2.0 unx     3930 b- defN 23-May-15 12:09 secretflow/utils/sigmoid.py
--rw-r--r--  2.0 unx     3308 b- defN 23-May-15 12:09 secretflow/utils/testing.py
--rw-r--r--  2.0 unx      585 b- defN 23-May-15 12:09 secretflow/utils/simulation/__init__.py
--rw-r--r--  2.0 unx    30745 b- defN 23-May-15 12:09 secretflow/utils/simulation/datasets.py
--rw-r--r--  2.0 unx     8941 b- defN 23-May-15 12:09 secretflow/utils/simulation/tf_gnn_model.py
--rw-r--r--  2.0 unx      769 b- defN 23-May-15 12:09 secretflow/utils/simulation/data/__init__.py
--rw-r--r--  2.0 unx     2548 b- defN 23-May-15 12:09 secretflow/utils/simulation/data/_utils.py
--rw-r--r--  2.0 unx     5389 b- defN 23-May-15 12:09 secretflow/utils/simulation/data/dataframe.py
--rw-r--r--  2.0 unx     4093 b- defN 23-May-15 12:09 secretflow/utils/simulation/data/ndarray.py
--rw-r--r--  2.0 unx    11356 b- defN 23-May-15 12:12 secretflow-0.8.2b3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4171 b- defN 23-May-15 12:12 secretflow-0.8.2b3.dist-info/METADATA
--rw-r--r--  2.0 unx      111 b- defN 23-May-15 12:12 secretflow-0.8.2b3.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-15 12:12 secretflow-0.8.2b3.dist-info/dependency_links.txt
--rw-r--r--  2.0 unx       50 b- defN 23-May-15 12:12 secretflow-0.8.2b3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       44 b- defN 23-May-15 12:12 secretflow-0.8.2b3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    30260 b- defN 23-May-15 12:12 secretflow-0.8.2b3.dist-info/RECORD
-295 files, 3805087 bytes uncompressed, 1238635 bytes compressed:  67.4%
+Zip file size: 1627745 bytes, number of entries: 341
+-rw-r--r--  2.0 unx     1321 b- defN 23-Jun-14 07:48 secretflow/__init__.py
+-rw-r--r--  2.0 unx     6478 b- defN 23-Jun-14 07:48 secretflow/cli.py
+-rw-r--r--  2.0 unx      607 b- defN 23-Jun-14 07:48 secretflow/version.py
+-rw-r--r--  2.0 unx      635 b- defN 23-Jun-14 07:48 secretflow/component/__init__.py
+-rw-r--r--  2.0 unx      628 b- defN 23-Jun-14 07:48 secretflow/component/__main__.py
+-rw-r--r--  2.0 unx    30621 b- defN 23-Jun-14 07:48 secretflow/component/component.py
+-rw-r--r--  2.0 unx    16205 b- defN 23-Jun-14 07:48 secretflow/component/data_utils.py
+-rw-r--r--  2.0 unx     3791 b- defN 23-Jun-14 07:48 secretflow/component/entry.py
+-rw-r--r--  2.0 unx     9676 b- defN 23-Jun-14 07:48 secretflow/component/eval_param_reader.py
+-rw-r--r--  2.0 unx     3377 b- defN 23-Jun-14 07:48 secretflow/component/i18n.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/component/ml/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/component/ml/boost/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/component/ml/boost/sgb/__init__.py
+-rw-r--r--  2.0 unx    12463 b- defN 23-Jun-14 07:48 secretflow/component/ml/boost/sgb/sgb.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/component/ml/boost/ss_xgb/__init__.py
+-rw-r--r--  2.0 unx    11692 b- defN 23-Jun-14 07:48 secretflow/component/ml/boost/ss_xgb/ss_xgb.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/component/ml/linear/__init__.py
+-rw-r--r--  2.0 unx    10564 b- defN 23-Jun-14 07:48 secretflow/component/ml/linear/ss_sgd.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/component/preprocessing/__init__.py
+-rw-r--r--  2.0 unx     2640 b- defN 23-Jun-14 07:48 secretflow/component/preprocessing/feature_filter.py
+-rw-r--r--  2.0 unx     3652 b- defN 23-Jun-14 07:48 secretflow/component/preprocessing/train_test_split.py
+-rw-r--r--  2.0 unx     8532 b- defN 23-Jun-14 07:48 secretflow/component/preprocessing/vert_woe_binning.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/component/psi/__init__.py
+-rw-r--r--  2.0 unx     7598 b- defN 23-Jun-14 07:48 secretflow/component/psi/two_party_balanced.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/component/stats/__init__.py
+-rw-r--r--  2.0 unx    13594 b- defN 23-Jun-14 07:48 secretflow/component/stats/biclassification_eval.py
+-rw-r--r--  2.0 unx     2137 b- defN 23-Jun-14 07:48 secretflow/component/stats/pva_eval.py
+-rw-r--r--  2.0 unx     3843 b- defN 23-Jun-14 07:48 secretflow/component/stats/ss_pearsonr.py
+-rw-r--r--  2.0 unx     3750 b- defN 23-Jun-14 07:48 secretflow/component/stats/ss_pvalue.py
+-rw-r--r--  2.0 unx     3626 b- defN 23-Jun-14 07:48 secretflow/component/stats/ss_vif.py
+-rw-r--r--  2.0 unx     2035 b- defN 23-Jun-14 07:48 secretflow/component/stats/table_statistics.py
+-rw-r--r--  2.0 unx      754 b- defN 23-Jun-14 07:48 secretflow/data/__init__.py
+-rw-r--r--  2.0 unx    14806 b- defN 23-Jun-14 07:48 secretflow/data/base.py
+-rw-r--r--  2.0 unx     1108 b- defN 23-Jun-14 07:48 secretflow/data/math_utils.py
+-rw-r--r--  2.0 unx    24878 b- defN 23-Jun-14 07:48 secretflow/data/ndarray.py
+-rw-r--r--  2.0 unx     5420 b- defN 23-Jun-14 07:48 secretflow/data/split.py
+-rw-r--r--  2.0 unx      694 b- defN 23-Jun-14 07:48 secretflow/data/horizontal/__init__.py
+-rw-r--r--  2.0 unx    15042 b- defN 23-Jun-14 07:48 secretflow/data/horizontal/dataframe.py
+-rw-r--r--  2.0 unx     2135 b- defN 23-Jun-14 07:48 secretflow/data/horizontal/io.py
+-rw-r--r--  2.0 unx     1555 b- defN 23-Jun-14 07:48 secretflow/data/horizontal/sampler.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-14 07:48 secretflow/data/io/__init__.py
+-rw-r--r--  2.0 unx     2112 b- defN 23-Jun-14 07:48 secretflow/data/io/oss.py
+-rw-r--r--  2.0 unx     2501 b- defN 23-Jun-14 07:48 secretflow/data/io/util.py
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-14 07:48 secretflow/data/mix/__init__.py
+-rw-r--r--  2.0 unx    15054 b- defN 23-Jun-14 07:48 secretflow/data/mix/dataframe.py
+-rw-r--r--  2.0 unx      694 b- defN 23-Jun-14 07:48 secretflow/data/vertical/__init__.py
+-rw-r--r--  2.0 unx    22944 b- defN 23-Jun-14 07:48 secretflow/data/vertical/dataframe.py
+-rw-r--r--  2.0 unx     6550 b- defN 23-Jun-14 07:48 secretflow/data/vertical/io.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Jun-14 07:48 secretflow/device/__init__.py
+-rw-r--r--  2.0 unx    22241 b- defN 23-Jun-14 07:48 secretflow/device/driver.py
+-rw-r--r--  2.0 unx     2981 b- defN 23-Jun-14 07:48 secretflow/device/global_state.py
+-rw-r--r--  2.0 unx    10795 b- defN 23-Jun-14 07:48 secretflow/device/link.py
+-rw-r--r--  2.0 unx     8100 b- defN 23-Jun-14 07:48 secretflow/device/proxy.py
+-rw-r--r--  2.0 unx      939 b- defN 23-Jun-14 07:48 secretflow/device/device/__init__.py
+-rw-r--r--  2.0 unx      889 b- defN 23-Jun-14 07:48 secretflow/device/device/_utils.py
+-rw-r--r--  2.0 unx     2264 b- defN 23-Jun-14 07:48 secretflow/device/device/base.py
+-rw-r--r--  2.0 unx    23141 b- defN 23-Jun-14 07:48 secretflow/device/device/heu.py
+-rw-r--r--  2.0 unx     6881 b- defN 23-Jun-14 07:48 secretflow/device/device/heu_object.py
+-rw-r--r--  2.0 unx     4706 b- defN 23-Jun-14 07:48 secretflow/device/device/pyu.py
+-rw-r--r--  2.0 unx     3589 b- defN 23-Jun-14 07:48 secretflow/device/device/register.py
+-rw-r--r--  2.0 unx    76168 b- defN 23-Jun-14 07:48 secretflow/device/device/spu.py
+-rw-r--r--  2.0 unx     7667 b- defN 23-Jun-14 07:48 secretflow/device/device/teeu.py
+-rw-r--r--  2.0 unx     2410 b- defN 23-Jun-14 07:48 secretflow/device/device/type_traits.py
+-rw-r--r--  2.0 unx      638 b- defN 23-Jun-14 07:48 secretflow/device/kernels/__init__.py
+-rw-r--r--  2.0 unx     5716 b- defN 23-Jun-14 07:48 secretflow/device/kernels/heu.py
+-rw-r--r--  2.0 unx     6842 b- defN 23-Jun-14 07:48 secretflow/device/kernels/pyu.py
+-rw-r--r--  2.0 unx    17619 b- defN 23-Jun-14 07:48 secretflow/device/kernels/spu.py
+-rw-r--r--  2.0 unx      923 b- defN 23-Jun-14 07:48 secretflow/device/kernels/teeu.py
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-14 07:48 secretflow/distributed/__init__.py
+-rw-r--r--  2.0 unx     6373 b- defN 23-Jun-14 07:48 secretflow/distributed/primitive.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/kuscia/__init__.py
+-rw-r--r--  2.0 unx     2380 b- defN 23-Jun-14 07:48 secretflow/kuscia/entry.py
+-rw-r--r--  2.0 unx     3651 b- defN 23-Jun-14 07:48 secretflow/kuscia/ray_config.py
+-rw-r--r--  2.0 unx     4495 b- defN 23-Jun-14 07:48 secretflow/kuscia/sf_config.py
+-rw-r--r--  2.0 unx     3229 b- defN 23-Jun-14 07:48 secretflow/kuscia/task_config.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/kuscia/proto/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/kuscia/proto/api/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/kuscia/proto/api/v1alpha1/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/kuscia/proto/api/v1alpha1/kusciatask/__init__.py
+-rw-r--r--  2.0 unx    11973 b- defN 23-Jun-14 07:48 secretflow/kuscia/proto/api/v1alpha1/kusciatask/kuscia_task_pb2.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/core/__init__.py
+-rw-r--r--  2.0 unx     2827 b- defN 23-Jun-14 07:48 secretflow/ml/boost/core/data_preprocess.py
+-rw-r--r--  2.0 unx     3161 b- defN 23-Jun-14 07:48 secretflow/ml/boost/core/order_map_tools.py
+-rw-r--r--  2.0 unx      654 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/__init__.py
+-rw-r--r--  2.0 unx     9580 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/homo_booster.py
+-rw-r--r--  2.0 unx     7462 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/homo_booster_worker.py
+-rw-r--r--  2.0 unx    11134 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/homo_decision_tree.py
+-rw-r--r--  2.0 unx     3043 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_param.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/boost_core/__init__.py
+-rw-r--r--  2.0 unx     4365 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/boost_core/callback.py
+-rw-r--r--  2.0 unx     7248 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/boost_core/core.py
+-rw-r--r--  2.0 unx     9292 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/boost_core/training.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_core/__init__.py
+-rw-r--r--  2.0 unx     4429 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_core/criterion.py
+-rw-r--r--  2.0 unx    18576 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_core/decision_tree.py
+-rw-r--r--  2.0 unx     9371 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_core/feature_histogram.py
+-rw-r--r--  2.0 unx     2535 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_core/feature_importance.py
+-rw-r--r--  2.0 unx     4218 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_core/loss_function.py
+-rw-r--r--  2.0 unx     2060 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_core/node.py
+-rw-r--r--  2.0 unx     9846 b- defN 23-Jun-14 07:48 secretflow/ml/boost/homo_boost/tree_core/splitter.py
+-rw-r--r--  2.0 unx      712 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/__init__.py
+-rw-r--r--  2.0 unx     7830 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/model.py
+-rw-r--r--  2.0 unx    19455 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/sgb.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/cache/__init__.py
+-rw-r--r--  2.0 unx     2642 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/cache/level_cache.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/distributed_tree/__init__.py
+-rw-r--r--  2.0 unx     3817 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/distributed_tree/distributed_tree.py
+-rw-r--r--  2.0 unx     2768 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/distributed_tree/split_tree.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/label_holder/__init__.py
+-rw-r--r--  2.0 unx     9642 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/label_holder/label_holder.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/preprocessing/__init__.py
+-rw-r--r--  2.0 unx     1238 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/preprocessing/params.py
+-rw-r--r--  2.0 unx     2432 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/preprocessing/preprocessing.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/__init__.py
+-rw-r--r--  2.0 unx     3706 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/boost.py
+-rw-r--r--  2.0 unx     1724 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/bucket_sum.py
+-rw-r--r--  2.0 unx      988 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/grad.py
+-rw-r--r--  2.0 unx     2807 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/node_select.py
+-rw-r--r--  2.0 unx     1465 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/pred.py
+-rw-r--r--  2.0 unx      765 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/random.py
+-rw-r--r--  2.0 unx      584 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/split_tree_trainer/__init__.py
+-rw-r--r--  2.0 unx     2840 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/split_tree_trainer/order_map_context.py
+-rw-r--r--  2.0 unx     2787 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/split_tree_trainer/shuffler.py
+-rw-r--r--  2.0 unx     4166 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/split_tree_trainer/split_tree_trainer.py
+-rw-r--r--  2.0 unx     5057 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/core/split_tree_trainer/splitter.py
+-rw-r--r--  2.0 unx      644 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/__init__.py
+-rw-r--r--  2.0 unx     4329 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/factory.py
+-rw-r--r--  2.0 unx      683 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/booster/__init__.py
+-rw-r--r--  2.0 unx     5409 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/booster/global_ordermap_booster.py
+-rw-r--r--  2.0 unx      983 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/__init__.py
+-rw-r--r--  2.0 unx     2010 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/component.py
+-rw-r--r--  2.0 unx     3194 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/logging.py
+-rw-r--r--  2.0 unx      780 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/__init__.py
+-rw-r--r--  2.0 unx     4960 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/bucket_sum_calculator.py
+-rw-r--r--  2.0 unx     5176 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/leaf_wise_bucket_sum_calculator.py
+-rw-r--r--  2.0 unx      661 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/cache/__init__.py
+-rw-r--r--  2.0 unx     2051 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/cache/level_wise_cache.py
+-rw-r--r--  2.0 unx     1893 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/cache/node_bucket_sum_cache_internal.py
+-rw-r--r--  2.0 unx     2583 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/cache/node_wise_bucket_sum_cache.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/__init__.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/data_preprocessor.py
+-rw-r--r--  2.0 unx      669 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/__init__.py
+-rw-r--r--  2.0 unx     5190 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/gradient_encryptor.py
+-rw-r--r--  2.0 unx      651 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/__init__.py
+-rw-r--r--  2.0 unx     1633 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/leaf_actor.py
+-rw-r--r--  2.0 unx     2588 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/leaf_manager.py
+-rw-r--r--  2.0 unx      654 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/loss_computer/__init__.py
+-rw-r--r--  2.0 unx     2651 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/loss_computer/loss_computer.py
+-rw-r--r--  2.0 unx      654 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/model_builder/__init__.py
+-rw-r--r--  2.0 unx     2655 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/model_builder/model_builder.py
+-rw-r--r--  2.0 unx      654 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/node_selector/__init__.py
+-rw-r--r--  2.0 unx     5865 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/node_selector/node_selector.py
+-rw-r--r--  2.0 unx      664 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/order_map_manager/__init__.py
+-rw-r--r--  2.0 unx     4121 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/order_map_manager/order_map_actor.py
+-rw-r--r--  2.0 unx     4649 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/order_map_manager/order_map_manager.py
+-rw-r--r--  2.0 unx      638 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/sampler/__init__.py
+-rw-r--r--  2.0 unx     8221 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/sampler/sampler.py
+-rw-r--r--  2.0 unx      641 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/shuffler/__init__.py
+-rw-r--r--  2.0 unx     3498 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/shuffler/shuffler.py
+-rw-r--r--  2.0 unx     2057 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/shuffler/worker_shuffler.py
+-rw-r--r--  2.0 unx      716 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/split_candidate_manager/__init__.py
+-rw-r--r--  2.0 unx     5248 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/split_candidate_manager/split_candidate_manager.py
+-rw-r--r--  2.0 unx      651 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/split_finder/__init__.py
+-rw-r--r--  2.0 unx     3339 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/split_finder/leaf_wise_split_finder.py
+-rw-r--r--  2.0 unx     4252 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/split_finder/split_finder.py
+-rw-r--r--  2.0 unx      667 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_actor.py
+-rw-r--r--  2.0 unx     6969 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_builder.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/tree_trainer/__init__.py
+-rw-r--r--  2.0 unx    12111 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/tree_trainer/leaf_wise_tree_trainer.py
+-rw-r--r--  2.0 unx    10901 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/tree_trainer/level_wise_tree_trainer.py
+-rw-r--r--  2.0 unx     1141 b- defN 23-Jun-14 07:48 secretflow/ml/boost/sgb_v/factory/components/tree_trainer/tree_trainer.py
+-rw-r--r--  2.0 unx      661 b- defN 23-Jun-14 07:48 secretflow/ml/boost/ss_xgb_v/__init__.py
+-rw-r--r--  2.0 unx    19627 b- defN 23-Jun-14 07:48 secretflow/ml/boost/ss_xgb_v/model.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-14 07:48 secretflow/ml/boost/ss_xgb_v/core/__init__.py
+-rw-r--r--  2.0 unx     8801 b- defN 23-Jun-14 07:48 secretflow/ml/boost/ss_xgb_v/core/node_split.py
+-rw-r--r--  2.0 unx     7747 b- defN 23-Jun-14 07:48 secretflow/ml/boost/ss_xgb_v/core/tree_worker.py
+-rw-r--r--  2.0 unx      980 b- defN 23-Jun-14 07:48 secretflow/ml/boost/ss_xgb_v/core/xgb_tree.py
+-rw-r--r--  2.0 unx     1013 b- defN 23-Jun-14 07:48 secretflow/ml/linear/__init__.py
+-rw-r--r--  2.0 unx    12354 b- defN 23-Jun-14 07:48 secretflow/ml/linear/fl_lr_mix.py
+-rw-r--r--  2.0 unx    19143 b- defN 23-Jun-14 07:48 secretflow/ml/linear/fl_lr_v.py
+-rw-r--r--  2.0 unx     1373 b- defN 23-Jun-14 07:48 secretflow/ml/linear/linear_model.py
+-rw-r--r--  2.0 unx      673 b- defN 23-Jun-14 07:48 secretflow/ml/linear/hess_sgd/__init__.py
+-rw-r--r--  2.0 unx    13354 b- defN 23-Jun-14 07:48 secretflow/ml/linear/hess_sgd/model.py
+-rw-r--r--  2.0 unx      639 b- defN 23-Jun-14 07:48 secretflow/ml/linear/ss_glm/__init__.py
+-rw-r--r--  2.0 unx    23754 b- defN 23-Jun-14 07:48 secretflow/ml/linear/ss_glm/model.py
+-rw-r--r--  2.0 unx      233 b- defN 23-Jun-14 07:48 secretflow/ml/linear/ss_glm/core/__init__.py
+-rw-r--r--  2.0 unx     5287 b- defN 23-Jun-14 07:48 secretflow/ml/linear/ss_glm/core/distribution.py
+-rw-r--r--  2.0 unx     2950 b- defN 23-Jun-14 07:48 secretflow/ml/linear/ss_glm/core/link.py
+-rw-r--r--  2.0 unx      653 b- defN 23-Jun-14 07:48 secretflow/ml/linear/ss_sgd/__init__.py
+-rw-r--r--  2.0 unx    21895 b- defN 23-Jun-14 07:48 secretflow/ml/linear/ss_sgd/model.py
+-rw-r--r--  2.0 unx      698 b- defN 23-Jun-14 07:48 secretflow/ml/nn/__init__.py
+-rw-r--r--  2.0 unx     8067 b- defN 23-Jun-14 07:48 secretflow/ml/nn/metrics.py
+-rw-r--r--  2.0 unx     3018 b- defN 23-Jun-14 07:48 secretflow/ml/nn/utils.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/applications/__init__.py
+-rw-r--r--  2.0 unx     5261 b- defN 23-Jun-14 07:48 secretflow/ml/nn/applications/sl_deep_fm.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/__init__.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/compress.py
+-rw-r--r--  2.0 unx    30826 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/fl_model.py
+-rw-r--r--  2.0 unx     2152 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/strategy_dispatcher.py
+-rw-r--r--  2.0 unx     3279 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/utils.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/__init__.py
+-rw-r--r--  2.0 unx    12678 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/fl_base.py
+-rw-r--r--  2.0 unx     4369 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/sampler.py
+-rw-r--r--  2.0 unx      904 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/strategy/__init__.py
+-rw-r--r--  2.0 unx     4071 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_g.py
+-rw-r--r--  2.0 unx     4105 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_u.py
+-rw-r--r--  2.0 unx     3834 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_w.py
+-rw-r--r--  2.0 unx     4677 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_prox.py
+-rw-r--r--  2.0 unx     5579 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_scr.py
+-rw-r--r--  2.0 unx     5453 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_stc.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/__init__.py
+-rw-r--r--  2.0 unx    13393 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/fl_base.py
+-rw-r--r--  2.0 unx     3605 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/sampler.py
+-rw-r--r--  2.0 unx      904 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/strategy/__init__.py
+-rw-r--r--  2.0 unx     3482 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_g.py
+-rw-r--r--  2.0 unx     3324 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_u.py
+-rw-r--r--  2.0 unx     3381 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_w.py
+-rw-r--r--  2.0 unx     3838 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/strategy/fed_prox.py
+-rw-r--r--  2.0 unx     5249 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/strategy/fed_scr.py
+-rw-r--r--  2.0 unx     5258 b- defN 23-Jun-14 07:48 secretflow/ml/nn/fl/backend/torch/strategy/fed_stc.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/__init__.py
+-rw-r--r--  2.0 unx    30239 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/sl_model.py
+-rw-r--r--  2.0 unx     2395 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/strategy_dispatcher.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/agglayer/__init__.py
+-rw-r--r--  2.0 unx    15812 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/agglayer/agg_layer.py
+-rw-r--r--  2.0 unx     3432 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/agglayer/agg_method.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/tensorflow/__init__.py
+-rw-r--r--  2.0 unx    27575 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/tensorflow/sl_base.py
+-rw-r--r--  2.0 unx     4487 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/tensorflow/utils.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/tensorflow/strategy/__init__.py
+-rw-r--r--  2.0 unx     6210 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/tensorflow/strategy/split_async.py
+-rw-r--r--  2.0 unx     5140 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/tensorflow/strategy/split_state_async.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/torch/__init__.py
+-rw-r--r--  2.0 unx    24467 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/torch/sl_base.py
+-rw-r--r--  2.0 unx      652 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/torch/strategy/__init__.py
+-rw-r--r--  2.0 unx     3569 b- defN 23-Jun-14 07:48 secretflow/ml/nn/sl/backend/torch/strategy/split_nn.py
+-rw-r--r--  2.0 unx      923 b- defN 23-Jun-14 07:48 secretflow/preprocessing/__init__.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Jun-14 07:48 secretflow/preprocessing/base.py
+-rw-r--r--  2.0 unx    11845 b- defN 23-Jun-14 07:48 secretflow/preprocessing/discretization.py
+-rw-r--r--  2.0 unx    13154 b- defN 23-Jun-14 07:48 secretflow/preprocessing/encoder.py
+-rw-r--r--  2.0 unx    14116 b- defN 23-Jun-14 07:48 secretflow/preprocessing/scaler.py
+-rw-r--r--  2.0 unx     5162 b- defN 23-Jun-14 07:48 secretflow/preprocessing/transformer.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/__init__.py
+-rw-r--r--  2.0 unx     7218 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/homo_binning.py
+-rw-r--r--  2.0 unx    11274 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/homo_binning_base.py
+-rw-r--r--  2.0 unx    12444 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/vert_woe_binning.py
+-rw-r--r--  2.0 unx    24664 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/vert_woe_binning_pyu.py
+-rw-r--r--  2.0 unx     3503 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/vert_woe_substitution.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/kernels/__init__.py
+-rw-r--r--  2.0 unx     2524 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/kernels/base_binning.py
+-rw-r--r--  2.0 unx     5281 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/kernels/chi_merge.py
+-rw-r--r--  2.0 unx     5291 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/kernels/quantile_binning.py
+-rw-r--r--  2.0 unx     6517 b- defN 23-Jun-14 07:48 secretflow/preprocessing/binning/kernels/quantile_summaries.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/protos/__init__.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/protos/component/__init__.py
+-rw-r--r--  2.0 unx    22818 b- defN 23-Jun-14 07:48 secretflow/protos/component/cluster_pb2.py
+-rw-r--r--  2.0 unx    35269 b- defN 23-Jun-14 07:48 secretflow/protos/component/comp_pb2.py
+-rw-r--r--  2.0 unx    19380 b- defN 23-Jun-14 07:48 secretflow/protos/component/data_pb2.py
+-rw-r--r--  2.0 unx     7199 b- defN 23-Jun-14 07:48 secretflow/protos/component/evaluation_pb2.py
+-rw-r--r--  2.0 unx    24482 b- defN 23-Jun-14 07:48 secretflow/protos/component/report_pb2.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/protos/pipeline/__init__.py
+-rw-r--r--  2.0 unx    13293 b- defN 23-Jun-14 07:48 secretflow/protos/pipeline/pipeline_pb2.py
+-rw-r--r--  2.0 unx      941 b- defN 23-Jun-14 07:48 secretflow/security/__init__.py
+-rw-r--r--  2.0 unx    11579 b- defN 23-Jun-14 07:48 secretflow/security/diffie_hellman.py
+-rw-r--r--  2.0 unx      946 b- defN 23-Jun-14 07:48 secretflow/security/aggregation/__init__.py
+-rw-r--r--  2.0 unx     1039 b- defN 23-Jun-14 07:48 secretflow/security/aggregation/_utils.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jun-14 07:48 secretflow/security/aggregation/aggregator.py
+-rw-r--r--  2.0 unx     4474 b- defN 23-Jun-14 07:48 secretflow/security/aggregation/plain_aggregator.py
+-rw-r--r--  2.0 unx    12148 b- defN 23-Jun-14 07:48 secretflow/security/aggregation/secure_aggregator.py
+-rw-r--r--  2.0 unx     5009 b- defN 23-Jun-14 07:48 secretflow/security/aggregation/sparse_plain_aggregator.py
+-rw-r--r--  2.0 unx     4179 b- defN 23-Jun-14 07:48 secretflow/security/aggregation/spu_aggregator.py
+-rw-r--r--  2.0 unx      858 b- defN 23-Jun-14 07:48 secretflow/security/compare/__init__.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-14 07:48 secretflow/security/compare/comparator.py
+-rw-r--r--  2.0 unx     2220 b- defN 23-Jun-14 07:48 secretflow/security/compare/device_comparator.py
+-rw-r--r--  2.0 unx     1871 b- defN 23-Jun-14 07:48 secretflow/security/compare/plain_comparator.py
+-rw-r--r--  2.0 unx     1762 b- defN 23-Jun-14 07:48 secretflow/security/compare/spu_comparator.py
+-rw-r--r--  2.0 unx      948 b- defN 23-Jun-14 07:48 secretflow/security/privacy/__init__.py
+-rw-r--r--  2.0 unx  2208676 b- defN 23-Jun-14 07:51 secretflow/security/privacy/_lib.cpython-38-darwin.so
+-rw-r--r--  2.0 unx     3012 b- defN 23-Jun-14 07:48 secretflow/security/privacy/strategy.py
+-rw-r--r--  2.0 unx     1855 b- defN 23-Jun-14 07:48 secretflow/security/privacy/strategy_fl.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/security/privacy/accounting/__init__.py
+-rw-r--r--  2.0 unx     1814 b- defN 23-Jun-14 07:48 secretflow/security/privacy/accounting/budget_accountant.py
+-rw-r--r--  2.0 unx     2508 b- defN 23-Jun-14 07:48 secretflow/security/privacy/accounting/gdp_accountant.py
+-rw-r--r--  2.0 unx     3670 b- defN 23-Jun-14 07:48 secretflow/security/privacy/accounting/log_utils.py
+-rw-r--r--  2.0 unx     5702 b- defN 23-Jun-14 07:48 secretflow/security/privacy/accounting/rdp_accountant.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/security/privacy/mechanism/__init__.py
+-rw-r--r--  2.0 unx     2167 b- defN 23-Jun-14 07:48 secretflow/security/privacy/mechanism/label_dp.py
+-rw-r--r--  2.0 unx     5420 b- defN 23-Jun-14 07:48 secretflow/security/privacy/mechanism/mechanism_fl.py
+-rw-r--r--  2.0 unx      668 b- defN 23-Jun-14 07:48 secretflow/security/privacy/mechanism/tensorflow/__init__.py
+-rw-r--r--  2.0 unx     2750 b- defN 23-Jun-14 07:48 secretflow/security/privacy/mechanism/tensorflow/layers.py
+-rw-r--r--  2.0 unx      668 b- defN 23-Jun-14 07:48 secretflow/security/privacy/mechanism/torch/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 23-Jun-14 07:48 secretflow/security/privacy/mechanism/torch/layers.py
+-rw-r--r--  2.0 unx     1159 b- defN 23-Jun-14 07:48 secretflow/stats/__init__.py
+-rw-r--r--  2.0 unx     4042 b- defN 23-Jun-14 07:48 secretflow/stats/biclassification_eval.py
+-rw-r--r--  2.0 unx     2386 b- defN 23-Jun-14 07:48 secretflow/stats/psi_eval.py
+-rw-r--r--  2.0 unx     2820 b- defN 23-Jun-14 07:48 secretflow/stats/pva_eval.py
+-rw-r--r--  2.0 unx     2995 b- defN 23-Jun-14 07:48 secretflow/stats/regression_eval.py
+-rw-r--r--  2.0 unx     4421 b- defN 23-Jun-14 07:48 secretflow/stats/score_card.py
+-rw-r--r--  2.0 unx     2421 b- defN 23-Jun-14 07:48 secretflow/stats/ss_pearsonr_v.py
+-rw-r--r--  2.0 unx     7265 b- defN 23-Jun-14 07:48 secretflow/stats/ss_pvalue_v.py
+-rw-r--r--  2.0 unx     3631 b- defN 23-Jun-14 07:48 secretflow/stats/ss_vif_v.py
+-rw-r--r--  2.0 unx     3262 b- defN 23-Jun-14 07:48 secretflow/stats/table_statistics.py
+-rw-r--r--  2.0 unx      726 b- defN 23-Jun-14 07:48 secretflow/stats/core/__init__.py
+-rw-r--r--  2.0 unx    20017 b- defN 23-Jun-14 07:48 secretflow/stats/core/biclassification_eval_core.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-Jun-14 07:48 secretflow/stats/core/psi_core.py
+-rw-r--r--  2.0 unx     1755 b- defN 23-Jun-14 07:48 secretflow/stats/core/pva_core.py
+-rw-r--r--  2.0 unx     1776 b- defN 23-Jun-14 07:48 secretflow/stats/core/utils.py
+-rw-r--r--  2.0 unx      662 b- defN 23-Jun-14 07:48 secretflow/utils/__init__.py
+-rw-r--r--  2.0 unx    13370 b- defN 23-Jun-14 07:48 secretflow/utils/cloudpickle.py
+-rw-r--r--  2.0 unx      400 b- defN 23-Jun-14 07:48 secretflow/utils/communicate.py
+-rw-r--r--  2.0 unx    11981 b- defN 23-Jun-14 07:48 secretflow/utils/compressor.py
+-rw-r--r--  2.0 unx     1084 b- defN 23-Jun-14 07:48 secretflow/utils/errors.py
+-rw-r--r--  2.0 unx      870 b- defN 23-Jun-14 07:48 secretflow/utils/hash.py
+-rw-r--r--  2.0 unx      978 b- defN 23-Jun-14 07:48 secretflow/utils/io.py
+-rw-r--r--  2.0 unx      964 b- defN 23-Jun-14 07:48 secretflow/utils/logging.py
+-rw-r--r--  2.0 unx     2842 b- defN 23-Jun-14 07:48 secretflow/utils/ndarray_bigint.py
+-rw-r--r--  2.0 unx     2489 b- defN 23-Jun-14 07:48 secretflow/utils/ndarray_encoding.py
+-rw-r--r--  2.0 unx      803 b- defN 23-Jun-14 07:48 secretflow/utils/random.py
+-rw-r--r--  2.0 unx     1330 b- defN 23-Jun-14 07:48 secretflow/utils/ray_compatibility.py
+-rw-r--r--  2.0 unx     3930 b- defN 23-Jun-14 07:48 secretflow/utils/sigmoid.py
+-rw-r--r--  2.0 unx     3308 b- defN 23-Jun-14 07:48 secretflow/utils/testing.py
+-rw-r--r--  2.0 unx      585 b- defN 23-Jun-14 07:48 secretflow/utils/simulation/__init__.py
+-rw-r--r--  2.0 unx    30743 b- defN 23-Jun-14 07:48 secretflow/utils/simulation/datasets.py
+-rw-r--r--  2.0 unx     8941 b- defN 23-Jun-14 07:48 secretflow/utils/simulation/tf_gnn_model.py
+-rw-r--r--  2.0 unx      769 b- defN 23-Jun-14 07:48 secretflow/utils/simulation/data/__init__.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-Jun-14 07:48 secretflow/utils/simulation/data/_utils.py
+-rw-r--r--  2.0 unx     5389 b- defN 23-Jun-14 07:48 secretflow/utils/simulation/data/dataframe.py
+-rw-r--r--  2.0 unx     4093 b- defN 23-Jun-14 07:48 secretflow/utils/simulation/data/ndarray.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-Jun-14 07:51 secretflow-0.8.3b0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4196 b- defN 23-Jun-14 07:51 secretflow-0.8.3b0.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-14 07:51 secretflow-0.8.3b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-14 07:51 secretflow-0.8.3b0.dist-info/dependency_links.txt
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-14 07:51 secretflow-0.8.3b0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-14 07:51 secretflow-0.8.3b0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    35167 b- defN 23-Jun-14 07:51 secretflow-0.8.3b0.dist-info/RECORD
+341 files, 4022641 bytes uncompressed, 1570121 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -6,44 +6,95 @@
 
 Filename: secretflow/version.py
 Comment: 
 
 Filename: secretflow/component/__init__.py
 Comment: 
 
+Filename: secretflow/component/__main__.py
+Comment: 
+
 Filename: secretflow/component/component.py
 Comment: 
 
+Filename: secretflow/component/data_utils.py
+Comment: 
+
 Filename: secretflow/component/entry.py
 Comment: 
 
-Filename: secretflow/component/node_reader.py
+Filename: secretflow/component/eval_param_reader.py
+Comment: 
+
+Filename: secretflow/component/i18n.py
 Comment: 
 
 Filename: secretflow/component/ml/__init__.py
 Comment: 
 
+Filename: secretflow/component/ml/boost/__init__.py
+Comment: 
+
+Filename: secretflow/component/ml/boost/sgb/__init__.py
+Comment: 
+
+Filename: secretflow/component/ml/boost/sgb/sgb.py
+Comment: 
+
+Filename: secretflow/component/ml/boost/ss_xgb/__init__.py
+Comment: 
+
+Filename: secretflow/component/ml/boost/ss_xgb/ss_xgb.py
+Comment: 
+
 Filename: secretflow/component/ml/linear/__init__.py
 Comment: 
 
 Filename: secretflow/component/ml/linear/ss_sgd.py
 Comment: 
 
 Filename: secretflow/component/preprocessing/__init__.py
 Comment: 
 
+Filename: secretflow/component/preprocessing/feature_filter.py
+Comment: 
+
 Filename: secretflow/component/preprocessing/train_test_split.py
 Comment: 
 
+Filename: secretflow/component/preprocessing/vert_woe_binning.py
+Comment: 
+
 Filename: secretflow/component/psi/__init__.py
 Comment: 
 
 Filename: secretflow/component/psi/two_party_balanced.py
 Comment: 
 
+Filename: secretflow/component/stats/__init__.py
+Comment: 
+
+Filename: secretflow/component/stats/biclassification_eval.py
+Comment: 
+
+Filename: secretflow/component/stats/pva_eval.py
+Comment: 
+
+Filename: secretflow/component/stats/ss_pearsonr.py
+Comment: 
+
+Filename: secretflow/component/stats/ss_pvalue.py
+Comment: 
+
+Filename: secretflow/component/stats/ss_vif.py
+Comment: 
+
+Filename: secretflow/component/stats/table_statistics.py
+Comment: 
+
 Filename: secretflow/data/__init__.py
 Comment: 
 
 Filename: secretflow/data/base.py
 Comment: 
 
 Filename: secretflow/data/math_utils.py
@@ -159,23 +210,53 @@
 
 Filename: secretflow/kuscia/__init__.py
 Comment: 
 
 Filename: secretflow/kuscia/entry.py
 Comment: 
 
+Filename: secretflow/kuscia/ray_config.py
+Comment: 
+
+Filename: secretflow/kuscia/sf_config.py
+Comment: 
+
 Filename: secretflow/kuscia/task_config.py
 Comment: 
 
+Filename: secretflow/kuscia/proto/__init__.py
+Comment: 
+
+Filename: secretflow/kuscia/proto/api/__init__.py
+Comment: 
+
+Filename: secretflow/kuscia/proto/api/v1alpha1/__init__.py
+Comment: 
+
+Filename: secretflow/kuscia/proto/api/v1alpha1/kusciatask/__init__.py
+Comment: 
+
+Filename: secretflow/kuscia/proto/api/v1alpha1/kusciatask/kuscia_task_pb2.py
+Comment: 
+
 Filename: secretflow/ml/__init__.py
 Comment: 
 
 Filename: secretflow/ml/boost/__init__.py
 Comment: 
 
+Filename: secretflow/ml/boost/core/__init__.py
+Comment: 
+
+Filename: secretflow/ml/boost/core/data_preprocess.py
+Comment: 
+
+Filename: secretflow/ml/boost/core/order_map_tools.py
+Comment: 
+
 Filename: secretflow/ml/boost/homo_boost/__init__.py
 Comment: 
 
 Filename: secretflow/ml/boost/homo_boost/homo_booster.py
 Comment: 
 
 Filename: secretflow/ml/boost/homo_boost/homo_booster_worker.py
@@ -315,26 +396,38 @@
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/__init__.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/component.py
 Comment: 
 
+Filename: secretflow/ml/boost/sgb_v/factory/components/logging.py
+Comment: 
+
 Filename: secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/__init__.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/bucket_sum_calculator.py
 Comment: 
 
+Filename: secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/leaf_wise_bucket_sum_calculator.py
+Comment: 
+
 Filename: secretflow/ml/boost/sgb_v/factory/components/cache/__init__.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/cache/level_wise_cache.py
 Comment: 
 
+Filename: secretflow/ml/boost/sgb_v/factory/components/cache/node_bucket_sum_cache_internal.py
+Comment: 
+
+Filename: secretflow/ml/boost/sgb_v/factory/components/cache/node_wise_bucket_sum_cache.py
+Comment: 
+
 Filename: secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/__init__.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/data_preprocessor.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/__init__.py
@@ -390,17 +483,26 @@
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/shuffler/shuffler.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/shuffler/worker_shuffler.py
 Comment: 
 
+Filename: secretflow/ml/boost/sgb_v/factory/components/split_candidate_manager/__init__.py
+Comment: 
+
+Filename: secretflow/ml/boost/sgb_v/factory/components/split_candidate_manager/split_candidate_manager.py
+Comment: 
+
 Filename: secretflow/ml/boost/sgb_v/factory/components/split_finder/__init__.py
 Comment: 
 
+Filename: secretflow/ml/boost/sgb_v/factory/components/split_finder/leaf_wise_split_finder.py
+Comment: 
+
 Filename: secretflow/ml/boost/sgb_v/factory/components/split_finder/split_finder.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/__init__.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_actor.py
@@ -408,14 +510,17 @@
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_builder.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/tree_trainer/__init__.py
 Comment: 
 
+Filename: secretflow/ml/boost/sgb_v/factory/components/tree_trainer/leaf_wise_tree_trainer.py
+Comment: 
+
 Filename: secretflow/ml/boost/sgb_v/factory/components/tree_trainer/level_wise_tree_trainer.py
 Comment: 
 
 Filename: secretflow/ml/boost/sgb_v/factory/components/tree_trainer/tree_trainer.py
 Comment: 
 
 Filename: secretflow/ml/boost/ss_xgb_v/__init__.py
@@ -429,17 +534,14 @@
 
 Filename: secretflow/ml/boost/ss_xgb_v/core/node_split.py
 Comment: 
 
 Filename: secretflow/ml/boost/ss_xgb_v/core/tree_worker.py
 Comment: 
 
-Filename: secretflow/ml/boost/ss_xgb_v/core/utils.py
-Comment: 
-
 Filename: secretflow/ml/boost/ss_xgb_v/core/xgb_tree.py
 Comment: 
 
 Filename: secretflow/ml/linear/__init__.py
 Comment: 
 
 Filename: secretflow/ml/linear/fl_lr_mix.py
@@ -480,14 +582,17 @@
 
 Filename: secretflow/ml/nn/__init__.py
 Comment: 
 
 Filename: secretflow/ml/nn/metrics.py
 Comment: 
 
+Filename: secretflow/ml/nn/utils.py
+Comment: 
+
 Filename: secretflow/ml/nn/applications/__init__.py
 Comment: 
 
 Filename: secretflow/ml/nn/applications/sl_deep_fm.py
 Comment: 
 
 Filename: secretflow/ml/nn/fl/__init__.py
@@ -543,17 +648,14 @@
 
 Filename: secretflow/ml/nn/fl/backend/torch/fl_base.py
 Comment: 
 
 Filename: secretflow/ml/nn/fl/backend/torch/sampler.py
 Comment: 
 
-Filename: secretflow/ml/nn/fl/backend/torch/utils.py
-Comment: 
-
 Filename: secretflow/ml/nn/fl/backend/torch/strategy/__init__.py
 Comment: 
 
 Filename: secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_g.py
 Comment: 
 
 Filename: secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_u.py
@@ -576,14 +678,23 @@
 
 Filename: secretflow/ml/nn/sl/sl_model.py
 Comment: 
 
 Filename: secretflow/ml/nn/sl/strategy_dispatcher.py
 Comment: 
 
+Filename: secretflow/ml/nn/sl/agglayer/__init__.py
+Comment: 
+
+Filename: secretflow/ml/nn/sl/agglayer/agg_layer.py
+Comment: 
+
+Filename: secretflow/ml/nn/sl/agglayer/agg_method.py
+Comment: 
+
 Filename: secretflow/ml/nn/sl/backend/__init__.py
 Comment: 
 
 Filename: secretflow/ml/nn/sl/backend/tensorflow/__init__.py
 Comment: 
 
 Filename: secretflow/ml/nn/sl/backend/tensorflow/sl_base.py
@@ -600,14 +711,23 @@
 
 Filename: secretflow/ml/nn/sl/backend/tensorflow/strategy/split_state_async.py
 Comment: 
 
 Filename: secretflow/ml/nn/sl/backend/torch/__init__.py
 Comment: 
 
+Filename: secretflow/ml/nn/sl/backend/torch/sl_base.py
+Comment: 
+
+Filename: secretflow/ml/nn/sl/backend/torch/strategy/__init__.py
+Comment: 
+
+Filename: secretflow/ml/nn/sl/backend/torch/strategy/split_nn.py
+Comment: 
+
 Filename: secretflow/preprocessing/__init__.py
 Comment: 
 
 Filename: secretflow/preprocessing/base.py
 Comment: 
 
 Filename: secretflow/preprocessing/discretization.py
@@ -642,14 +762,17 @@
 
 Filename: secretflow/preprocessing/binning/kernels/__init__.py
 Comment: 
 
 Filename: secretflow/preprocessing/binning/kernels/base_binning.py
 Comment: 
 
+Filename: secretflow/preprocessing/binning/kernels/chi_merge.py
+Comment: 
+
 Filename: secretflow/preprocessing/binning/kernels/quantile_binning.py
 Comment: 
 
 Filename: secretflow/preprocessing/binning/kernels/quantile_summaries.py
 Comment: 
 
 Filename: secretflow/protos/__init__.py
@@ -657,30 +780,30 @@
 
 Filename: secretflow/protos/component/__init__.py
 Comment: 
 
 Filename: secretflow/protos/component/cluster_pb2.py
 Comment: 
 
-Filename: secretflow/protos/component/comp_def_pb2.py
+Filename: secretflow/protos/component/comp_pb2.py
 Comment: 
 
-Filename: secretflow/protos/component/data_def_pb2.py
+Filename: secretflow/protos/component/data_pb2.py
 Comment: 
 
 Filename: secretflow/protos/component/evaluation_pb2.py
 Comment: 
 
-Filename: secretflow/protos/component/node_def_pb2.py
+Filename: secretflow/protos/component/report_pb2.py
 Comment: 
 
-Filename: secretflow/protos/kuscia/__init__.py
+Filename: secretflow/protos/pipeline/__init__.py
 Comment: 
 
-Filename: secretflow/protos/kuscia/kuscia_task_pb2.py
+Filename: secretflow/protos/pipeline/pipeline_pb2.py
 Comment: 
 
 Filename: secretflow/security/__init__.py
 Comment: 
 
 Filename: secretflow/security/diffie_hellman.py
 Comment: 
@@ -720,45 +843,57 @@
 
 Filename: secretflow/security/compare/spu_comparator.py
 Comment: 
 
 Filename: secretflow/security/privacy/__init__.py
 Comment: 
 
-Filename: secretflow/security/privacy/_lib.cpython-38-x86_64-linux-gnu.so
+Filename: secretflow/security/privacy/_lib.cpython-38-darwin.so
 Comment: 
 
 Filename: secretflow/security/privacy/strategy.py
 Comment: 
 
 Filename: secretflow/security/privacy/strategy_fl.py
 Comment: 
 
 Filename: secretflow/security/privacy/accounting/__init__.py
 Comment: 
 
+Filename: secretflow/security/privacy/accounting/budget_accountant.py
+Comment: 
+
 Filename: secretflow/security/privacy/accounting/gdp_accountant.py
 Comment: 
 
 Filename: secretflow/security/privacy/accounting/log_utils.py
 Comment: 
 
 Filename: secretflow/security/privacy/accounting/rdp_accountant.py
 Comment: 
 
 Filename: secretflow/security/privacy/mechanism/__init__.py
 Comment: 
 
+Filename: secretflow/security/privacy/mechanism/label_dp.py
+Comment: 
+
+Filename: secretflow/security/privacy/mechanism/mechanism_fl.py
+Comment: 
+
 Filename: secretflow/security/privacy/mechanism/tensorflow/__init__.py
 Comment: 
 
 Filename: secretflow/security/privacy/mechanism/tensorflow/layers.py
 Comment: 
 
-Filename: secretflow/security/privacy/mechanism/tensorflow/mechanism_fl.py
+Filename: secretflow/security/privacy/mechanism/torch/__init__.py
+Comment: 
+
+Filename: secretflow/security/privacy/mechanism/torch/layers.py
 Comment: 
 
 Filename: secretflow/stats/__init__.py
 Comment: 
 
 Filename: secretflow/stats/biclassification_eval.py
 Comment: 
@@ -804,14 +939,17 @@
 
 Filename: secretflow/utils/__init__.py
 Comment: 
 
 Filename: secretflow/utils/cloudpickle.py
 Comment: 
 
+Filename: secretflow/utils/communicate.py
+Comment: 
+
 Filename: secretflow/utils/compressor.py
 Comment: 
 
 Filename: secretflow/utils/errors.py
 Comment: 
 
 Filename: secretflow/utils/hash.py
@@ -858,29 +996,29 @@
 
 Filename: secretflow/utils/simulation/data/dataframe.py
 Comment: 
 
 Filename: secretflow/utils/simulation/data/ndarray.py
 Comment: 
 
-Filename: secretflow-0.8.2b3.dist-info/LICENSE
+Filename: secretflow-0.8.3b0.dist-info/LICENSE
 Comment: 
 
-Filename: secretflow-0.8.2b3.dist-info/METADATA
+Filename: secretflow-0.8.3b0.dist-info/METADATA
 Comment: 
 
-Filename: secretflow-0.8.2b3.dist-info/WHEEL
+Filename: secretflow-0.8.3b0.dist-info/WHEEL
 Comment: 
 
-Filename: secretflow-0.8.2b3.dist-info/dependency_links.txt
+Filename: secretflow-0.8.3b0.dist-info/dependency_links.txt
 Comment: 
 
-Filename: secretflow-0.8.2b3.dist-info/entry_points.txt
+Filename: secretflow-0.8.3b0.dist-info/entry_points.txt
 Comment: 
 
-Filename: secretflow-0.8.2b3.dist-info/top_level.txt
+Filename: secretflow-0.8.3b0.dist-info/top_level.txt
 Comment: 
 
-Filename: secretflow-0.8.2b3.dist-info/RECORD
+Filename: secretflow-0.8.3b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## secretflow/cli.py

```diff
@@ -8,32 +8,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import click
-from secretflow.version import __version__
-from secretflow.component.entry import COMP_LIST, COMP_MAP
+import base64
 import json
+import logging
+import os
+import sys
+from contextlib import redirect_stderr, redirect_stdout
+
+import click
 from google.protobuf.json_format import MessageToJson
 
+from secretflow.component.entry import COMP_LIST, COMP_MAP, comp_eval
+from secretflow.protos.component.cluster_pb2 import SFClusterConfig
+from secretflow.protos.component.evaluation_pb2 import NodeEvalParam
+from secretflow.utils.logging import LOG_FORMAT, get_logging_level, set_logging_level
+from secretflow.version import __version__
+
 
 def print_version(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
-    click.echo(f'SecretFlow version {__version__}.')
+    click.echo(f"SecretFlow version {__version__}.")
     ctx.exit()
 
 
 @click.group()
 @click.option(
-    '--version',
-    '-v',
+    "--version",
+    "-v",
     is_flag=True,
     callback=print_version,
     expose_value=False,
     is_eager=True,
 )
 def cli():
     """Welcome to use cli of SecretFlow."""
@@ -45,64 +55,147 @@
     """Get information of components in SecretFlow package."""
     pass
 
 
 @component.command()
 def ls():
     """List all components."""
-    click.echo('{:<40} {:<40} {:<20}'.format('DOMAIN', 'NAME', 'VERSION'))
-    click.echo('-' * 105)
+    click.echo("{:<40} {:<40} {:<20}".format("DOMAIN", "NAME", "VERSION"))
+    click.echo("-" * 105)
     for comp in COMP_LIST.comps:
-        click.echo('{:<40} {:<40} {:<20}'.format(comp.domain, comp.name, comp.version))
+        click.echo("{:<40} {:<40} {:<20}".format(comp.domain, comp.name, comp.version))
 
 
 @component.command()
-@click.option('--file', '-f', required=False, type=click.File(mode='w'))
+@click.option("--file", "-f", required=False, type=click.File(mode="w"))
 @click.option(
-    '--all',
-    '-a',
+    "--all",
+    "-a",
     is_flag=True,
 )
-@click.argument('comp_id', required=False)
+@click.argument("comp_id", required=False)
 def inspect(comp_id, all, file):
     """Display definition of components. The format of comp_id is {domain}/{name}:{version}"""
 
     if all:
         click.echo(f"You are inspecting the compelete comp list.")
-        click.echo('-' * 105)
+        click.echo("-" * 105)
         if file:
             click.echo(
                 json.dumps(json.loads(MessageToJson(COMP_LIST)), indent=2), file=file
             )
-            click.echo(f'Saved to {file.name}.')
+            click.echo(f"Saved to {file.name}.")
         else:
             click.echo(json.dumps(json.loads(MessageToJson(COMP_LIST)), indent=2))
 
     elif comp_id:
         if comp_id in COMP_MAP:
             click.echo(
                 f"You are inspecting definition of component with id [{comp_id}]."
             )
-            click.echo('-' * 105)
+            click.echo("-" * 105)
             if file:
                 click.echo(
                     json.dumps(
                         json.loads(MessageToJson(COMP_MAP[comp_id].definition())),
                         indent=2,
                     ),
                     file=file,
                 )
-                click.echo(f'Saved to {file.name}.')
+                click.echo(f"Saved to {file.name}.")
             else:
                 click.echo(
                     json.dumps(
                         json.loads(MessageToJson(COMP_MAP[comp_id].definition())),
                         indent=2,
                     )
                 )
         else:
             click.echo(f"Component with id [{comp_id}] is not found.")
 
     else:
         click.echo(
-            'You must provide comp_id or use --all/-a for the compelete comp list.'
+            "You must provide comp_id or use --all/-a for the compelete comp list."
         )
+
+
+@component.command()
+@click.option(
+    "--log_file",
+    required=False,
+    type=click.Path(dir_okay=False, writable=True),
+    help="log file. if not specified, logging to stdout",
+)
+@click.option(
+    "--result_file",
+    required=True,
+    type=click.Path(dir_okay=False, writable=True),
+    help="result file. component saved in file with json format",
+)
+@click.option("--log_level", required=False, default="INFO")
+@click.option("--mem_trace", is_flag=True)
+@click.option("--eval_param", required=True, help="base64ed NodeEvalParam binary")
+@click.option("--cluster", required=True, help="base64ed SFClusterConfig binary")
+def run(eval_param, cluster, log_file, result_file, log_level, mem_trace):
+    def _get_peak_mem() -> float:
+        # only works inside docker
+        # use docker's default cgroup
+        cgroup_v1_path = "/sys/fs/cgroup/memory/memory.max_usage_in_bytes"
+        cgroup_v2_path = "/sys/fs/cgroup/memory.peak"
+        try:
+            if os.path.exists(cgroup_v1_path):
+                max_path = cgroup_v1_path
+            else:
+                max_path = cgroup_v2_path
+            with open(max_path, "r") as f:
+                max_usage = int(f.read())
+            return float(max_usage) / (1024**3)
+        except Exception as e:
+            logging.error(f"get_peak_mem error {e}")
+            return 0
+
+    set_logging_level(log_level)
+    logging.basicConfig(level=get_logging_level(), format=LOG_FORMAT)
+
+    ret = {
+        "mem_peak": 0,
+        "run_time": 0,
+        "result": None,
+        "error_msg": None,
+        "error_code": 0,
+    }
+    try:
+        eval = NodeEvalParam()
+        eval.ParseFromString(base64.b64decode(eval_param.encode('utf-8')))
+        clu = SFClusterConfig()
+        clu.ParseFromString(base64.b64decode(cluster.encode('utf-8')))
+    except Exception as e:
+        ret["error_msg"] = f"parse argv err: {e}"
+        ret["error_code"] = -1  # TODO: use real code
+        logging.error(ret["error_msg"])
+        with open(result_file, "w") as f:
+            f.write(json.dumps(ret))
+        sys.exit(-1)
+
+    try:
+        if log_file:
+            with open(log_file, "w") as f:
+                with redirect_stdout(f), redirect_stderr(f):
+                    result = comp_eval(eval, clu, tracer_report=True)
+        else:
+            result = comp_eval(eval, clu, tracer_report=True)
+
+        if mem_trace:
+            ret["mem_peak"] = _get_peak_mem()
+        ret["run_time"] = result["tracer_report"]["run_time"]
+        result = result["eval_result"]
+        ret["result"] = base64.b64encode(result.SerializeToString()).decode('utf-8')
+    except Exception as e:
+        ret["error_msg"] = f"run comp err: {e}"
+        ret["error_code"] = -1  # TODO: use real code
+        logging.error(ret["error_msg"])
+
+    with open(result_file, "w") as f:
+        f.write(json.dumps(ret))
+
+    if ret["error_code"] != 0:
+        sys.exit(-1)
```

## secretflow/version.py

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.8.2b3"
+__version__ = "0.8.3b0"
```

## secretflow/component/__init__.py

```diff
@@ -7,7 +7,9 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from .entry import generate_comp_list, comp_eval
```

## secretflow/component/component.py

```diff
@@ -8,531 +8,584 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
+import logging
 import math
+import threading
+import time
 from dataclasses import dataclass
 from enum import Enum, unique
-from typing import List, Union
+from typing import Dict, List, Union
 
-from secretflow.component.node_reader import NodeReader
-from secretflow.protos.component.comp_def_pb2 import (
-    AtomicParameterDef,
-    AtomicParameterType,
+import cleantext
+import spu
+
+from secretflow.component.data_utils import DistDataType, check_dist_data, check_io_def
+from secretflow.component.eval_param_reader import EvalParamReader
+from secretflow.device.driver import init, shutdown
+from secretflow.protos.component.cluster_pb2 import SFClusterConfig
+from secretflow.protos.component.comp_pb2 import (
+    AttributeDef,
+    AttrType,
     ComponentDef,
     IoDef,
-    ModelDef,
-    ParameterNode,
-    ParameterNodeType,
-    SFDataType,
-    TableDef,
 )
-from secretflow.protos.component.node_def_pb2 import NodeDef
+from secretflow.protos.component.evaluation_pb2 import NodeEvalParam, NodeEvalResult
+
+
+def clean_text(x: str) -> str:
+    return cleantext.clean(x, lower=False, no_line_breaks=True)
+
+
+class CompDeclError(Exception):
+    ...
+
+
+class CompEvalError(Exception):
+    ...
+
+
+class CompTracer:
+    def __init__(self) -> None:
+        self.lock = threading.Lock()
+        self.io_time = 0
+        self.run_time = 0
+
+    def trace_io(self):
+        class _CompTracer:
+            def __init__(self, tracer: CompTracer) -> None:
+                self.tracer = tracer
+
+            def __enter__(self):
+                self.start_time = time.time()
+
+            def __exit__(self, *_):
+                io_time = time.time() - self.start_time
+                with self.tracer.lock:
+                    self.tracer.io_time += io_time
+
+        return _CompTracer(self)
+
+    def trace_running(self):
+        class _CompTracer:
+            def __init__(self, tracer: CompTracer) -> None:
+                self.tracer = tracer
+
+            def __enter__(self):
+                self.start_time = time.time()
+
+            def __exit__(self, *_):
+                running_time = time.time() - self.start_time
+                with self.tracer.lock:
+                    self.tracer.run_time += running_time
+
+        return _CompTracer(self)
+
+    def report(self) -> Dict[str, float]:
+        return {"io_time": self.io_time, "run_time": self.run_time}
 
 
 @unique
 class IoType(Enum):
     INPUT = 1
     OUTPUT = 2
 
 
 @dataclass
 class TableColParam:
     name: str
     desc: str
-    col_list_min_cnt: int = None
-    col_list_max_cnt: int = None
+    col_min_cnt_inclusive: int = None
+    col_max_cnt_inclusive: int = None
+
+
+@dataclass
+class CompEvalContext:
+    local_fs_wd: str = None
+    spu_configs: Dict = None
+    tracer = CompTracer()
 
 
 class Component:
-    def __init__(self, name: str, domain='', version='', desc='') -> None:
+    def __init__(self, name: str, domain="", version="", desc="") -> None:
         self.name = name
         self.domain = domain
         self.version = version
-        self.desc = desc
+        self.desc = clean_text(desc)
 
         self.__definition = None
         self.__eval_callback = None
-        self.__comp_param_decls = []
+        self.__comp_attr_decls = []
         self.__input_io_decls = []
         self.__output_io_decls = []
         self.__argnames = set()
 
-    def float_param(
+    def _check_reserved_words(self, word: str):
+        RESERVED = ["input", "output"]
+        if word in RESERVED:
+            raise CompDeclError(f"{word} is a reserved word.")
+
+    def float_attr(
         self,
         name: str,
         desc: str,
         is_list: bool,
         is_optional: bool,
         default_value: Union[List[float], float] = None,
         allowed_values: List[float] = None,
         lower_bound: float = None,
         upper_bound: float = None,
         lower_bound_inclusive: bool = False,
         upper_bound_inclusive: bool = False,
-        list_min_lenth_inclusive: int = None,
+        list_min_length_inclusive: int = None,
         list_max_length_inclusive: int = None,
     ):
         # sanity checks
-        if not is_optional and default_value is None:
-            raise RuntimeError('default_value must be provided if not optional ')
+        self._check_reserved_words(name)
+
+        if is_optional and default_value is None:
+            raise CompDeclError(
+                f"attr {name}: default_value must be provided if optional."
+            )
 
         if allowed_values is not None and (
             lower_bound is not None or upper_bound is not None
         ):
-            raise RuntimeError(
-                'allowed_values and bounds could not be set at the same time.'
+            raise CompDeclError(
+                "allowed_values and bounds could not be set at the same time."
             )
 
         if allowed_values is not None and default_value is not None:
             if is_list:
                 for v in default_value:
                     if v not in allowed_values:
-                        raise RuntimeError(
-                            f'default_value {v} is not in allowed_values {allowed_values}'
+                        raise CompDeclError(
+                            f"default_value {v} is not in allowed_values {allowed_values}"
                         )
             else:
                 if default_value not in allowed_values:
-                    raise RuntimeError(
-                        f'default_value {default_value} is not in allowed_values {allowed_values}'
+                    raise CompDeclError(
+                        f"default_value {default_value} is not in allowed_values {allowed_values}"
                     )
 
         if (
             lower_bound is not None
             and upper_bound is not None
             and lower_bound > upper_bound
         ):
-            raise RuntimeError(
-                f'lower_bound {lower_bound} is greater than upper_bound {upper_bound}'
+            raise CompDeclError(
+                f"lower_bound {lower_bound} is greater than upper_bound {upper_bound}"
             )
 
         if default_value is not None:
             if lower_bound is not None:
                 if is_list:
                     for v in default_value:
                         if not (
                             v > lower_bound
                             or (lower_bound_inclusive and math.isclose(v, lower_bound))
                         ):
-                            raise RuntimeError(
-                                f'default_value {v} fails bound check: lower_bound {lower_bound}, lower_bound_inclusive {lower_bound_inclusive}'
+                            raise CompDeclError(
+                                f"default_value {v} fails bound check: lower_bound {lower_bound}, lower_bound_inclusive {lower_bound_inclusive}"
                             )
                 else:
                     if not (
                         default_value > lower_bound
                         or (
                             lower_bound_inclusive
                             and math.isclose(default_value, lower_bound)
                         )
                     ):
-                        raise RuntimeError(
-                            f'default_value {default_value} fails bound check: lower_bound {lower_bound}, lower_bound_inclusive {lower_bound_inclusive}'
+                        raise CompDeclError(
+                            f"default_value {default_value} fails bound check: lower_bound {lower_bound}, lower_bound_inclusive {lower_bound_inclusive}"
                         )
 
         if default_value is not None:
             if upper_bound is not None:
                 if is_list:
                     for v in default_value:
                         if not (
                             v < upper_bound
                             or (upper_bound_inclusive and math.isclose(v, upper_bound))
                         ):
-                            raise RuntimeError(
-                                f'default_value {v} fails bound check: upper_bound {upper_bound}, upper_bound_inclusive {upper_bound_inclusive}'
+                            raise CompDeclError(
+                                f"default_value {v} fails bound check: upper_bound {upper_bound}, upper_bound_inclusive {upper_bound_inclusive}"
                             )
                 else:
                     if not (
                         default_value < upper_bound
                         or (
                             upper_bound_inclusive
                             and math.isclose(default_value, upper_bound)
                         )
                     ):
-                        raise RuntimeError(
-                            f'default_value {default_value} fails bound check: upper_bound {upper_bound}, upper_bound_inclusive {upper_bound_inclusive}'
+                        raise CompDeclError(
+                            f"default_value {default_value} fails bound check: upper_bound {upper_bound}, upper_bound_inclusive {upper_bound_inclusive}"
                         )
 
         if (
-            list_min_lenth_inclusive is not None
+            list_min_length_inclusive is not None
             and list_max_length_inclusive is not None
-            and list_min_lenth_inclusive > list_max_length_inclusive
+            and list_min_length_inclusive > list_max_length_inclusive
         ):
-            raise RuntimeError(
-                f'list_min_lenth_inclusive {list_min_lenth_inclusive} should not be greater than list_max_length_inclusive {list_max_length_inclusive}.'
+            raise CompDeclError(
+                f"list_min_length_inclusive {list_min_length_inclusive} should not be greater than list_max_length_inclusive {list_max_length_inclusive}."
             )
 
         # create pb
-        node = ParameterNode(
+        attr = AttributeDef(
             name=name,
-            doc_string=desc,
-            type=ParameterNodeType.ATOMIC,
-            atomic=AtomicParameterDef(
-                type=AtomicParameterType.APT_FLOATS
-                if is_list
-                else AtomicParameterType.APT_FLOAT,
+            desc=clean_text(desc),
+            type=AttrType.AT_FLOATS if is_list else AttrType.AT_FLOAT,
+            atomic=AttributeDef.AtomicAttrDesc(
                 is_optional=is_optional,
             ),
         )
 
         if default_value is not None:
             if is_list:
-                node.atomic.default_value.fs.extend(default_value)
+                attr.atomic.default_value.fs.extend(default_value)
             else:
-                node.atomic.default_value.f = default_value
+                attr.atomic.default_value.f = default_value
 
         if allowed_values is not None:
-            node.atomic.allowed_values.fs.extend(allowed_values)
+            attr.atomic.allowed_values.fs.extend(allowed_values)
 
         if lower_bound is not None:
-            node.atomic.has_lower_bound = True
-            node.atomic.lower_bound_inclusive = lower_bound_inclusive
-            node.atomic.lower_bound.f = lower_bound
+            attr.atomic.has_lower_bound = True
+            attr.atomic.lower_bound_inclusive = lower_bound_inclusive
+            attr.atomic.lower_bound.f = lower_bound
 
         if upper_bound is not None:
-            node.atomic.has_upper_bound = True
-            node.atomic.upper_bound_inclusive = upper_bound_inclusive
-            node.atomic.upper_bound.f = upper_bound
+            attr.atomic.has_upper_bound = True
+            attr.atomic.upper_bound_inclusive = upper_bound_inclusive
+            attr.atomic.upper_bound.f = upper_bound
 
         if is_list:
-            if list_min_lenth_inclusive is not None:
-                node.atomic.list_min_lenth_inclusive = list_min_lenth_inclusive
+            if list_min_length_inclusive is not None:
+                attr.atomic.list_min_length_inclusive = list_min_length_inclusive
             else:
-                node.atomic.list_min_lenth_inclusive = 0
+                attr.atomic.list_min_length_inclusive = 0
 
             if list_max_length_inclusive is not None:
-                node.atomic.list_max_length_inclusive = list_max_length_inclusive
+                attr.atomic.list_max_length_inclusive = list_max_length_inclusive
             else:
-                node.atomic.list_max_length_inclusive = -1
+                attr.atomic.list_max_length_inclusive = -1
 
         # append
-        self.__comp_param_decls.append(node)
+        self.__comp_attr_decls.append(attr)
 
-    def int_param(
+    def int_attr(
         self,
         name: str,
         desc: str,
         is_list: bool,
         is_optional: bool,
         default_value: Union[List[int], int] = None,
         allowed_values: List[int] = None,
         lower_bound: int = None,
         upper_bound: int = None,
         lower_bound_inclusive: bool = False,
         upper_bound_inclusive: bool = False,
-        list_min_lenth_inclusive: int = None,
+        list_min_length_inclusive: int = None,
         list_max_length_inclusive: int = None,
     ):
         # sanity checks
-        if not is_optional and default_value is None:
-            raise RuntimeError('default_value must be provided if not optional ')
+        self._check_reserved_words(name)
+
+        if is_optional and default_value is None:
+            raise CompDeclError(
+                f"attr {name}: default_value must be provided if optional."
+            )
 
         if allowed_values is not None and (
             lower_bound is not None or upper_bound is not None
         ):
-            raise RuntimeError(
-                'allowed_values and bounds could not be set at the same time.'
+            raise CompDeclError(
+                "allowed_values and bounds could not be set at the same time."
             )
 
         if allowed_values is not None and default_value is not None:
             if is_list:
                 for v in default_value:
                     if v not in allowed_values:
-                        raise RuntimeError(
-                            f'default_value {v} is not in allowed_values {allowed_values}'
+                        raise CompDeclError(
+                            f"default_value {v} is not in allowed_values {allowed_values}"
                         )
             else:
                 if default_value not in allowed_values:
-                    raise RuntimeError(
-                        f'default_value {default_value} is not in allowed_values {allowed_values}'
+                    raise CompDeclError(
+                        f"default_value {default_value} is not in allowed_values {allowed_values}"
                     )
 
         if (
             lower_bound is not None
             and upper_bound is not None
             and lower_bound > upper_bound
         ):
-            raise RuntimeError(
-                f'lower_bound {lower_bound} is greater than upper_bound {upper_bound}'
+            raise CompDeclError(
+                f"lower_bound {lower_bound} is greater than upper_bound {upper_bound}"
             )
 
         if default_value is not None:
             if lower_bound is not None:
                 if is_list:
                     for v in default_value:
                         if not (
                             v > lower_bound
                             or (lower_bound_inclusive and v == lower_bound)
                         ):
-                            raise RuntimeError(
-                                f'default_value {v} fails bound check: lower_bound {lower_bound}, lower_bound_inclusive {lower_bound_inclusive}'
+                            raise CompDeclError(
+                                f"default_value {v} fails bound check: lower_bound {lower_bound}, lower_bound_inclusive {lower_bound_inclusive}"
                             )
                 else:
                     if not (
                         default_value > lower_bound
                         or (lower_bound_inclusive and default_value == lower_bound)
                     ):
-                        raise RuntimeError(
-                            f'default_value {default_value} fails bound check: lower_bound {lower_bound}, lower_bound_inclusive {lower_bound_inclusive}'
+                        raise CompDeclError(
+                            f"default_value {default_value} fails bound check: lower_bound {lower_bound}, lower_bound_inclusive {lower_bound_inclusive}"
                         )
 
         if default_value is not None:
             if upper_bound is not None:
                 if is_list:
                     for v in default_value:
                         if not (
                             v < upper_bound
                             or (upper_bound_inclusive and v == upper_bound)
                         ):
-                            raise RuntimeError(
-                                f'default_value {v} fails bound check: upper_bound {upper_bound}, upper_bound_inclusive {upper_bound_inclusive}'
+                            raise CompDeclError(
+                                f"default_value {v} fails bound check: upper_bound {upper_bound}, upper_bound_inclusive {upper_bound_inclusive}"
                             )
                 else:
                     if not (
                         default_value < upper_bound
                         or (upper_bound_inclusive and default_value == upper_bound)
                     ):
-                        raise RuntimeError(
-                            f'default_value {default_value} fails bound check: upper_bound {upper_bound}, upper_bound_inclusive {upper_bound_inclusive}'
+                        raise CompDeclError(
+                            f"default_value {default_value} fails bound check: upper_bound {upper_bound}, upper_bound_inclusive {upper_bound_inclusive}"
                         )
 
         if (
-            list_min_lenth_inclusive is not None
+            list_min_length_inclusive is not None
             and list_max_length_inclusive is not None
-            and list_min_lenth_inclusive > list_max_length_inclusive
+            and list_min_length_inclusive > list_max_length_inclusive
         ):
-            raise RuntimeError(
-                f'list_min_lenth_inclusive {list_min_lenth_inclusive} should not be greater than list_max_length_inclusive {list_max_length_inclusive}.'
+            raise CompDeclError(
+                f"list_min_length_inclusive {list_min_length_inclusive} should not be greater than list_max_length_inclusive {list_max_length_inclusive}."
             )
 
         # create pb
-        node = ParameterNode(
+        attr = AttributeDef(
             name=name,
-            doc_string=desc,
-            type=ParameterNodeType.ATOMIC,
-            atomic=AtomicParameterDef(
-                type=AtomicParameterType.APT_INTS
-                if is_list
-                else AtomicParameterType.APT_INT,
+            desc=clean_text(desc),
+            type=AttrType.AT_INTS if is_list else AttrType.AT_INT,
+            atomic=AttributeDef.AtomicAttrDesc(
                 is_optional=is_optional,
             ),
         )
 
         if default_value is not None:
             if is_list:
-                node.atomic.default_value.i64s.extend(default_value)
+                attr.atomic.default_value.i64s.extend(default_value)
             else:
-                node.atomic.default_value.i64 = default_value
+                attr.atomic.default_value.i64 = default_value
 
         if allowed_values is not None:
-            node.atomic.allowed_values.i64s.extend(allowed_values)
+            attr.atomic.allowed_values.i64s.extend(allowed_values)
 
         if lower_bound is not None:
-            node.atomic.has_lower_bound = True
-            node.atomic.lower_bound_inclusive = lower_bound_inclusive
-            node.atomic.lower_bound.i64 = lower_bound
+            attr.atomic.has_lower_bound = True
+            attr.atomic.lower_bound_inclusive = lower_bound_inclusive
+            attr.atomic.lower_bound.i64 = lower_bound
 
         if upper_bound is not None:
-            node.atomic.has_upper_bound = True
-            node.atomic.upper_bound_inclusive = upper_bound_inclusive
-            node.atomic.upper_bound.i64 = upper_bound
+            attr.atomic.has_upper_bound = True
+            attr.atomic.upper_bound_inclusive = upper_bound_inclusive
+            attr.atomic.upper_bound.i64 = upper_bound
 
         if is_list:
-            if list_min_lenth_inclusive is not None:
-                node.atomic.list_min_lenth_inclusive = list_min_lenth_inclusive
+            if list_min_length_inclusive is not None:
+                attr.atomic.list_min_length_inclusive = list_min_length_inclusive
             else:
-                node.atomic.list_min_lenth_inclusive = 0
+                attr.atomic.list_min_length_inclusive = 0
 
             if list_max_length_inclusive is not None:
-                node.atomic.list_max_length_inclusive = list_max_length_inclusive
+                attr.atomic.list_max_length_inclusive = list_max_length_inclusive
             else:
-                node.atomic.list_max_length_inclusive = -1
+                attr.atomic.list_max_length_inclusive = -1
 
         # append
-        self.__comp_param_decls.append(node)
+        self.__comp_attr_decls.append(attr)
 
-    def str_param(
+    def str_attr(
         self,
         name: str,
         desc: str,
         is_list: bool,
         is_optional: bool,
         default_value: Union[List[str], str] = None,
         allowed_values: List[str] = None,
-        list_min_lenth_inclusive: int = None,
+        list_min_length_inclusive: int = None,
         list_max_length_inclusive: int = None,
     ):
         # sanity checks
-        if not is_optional and default_value is None:
-            raise RuntimeError('default_value must be provided if not optional ')
+        self._check_reserved_words(name)
+
+        if is_optional and default_value is None:
+            raise CompDeclError(
+                f"attr {name}: default_value must be provided if optional."
+            )
 
         if allowed_values is not None and default_value is not None:
             if is_list:
                 for v in default_value:
                     if v not in allowed_values:
-                        raise RuntimeError(
-                            f'default_value {v} is not in allowed_values {allowed_values}'
+                        raise CompDeclError(
+                            f"default_value {v} is not in allowed_values {allowed_values}"
                         )
             else:
                 if default_value not in allowed_values:
-                    raise RuntimeError(
-                        f'default_value {default_value} is not in allowed_values {allowed_values}'
+                    raise CompDeclError(
+                        f"default_value {default_value} is not in allowed_values {allowed_values}"
                     )
 
         if (
-            list_min_lenth_inclusive is not None
+            list_min_length_inclusive is not None
             and list_max_length_inclusive is not None
-            and list_min_lenth_inclusive > list_max_length_inclusive
+            and list_min_length_inclusive > list_max_length_inclusive
         ):
-            raise RuntimeError(
-                f'list_min_lenth_inclusive {list_min_lenth_inclusive} should not be greater than list_max_length_inclusive {list_max_length_inclusive}.'
+            raise CompDeclError(
+                f"list_min_length_inclusive {list_min_length_inclusive} should not be greater than list_max_length_inclusive {list_max_length_inclusive}."
             )
 
         # create pb
-        node = ParameterNode(
+        node = AttributeDef(
             name=name,
-            doc_string=desc,
-            type=ParameterNodeType.ATOMIC,
-            atomic=AtomicParameterDef(
-                type=AtomicParameterType.APT_STRINGS
-                if is_list
-                else AtomicParameterType.APT_STRING,
+            desc=clean_text(desc),
+            type=AttrType.AT_STRINGS if is_list else AttrType.AT_STRING,
+            atomic=AttributeDef.AtomicAttrDesc(
                 is_optional=is_optional,
             ),
         )
 
         if default_value is not None:
             if is_list:
                 node.atomic.default_value.ss.extend(default_value)
             else:
                 node.atomic.default_value.s = default_value
 
         if allowed_values is not None:
             node.atomic.allowed_values.ss.extend(allowed_values)
 
         if is_list:
-            if list_min_lenth_inclusive is not None:
-                node.atomic.list_min_lenth_inclusive = list_min_lenth_inclusive
+            if list_min_length_inclusive is not None:
+                node.atomic.list_min_length_inclusive = list_min_length_inclusive
             else:
-                node.atomic.list_min_lenth_inclusive = 0
+                node.atomic.list_min_length_inclusive = 0
 
             if list_max_length_inclusive is not None:
                 node.atomic.list_max_length_inclusive = list_max_length_inclusive
             else:
                 node.atomic.list_max_length_inclusive = -1
 
         # append
-        self.__comp_param_decls.append(node)
+        self.__comp_attr_decls.append(node)
 
-    def bool_param(
+    def bool_attr(
         self,
         name: str,
         desc: str,
         is_list: bool,
         is_optional: bool,
         default_value: Union[List[bool], bool] = None,
-        list_min_lenth_inclusive: int = None,
+        list_min_length_inclusive: int = None,
         list_max_length_inclusive: int = None,
     ):
         # sanity checks
-        if not is_optional and default_value is None:
-            raise RuntimeError('default_value must be provided if not optional ')
+        self._check_reserved_words(name)
+
+        if is_optional and default_value is None:
+            raise CompDeclError(
+                f"attr {name}: default_value must be provided if optional."
+            )
 
         if (
-            list_min_lenth_inclusive is not None
+            list_min_length_inclusive is not None
             and list_max_length_inclusive is not None
-            and list_min_lenth_inclusive > list_max_length_inclusive
+            and list_min_length_inclusive > list_max_length_inclusive
         ):
-            raise RuntimeError(
-                f'list_min_lenth_inclusive {list_min_lenth_inclusive} should not be greater than list_max_length_inclusive {list_max_length_inclusive}.'
+            raise CompDeclError(
+                f"list_min_length_inclusive {list_min_length_inclusive} should not be greater than list_max_length_inclusive {list_max_length_inclusive}."
             )
 
         # create pb
-        node = ParameterNode(
+        node = AttributeDef(
             name=name,
-            doc_string=desc,
-            type=ParameterNodeType.ATOMIC,
-            atomic=AtomicParameterDef(
-                type=AtomicParameterType.APT_BOOLS
-                if is_list
-                else AtomicParameterType.APT_BOOL,
+            desc=clean_text(desc),
+            type=AttrType.AT_BOOLS if is_list else AttrType.AT_BOOL,
+            atomic=AttributeDef.AtomicAttrDesc(
                 is_optional=is_optional,
             ),
         )
 
         if default_value is not None:
             if is_list:
                 node.atomic.default_value.bs.extend(default_value)
             else:
                 node.atomic.default_value.b = default_value
 
         if is_list:
-            if list_min_lenth_inclusive is not None:
-                node.atomic.list_min_lenth_inclusive = list_min_lenth_inclusive
+            if list_min_length_inclusive is not None:
+                node.atomic.list_min_length_inclusive = list_min_length_inclusive
             else:
-                node.atomic.list_min_lenth_inclusive = 0
+                node.atomic.list_min_length_inclusive = 0
 
             if list_max_length_inclusive is not None:
                 node.atomic.list_max_length_inclusive = list_max_length_inclusive
             else:
                 node.atomic.list_max_length_inclusive = -1
 
         # append
-        self.__comp_param_decls.append(node)
+        self.__comp_attr_decls.append(node)
 
-    def table_io(
+    def io(
         self,
         io_type: IoType,
         name: str,
         desc: str,
-        types: List['TableType'],
+        types: List[DistDataType],
         col_params: List[TableColParam] = None,
     ):
         # create pb
-        table = TableDef(types=types)
-
-        if col_params is not None:
-            for col_param in col_params:
-                col = table.cols.add()
-                col.name = col_param.name
-                col.doc_string = col_param.desc
-                if col_param.col_list_min_cnt is not None:
-                    col.col_list_min_cnt = col_param.col_list_min_cnt
-                if col_param.col_list_max_cnt is not None:
-                    col.col_list_max_cnt = col_param.col_list_max_cnt
-
+        self._check_reserved_words(name)
+        types = [str(t) for t in types]
         io_def = IoDef(
             name=name,
-            doc_string=desc,
-            data=[IoDef.SFDataDef(type=SFDataType.TABLE, table=table)],
+            desc=clean_text(desc),
+            types=types,
         )
 
-        # append
-        if io_type == IoType.INPUT:
-            self.__input_io_decls.append(io_def)
-        else:
-            self.__output_io_decls.append(io_def)
-
-    def model_io(
-        self,
-        io_type: IoType,
-        name: str,
-        desc: str,
-        types: List[str],
-    ):
-        # create pb
-        model = ModelDef(types=types)
+        if col_params is not None:
+            for col_param in col_params:
+                col = io_def.attrs.add()
+                col.name = col_param.name
+                col.desc = clean_text(col_param.desc)
+                if col_param.col_min_cnt_inclusive is not None:
+                    col.col_min_cnt_inclusive = col_param.col_min_cnt_inclusive
+                if col_param.col_max_cnt_inclusive is not None:
+                    col.col_max_cnt_inclusive = col_param.col_max_cnt_inclusive
 
-        io_def = IoDef(
-            name=name,
-            doc_string=desc,
-            data=[IoDef.SFDataDef(type=SFDataType.MODEL, model=model)],
-        )
+        check_io_def(io_def)
 
         # append
         if io_type == IoType.INPUT:
             self.__input_io_decls.append(io_def)
         else:
             self.__output_io_decls.append(io_def)
 
@@ -547,64 +600,252 @@
         return decorator
 
     def definition(self):
         if self.__definition is None:
             comp_def = ComponentDef(
                 domain=self.domain,
                 name=self.name,
-                doc_string=self.desc,
+                desc=self.desc,
                 version=self.version,
             )
 
-            for p in self.__comp_param_decls:
-                if p.name in self.__argnames:
-                    raise RuntimeError(f'param {p.name} is duplicate.')
-                self.__argnames.add(p.name)
-                new_p = comp_def.params.add()
-                new_p.CopyFrom(p)
+            for a in self.__comp_attr_decls:
+                if a.name in self.__argnames:
+                    raise CompDeclError(f"attr {a.name} is duplicate.")
+                self.__argnames.add(a.name)
+                new_a = comp_def.attrs.add()
+                new_a.CopyFrom(a)
 
             for io in self.__input_io_decls:
                 if io.name in self.__argnames:
-                    raise RuntimeError(f'input {io.name} is duplicate.')
+                    raise CompDeclError(f"input {io.name} is duplicate.")
                 self.__argnames.add(io.name)
+
+                for input_attr in io.attrs:
+                    input_attr_full_name = "_".join([io.name, input_attr.name])
+                    self.__argnames.add(input_attr_full_name)
+
                 new_io = comp_def.inputs.add()
                 new_io.CopyFrom(io)
 
             for io in self.__output_io_decls:
                 if io.name in self.__argnames:
-                    raise RuntimeError(f'input {io.name} is duplicate.')
+                    raise CompDeclError(f"output {io.name} is duplicate.")
                 self.__argnames.add(io.name)
                 new_io = comp_def.outputs.add()
                 new_io.CopyFrom(io)
 
             self.__definition = comp_def
 
         return self.__definition
 
-    def eval(self, instance: NodeDef, secretflow_cluster_config):
+    def _setup_sf_cluster(self, config: SFClusterConfig):
+        cluster_config = {
+            "parties": {},
+            "self_party": config.private_config.self_party,
+        }
+        for party, addr in zip(
+            list(config.public_config.rayfed_config.parties),
+            list(config.public_config.rayfed_config.addresses),
+        ):
+            cluster_config["parties"][party] = {"address": addr}
+
+        import multiprocess
+
+        init(
+            address=config.private_config.ray_head_addr,
+            num_cpus=32,
+            log_to_driver=True,
+            cluster_config=cluster_config,
+            omp_num_threads=multiprocess.cpu_count(),
+        )
+
+    def _check_storage(self, config: SFClusterConfig):
+        # only local fs is supported at this moment.
+        storage = config.private_config.storage_config
+        if storage.type and storage.type != "local_fs":
+            raise CompEvalError("only local_fs is supported.")
+        return storage.local_fs.wd
+
+    def _parse_runtime_config(self, key: str, raw: str):
+        if key == "protocol":
+            if raw == "REF2K":
+                return spu.spu_pb2.REF2K
+            elif raw == "SEMI2K":
+                return spu.spu_pb2.SEMI2K
+            elif raw == "ABY3":
+                return spu.spu_pb2.ABY3
+            elif raw == "CHEETAH":
+                return spu.spu_pb2.CHEETAH
+            else:
+                raise CompEvalError(f"unsupported spu protocol: {raw}")
+
+        elif key == "field":
+            if raw == "FM32":
+                return spu.spu_pb2.FM32
+            elif raw == "FM64":
+                return spu.spu_pb2.FM64
+            elif raw == "FM128":
+                return spu.spu_pb2.FM128
+            else:
+                raise CompEvalError(f"unsupported spu field: {raw}")
+
+        elif key == "fxp_fraction_bits":
+            return int(raw)
+
+        else:
+            raise CompEvalError(f"unsupported runtime config: {key}, raw {raw}")
+
+    def _extract_device_config(self, config: SFClusterConfig):
+        spu_configs = {}
+        spu_addresses = {spu.name: spu for spu in config.public_config.spu_configs}
+
+        heu_config = None
+
+        for device in config.desc.devices:
+            if len(set(device.parties)) != len(device.parties):
+                raise CompEvalError(f"parties of device {device.name} are not unique.")
+            if device.type.lower() == "spu":
+                if device.name not in spu_addresses:
+                    raise CompEvalError(
+                        f"addresses of spu {device.name} is not available."
+                    )
+
+                addresses = spu_addresses[device.name]
+
+                # check parties
+                if len(set(addresses.parties)) != len(addresses.parties):
+                    raise CompEvalError(
+                        f"parties in addresses of device {device.name} are not unique."
+                    )
+
+                if set(addresses.parties) != set(device.parties):
+                    raise CompEvalError(
+                        f"parties in addresses of device {device.name} do not match those in desc."
+                    )
+
+                spu_config_json = json.loads(device.config)
+                cluster_def = {
+                    "nodes": [
+                        {
+                            "party": p,
+                            "address": addresses.addresses[idx],
+                            "listen_address": addresses.listen_addresses[idx]
+                            if len(addresses.listen_addresses)
+                            else "",
+                        }
+                        for idx, p in enumerate(list(addresses.parties))
+                    ]
+                }
+
+                # parse runtime config
+                if "runtime_config" in spu_config_json:
+                    cluster_def["runtime_config"] = {}
+                    SUPPORTED_RUNTIME_CONFIG_ITEM = [
+                        "protocol",
+                        "field",
+                        "fxp_fraction_bits",
+                    ]
+                    raw_runtime_config = spu_config_json["runtime_config"]
+
+                    for k, v in raw_runtime_config.items():
+                        if k not in SUPPORTED_RUNTIME_CONFIG_ITEM:
+                            logging.warning(f"runtime config item {k} is not parsed.")
+                        else:
+                            cluster_def["runtime_config"][
+                                k
+                            ] = self._parse_runtime_config(k, v)
+
+                spu_configs[device.name] = {"cluster_def": cluster_def}
+
+                if "link_desc" in spu_config_json:
+                    spu_configs[device.name]["link_desc"] = spu_config_json["link_desc"]
+            elif device.type == "heu":
+                assert heu_config is None, "only support one heu config"
+                heu_config_json = json.loads(device.config)
+                assert isinstance(heu_config_json, dict)
+                SUPPORTED_HEU_CONFIG_ITEM = ["mode", "schema", "key_size"]
+                heu_config = {}
+                for k in SUPPORTED_HEU_CONFIG_ITEM:
+                    assert (
+                        k in heu_config_json
+                    ), f"missing {k} config in heu config {device.config}"
+                    heu_config[k] = heu_config_json.pop(k)
+                assert (
+                    len(heu_config_json) == 0
+                ), f"unknown {list(heu_config_json.keys())} config in heu config {device.config}"
+            else:
+                raise CompEvalError(f"unsupported device type {device.type}")
+
+        return spu_configs, heu_config
+
+    def eval(
+        self,
+        param: NodeEvalParam,
+        cluster_config: SFClusterConfig = None,
+        tracer_report: bool = False,
+    ) -> Union[NodeEvalResult, Dict]:
         definition = self.definition()
 
         # sanity check on __eval_callback
         from inspect import signature
 
-        PREDEFIND_PARAM = ['ctx']
+        PREDEFIND_PARAM = ["ctx"]
 
         sig = signature(self.__eval_callback)
-        for param in sig.parameters.values():
-            if param.kind != param.KEYWORD_ONLY:
-                raise RuntimeError(f'param {param.name} must be KEYWORD_ONLY.')
-            if param.name not in PREDEFIND_PARAM and param.name not in self.__argnames:
-                raise RuntimeError(f'param {param.name} is not allowed.')
+        for p in sig.parameters.values():
+            if p.kind != p.KEYWORD_ONLY:
+                raise CompEvalError(f"param {p.name} must be KEYWORD_ONLY.")
+            if p.name not in PREDEFIND_PARAM and p.name not in self.__argnames:
+                raise CompEvalError(f"param {p.name} is not allowed.")
+
+        # sanity check on sf config
+        ctx = CompEvalContext()
+
+        if cluster_config is not None:
+            ctx.local_fs_wd = self._check_storage(cluster_config)
+            ctx.spu_configs, ctx.heu_config = self._extract_device_config(
+                cluster_config
+            )
 
-        reader = NodeReader(instance=instance, definition=definition)
-        kwargs = {'ctx': secretflow_cluster_config}
+        reader = EvalParamReader(instance=param, definition=definition)
+        kwargs = {"ctx": ctx}
 
-        for p in definition.params:
-            kwargs[p.name] = reader.get_param(prefixes='', name=p.name)
+        for a in definition.attrs:
+            kwargs[a.name] = reader.get_attr(name=a.name)
 
         for input in definition.inputs:
             kwargs[input.name] = reader.get_input(name=input.name)
 
+            for input_attr in input.attrs:
+                input_attr_full_name = "_".join([input.name, input_attr.name])
+                kwargs[input_attr_full_name] = reader.get_input_attrs(
+                    input_name=input.name, attr_name=input_attr.name
+                )
+
         for output in definition.outputs:
-            kwargs[output.name] = reader.get_output(name=output.name)
+            kwargs[output.name] = reader.get_output_uri(name=output.name)
+
+        if cluster_config is not None:
+            self._setup_sf_cluster(cluster_config)
+        try:
+            ret = self.__eval_callback(**kwargs)
+        except Exception as e:
+            logging.error(f"eval on {param} failed, error <{e}>")
+            # TODO: use error_code in report
+            raise e from None
+        finally:
+            if cluster_config is not None:
+                shutdown()
 
-        return self.__eval_callback(**kwargs)
+        # check output
+        for output in definition.outputs:
+            check_dist_data(ret[output.name], output)
+
+        res = NodeEvalResult(
+            outputs=[ret[output.name] for output in definition.outputs]
+        )
+
+        if tracer_report:
+            return {"eval_result": res, "tracer_report": ctx.tracer.report()}
+        else:
+            return res
```

## secretflow/component/entry.py

```diff
@@ -9,38 +9,68 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from secretflow.component.ml.linear.ss_sgd import ss_sgd_predict_comp, ss_sgd_train_comp
+from secretflow.component.preprocessing.feature_filter import feature_filter_comp
 from secretflow.component.preprocessing.train_test_split import train_test_split_comp
+from secretflow.component.preprocessing.vert_woe_binning import (
+    vert_woe_binning_comp,
+    vert_woe_substitution_comp,
+)
 from secretflow.component.psi.two_party_balanced import two_party_balanced_psi_comp
-from secretflow.protos.component.comp_def_pb2 import CompListDef
-from secretflow.protos.component.node_def_pb2 import NodeDef
+from secretflow.component.stats.biclassification_eval import biclassification_eval_comp
+from secretflow.component.stats.pva_eval import pva_value_comp
+from secretflow.component.stats.ss_pearsonr import ss_pearsonr_comp
+from secretflow.component.stats.ss_pvalue import ss_pvalue_comp
+from secretflow.component.stats.ss_vif import ss_vif_comp
+from secretflow.component.stats.table_statistics import table_statistics_comp
+from secretflow.protos.component.cluster_pb2 import SFClusterConfig
+from secretflow.protos.component.comp_pb2 import CompListDef, ComponentDef
+from secretflow.protos.component.evaluation_pb2 import NodeEvalParam, NodeEvalResult
+from secretflow.component.ml.boost.sgb.sgb import sgb_predict_comp, sgb_train_comp
+from secretflow.component.ml.boost.ss_xgb.ss_xgb import (
+    ss_xgb_predict_comp,
+    ss_xgb_train_comp,
+)
 
 ALL_COMPONENTS = [
     train_test_split_comp,
     two_party_balanced_psi_comp,
     ss_sgd_train_comp,
     ss_sgd_predict_comp,
+    feature_filter_comp,
+    vert_woe_binning_comp,
+    vert_woe_substitution_comp,
+    ss_vif_comp,
+    ss_pearsonr_comp,
+    ss_pvalue_comp,
+    table_statistics_comp,
+    biclassification_eval_comp,
+    pva_value_comp,
+    sgb_predict_comp,
+    sgb_train_comp,
+    ss_xgb_predict_comp,
+    ss_xgb_train_comp,
 ]
-COMP_LIST_NAME = 'experimental'
-COMP_LIST_DOC_STRING = 'Some experimental componments. Not production ready.'
-COMP_LIST_VERSION = '0.0.1'
+COMP_LIST_NAME = "experimental"
+COMP_LIST_DESC = "Some experimental componments. Not production ready."
+COMP_LIST_VERSION = "0.0.1"
 
 
 def gen_key(domain: str, name: str, version: str) -> str:
-    return f'{domain}/{name}:{version}'
+    return f"{domain}/{name}:{version}"
 
 
 def generate_comp_list():
     comp_list = CompListDef()
     comp_list.name = COMP_LIST_NAME
-    comp_list.doc_string = COMP_LIST_DOC_STRING
+    comp_list.desc = COMP_LIST_DESC
     comp_list.version = COMP_LIST_VERSION
     comp_map = {}
     all_comp_defs = []
     for x in ALL_COMPONENTS:
         x_def = x.definition()
         comp_map[gen_key(x_def.domain, x_def.name, x_def.version)] = x
         all_comp_defs.append(x_def)
@@ -49,14 +79,25 @@
     comp_list.comps.extend(all_comp_defs)
     return comp_list, comp_map
 
 
 COMP_LIST, COMP_MAP = generate_comp_list()
 
 
-def eval(instance: NodeDef, secretflow_cluster_config):
-    key = gen_key(instance.domain, instance.name, instance.version)
+def get_comp_def(domain: str, name: str, version: str) -> ComponentDef:
+    key = gen_key(domain, name, version)
+    assert key in COMP_MAP
+    return COMP_MAP[key].definition()
+
+
+# FIXME(junfeng): Should load storage config from .sf_storage JSON file
+def comp_eval(
+    param: NodeEvalParam,
+    cluster_config: SFClusterConfig,
+    tracer_report: bool = False,
+) -> NodeEvalResult:
+    key = gen_key(param.domain, param.name, param.version)
     if key in COMP_MAP:
         comp = COMP_MAP[key]
-        comp.eval(instance, secretflow_cluster_config)
+        return comp.eval(param, cluster_config, tracer_report=tracer_report)
     else:
         raise RuntimeError("component is not found.")
```

## secretflow/component/ml/linear/ss_sgd.py

```diff
@@ -8,266 +8,374 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
+import os
 
-from secretflow.component.component import Component, IoType
-from secretflow.data.vertical import read_csv
+import pandas as pd
+
+from secretflow.component.component import CompEvalError, Component, IoType
+from secretflow.component.data_utils import (
+    DistDataType,
+    extract_table_header,
+    load_table,
+    model_dumps,
+    model_loads,
+)
 from secretflow.device.device.pyu import PYU
-from secretflow.device.device.spu import SPU
+from secretflow.device.device.spu import SPU, SPUObject
 from secretflow.device.driver import wait
-from secretflow.ml.linear import LinearModel, SSRegression
-from secretflow.protos.component.comp_def_pb2 import TableType
+from secretflow.ml.linear import LinearModel, RegType, SSRegression
+from secretflow.protos.component.data_pb2 import DistData, IndividualTable, TableSchema
+from secretflow.utils.sigmoid import SigType
 
 ss_sgd_train_comp = Component(
     "ss_sgd_train",
     domain="ml.linear",
     version="0.0.1",
-    desc="""This method provides both linear and logistic regression
-    linear models for vertical split dataset setting by using secret sharing
-    with mini batch SGD training solver. SS-SGD is short for secret sharing SGD training.
+    desc="""Train both linear and logistic regression
+    linear models for vertical partitioning dataset with mini batch SGD training solver by using secret sharing.
+    SS-SGD is short for secret sharing SGD training.
     """,
 )
-ss_sgd_train_comp.int_param(
+ss_sgd_train_comp.int_attr(
     name="epochs",
-    desc="iteration rounds.",
+    desc="The number of complete pass through the training data.",
     is_list=False,
     is_optional=True,
-    default_value=1,
+    default_value=10,
     allowed_values=None,
     lower_bound=1,
     upper_bound=None,
     lower_bound_inclusive=True,
 )
-ss_sgd_train_comp.float_param(
+ss_sgd_train_comp.float_attr(
     name="learning_rate",
-    desc="controls how much to change the model in one epoch.",
+    desc="The step size at each iteration in one iteration.",
     is_list=False,
     is_optional=True,
     default_value=0.1,
 )
-ss_sgd_train_comp.int_param(
+ss_sgd_train_comp.int_attr(
     name="batch_size",
-    desc="how many samples use in one calculation.",
+    desc="The number of training examples utilized in one iteration.",
     is_list=False,
     is_optional=True,
     default_value=1024,
 )
-ss_sgd_train_comp.str_param(
+ss_sgd_train_comp.str_attr(
     name="sig_type",
-    desc="sigmoid approximation type.",
+    desc="Sigmoid approximation type.",
     is_list=False,
     is_optional=True,
     default_value="t1",
     allowed_values=["real", "t1", "t3", "t5", "df", "sr", "mix"],
 )
-ss_sgd_train_comp.str_param(
+ss_sgd_train_comp.str_attr(
     name="reg_type",
-    desc="Linear or Logistic regression",
+    desc="Regression type",
     is_list=False,
     is_optional=True,
     default_value="logistic",
     allowed_values=["linear", "logistic"],
 )
-ss_sgd_train_comp.str_param(
+ss_sgd_train_comp.str_attr(
     name="penalty",
-    desc="The penalty (aka regularization term) to be used.",
+    desc="The penalty(aka regularization term) to be used.",
     is_list=False,
     is_optional=True,
     default_value="None",
     allowed_values=["None", "l1", "l2"],
 )
-ss_sgd_train_comp.float_param(
+ss_sgd_train_comp.float_attr(
     name="l2_norm",
     desc="L2 regularization term.",
     is_list=False,
     is_optional=True,
     default_value=0.5,
 )
-ss_sgd_train_comp.float_param(
+ss_sgd_train_comp.float_attr(
     name="eps",
-    desc="""If the W's change rate is less than this threshold,
+    desc="""If the change rate of weights is less than this threshold,
             the model is considered to be converged,
-            and the training stops early. 0 disable.""",
+            and the training stops early. 0 to disable.""",
     is_list=False,
     is_optional=True,
     default_value=0.001,
 )
-ss_sgd_train_comp.table_io(
-    io_type=IoType.INPUT,
-    name="x",
-    desc="features",
-    types=[TableType.VERTICAL_PARTITIONING_TABLE],
-    col_params=None,
-)
-ss_sgd_train_comp.table_io(
+ss_sgd_train_comp.io(
     io_type=IoType.INPUT,
-    name="y",
-    desc="label",
-    types=[TableType.VERTICAL_PARTITIONING_TABLE],
+    name="train_dataset",
+    desc="Input train dataset.",
+    types=[DistDataType.VERTICAL_TABLE],
     col_params=None,
 )
-ss_sgd_train_comp.model_io(
-    io_type=IoType.OUTPUT, name="output", desc="output", types=["ss_sgb"]
+ss_sgd_train_comp.io(
+    io_type=IoType.OUTPUT,
+    name="output_model",
+    desc="Output model",
+    types=[DistDataType.SS_SGD_MODEL],
 )
 
+# current version 0.1
+MODEL_MAX_MAJOR_VERSION = 0
+MODEL_MAX_MINOR_VERSION = 1
+
 
 @ss_sgd_train_comp.eval_fn
 def ss_sgd_train_eval_fn(
     *,
     ctx,
     epochs,
     learning_rate,
     batch_size,
     sig_type,
     reg_type,
     penalty,
     l2_norm,
     eps,
-    x,
-    y,
-    output,
+    train_dataset,
+    output_model,
 ):
-    """This method provides both linear and logistic regression
-    linear models for vertical split dataset setting by using secret sharing
-    with mini batch SGD training solver. SS-SGD is short for secret sharing SGD training.
-    """
-
-    x_parties = x.table_metadata.vertical_partitioning.parties
-    x_paths = x.table_metadata.vertical_partitioning.paths
-
-    y_parties = y.table_metadata.vertical_partitioning.parties
-    y_paths = y.table_metadata.vertical_partitioning.paths
-
-    model_public_path = output.model_metadata.public_file_path
-    model_parties = output.model_metadata.parties
-    model_party_paths = output.model_metadata.party_dir_paths
-
-    spu = SPU(
-        ctx['spu'],
-        link_desc={
-            'connect_retry_times': 60,
-            'connect_retry_interval_ms': 1000,
-            'brpc_channel_protocol': "http",
-            "brpc_channel_connection_type": "pooled",
-            'recv_timeout_ms': 1200 * 1000,  # 1200s
-            'http_timeout_ms': 1200 * 1000,  # 1200s
-        },
-    )
+    # only local fs is supported at this moment.
+    local_fs_wd = ctx.local_fs_wd
 
-    reg = SSRegression(spu)
-    pyus = {k: PYU(k) for k in ctx['pyu']}
+    if ctx.spu_configs is None or len(ctx.spu_configs) == 0:
+        raise CompEvalError("spu config is not found.")
+    if len(ctx.spu_configs) > 1:
+        raise CompEvalError("only support one spu")
+    spu_config = next(iter(ctx.spu_configs.values()))
 
-    x_filepath = {pyus[k]: p for k, p in zip(x_parties, x_paths)}
-    y_filepath = {pyus[k]: p for k, p in zip(y_parties, y_paths)}
+    spu = SPU(spu_config["cluster_def"], spu_config["link_desc"])
 
-    x = read_csv(x_filepath, no_header=True)
-    y = read_csv(y_filepath, no_header=True)
+    reg = SSRegression(spu)
 
-    reg.fit(
-        x=x,
-        y=y,
-        epochs=epochs,
-        learning_rate=learning_rate,
-        batch_size=batch_size,
-        sig_type=sig_type,
-        reg_type=reg_type,
-        penalty=penalty,
-        l2_norm=l2_norm,
-        eps=eps,
-    )
+    y = load_table(ctx, train_dataset, load_labels=True)
+    x = load_table(ctx, train_dataset, load_features=True)
 
-    model = reg.save_model()
+    with ctx.tracer.trace_running():
+        reg.fit(
+            x=x,
+            y=y,
+            epochs=epochs,
+            learning_rate=learning_rate,
+            batch_size=batch_size,
+            sig_type=sig_type,
+            reg_type=reg_type,
+            penalty=penalty,
+            l2_norm=l2_norm,
+            eps=eps,
+        )
 
-    dir_path = {k: v for k, v in zip(model_parties, model_party_paths)}
+    model = reg.save_model()
 
-    record = model.dump(dir_path=dir_path)
+    model_meta = {"reg_type": model.reg_type.value, "sig_type": model.sig_type.value}
 
-    with open(model_public_path, 'wb') as f:
-        import cloudpickle as pickle
+    model_db = model_dumps(
+        "ss_sgd",
+        DistDataType.SS_SGD_MODEL,
+        MODEL_MAX_MAJOR_VERSION,
+        MODEL_MAX_MINOR_VERSION,
+        [model.weights],
+        json.dumps(model_meta),
+        local_fs_wd,
+        output_model,
+        train_dataset.sys_info,
+    )
 
-        pickle.dump(record, f)
+    return {"output_model": model_db}
 
 
 ss_sgd_predict_comp = Component(
     "ss_sgd_predict",
     domain="ml.linear",
     version="0.0.1",
-    desc="Predict using the model.",
+    desc="Predict using the SS-SGD model.",
 )
-ss_sgd_predict_comp.int_param(
+ss_sgd_predict_comp.int_attr(
     name="batch_size",
-    desc="how many samples use in one calculation.",
+    desc="The number of training examples utilized in one iteration.",
     is_list=False,
     is_optional=True,
     default_value=1024,
 )
-ss_sgd_predict_comp.table_io(
+ss_sgd_predict_comp.str_attr(
+    name="receiver",
+    desc="Party of receiver.",
+    is_list=False,
+    is_optional=False,
+)
+ss_sgd_predict_comp.str_attr(
+    name="pred_name",
+    desc="Column name for predictions.",
+    is_list=False,
+    is_optional=True,
+    default_value="pred",
+    allowed_values=None,
+)
+ss_sgd_predict_comp.bool_attr(
+    name="save_ids",
+    desc=(
+        "Whether to save ids columns into output prediction table. "
+        "If true, input feature_dataset must contain id columns, and receiver party must be id owner."
+    ),
+    is_list=False,
+    is_optional=True,
+    default_value=False,
+)
+ss_sgd_predict_comp.bool_attr(
+    name="save_label",
+    desc=(
+        "Whether or not to save real label columns into output pred file. "
+        "If ture, input feature_dataset must contain label columns and receiver party must be label owner."
+    ),
+    is_list=False,
+    is_optional=True,
+    default_value=False,
+)
+ss_sgd_predict_comp.io(
     io_type=IoType.INPUT,
-    name="x",
-    desc="features",
-    types=[TableType.VERTICAL_PARTITIONING_TABLE],
-    col_params=None,
+    name="model",
+    desc="Input model.",
+    types=[DistDataType.SS_SGD_MODEL],
 )
-ss_sgd_predict_comp.model_io(
-    io_type=IoType.INPUT, name="model", desc="model", types=["ss_sgb"]
+ss_sgd_predict_comp.io(
+    io_type=IoType.INPUT,
+    name="feature_dataset",
+    desc="Input feature dataset.",
+    types=[DistDataType.VERTICAL_TABLE],
+    col_params=None,
 )
-ss_sgd_predict_comp.table_io(
+ss_sgd_predict_comp.io(
     io_type=IoType.OUTPUT,
-    name="y",
-    desc="label",
-    types=[TableType.INDIVIDUAL_TABLE],
+    name="pred",
+    desc="Output prediction.",
+    types=[DistDataType.INDIVIDUAL_TABLE],
     col_params=None,
 )
 
 
-@ss_sgd_predict_comp.eval_fn
-def ss_sgd_predict_eval_fn(*, ctx, batch_size, x, model, y):
-    x_parties = x.table_metadata.vertical_partitioning.parties
-    x_paths = x.table_metadata.vertical_partitioning.paths
-
-    model_public_path = model.model_metadata.public_file_path
-
-    y_party = y.table_metadata.indivial.party
-    y_path = y.table_metadata.indivial.path
-
-    spu = SPU(
-        ctx['spu'],
-        link_desc={
-            'connect_retry_times': 60,
-            'connect_retry_interval_ms': 1000,
-            'brpc_channel_protocol': "http",
-            "brpc_channel_connection_type": "pooled",
-            'recv_timeout_ms': 1200 * 1000,  # 1200s
-            'http_timeout_ms': 1200 * 1000,  # 1200s
-        },
+def load_ss_sgd_model(ctx, spu, model) -> LinearModel:
+    model_objs, model_meta_str = model_loads(
+        model,
+        MODEL_MAX_MAJOR_VERSION,
+        MODEL_MAX_MINOR_VERSION,
+        DistDataType.SS_SGD_MODEL,
+        # only local fs is supported at this moment.
+        ctx.local_fs_wd,
+        spu=spu,
+    )
+    assert len(model_objs) == 1 and isinstance(
+        model_objs[0], SPUObject
+    ), f"model_objs {model_objs}, model_meta_str {model_meta_str}"
+
+    model_meta = json.loads(model_meta_str)
+    assert (
+        isinstance(model_meta, dict)
+        and "reg_type" in model_meta
+        and "sig_type" in model_meta
+    )
+    model = LinearModel(
+        weights=model_objs[0],
+        reg_type=RegType(model_meta["reg_type"]),
+        sig_type=SigType(model_meta["sig_type"]),
     )
-    pyus = {k: PYU(k) for k in ctx['pyu']}
 
-    with open(model_public_path, 'rb') as f:
-        import cloudpickle as pickle
+    return model
 
-        record = pickle.load(f)
 
-    model = LinearModel.load(record=record, spu=spu)
-    x_filepath = {pyus[k]: p for k, p in zip(x_parties, x_paths)}
-    x = read_csv(x_filepath, no_header=True)
+@ss_sgd_predict_comp.eval_fn
+def ss_sgd_predict_eval_fn(
+    *,
+    ctx,
+    batch_size,
+    feature_dataset,
+    model,
+    receiver,
+    pred_name,
+    pred,
+    save_ids,
+    save_label,
+):
+    if ctx.spu_configs is None or len(ctx.spu_configs) == 0:
+        raise CompEvalError("spu config is not found.")
+    if len(ctx.spu_configs) > 1:
+        raise CompEvalError("only support one spu")
+    spu_config = next(iter(ctx.spu_configs.values()))
+
+    spu = SPU(spu_config["cluster_def"], spu_config["link_desc"])
+
+    model = load_ss_sgd_model(ctx, spu, model)
 
     reg = SSRegression(spu)
     reg.load_model(model)
 
-    pyu = pyus[y_party]
-    y = reg.predict(
-        x=x,
-        batch_size=batch_size,
-        to_pyu=pyu,
-    )
+    x = load_table(ctx, feature_dataset, load_features=True)
 
-    def save_csv(x, path):
-        import numpy
+    with ctx.tracer.trace_running():
+        pyu = PYU(receiver)
+        pyu_y = reg.predict(
+            x=x,
+            batch_size=batch_size,
+            to_pyu=pyu,
+        )
+
+        y_path = os.path.join(ctx.local_fs_wd, pred)
+
+        if save_ids:
+            ids = load_table(ctx, feature_dataset, load_ids=True)
+            assert pyu in ids.partitions
+            ids_name = extract_table_header(feature_dataset, load_ids=True)
+            assert receiver in ids_name
+            ids = ids.partitions[pyu].data
+            ids_name = list(ids_name[receiver].keys())
+        else:
+            ids = None
+            ids_name = None
+
+        if save_label:
+            label = load_table(ctx, feature_dataset, load_labels=True)
+            assert pyu in label.partitions
+            label_name = extract_table_header(feature_dataset, load_labels=True)
+            assert receiver in label_name
+            label = label.partitions[pyu].data
+            label_name = list(label_name[receiver].keys())
+        else:
+            label = None
+            label_name = None
+
+        def save_csv(x, label, ids, path):
+            x = pd.DataFrame(x, columns=[pred_name])
+
+            if label is not None:
+                label = pd.DataFrame(label, columns=label_name)
+                x = pd.concat([x, label], axis=1)
+            if ids is not None:
+                ids = pd.DataFrame(ids, columns=ids_name)
+                x = pd.concat([x, ids], axis=1)
+
+            x.to_csv(path, index=False)
+
+        wait(pyu(save_csv)(pyu_y.partitions[pyu], label, ids, y_path))
+
+    y_db = DistData(
+        name="train",
+        type=str(DistDataType.INDIVIDUAL_TABLE),
+        data_refs=[DistData.DataRef(uri=pred, party=receiver, format="csv")],
+    )
 
-        numpy.savetxt(path, x, delimiter=",")
+    meta = IndividualTable(
+        schema=TableSchema(
+            ids=ids_name if ids_name is not None else [],
+            types=["f32"],
+            features=[pred_name],
+            labels=label_name if label_name is not None else [],
+        ),
+        num_lines=x.shape[0],
+    )
+    y_db.meta.Pack(meta)
 
-    wait(pyu(save_csv)(y.partitions[pyu], y_path))
+    return {"pred": y_db}
```

## secretflow/component/preprocessing/train_test_split.py

```diff
@@ -10,116 +10,116 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from secretflow.component.component import Component, IoType
+from secretflow.component.data_utils import (
+    DistDataType,
+    dump_vertical_table,
+    load_table,
+)
 from secretflow.data.split import train_test_split as train_test_split_fn
-from secretflow.data.vertical import read_csv
-from secretflow.device.device.pyu import PYU
-from secretflow.device.driver import wait
-from secretflow.protos.component.comp_def_pb2 import TableType
+from secretflow.protos.component.data_pb2 import VerticalTable
 
 train_test_split_comp = Component(
     "train_test_split",
     domain="preprocessing",
     version="0.0.1",
-    desc="""Split arrays or matrices into random train and test subsets.
-    Check: https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html
+    desc="""Split datasets into random train and test subsets.
+    Plese check: https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html
     """,
 )
 
 
-train_test_split_comp.float_param(
+train_test_split_comp.float_attr(
     name="train_size",
-    desc="proportion of the dataset to include in the train split.",
+    desc="Proportion of the dataset to include in the train subset.",
     is_list=False,
     is_optional=True,
     default_value=0.75,
     allowed_values=None,
     lower_bound=0.0,
     upper_bound=1.0,
     lower_bound_inclusive=True,
     upper_bound_inclusive=True,
 )
-train_test_split_comp.float_param(
+train_test_split_comp.float_attr(
     name="test_size",
-    desc="proportion of the dataset to include in the test split.",
+    desc="Proportion of the dataset to include in the test subset.",
     is_list=False,
     is_optional=True,
     default_value=0.25,
     allowed_values=None,
     lower_bound=0.0,
     upper_bound=1.0,
     lower_bound_inclusive=True,
     upper_bound_inclusive=True,
 )
-train_test_split_comp.int_param(
+train_test_split_comp.int_attr(
     name="random_state",
-    desc="Controls the shuffling applied to the data before applying the split.",
+    desc="Specify the random seed of the shuffling.",
     is_list=False,
     is_optional=True,
     default_value=1234,
 )
-train_test_split_comp.bool_param(
+train_test_split_comp.bool_attr(
     name="shuffle",
-    desc="Whether or not to shuffle the data before splitting.",
+    desc="Whether to shuffle the data before splitting.",
     is_list=False,
     is_optional=True,
     default_value=True,
 )
-train_test_split_comp.table_io(
+train_test_split_comp.io(
     io_type=IoType.INPUT,
-    name="input",
-    desc="input",
-    types=[TableType.VERTICAL_PARTITIONING_TABLE],
+    name="input_data",
+    desc="Input dataset.",
+    types=[DistDataType.VERTICAL_TABLE],
     col_params=None,
 )
-train_test_split_comp.table_io(
+train_test_split_comp.io(
     io_type=IoType.OUTPUT,
     name="train",
-    desc="train",
-    types=[TableType.VERTICAL_PARTITIONING_TABLE],
+    desc="Output train dataset.",
+    types=[DistDataType.VERTICAL_TABLE],
     col_params=None,
 )
-train_test_split_comp.table_io(
+train_test_split_comp.io(
     io_type=IoType.OUTPUT,
     name="test",
-    desc="test",
-    types=[TableType.VERTICAL_PARTITIONING_TABLE],
+    desc="Output test dataset.",
+    types=[DistDataType.VERTICAL_TABLE],
     col_params=None,
 )
 
 
 @train_test_split_comp.eval_fn
 def train_test_split_eval_fn(
-    *, ctx, train_size, test_size, random_state, shuffle, input, train, test
+    *, ctx, train_size, test_size, random_state, shuffle, input_data, train, test
 ):
-    input_parties = input.table_metadata.vertical_partitioning.parties
-    input_paths = input.table_metadata.vertical_partitioning.paths
+    input_df = load_table(
+        ctx, input_data, load_features=True, load_ids=True, load_labels=True
+    )
 
-    train_parties = train.table_metadata.vertical_partitioning.parties
-    train_paths = train.table_metadata.vertical_partitioning.paths
+    pyus = list(input_df.partitions.keys())
+    assert len(pyus) == 2
 
-    test_parties = test.table_metadata.vertical_partitioning.parties
-    test_paths = test.table_metadata.vertical_partitioning.paths
+    with ctx.tracer.trace_running():
+        train_df, test_df = train_test_split_fn(
+            input_df,
+            train_size=train_size,
+            test_size=test_size,
+            random_state=random_state,
+            shuffle=shuffle,
+        )
+
+    in_meta = VerticalTable()
+    input_data.meta.Unpack(in_meta)
 
-    pyus = {k: PYU(k) for k in ctx['pyu']}
-    assert len(pyus) == 2
+    in_meta.num_lines = train_df.shape[0]
+    train_db = dump_vertical_table(ctx, train_df, train, in_meta, input_data.sys_info)
 
-    input_dict = {pyus[k]: v for k, v in zip(input_parties, input_paths)}
-    train_dict = {pyus[k]: v for k, v in zip(train_parties, train_paths)}
-    test_dict = {pyus[k]: v for k, v in zip(test_parties, test_paths)}
-
-    input_df = read_csv(input_dict)
-
-    train_df, test_df = train_test_split_fn(
-        input_df,
-        train_size=train_size,
-        test_size=test_size,
-        random_state=random_state,
-        shuffle=shuffle,
-    )
+    in_meta.num_lines = test_df.shape[0]
+    test_db = dump_vertical_table(ctx, test_df, test, in_meta, input_data.sys_info)
 
-    wait(train_df.to_csv(train_dict, index=False))
-    wait(test_df.to_csv(test_dict, index=False))
+    return {"train": train_db, "test": test_db}
```

## secretflow/component/psi/two_party_balanced.py

```diff
@@ -8,175 +8,252 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
 
-from secretflow.component.component import Component, IoType, TableColParam
+from secretflow.component.component import (
+    CompEvalError,
+    Component,
+    IoType,
+    TableColParam,
+)
+from secretflow.component.data_utils import (
+    DistDataType,
+    extract_distdata_info,
+    merge_individuals_to_vtable,
+    extract_table_header,
+)
 from secretflow.device.device.pyu import PYU
 from secretflow.device.device.spu import SPU
-from secretflow.protos.component.comp_def_pb2 import TableType
+from secretflow.protos.component.data_pb2 import (
+    DistData,
+    IndividualTable,
+    VerticalTable,
+)
+from typing import List
 
 two_party_balanced_psi_comp = Component(
     "two_party_balanced_psi",
     domain="psi",
     version="0.0.1",
     desc="Balanced PSI between two parties.",
 )
 
-two_party_balanced_psi_comp.str_param(
+two_party_balanced_psi_comp.str_attr(
     name="receiver",
     desc="Which party can get joined data.",
     is_list=False,
-    is_optional=True,
+    is_optional=False,
 )
-two_party_balanced_psi_comp.str_param(
+two_party_balanced_psi_comp.str_attr(
     name="protocol",
     desc="PSI protocol.",
     is_list=False,
-    is_optional=False,
+    is_optional=True,
     default_value="ECDH_PSI_2PC",
     allowed_values=["ECDH_PSI_2PC", "KKRT_PSI_2PC", "BC22_PSI_2PC"],
 )
-two_party_balanced_psi_comp.bool_param(
+two_party_balanced_psi_comp.bool_attr(
     name="precheck_input",
-    desc="Whether to check input data before join.",
-    is_list=False,
-    is_optional=False,
-    default_value=True,
-)
-two_party_balanced_psi_comp.bool_param(
-    name="sort",
-    desc="Whether sort data by key after join.",
-    is_list=False,
-    is_optional=False,
-    default_value=True,
-)
-two_party_balanced_psi_comp.bool_param(
-    name="broadcast_result",
-    desc="Whether to broadcast joined data to all parties.",
+    desc="Whether to check input data before joining.",
     is_list=False,
-    is_optional=False,
+    is_optional=True,
     default_value=True,
 )
-two_party_balanced_psi_comp.int_param(
+two_party_balanced_psi_comp.int_attr(
     name="bucket_size",
-    desc="Whether to broadcast joined data to all parties.",
+    desc="Specify the hash bucket size used in PSI. Larger values consume more memory.",
     is_list=False,
-    is_optional=False,
+    is_optional=True,
     default_value=1048576,
 )
-two_party_balanced_psi_comp.str_param(
+two_party_balanced_psi_comp.str_attr(
     name="curve_type",
-    desc="curve for ecdh psi.",
+    desc="Curve type for ECDH PSI.",
     is_list=False,
-    is_optional=False,
+    is_optional=True,
     default_value="CURVE_FOURQ",
     allowed_values=["CURVE_25519", "CURVE_FOURQ", "CURVE_SM2", "CURVE_SECP256K1"],
 )
-two_party_balanced_psi_comp.table_io(
+two_party_balanced_psi_comp.io(
     io_type=IoType.INPUT,
     name="receiver_input",
-    desc="input for receiver",
-    types=[TableType.INDIVIDUAL_TABLE],
-    col_params=[TableColParam(name="key", desc="Column(s) used to join.")],
+    desc="Input for receiver",
+    types=[DistDataType.INDIVIDUAL_TABLE],
+    col_params=[
+        TableColParam(
+            name="key",
+            desc="Column(s) used to join. If not provided, ids of the dataset will be used.",
+        )
+    ],
 )
-two_party_balanced_psi_comp.table_io(
+two_party_balanced_psi_comp.io(
     io_type=IoType.INPUT,
     name="sender_input",
-    desc="input for sender",
-    types=[TableType.INDIVIDUAL_TABLE],
-    col_params=[TableColParam(name="key", desc="Column(s) used to join.")],
-)
-two_party_balanced_psi_comp.table_io(
-    io_type=IoType.OUTPUT,
-    name="receiver_output",
-    desc="output for receiver",
-    types=[TableType.INDIVIDUAL_TABLE],
+    desc="Input for sender",
+    types=[DistDataType.INDIVIDUAL_TABLE],
+    col_params=[
+        TableColParam(
+            name="key",
+            desc="Column(s) used to join. If not provided, ids of the dataset will be used.",
+        )
+    ],
 )
-two_party_balanced_psi_comp.table_io(
+two_party_balanced_psi_comp.io(
     io_type=IoType.OUTPUT,
-    name="sender_output",
-    desc="output for sender",
-    types=[TableType.INDIVIDUAL_TABLE],
+    name="psi_output",
+    desc="Output",
+    types=[DistDataType.VERTICAL_TABLE],
 )
 
 
+# We would respect user-specified ids even ids are set in TableSchema.
+def modify_schema(x: DistData, keys: List[str]) -> DistData:
+    new_x = DistData()
+    new_x.CopyFrom(x)
+    if len(keys) == 0:
+        return new_x
+    assert x.type == "sf.table.individual"
+    imeta = IndividualTable()
+    assert x.meta.Unpack(imeta)
+
+    new_meta = IndividualTable()
+    names = []
+    types = []
+
+    # copy current ids to features and clean current ids.
+    for id in imeta.schema.ids:
+        names.append(id)
+        types.append("str")
+
+    for f, t in zip(list(imeta.schema.features), list(imeta.schema.types)):
+        names.append(f)
+        types.append(t)
+
+    for k in keys:
+        if k not in names:
+            raise CompEvalError(f"key {k} is not found as id or feature.")
+
+    for n, t in zip(names, types):
+        if n in keys:
+            new_meta.schema.ids.append(n)
+        else:
+            new_meta.schema.features.append(n)
+            new_meta.schema.types.append(t)
+
+    new_meta.schema.labels.extend(list(imeta.schema.labels))
+    new_meta.num_lines = imeta.num_lines
+
+    new_x.meta.Pack(new_meta)
+
+    return new_x
+
+
 @two_party_balanced_psi_comp.eval_fn
 def two_party_balanced_psi_eval_fn(
     *,
     ctx,
     receiver,
     protocol,
     precheck_input,
-    sort,
-    broadcast_result,
     bucket_size,
     curve_type,
     receiver_input,
+    receiver_input_key,
     sender_input,
-    receiver_output,
-    sender_output,
+    sender_input_key,
+    psi_output,
 ):
-    receiver_input_path = receiver_input.table_metadata.indivial.path
-    receiver_input_party = receiver_input.table_metadata.indivial.party
-    for col_param in receiver_input.table_params.col_params:
-        if col_param.name == "key":
-            receiver_keys = list(col_param.cols)
-
-    sender_input_path = sender_input.table_metadata.indivial.path
-    sender_input_party = sender_input.table_metadata.indivial.party
-    for col_param in sender_input.table_params.col_params:
-        if col_param.name == "key":
-            sender_keys = list(col_param.cols)
-
-    receiver_output_path = receiver_output.table_metadata.indivial.path
-    receiver_output_party = receiver_output.table_metadata.indivial.party
-
-    sender_output_path = sender_output.table_metadata.indivial.path
-    sender_output_party = sender_output.table_metadata.indivial.party
-
-    spu = SPU(
-        ctx['spu'],
-        link_desc={
-            'connect_retry_times': 60,
-            'connect_retry_interval_ms': 1000,
-            'brpc_channel_protocol': "http",
-            "brpc_channel_connection_type": "pooled",
-            'recv_timeout_ms': 1200 * 1000,  # 1200s
-            'http_timeout_ms': 1200 * 1000,  # 1200s
-        },
+    receiver_path_format = extract_distdata_info(receiver_input)
+    assert len(receiver_path_format) == 1
+    receiver_party = list(receiver_path_format.keys())[0]
+    sender_path_format = extract_distdata_info(sender_input)
+    sender_party = list(sender_path_format.keys())[0]
+
+    # only local fs is supported at this moment.
+    local_fs_wd = ctx.local_fs_wd
+
+    if ctx.spu_configs is None or len(ctx.spu_configs) == 0:
+        raise CompEvalError("spu config is not found.")
+    if len(ctx.spu_configs) > 1:
+        raise CompEvalError("only support one spu")
+    spu_config = next(iter(ctx.spu_configs.values()))
+
+    import logging
+
+    logging.warning(spu_config)
+
+    spu = SPU(spu_config["cluster_def"], spu_config["link_desc"])
+
+    receiver_pyu = PYU(receiver_party)
+    sender_pyu = PYU(sender_party)
+
+    # If receiver_input_key is not provided, try to get receiver_input_key from ids of receiver_input.
+    if len(receiver_input_key) == 0:
+        receiver_input_key = list(
+            extract_table_header(receiver_input, load_ids=True)[receiver_party].keys()
+        )
+
+    # If sender_input_key is not provided, try to get sender_input_key from ids of sender_input.
+    if len(sender_input_key) == 0:
+        sender_input_key = list(
+            extract_table_header(sender_input, load_ids=True)[sender_party].keys()
+        )
+
+    with ctx.tracer.trace_running():
+        join_count = spu.psi_join_csv(
+            key={receiver_pyu: receiver_input_key, sender_pyu: sender_input_key},
+            input_path={
+                receiver_pyu: os.path.join(
+                    local_fs_wd, receiver_path_format[receiver_party].uri
+                ),
+                sender_pyu: os.path.join(
+                    local_fs_wd, sender_path_format[sender_party].uri
+                ),
+            },
+            output_path={
+                receiver_pyu: os.path.join(local_fs_wd, psi_output),
+                sender_pyu: os.path.join(local_fs_wd, psi_output),
+            },
+            receiver=receiver,
+            join_party=sender_party,
+            protocol=protocol,
+            precheck_input=precheck_input,
+            bucket_size=bucket_size,
+            curve_type=curve_type,
+        )[0]["join_count"]
+
+    output_db = DistData(
+        name=psi_output,
+        type=str(DistDataType.VERTICAL_TABLE),
+        sys_info=receiver_input.sys_info,
+        data_refs=[
+            DistData.DataRef(
+                uri=psi_output,
+                party=receiver_party,
+                format="csv",
+            ),
+            DistData.DataRef(
+                uri=psi_output,
+                party=sender_party,
+                format="csv",
+            ),
+        ],
     )
 
-    assert receiver_input_party == receiver_output_party
-    assert sender_input_party == sender_output_party
-    assert receiver_input_party != sender_input_party
-
-    pyus = {k: PYU(k) for k in ctx['pyu']}
-
-    assert receiver == receiver_input_party
-
-    assert len(pyus) == 2
-    assert receiver in pyus.keys()
-
-    receiver_pyu = pyus[receiver]
-    sender_pyu = pyus[sender_input_party]
-
-    spu.psi_join_csv(
-        key={receiver_pyu: receiver_keys, sender_pyu: sender_keys},
-        input_path={
-            receiver_pyu: receiver_input_path,
-            sender_pyu: sender_input_path,
-        },
-        output_path={
-            receiver_pyu: receiver_output_path,
-            sender_pyu: sender_output_path,
-        },
-        receiver=receiver,
-        join_party=sender_input_party,
-        protocol=protocol,
-        precheck_input=precheck_input,
-        bucket_size=bucket_size,
-        curve_type=curve_type,
+    output_db = merge_individuals_to_vtable(
+        [
+            modify_schema(receiver_input, receiver_input_key),
+            modify_schema(sender_input, sender_input_key),
+        ],
+        output_db,
     )
+    vmeta = VerticalTable()
+    assert output_db.meta.Unpack(vmeta)
+    vmeta.num_lines = join_count
+    output_db.meta.Pack(vmeta)
+
+    return {"psi_output": output_db}
```

## secretflow/data/horizontal/__init__.py

```diff
@@ -9,14 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .dataframe import HDataFrame
-from .io import read_csv, to_csv
+from .io import read_csv
 
 __all__ = [
     "HDataFrame",
     "read_csv",
-    "to_csv",
 ]
```

## secretflow/data/horizontal/io.py

```diff
@@ -38,36 +38,23 @@
 
     Returns:
         HDataFrame
 
     Examples:
         >>> read_csv({PYU('alice'): 'alice.csv', PYU('bob'): 'bob.csv'})
     """
-    assert filepath, 'File path shall not be empty!'
+    assert filepath, "File path shall not be empty!"
     df = HDataFrame(aggregator=aggregator, comparator=comparator)
     for device, path in filepath.items():
         df.partitions[device] = Partition(device(read_csv_wrapper)(path, **kwargs))
     # Check column and dtype.
     dtypes = None
     for part in df.partitions.values():
         if dtypes is None:
             dtypes = part.dtypes
         else:
             dtypes_next = part.dtypes
             assert dtypes.equals(
                 dtypes_next
-            ), f'Different dtypes: {dtypes} vs {dtypes_next}'
+            ), f"Different dtypes: {dtypes} vs {dtypes_next}"
 
     return df
-
-
-def to_csv(df: HDataFrame, file_uris: Dict[PYU, str], **kwargs):
-    """Write object to a comma-separated values (csv) file.
-
-    Args:
-        df: the HDataFrame to save.
-        file_uris: the file path of each PYU.
-        kwargs: all other arguments are same with :py:meth:`pandas.DataFrame.to_csv`.
-    """
-    return [
-        df.partitions[device].to_csv(uri, **kwargs) for device, uri in file_uris.items()
-    ]
```

## secretflow/data/vertical/__init__.py

```diff
@@ -9,14 +9,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .dataframe import VDataFrame
-from .io import read_csv, to_csv
+from .io import read_csv
 
 __all__ = [
     "VDataFrame",
     "read_csv",
-    "to_csv",
 ]
```

## secretflow/data/vertical/io.py

```diff
@@ -20,15 +20,15 @@
 from secretflow.device import PYU, SPU, Device
 from secretflow.utils.errors import InvalidArgumentError
 from secretflow.utils.random import global_random
 
 
 def read_csv(
     filepath: Dict[PYU, str],
-    delimiter=',',
+    delimiter=",",
     dtypes: Dict[PYU, Dict[str, type]] = None,
     spu: SPU = None,
     keys: Union[str, List[str], Dict[Device, List[str]]] = None,
     drop_keys: Union[str, List[str], Dict[Device, List[str]]] = None,
     psi_protocl=None,
     no_header: bool = False,
 ) -> VDataFrame:
@@ -69,18 +69,18 @@
             doesn't allow duplicate column names.
         psi_protocl: Specified protocol for PSI. Default 'KKRT_PSI_2PC' for 2
             parties, 'ECDH_PSI_3PC' for 3 parties.
 
     Returns:
         A aligned VDataFrame.
     """
-    assert spu is None or keys is not None, f'keys required when spu provided'
-    assert spu is None or drop_keys is not None, f'drop_keys required when spu provided'
+    assert spu is None or keys is not None, f"keys required when spu provided"
+    assert spu is None or drop_keys is not None, f"drop_keys required when spu provided"
     if spu is not None:
-        assert len(filepath) <= 3, f'only support 2 or 3 parties for now'
+        assert len(filepath) <= 3, f"only support 2 or 3 parties for now"
 
     def get_keys(
         device: Device, x: Union[str, List[str], Dict[Device, List[str]]] = None
     ) -> List[str]:
         if x:
             if isinstance(x, str):
                 return [x]
@@ -96,18 +96,18 @@
                 raise InvalidArgumentError(f"Illegal type for keys,got {type(x)}")
         else:
             return []
 
     filepath_actual = filepath
     if spu is not None:
         if psi_protocl is None:
-            psi_protocl = 'KKRT_PSI_2PC' if len(filepath) == 2 else 'ECDH_PSI_3PC'
+            psi_protocl = "KKRT_PSI_2PC" if len(filepath) == 2 else "ECDH_PSI_3PC"
         rand_suffix = global_random(list(filepath.keys())[0], 100000)
         output_file = {
-            pyu: f'{path}.psi_output_{rand_suffix}' for pyu, path in filepath.items()
+            pyu: f"{path}.psi_output_{rand_suffix}" for pyu, path in filepath.items()
         }
         spu.psi_csv(
             keys,
             input_path=filepath,
             output_path=output_file,
             protocol=psi_protocl,
             receiver=list(filepath.keys())[0].party,
@@ -117,15 +117,15 @@
     partitions = {}
     for device, path in filepath_actual.items():
         usecols = dtypes[device].keys() if dtypes is not None else None
         dtype = dtypes[device] if dtypes is not None else None
         partitions[device] = Partition(
             device(read_csv_wrapper)(
                 path,
-                auto_gen_header_prefix=str(device) if no_header else '',
+                auto_gen_header_prefix=str(device) if no_header else "",
                 delimiter=delimiter,
                 usecols=usecols,
                 dtype=dtype,
             )
         )
 
     if drop_keys:
@@ -157,26 +157,13 @@
     for device, partition in partitions.items():
         n = len(partition)
         dtype = partition.dtypes
 
         if length is None:
             length = n
         else:
-            assert length == n, f'number of samples must be equal across all devices'
+            assert length == n, f"number of samples must be equal across all devices"
 
         for col in dtype.index:
-            assert col not in unique_cols, f'col {col} duplicate in multiple devices'
+            assert col not in unique_cols, f"col {col} duplicate in multiple devices"
             unique_cols.add(col)
     return VDataFrame(partitions)
-
-
-def to_csv(df: VDataFrame, file_uris: Dict[PYU, str], **kwargs):
-    """Write object to a comma-separated values (csv) file.
-
-    Args:
-        df: the VDataFrame to save.
-        file_uris: the file path of each PYU.
-        kwargs: all other arguments are same with :py:meth:`pandas.DataFrame.to_csv`.
-    """
-    return [
-        df.partitions[device].to_csv(uri, **kwargs) for device, uri in file_uris.items()
-    ]
```

## secretflow/device/driver.py

```diff
@@ -236,49 +236,49 @@
             .. code:: python
 
                 # For alice
                 {
                     'parties': {
                         'alice': {
                             # The address for other parties.
-                            'address': '127.0.0.1:10001',
+                            'address': '127.0.0.1:20001',
                             # (Optional) the listen address, the `address` will
                             # be used if not prodived.
-                            'listen_addr': '0.0.0.0:10001'
+                            'listen_addr': '0.0.0.0:20001'
                         },
                         'bob': {
                             # The address for other parties.
-                            'address': '127.0.0.1:10002',
+                            'address': '127.0.0.1:20002',
                             # (Optional) the listen address, the `address` will
                             # be used if not prodived.
-                            'listen_addr': '0.0.0.0:10002'
+                            'listen_addr': '0.0.0.0:20002'
                         },
                     },
-                    'self_party': alice
+                    'self_party': 'alice'
                 }
 
                 # For bob
                 {
                     'parties': {
                         'alice': {
                             # The address for other parties.
-                            'address': '127.0.0.1:10001',
+                            'address': '127.0.0.1:20001',
                             # (Optional) the listen address, the `address` will
                             # be used if not prodived.
-                            'listen_addr': '0.0.0.0:10001'
+                            'listen_addr': '0.0.0.0:20001'
                         },
                         'bob': {
                             # The address for other parties.
-                            'address': '127.0.0.1:10002',
+                            'address': '127.0.0.1:20002',
                             # (Optional) the listen address, the `address` will
                             # be used if not prodived.
-                            'listen_addr': '0.0.0.0:10002'
+                            'listen_addr': '0.0.0.0:20002'
                         },
                     },
-                    'self_party': bob
+                    'self_party': 'bob'
                 }
         num_cpus: Number of CPUs the user wishes to assign to each raylet.
         log_to_driver: Whether direct output of worker processes on all nodes
             to driver.
         omp_num_threads: set environment variable `OMP_NUM_THREADS`. It works
             only when address is None.
         logging_level: optional; works only in production mode.
@@ -287,14 +287,15 @@
         cross_silo_grpc_retry_policy: optional, works only in production mode.
             a dict descibes the retry policy for cross silo rpc call.
             If None, the following default retry policy will be used.
             More details please refer to
             `retry-policy <https://github.com/grpc/proposal/blob/master/A6-client-retries.md#retry-policy>`_.
 
             .. code:: python
+
                 {
                     "maxAttempts": 4,
                     "initialBackoff": "0.1s",
                     "maxBackoff": "1s",
                     "backoffMultiplier": 2,
                     "retryableStatusCodes": [
                         "UNAVAILABLE"
@@ -307,87 +308,92 @@
             The size must be strictly less than 2GB, i.e. 2 * (1024 ** 3).
         cross_silo_serializing_allowed_list: optional, works only in production mode.
             A dict describes the package or class list allowed for cross-silo
             serializing(deserializating). It's used for avoiding pickle deserializing
             execution attack when crossing silos. E.g.
 
             .. code:: python
+
                 {
                     "numpy.core.numeric": ["*"],
                     "numpy": ["dtype"],
                 }
         cross_silo_timeout_in_seconds: The timeout in seconds of a cross-silo RPC call.
             It's 3600 by default.
         exit_on_failure_cross_silo_sending: optional, works only in production mode.
             whether exit when failure on cross-silo sending. If True, a SIGTERM
             will be signaled to self if failed to sending cross-silo data.
         enable_waiting_for_other_parties_ready: wait for other parties ready if True.
         tls_config: optional, a dict describes the tls certificate and key infomations. E.g.
 
             .. code:: python
+
                 {
                     'key': 'server key in pem.'
                     'cert': 'server certificate in pem.',
                     'ca_cert': 'root ca certificate of other parties.'
                 }
 
         auth_manager_config: optional, a dict describes the config about authority manager
             service. Authority manager helps manage the authority of TEE data.
             This parameter is for TEE users only. An example,
 
             .. code:: python
+
                 {
                     'host': 'host of authority manager service.'
                     'mr_enclave': 'mr_enclave of authority manager.',
                     'ca_cert': 'optional, root ca certificate of authority manager.'
                 }
         party_key_pair: optional, a dict describes the asymmetric key pair.
             This is required for party who wants to send data to TEEU.
             E.g.
 
-            # For alice
             .. code:: python
+
+                # For alice
                 {
                     'alice': {
                         'public_key': 'RSA public key of alice in pem.',
                         'private_key': 'RSA private key of alice in pem.',
                     }
                 }
 
-            # For bob
-            .. code:: python
+                # For bob
                 {
                     'bob': {
                         'public_key': 'RSA public key of bob in pem.',
                         'private_key': 'RSA private key of bob in pem.',
                     }
                 }
         tee_simulation: optional, enable TEE simulation if True.
             When simulation is enabled, the remote attestation for auth manager
             will be ignored. This is for test only and keep it False when for production.
         **kwargs: see :py:meth:`ray.init` parameters.
     """
     set_logging_level(logging_level)
     simluation_mode = True if parties else False
+
     if auth_manager_config and simluation_mode:
         raise InvalidArgumentError(
             'TEE abilities is available only in production mode.'
             'Please run SecretFlow in production mode.'
         )
 
     if ray_version_less_than_2_0_0():
         if address:
             local_mode = False
         else:
             local_mode = True
     else:
         local_mode = address == 'local'
     if not local_mode and num_cpus is not None:
-        raise InvalidArgumentError(
-            'When connecting to an existing cluster, num_cpus must not be provided.'
+        num_cpus = None
+        logging.warning(
+            'When connecting to an existing cluster, num_cpus must not be provided. Num_cpus is neglected at this moment.'
         )
     if local_mode and num_cpus is None:
         num_cpus = multiprocess.cpu_count()
         if simluation_mode:
             # Give num_cpus a min value for better simulation.
             num_cpus = max(num_cpus, 32)
 
@@ -491,22 +497,39 @@
             cross_silo_messages_max_size_in_bytes=cross_silo_messages_max_size_in_bytes,
             cross_silo_timeout_in_seconds=cross_silo_timeout_in_seconds,
             exit_on_failure_cross_silo_sending=exit_on_failure_cross_silo_sending,
             enable_waiting_for_other_parties_ready=enable_waiting_for_other_parties_ready,
             **kwargs,
         )
 
+        global g_all_parties
+        global g_self_party
+        g_all_parties = all_parties
+        g_self_party = self_party
+
+
+def barrier():
+    global g_all_parties
+    global g_self_party
+
+    if sfd.production_mode():
+        barriers = []
+        for party in g_all_parties:
+            barriers.append(PYU(party)(lambda: None)())
+        reveal(barriers)
+
 
 def shutdown():
     """Disconnect the worker, and terminate processes started by secretflow.init().
 
     This will automatically run at the end when a Python process that uses Ray exits.
     It is ok to run this twice in a row. The primary use case for this function
     is to cleanup state between tests.
     """
+    barrier()
     sfd.shutdown()
 
 
 def _parse_tls_config(
     tls_config: Dict[str, str], party: str
 ) -> Dict[str, global_state.PartyCert]:
     party_certs = {}
```

## secretflow/device/device/heu.py

```diff
@@ -336,14 +336,17 @@
             param.get("schema", "paillier"),
             param['key_pair']['generate'].get('bit_size', 2048),
         )
         super().__init__(
             heu_id, config['sk_keeper']['party'], self.hekit, cleartext_type, encoder
         )
 
+    def __repr__(self) -> str:
+        return f"HEUSkKeeper(heu_id={self.heu_id}, party={self.party})"
+
     def public_key(self):
         return self.hekit.public_key()
 
     def dump_pk(self, path):
         """Dump public key to the specified file."""
         pk = self.hekit.public_key()
         Path(path).parent.mkdir(parents=True, exist_ok=True)
@@ -393,14 +396,17 @@
     def __init__(
         self, heu_id, party: str, config, pk, cleartext_type: np.dtype, encoder
     ):
         self.config = config
         self.hekit = hnp.setup(pk)
         super().__init__(heu_id, party, self.hekit, cleartext_type, encoder)
 
+    def __repr__(self) -> str:
+        return f"HEUEvaluator(heu_id={self.heu_id}, party={self.party})"
+
     def dump(self, data, path):
         """Dump data to file."""
         assert isinstance(data, (hnp.CiphertextArray, hnp.PlaintextArray)), (
             f'value must be hnp array, ' f'got {type(data)} instead.'
         )
 
         Path(path).parent.mkdir(parents=True, exist_ok=True)
```

## secretflow/device/device/heu_object.py

```diff
@@ -7,16 +7,19 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from typing import List, Union
 import jax.tree_util
 import ray
+import numpy as np
 
 from secretflow.device.device.pyu import PYUObject
 
 from .base import DeviceObject
 from .register import dispatch
 
 
@@ -177,18 +180,31 @@
                 self.data, subgroup_map, order_map, bucket_num, cumsum
             ),
             self.location,
             self.is_plain,
         )
 
     def batch_feature_wise_bucket_sum(
-        self, subgroup_map, order_map, bucket_num, cumsum=False
-    ):
-        """
-        Sum of HEUObject selected elements
+        self,
+        subgroup_map: List[Union[PYUObject, np.ndarray]],
+        order_map: Union[PYUObject, np.ndarray],
+        bucket_num: int,
+        cumsum=False,
+    ) -> List["HEUObject"]:
+        """Calculate a list o bucket sum arrays.
+        A bucket sum array has dim 2 and shape (feature_num * bucket_sum, self.col_num).
+
+        Args:
+            subgroup_map (List[Union[PYUObject, np.ndarray]]): elements in each subset of elements of self.
+            order_map (Union[PYUObject, np.ndarray]): shape (self.row_num, feature_num). map[i,j] = k means element i, feature j is in bucket k.
+            bucket_num (int): how many bucket to split each feature into.
+            cumsum (bool, optional): whether calculate the cumulative sums or individual sums. Defaults to False.
+
+        Return:
+            a list of bucket sum array in HEUObject.
         """
 
         def process_data(x):
             res = x
             if isinstance(x, PYUObject):
                 res = x.data
             return res
```

## secretflow/device/device/pyu.py

```diff
@@ -51,18 +51,18 @@
             party (str): Party name where this device is located.
         """
         super().__init__(DeviceType.PYU)
 
         self.party = party
 
     def __str__(self) -> str:
-        return f'{self.party}'
+        return self.party
 
     def __repr__(self) -> str:
-        return str(self)
+        return f"PYURuntime({self.party})"
 
     def __eq__(self, other):
         return type(other) == type(self) and str(other) == str(self)
 
     def __lt__(self, other):
         return type(other) == type(self) and str(self) < str(other)
```

## secretflow/device/device/spu.py

```diff
@@ -272,14 +272,15 @@
     def __init__(
         self,
         rank: int,
         cluster_def: Dict,
         link_desc: Dict = None,
         log_options: spu_logging.LogOptions = spu_logging.LogOptions(),
         use_link: bool = True,
+        id: str = None,
     ):
         """wrapper of spu.Runtime.
 
         Args:
             rank (int): rank of runtime
             cluster_def (Dict): config of spu cluster
             link_desc (Dict, optional): link config. Defaults to None.
@@ -292,14 +293,15 @@
         self.cluster_def = cluster_def
 
         desc = spu_link.Desc()
         tls_opts = None
         for i, node in enumerate(cluster_def['nodes']):
             address = node['address']
             if i == rank:
+                self.party = node['party']
                 tls_opts = node.get('tls_opts', None)
                 if node.get('listen_address', ''):
                     address = node['listen_address']
             desc.add_party(node['party'], address)
         _fill_link_desc_attrs(link_desc=link_desc, tls_opts=tls_opts, desc=desc)
 
         if use_link:
@@ -308,14 +310,18 @@
             self.link = None
 
         self.conf = json_format.Parse(
             json.dumps(cluster_def['runtime_config']), spu.RuntimeConfig()
         )
         self.runtime = spu.Runtime(self.link, self.conf)
         self.share_seq_id = 0
+        self.id = id
+
+    def __repr__(self):
+        return f"SPURuntime(device_id={self.id}, party={self.party})"
 
     def get_new_share_name(self) -> str:
         self.share_seq_id += 1
         return f"{self.share_seq_id}"
 
     def infeed_share(self, val: Any) -> Any:
         flatten_val, flatten_tree = jax.tree_util.tree_flatten(val)
@@ -548,15 +554,14 @@
 
             if report['intersection_count'] == -1:
                 # can not get result, return None
                 return None
             else:
                 # load result dataframe from temp file
                 return pd.read_csv(output_path)
-            
 
     def psi_csv(
         self,
         key: Union[str, List[str]],
         input_path: str,
         output_path: str,
         receiver: str,
@@ -1179,14 +1184,160 @@
             report = pir.pir_client(self.link, config)
 
         return {
             'party': party,
             'data_count': report.data_count,
         }
 
+    def pir_memory_query(
+        self,
+        server: str,
+        config: Dict,
+        protocol="KEYWORD_PIR_LABELED_PSI",
+    ):
+        """Private information retrival online query phase.
+        Args:
+            server (str): Which party is pir server.
+            config (dict): Server/Client config dict
+                For example:
+
+                .. code:: python
+
+                    {
+                        # client config
+                        alice: {
+                            'input_path': '/path/intput.csv',
+                            'key_columns': 'id',
+                            'output_path': '/path/output.csv',
+                        },
+                        # server config
+                        bob: {
+                            'input_path': '/path/server.csv',
+                            'key_columns': 'id',
+                            'label_columns': 'label',
+                            'num_per_query': '1',
+                            'label_max_len': '20',
+                        },
+                    }
+
+                server config dict must have:
+                    'input_path', 'key_columns', 'label_columns', 'oprf_key_path',
+                    'num_per_query', 'label_max_len'
+                    input_path (str): Client's CSV file path. comma separated and contains header.
+                        Use an absolute path.
+                    key_columns (str, List[str]): Column(s) used as pir key
+                    label_columns (str, List[str]): Column(s) used as pir label
+                    num_per_query (int): Items number per query.
+                    label_max_len (int): Max number bytes of label, padding data to label_max_len
+                        Max label bytes length add 4 bytes(len).
+                client config dict must have:
+                    'input_path','key_columns', 'output_path'
+                    input_path (str): Client's CSV file path. comma separated and contains header.
+                        Use an absolute path.
+                    key_columns (str, List[str]): Column(s) used as pir key
+                    output_path (str): Query result save to output_path, csv format.
+        Returns:
+            Dict: PIR report output by SPU.
+        """
+
+        pir_client_config_names = [
+            'input_path',
+            'key_columns',
+            'output_path',
+        ]
+        pir_setup_config_names = [
+            'input_path',
+            'key_columns',
+            'label_columns',
+            'num_per_query',
+            'label_max_len',
+        ]
+
+        party = self.cluster_def['nodes'][self.rank]['party']
+        server_rank = -1
+        for i, node in enumerate(self.cluster_def['nodes']):
+            if node['party'] == server:
+                server_rank = i
+                break
+        assert server_rank >= 0, f'invalid server: {server}'
+
+        if self.rank == server_rank:
+            # check config dict
+            for name, value in config.items():
+                assert (
+                    isinstance(name, str) and name
+                ), f'Link desc param name shall be a valid string but got {type(name)}.'
+                if name not in pir_setup_config_names:
+                    raise InvalidArgumentError(
+                        f'Unsupported param {name} in pir server config desc, '
+                        f'{pir_setup_config_names} are now available only.'
+                    )
+
+            for name in pir_setup_config_names:
+                if name not in config.keys():
+                    raise InvalidArgumentError(
+                        f'param {name} must in pir server config'
+                    )
+
+            packed_bytes = struct.pack('?is', True, 1, b'\x00')
+            self.link.send(self.link.next_rank(), packed_bytes)
+            logging.info(f"rank:{self.rank} send {len(packed_bytes)} sync status")
+
+            config = pir.PirSetupConfig(
+                pir_protocol=pir.PirProtocol.Value(protocol),
+                store_type=pir.KvStoreType.Value("LEVELDB_KV_STORE"),
+                input_path=config['input_path'],
+                key_columns=config['key_columns'],
+                label_columns=config['label_columns'],
+                num_per_query=config['num_per_query'],
+                label_max_len=config['label_max_len'],
+                oprf_key_path='',
+                setup_path='::memory',
+            )
+            report = pir.pir_memory_server(self.link, config)
+
+        else:
+            # check config dict
+            for name, value in config.items():
+                assert (
+                    isinstance(name, str) and name
+                ), f'Link desc param name shall be a valid string but got {type(name)}.'
+                if name not in pir_client_config_names:
+                    raise InvalidArgumentError(
+                        f'Unsupported param {name} in pir client config desc, '
+                        f'{pir_client_config_names} are now available only.'
+                    )
+
+            for name in pir_client_config_names:
+                if name not in config.keys():
+                    raise InvalidArgumentError(
+                        f'param {name} must in pir client config'
+                    )
+
+            if isinstance(config['key_columns'], str):
+                key_columns = [config['key_columns']]
+            elif isinstance(config['key_columns'], List):
+                key_columns = config['key_columns']
+
+            recv_bytes = self.link.recv(self.link.next_rank())
+            logging.info(f"rank:{self.rank} recv {len(recv_bytes)} sync status")
+
+            config = pir.PirClientConfig(
+                pir_protocol=pir.PirProtocol.Value(protocol),
+                input_path=config['input_path'],
+                key_columns=key_columns,
+                output_path=config['output_path'],
+            )
+            report = pir.pir_client(self.link, config)
+
+        return {
+            'party': party,
+            'data_count': report.data_count,
+        }
+
 
 def _argnames_partial_except(fn, static_argnames, kwargs):
     if static_argnames is None:
         return fn, kwargs
 
     assert isinstance(
         static_argnames, (str, Iterable)
@@ -1243,14 +1394,15 @@
 class SPU(Device):
     def __init__(
         self,
         cluster_def: Dict,
         link_desc: Dict = None,
         log_options: spu_logging.LogOptions = spu_logging.LogOptions(),
         use_link: bool = True,
+        id: str = None,
     ):
         """SPU device constructor.
 
         Args:
             cluster_def: SPU cluster definition. More details refer to
                 `SPU runtime config <https://www.secretflow.org.cn/docs/spu/en/reference/runtime_config.html>`_.
 
@@ -1342,28 +1494,30 @@
             json.dumps(cluster_def['runtime_config']), spu.RuntimeConfig()
         )
         self.world_size = len(self.cluster_def['nodes'])
         self.actors = {}
         self._task_id = -1
         self.io = SPUIO(self.conf, self.world_size)
         self.use_link = use_link
+        self.id = id
         self.init()
 
     def init(self):
         """Init SPU runtime in each party"""
         for rank, node in enumerate(self.cluster_def['nodes']):
             self.actors[node['party']] = (
                 sfd.remote(SPURuntime)
                 .party(node['party'])
                 .remote(
                     rank,
                     self.cluster_def,
                     self.link_desc,
                     self.log_options,
                     self.use_link,
+                    self.id,
                 )
             )
 
     def reset(self):
         """Reset spu to clear corrupted internal state, for test only"""
         self.shutdown()
         time.sleep(0.5)
@@ -1388,16 +1542,18 @@
 
                 return SPUObject(self, meta, shares_name)
 
         return jax.tree_util.tree_map(place, (args, kwargs))
 
     def dump(self, obj: SPUObject, paths: List[str]):
         assert obj.device == self, "obj must be owned by this device."
+        ret = []
         for i, actor in enumerate(self.actors.values()):
-            actor.dump.remote(obj.meta, obj.shares_name[i], paths[i])
+            ret.append(actor.dump.remote(obj.meta, obj.shares_name[i], paths[i]))
+        return ret
 
     def load(self, paths: List[str]) -> SPUObject:
         outputs = [None] * self.world_size
         for i, actor in enumerate(self.actors.values()):
             actor_out = actor.load.options(num_returns=2).remote(paths[i])
 
             outputs[i] = actor_out
@@ -1802,7 +1958,65 @@
         return dispatch(
             'pir_query',
             self,
             server,
             config,
             protocol,
         )
+
+    def pir_memory_query(
+        self,
+        server: str,
+        config: Dict,
+        protocol="KEYWORD_PIR_LABELED_PSI",
+    ):
+        """Private information retrival online query.
+        Args:
+            server (str): Which party is pir server.
+            config (dict): Server/Client config dict
+                For example
+
+                .. code:: python
+
+                    {
+                        # client config
+                        alice: {
+                            'input_path': '/path/intput.csv',
+                            'key_columns': 'id',
+                            'output_path': '/path/output.csv',
+                        },
+                        # server config
+                        bob: {
+                            'input_path': '/path/server.csv',
+                            'key_columns': 'id',
+                            'label_columns': 'label',
+                            'num_per_query': '1',
+                            'label_max_len': '20',
+                        },
+                    }
+
+                server config dict must have:
+                    'input_path', 'key_columns', 'label_columns', 'oprf_key_path',
+                    'num_per_query', 'label_max_len'
+                    input_path (str): Client's CSV file path. comma separated and contains header.
+                        Use an absolute path.
+                    key_columns (str, List[str]): Column(s) used as pir key
+                    label_columns (str, List[str]): Column(s) used as pir label
+                    num_per_query (int): Items number per query.
+                    label_max_len (int): Max number bytes of label, padding data to label_max_len
+                        Max label bytes length add 4 bytes(len).
+                client config dict must have:
+                    'input_path','key_columns', 'output_path'
+                    input_path (str): Client's CSV file path. comma separated and contains header.
+                        Use an absolute path.
+                    key_columns (str, List[str]): Column(s) used as pir key
+                    output_path (str): Query result save to output_path, csv format.
+        Returns:
+            Dict: PIR report output by SPU.
+        """
+        return dispatch(
+            'pir_memory_query',
+            self,
+            server,
+            config,
+            protocol,
+        )
```

## secretflow/device/device/type_traits.py

```diff
@@ -40,30 +40,30 @@
 
 HEU_SPU_DT_SWITCHER = {
     "DT_I1": spu_pb2.DataType.DT_I1,
     "DT_I8": spu_pb2.DataType.DT_I8,
     "DT_I16": spu_pb2.DataType.DT_I16,
     "DT_I32": spu_pb2.DataType.DT_I32,
     "DT_I64": spu_pb2.DataType.DT_I64,
-    "DT_FXP": spu_pb2.DataType.DT_FXP,
+    "DT_FXP": spu_pb2.DataType.DT_F32,
 }
 
 
 def heu_datatype_to_spu(heu_dt):
     assert heu_dt in HEU_SPU_DT_SWITCHER, f"Unsupported heu datatype {heu_dt}"
     return HEU_SPU_DT_SWITCHER.get(heu_dt)
 
 
 SPU_HEU_DT_SWITCHER = {
     spu_pb2.DataType.DT_I1: "DT_I1",
     spu_pb2.DataType.DT_I8: "DT_I8",
     spu_pb2.DataType.DT_I16: "DT_I16",
     spu_pb2.DataType.DT_I32: "DT_I32",
     spu_pb2.DataType.DT_I64: "DT_I64",
-    spu_pb2.DataType.DT_FXP: "DT_FXP",
+    spu_pb2.DataType.DT_F32: "DT_FXP",
 }
 
 
 def spu_datatype_to_heu(spu_dt):
     assert spu_dt in SPU_HEU_DT_SWITCHER, f"Unsupported spu datatype {spu_dt}"
     return SPU_HEU_DT_SWITCHER.get(spu_dt)
```

## secretflow/device/kernels/spu.py

```diff
@@ -521,7 +521,39 @@
                 iconfig,
                 protocol,
             )
         )
 
     # wait for all tasks done
     return sfd.get(res)
+
+
+@register(DeviceType.SPU)
+def pir_memory_query(
+    device: SPU,
+    server: str,
+    config: Dict[Device, Dict],
+    protocol="KEYWORD_PIR_LABELED_PSI",
+):
+    assert isinstance(device, SPU), f'device must be SPU device'
+    assert isinstance(server, str), f'server must be str'
+    assert isinstance(config, Dict), f'config must be str'
+
+    assert server in device.actors.keys(), f'invalid server party name {server}'
+
+    assert 2 == len(
+        device.actors
+    ), f'unexpected number({len(device.actors)}) of partys, should be 2'
+
+    res = []
+    for dev, iconfig in config.items():
+        actor = device.actors[dev.party]
+        res.append(
+            actor.pir_memory_query.remote(
+                server,
+                iconfig,
+                protocol,
+            )
+        )
+
+    # wait for all tasks done
+    return sfd.get(res)
```

## secretflow/kuscia/entry.py

```diff
@@ -9,106 +9,67 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-import multiprocessing
 import subprocess
 import sys
 
-from absl import app, flags
+import click
 
-import secretflow as sf
-from secretflow.component.entry import run
-from secretflow.kuscia.task_config import TaskConfig
+from secretflow.component.entry import comp_eval
+from secretflow.kuscia.ray_config import RayConfig
+from secretflow.kuscia.sf_config import get_sf_cluster_config
+from secretflow.kuscia.task_config import KusicaTaskConfig
 
-_LOG_FORMAT = '%(asctime)s|{}|%(levelname)s|fascia|%(filename)s:%(funcName)s:%(lineno)d| %(message)s'
+_LOG_FORMAT = "%(asctime)s|{}|%(levelname)s|fascia|%(filename)s:%(funcName)s:%(lineno)d| %(message)s"
 
-flags.DEFINE_string("task_config_path", None, "Task config file path.")
-FLAGS = flags.FLAGS
 
-_RAY_GRPC_ENV = 'RAY_BACKEND_LOG_LEVEL=debug ' 'RAY_grpc_enable_http_proxy=true '
+def start_ray(ray_conf: RayConfig):
+    logging.info(f"ray_conf: {ray_conf}")
 
-
-def start_ray(task_conf: TaskConfig):
-    logging.info(f'task_conf: {task_conf}')
-
-    ray_cmd = (
-        f'{_RAY_GRPC_ENV}'
-        f'OMP_NUM_THREADS={multiprocessing.cpu_count()} '
-        'ray start --head --include-dashboard=false --disable-usage-stats'
-        f' --num-cpus=8'
-        f' --node-ip-address={task_conf.ray_node_ip_address}'
-        f' --port={task_conf.ray_gcs_port}'
-    )
-
-    if task_conf.ray_node_manager_port:
-        ray_cmd += f' --node-manager-port={task_conf.ray_node_manager_port}'
-    if task_conf.ray_object_manager_port:
-        ray_cmd += f' --object-manager-port={task_conf.ray_object_manager_port}'
-    if task_conf.ray_client_server_port:
-        ray_cmd += f' --ray-client-server-port={task_conf.ray_client_server_port}'
-    if task_conf.ray_worker_ports:
-        ray_cmd += (
-            f' --worker-port-list={",".join(map(str, task_conf.ray_worker_ports))}'
-        )
+    ray_cmd = ray_conf.generate_ray_cmd()
 
     logging.info(
-        f'Trying to start ray head node at {task_conf.ray_node_ip_address}, start command: {ray_cmd}'
+        f"Trying to start ray head node at {ray_conf.ray_node_ip_address}, start command: {ray_cmd}"
     )
 
     process = subprocess.run(ray_cmd, capture_output=True, shell=True)
+
     if process.returncode != 0:
-        err_msg = f'Failed to start ray head node, start command: {ray_cmd}, stderr: {process.stderr}'
+        err_msg = f"Failed to start ray head node, start command: {ray_cmd}, stderr: {process.stderr}"
         logging.critical(err_msg)
-        logging.critical(f'This processor will exit now!')
+        logging.critical("This process will exit now!")
         sys.exit(-1)
     else:
         logging.info(process.stdout)
         logging.info(
-            f'Succeeded to start ray head node at {task_conf.ray_node_ip_address}.'
+            f"Succeeded to start ray head node at {ray_conf.ray_node_ip_address}."
         )
 
-        logging.info(
-            f'Starting secretflow with cluster config: {task_conf.cluster_config}'
-        )
-        retry_policy = {
-            "maxAttempts": 5,
-            "initialBackoff": "20s",
-            "maxBackoff": "20s",
-            "backoffMultiplier": 1,
-            "retryableStatusCodes": ["UNAVAILABLE"],
-        }
-        sf.init(
-            address=f'{task_conf.ray_node_ip_address}:{task_conf.ray_gcs_port}',
-            cluster_config=task_conf.cluster_config,
-            logging_level='debug',
-            cross_silo_grpc_retry_policy=retry_policy,
-            cross_silo_send_max_retries=3,
-        )
-
-
-def main(argv):
-    del argv
 
-    task_conf = TaskConfig().parse_from_file(FLAGS.task_config_path)
+@click.command()
+@click.argument("task_config_path", type=click.Path(exists=True))
+def main(task_config_path):
+    task_conf = KusicaTaskConfig.from_file(task_config_path)
 
     logging.basicConfig(
         stream=sys.stdout,
         level=logging.DEBUG,
         format=_LOG_FORMAT.format(task_conf.party_name),
         force=True,
     )
 
-    start_ray(task_conf)
+    ray_config = RayConfig.from_kuscia_task_config(task_conf)
+    start_ray(ray_config)
 
-    run(task_conf.comp_node, task_conf.spu_cluster_config)
-    logging.info('Succeeded to run component.')
+    sf_cluster_config = get_sf_cluster_config(task_conf)
+    res = comp_eval(task_conf.sf_node_eval_param, sf_cluster_config)
+    logging.info(f"Succeeded to run component. The result is {res}")
 
-    sf.shutdown()
     sys.exit(0)
 
 
 if __name__ == "__main__":
-    app.run(main)
+    main()
```

## secretflow/kuscia/task_config.py

```diff
@@ -8,138 +8,85 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import functools
 from dataclasses import dataclass
-from typing import Dict, List, Union
+from typing import Dict
 
-import spu
-import yaml
 from google.protobuf import json_format
 
-from secretflow.protos.component.node_def_pb2 import NodeDef
-from secretflow.protos.kuscia.kuscia_task_pb2 import AllocatedPorts, ClusterDefine
+from secretflow.protos.component.cluster_pb2 import SFClusterDesc, StorageConfig
+from secretflow.protos.component.evaluation_pb2 import NodeEvalParam
+from secretflow.kuscia.proto.api.v1alpha1.kusciatask.kuscia_task_pb2 import (
+    AllocatedPorts,
+    ClusterDefine,
+)
 
 
 @dataclass
-class TaskConfig:
-    task_id: str = None
-    party_id: int = None
-    party_name: str = None
-
-    ray_node_ip_address: str = None
-    ray_gcs_port: int = None
-    ray_node_manager_port: int = None
-    ray_object_manager_port: int = None
-    ray_client_server_port: int = None
-    ray_worker_ports: List[int] = None
-    spu_port: int = None
-    fed_port: int = None
-
-    cluster_config: Dict[str, Union[str, Dict[str, str]]] = None
-
-    spu_cluster_config: Dict[
-        str,
-        Union[
-            List[str],
-            Dict[str, Union[List[Dict[str, str]], Dict[str, Union[int, bool]]]],
-        ],
-    ] = None
-
-    comp_node: NodeDef = None
+class KusicaTaskConfig:
+    task_id: str
+    task_cluster_def: ClusterDefine
+    task_allocated_ports: AllocatedPorts
+    sf_node_eval_param: NodeEvalParam = None
+    sf_cluster_desc: SFClusterDesc = None
+    sf_storage_config: Dict[str, StorageConfig] = None
+
+    @functools.cached_property
+    def party_name(self):
+        party_id = self.task_cluster_def.self_party_idx
+        return self.task_cluster_def.parties[party_id].name
+
+    # NOTE(junfeng): the format of kuscia task is subject to modify.
+    @classmethod
+    def from_json(cls, req: Dict):
+        task_id = req["task_id"]
+        task_cluster_def = ClusterDefine()
+        json_format.Parse(req["task_cluster_def"], task_cluster_def)
+        task_allocated_ports = AllocatedPorts()
+        json_format.Parse(req["allocated_ports"], task_allocated_ports)
+
+        if "task_input_config" in req:
+            sf_node_eval_param = NodeEvalParam()
+            json_format.ParseDict(
+                req["task_input_config"]["sf_node_eval_param"], sf_node_eval_param
+            )
+            sf_cluster_desc = SFClusterDesc()
+            json_format.ParseDict(
+                req["task_input_config"]["sf_cluster_desc"], sf_cluster_desc
+            )
 
-    def parse_from_file(self, task_config_path: str):
-        with open(task_config_path) as f:
-            cluster_define = ClusterDefine()
-            allocated_port = AllocatedPorts()
-            self.comp_node = NodeDef()
-
-            configs = yaml.safe_load(f)
-            self.task_id = configs['task_id']
-            json_format.Parse(configs['task_input_config'], self.comp_node)
-            json_format.Parse(configs['task_input_cluster_def'], cluster_define)
-            json_format.Parse(configs['allocated_ports'], allocated_port)
-
-            self.party_id = cluster_define.self_party_idx
-            self.party_name = cluster_define.parties[self.party_id].name
-            self.ray_worker_ports = []
-            self.cluster_config = {}
-
-            self.spu_cluster_config = {}
-            self.spu_cluster_config["pyu"] = []
-            self.spu_cluster_config["spu"] = {"nodes": []}
-
-            for port in allocated_port.ports:
-                if port.name.startswith('ray-worker'):
-                    self.ray_worker_ports.append(port.port)
-                elif port.name == 'spu':
-                    self.spu_port = port.port
-                elif port.name == 'node-manager':
-                    self.ray_node_manager_port = port.port
-                elif port.name == 'object-manager':
-                    self.ray_object_manager_port = port.port
-                elif port.name == 'client-server':
-                    self.ray_client_server_port = port.port
-                elif port.name == 'fed':
-                    self.fed_port = port.port
-
-            self.cluster_config['parties'] = {}
-            for party in cluster_define.parties:
-                self.spu_cluster_config["pyu"].append(party.name)
-                if party.name != self.party_name:
-                    for service in party.services:
-                        if service.port_name == 'fed':
-                            if len(service.endpoints[0].split(':')) < 2:
-                                service.endpoints[0] += ':80'
-                            self.cluster_config['parties'][party.name] = {
-                                'address': service.endpoints[0]
-                            }
-                        elif service.port_name == 'spu':
-                            if len(service.endpoints[0].split(':')) < 2:
-                                service.endpoints[0] += ':80'
-                            self.spu_cluster_config["spu"]["nodes"].append(
-                                {
-                                    'party': party.name,
-                                    'id': f'{party.name}:0',
-                                    # add "http://" to force brpc to set the correct Host
-                                    'address': f'http://{service.endpoints[0]}',
-                                }
-                            )
-                else:
-                    for service in cluster_define.parties[self.party_id].services:
-                        if service.port_name == 'global':
-                            segs = service.endpoints[0].split(':')
-                            self.ray_node_ip_address = segs[0]
-                            if len(segs) == 2:
-                                self.ray_gcs_port = int(segs[1])
-                            else:
-                                self.ray_gcs_port = 80
-
-            self.cluster_config['parties'][self.party_name] = {
-                'address': f'0.0.0.0:{self.fed_port}'
-            }
-            self.cluster_config['self_party'] = self.party_name
-
-            self.spu_cluster_config['spu']['nodes'].append(
-                {
-                    'party': self.party_name,
-                    'id': f'{self.party_name}:0',
-                    'address': f'0.0.0.0:{self.spu_port}',
-                }
+            sf_storage_config = {}
+            for storage_party, config in req["task_input_config"][
+                "sf_storage_config"
+            ].items():
+                storage_config_pb = StorageConfig()
+                json_format.ParseDict(config, storage_config_pb)
+                sf_storage_config[storage_party] = storage_config_pb
+
+            return cls(
+                task_id,
+                task_cluster_def,
+                task_allocated_ports,
+                sf_node_eval_param,
+                sf_cluster_desc,
+                sf_storage_config,
+            )
+        else:
+            return cls(
+                task_id,
+                task_cluster_def,
+                task_allocated_ports,
             )
-            self.spu_cluster_config['spu']['nodes'].sort(key=lambda x: x['party'])
 
-            if len(cluster_define.parties) == 2:
-                self.spu_cluster_config['spu']['runtime_config'] = {
-                    'protocol': spu.spu_pb2.SEMI2K,
-                    'field': spu.spu_pb2.FM128,
-                }
-            elif len(cluster_define.parties) == 3:
-                self.spu_cluster_config['spu']['runtime_config'] = {
-                    'protocol': spu.spu_pb2.ABY3,
-                    'field': spu.spu_pb2.FM64,
-                }
+    @classmethod
+    def from_file(cls, task_config_path: str):
+        with open(task_config_path) as f:
+            import json
 
-        return self
+            configs = json.load(f)
+            configs["task_input_config"] = json.loads(configs["task_input_config"])
+            return cls.from_json(configs)
```

## secretflow/ml/boost/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Ant Group Co., Ltd.
+# Copyright 2023 Ant Group Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

## secretflow/ml/boost/homo_boost/homo_decision_tree.py

```diff
@@ -18,17 +18,16 @@
 
 """ Homo Decision Tree """
 import logging
 from concurrent.futures import ThreadPoolExecutor
 from functools import reduce
 
 import numpy as np
-
+import pandas as pd
 import secretflow.device.link as link
-from secretflow.data.horizontal import HDataFrame
 from secretflow.ml.boost.homo_boost.tree_core.decision_tree import DecisionTree
 from secretflow.ml.boost.homo_boost.tree_core.feature_histogram import (
     FeatureHistogram,
     HistogramBag,
 )
 from secretflow.ml.boost.homo_boost.tree_core.node import Node
 from secretflow.ml.boost.homo_boost.tree_param import TreeParam
@@ -49,24 +48,23 @@
         label_key: unique column name for label key
 
     """
 
     def __init__(
         self,
         tree_param: TreeParam = None,
-        data: HDataFrame = None,
+        data: pd.DataFrame = None,
         bin_split_points: np.ndarray = None,
         group_id: int = None,
         tree_id: int = None,
         iter_round: int = None,
         hess_key: str = "hess",
         grad_key: str = "grad",
         label_key: str = "label",
     ):
-
         super(HomoDecisionTree, self).__init__(
             tree_param, grad_key=grad_key, hess_key=hess_key, label_key=label_key
         )
 
         self.data = data
 
         self.bin_split_points = bin_split_points
@@ -125,15 +123,14 @@
             self.valid_features = link.recv_from_server(
                 name=self.key('valid_features_bylevel'),
                 version=self._sync_version,
             )
 
     def cal_root_node(self):
         if self.role == link.CLIENT:
-
             g_sum, h_sum = self.get_grad_hess_sum(self.data)
             # initialize node
             link.send_to_server(
                 name=self.key('root_g_sum'), value=g_sum, version=self._sync_version
             )
             link.send_to_server(
                 name=self.key('root_h_sum'), value=h_sum, version=self._sync_version
@@ -261,15 +258,14 @@
             if self.role == link.CLIENT:
                 logging.debug(f'start to fit layer {dep}')
                 agg_local_histograms = []
 
                 for batch_id, idx in enumerate(
                     range(0, len(self.cur_layer_node), self.max_split_nodes)
                 ):
-
                     local_hist_bags = HomoDecisionTree.cal_local_hist_bags(
                         self.cur_layer_node[idx : idx + self.max_split_nodes],
                         self.cur_layer_datas[idx : idx + self.max_split_nodes],
                         self.bin_split_points,
                         self.valid_features,
                         self.use_missing,
                         self.grad_key,
```

## secretflow/ml/boost/homo_boost/boost_core/core.py

```diff
@@ -15,19 +15,19 @@
 import logging
 import os
 import pathlib
 import uuid
 from typing import Callable, Dict, List, Union
 
 import numpy
+import pandas as pd
 import xgboost.core as xgb_core
+from sklearn.model_selection import train_test_split
 
 import secretflow.device.link as link
-from secretflow.data.horizontal import HDataFrame
-from secretflow.data.split import train_test_split
 from secretflow.ml.boost.homo_boost.homo_decision_tree import HomoDecisionTree
 from secretflow.ml.boost.homo_boost.tree_param import TreeParam
 from secretflow.utils.errors import InvalidArgumentError
 
 
 class FedBooster(xgb_core.Booster):
     """Federated Booster internal
@@ -66,15 +66,15 @@
         )
         self.save_model(self.model_path)
 
     def federate_update(
         self,
         params: Dict,
         dtrain: xgb_core.DMatrix,
-        hdata: HDataFrame,
+        hdata: pd.DataFrame,
         bin_split_points: List,
         iter_round: int = None,
         fobj: Callable = None,
     ):
         """
         federated update function, a variant in xgboost update
         Args:
@@ -108,21 +108,14 @@
             base_score=params['base_score'] if 'base_score' in params else 0.5,
             random_state=params['random_state'] if 'random_state' in params else 1234,
             num_parallel=params['n_thread'] if 'n_thread' in params else None,
             subsample=params['subsample'] if 'subsample' in params else 1.0,
             decimal=params['decimal'] if 'decimal' in params else 10,
             num_class=params['num_class'] if 'num_class' in params else 0,
         )
-        # sample by row
-        if tree_param.subsample < 1.0:
-            train_data, _ = train_test_split(
-                hdata, ratio=tree_param.subsample, random_state=tree_param.random_state
-            )
-        else:
-            train_data = hdata
 
         pred = self.predict(dtrain, output_margin=True, training=True)
         grad, hess = fobj(pred, dtrain)
         group_num = numpy.expand_dims(pred, axis=-1).shape[1]
 
         # single thread
         if group_num > 2:
@@ -139,14 +132,23 @@
                     grad[:, group_id],
                     hess[:, group_id],
                 )
             else:
                 hdata[self.grad_key], hdata[self.hess_key] = grad, hess
 
             tree_id = iter_round * group_num + group_id
+            # sample by row
+            if tree_param.subsample < 1.0:
+                train_data, _ = train_test_split(
+                    hdata,
+                    train_size=tree_param.subsample,
+                    random_state=tree_param.random_state,
+                )
+            else:
+                train_data = hdata
             decision_tree = HomoDecisionTree(
                 tree_param=tree_param,
                 data=train_data,
                 bin_split_points=bin_split_points,
                 group_id=group_id,
                 tree_id=tree_id,
                 iter_round=iter_round,
```

## secretflow/ml/boost/homo_boost/tree_core/decision_tree.py

```diff
@@ -55,15 +55,14 @@
         tree_id: int = None,
         group_id: int = None,
         iter_round: int = None,
         grad_key: str = "grad",
         hess_key: str = "hess",
         label_key: str = "label",
     ):
-
         # input parameters
         self.criterion_method = tree_param.criterion_method
         self.criterion_params = [
             tree_param.reg_lambda,
             tree_param.reg_alpha,
             tree_param.decimal,
         ]
```

## secretflow/ml/boost/sgb_v/model.py

```diff
@@ -10,26 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 from pathlib import Path
-from typing import Dict, Union
+from typing import Dict, Union, List
 
 import jax.numpy as jnp
 
 from secretflow.data import FedNdarray, PartitionWay
 from secretflow.data.vertical import VDataFrame
 from secretflow.device import PYU, PYUObject, reveal, wait
 
 from .core.distributed_tree.distributed_tree import DistributedTree
 from .core.distributed_tree.distributed_tree import from_dict as dt_from_dict
 from .core.preprocessing.params import RegType
-from .core.preprocessing.preprocessing import prepare_dataset
+from secretflow.ml.boost.core.data_preprocess import prepare_dataset
 from .core.pure_numpy_ops.pred import sigmoid
 
 
 common_path_postfix = "/common.json"
 leaf_weight_postfix = "/leaf_weight.json"
 split_tree_postfix = "/split_tree.json"
 
@@ -45,16 +45,15 @@
             label_holder: PYU device, label holder's PYU device.
             objective: RegType, specifies doing logistic regression or regression
             base: float
         """
         self.label_holder = label_holder
         self.objective = objective
         self.base = base
-        # List[DistributedTree]
-        self.trees = list()
+        self.trees: List[DistributedTree] = list()
 
     def _insert_distributed_tree(self, tree: DistributedTree):
         self.trees.append(tree)
 
     def predict(
         self,
         dtrain: Union[FedNdarray, VDataFrame],
```

## secretflow/ml/boost/sgb_v/sgb.py

```diff
@@ -26,31 +26,33 @@
 from secretflow.device import HEU, PYU, PYUObject, reveal, wait
 from secretflow.device.device.heu import HEUMoveConfig
 
 from .core.cache.level_cache import LevelCache
 from .core.distributed_tree.distributed_tree import DistributedTree
 from .core.label_holder.label_holder import LabelHolder
 from .core.preprocessing.params import LabelHolderInfo
-from .core.preprocessing.preprocessing import prepare_dataset, validate_sgb_params_dict
+from .core.preprocessing.preprocessing import validate_sgb_params_dict
+from secretflow.ml.boost.core.data_preprocess import validate
 from .core.split_tree_trainer.split_tree_trainer import SplitTreeTrainer as Worker
 from .model import SgbModel
 
 logging.basicConfig(
-    format='%(asctime)s %(levelname)-8s %(message)s',
+    format="%(asctime)s %(levelname)-8s %(message)s",
     level=logging.INFO,
-    datefmt='%Y-%m-%d %H:%M:%S',
+    datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
 class Sgb:
     """
     This class provides both classification and regression tree boosting (also known as GBDT, GBM)
     for vertical split dataset setting by using secure boost.
 
     SGB is short for SecureBoost. Compared to its safer counterpart SS-XGB, SecureBoost focused on protecting label holder.
+    Check https://arxiv.org/abs/1901.08755.
 
     Args:
         heu: secret device running homomorphic encryptions
 
     """
 
     def __init__(self, heu: HEU) -> None:
@@ -60,29 +62,25 @@
     def _prepare(
         self,
         params: Dict,
         dataset: Union[FedNdarray, VDataFrame],
         label: Union[FedNdarray, VDataFrame],
         audit_paths: Dict = {},
     ) -> None:
-        x, x_shape = prepare_dataset(dataset)
-        y, y_shape = prepare_dataset(label)
-        assert len(x_shape) == 2, "only support 2D-array on dtrain"
-        assert len(y_shape) == 1 or y_shape[1] == 1, "label only support one label col"
+        x, _, y, y_shape = validate(dataset, label)
+
         self.samples = y_shape[0]
-        assert self.samples == x_shape[0], "dtrain & label are not aligned"
-        assert len(y.partitions) == 1, "label only support one partition"
-        label_holder = [*y.partitions.keys()][0]
+        label_holder = y.device
         assert (
             label_holder.party == self.heu.sk_keeper_name()
         ), f"HEU sk keeper party {self.heu.sk_keeper_name()}, mismatch with label_holder device's party {label_holder.party}"
         # determine label_holder from label holder
         self.label_holder = label_holder
 
-        self.y = list(y.partitions.values())[0]
+        self.y = y
         self.workers = [Worker(idx, device=pyu) for idx, pyu in enumerate(x.partitions)]
         self.x = x.partitions
 
         validated_params = validate_sgb_params_dict(params)
 
         self.subsample = validated_params.subsample
         self.seed = validated_params.seed
@@ -137,14 +135,15 @@
             for worker in self.workers
             if worker.device != self.label_holder
         }
 
     def _tree_setup(self, tree_num) -> None:
         col_choices = {}
         works_buckets_count = []
+        self.train_label_holder.reset()
         for pyu_work in self.workers:
             choices, count = pyu_work.tree_setup(self.colsample)
             works_buckets_count.append(count)
             if self.colsample < 1:
                 # 1. column sample choices is generate by public param 'seed', choices is not a private value
                 col_choices[pyu_work.device] = choices
 
@@ -173,23 +172,23 @@
             path = None
 
         encypted_gh = (
             self.train_label_holder.get_gh()
             .to(self.heu, move_config(self.label_holder, self.gh_encoder))
             .encrypt(path)
         )
+
         # encrypt once, send once.
         self.encrypted_gh = {
             worker.device: encypted_gh.to(
                 self.heu, move_config(worker.device, self.gh_encoder)
             )
             for worker in self.workers
             if worker.device != self.label_holder
         }
-        wait([self.train_label_holder.get_gh(), *self.encrypted_gh.values()])
         self._sub_sampling()
 
     def train(
         self,
         params: Dict,
         dtrain: Union[FedNdarray, VDataFrame],
         label: Union[FedNdarray, VDataFrame],
@@ -279,15 +278,14 @@
             logging.info(
                 f"epoch {cur_tree_num - 1} time {time.perf_counter() - start}s"
             )
 
         return model
 
     def _train_tree(self, tree_num: int) -> DistributedTree:
-        self.train_label_holder.clear_leaves()
         root_select = self.train_label_holder.root_select()
 
         split_node_selects = root_select
         split_node_indices = [0]
         for level in range(self.depth):
             split_node_selects, split_node_indices = self._train_level(
                 split_node_selects, split_node_indices, level, tree_num
```

## secretflow/ml/boost/sgb_v/core/__init__.py

 * *Ordering differences only*

```diff
@@ -6,8 +6,8 @@
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitations under the License.
```

## secretflow/ml/boost/sgb_v/core/cache/__init__.py

 * *Ordering differences only*

```diff
@@ -6,8 +6,8 @@
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
+# limitations under the License.
```

## secretflow/ml/boost/sgb_v/core/cache/level_cache.py

```diff
@@ -17,14 +17,18 @@
 
 # level cache is not embeded in split tree trainer because HEUObject in PYUObject is not well-defined.
 class LevelCache:
     def __init__(self):
         self.level_nodes_GH = []
         self.cache = None
 
+    def reset(self):
+        self.cache = None
+        self.level_nodes_GH = []
+
     def reset_level_nodes_GH(self):
         self.level_nodes_GH = []
 
     def collect_level_node_GH(self, child_GHL, idx, is_left):
         """collect one level node GH
         Args:
             child_GHL (PYUObject or HEUObject): PYUObject if self.pyu is not None.
```

## secretflow/ml/boost/sgb_v/core/distributed_tree/split_tree.py

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import List, Dict
+from typing import Dict, List
 
 import numpy as np
 from heu import numpy as hnp
 
 
 class SplitTree:
     """Each party will hold one split tree.
@@ -48,14 +48,15 @@
             x: dataset from this partition.
             tree: tree model store by this partition.
 
         Return:
             leaf nodes' selects: List[np.array], length equals leaf number.
         """
         x = x if isinstance(x, np.ndarray) else np.array(x)
+
         return hnp.tree_predict_with_indices(
             x,
             self.split_features,
             self.split_values,
             self.split_indices,
             self.leaf_indices,
         )
```

## secretflow/ml/boost/sgb_v/core/label_holder/label_holder.py

```diff
@@ -53,14 +53,23 @@
         self.level_cache = LevelCache()
         self.leaf_node_selects = []
         self.leaf_node_indices = []
 
     def set_y(self, y: np.ndarray):
         self.y = y.reshape((y.shape[0], 1))
 
+    def reset(self):
+        self.sub_choices = None
+        self.level_cache.reset()
+        self.leaf_node_selects = []
+        self.leaf_node_indices = []
+        self.gh = None
+        self.g = None
+        self.h = None
+
     def init_pred(self) -> np.ndarray:
         """Produce dummy prediction, used at the begin of training in SGB."""
         base = self.base_score
         sample_num = self.sample_num
         return init_pred(base=base, samples=sample_num)
 
     def root_select(self) -> List[np.ndarray]:
```

## secretflow/ml/boost/sgb_v/core/preprocessing/preprocessing.py

```diff
@@ -8,53 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import math
-from typing import Tuple, Union
-
-from secretflow.data import FedNdarray, PartitionWay
-from secretflow.data.vertical import VDataFrame
-
 from .params import RegType, SGBTrainParams
 
 
-def prepare_dataset(
-    ds: Union[FedNdarray, VDataFrame]
-) -> Tuple[FedNdarray, Tuple[int, int]]:
-    """
-    check data setting and get total shape.
-
-    Args:
-        ds: input dataset
-
-    Return:
-        First: dataset in unified type
-        Second: shape concat all partition.
-    """
-    assert isinstance(
-        ds, (FedNdarray, VDataFrame)
-    ), f"ds should be FedNdarray or VDataFrame, got {type(ds)}"
-
-    ds = ds if isinstance(ds, FedNdarray) else ds.values
-
-    assert ds.partition_way == PartitionWay.VERTICAL, (
-        "SGB Only support vertical dataset, "
-        "for horizontal dataset please use secreflow.ml.boost.homo_boost"
-    )
-
-    shape = ds.shape
-    assert math.prod(shape), f"not support empty dataset, shape {shape}"
-
-    return ds, shape
-
-
 def validate_sgb_params_dict(params: dict) -> SGBTrainParams:
     trees = int(params.pop('num_boost_round', 10))
     assert 1 <= trees <= 1024, f"num_boost_round should in [1, 1024], got {trees}"
 
     depth = int(params.pop('max_depth', 5))
     assert depth > 0 and depth <= 16, f"max_depth should in [1, 16], got {depth}"
 
@@ -79,15 +43,15 @@
     assert (
         subsample > 0 and subsample <= 1
     ), f"subsample should in (0, 1], got {subsample}"
 
     colsample = float(params.pop('colsample_by_tree', 1))
     assert (
         colsample > 0 and colsample <= 1
-    ), f"colsample_bytree should in (0, 1], got {colsample}"
+    ), f"colsample_by_tree should in (0, 1], got {colsample}"
 
     base = float(params.pop('base_score', 0))
 
     sketch = params.pop('sketch_eps', 0.1)
     assert sketch > 0 and sketch <= 1, f"sketch_eps should in (0, 1], got {sketch}"
     seed = int(params.pop('seed', 42))
```

## secretflow/ml/boost/sgb_v/core/pure_numpy_ops/boost.py

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List, Tuple
+
 import numpy as np
 
 
 def compute_obj(G: np.ndarray, H: np.ndarray, reg_lambda: float) -> np.ndarray:
     """
     compute objective values of input buckets.
 
@@ -33,15 +34,14 @@
 def compute_weight_from_node_select(
     node_select: np.ndarray,
     g: np.ndarray,
     h: np.ndarray,
     reg_lambda: float,
     learning_rate: float,
 ) -> np.ndarray:
-
     g_sum = np.matmul(node_select, g)
     h_sum = np.matmul(node_select, h)
 
     return compute_weight(g_sum, h_sum, reg_lambda, learning_rate)
 
 
 def compute_weight(
@@ -58,21 +58,17 @@
     Return:
         weight values.
     """
     w = -((G / (H + reg_lambda)) * learning_rate)
     return np.select([H == 0], [0], w)
 
 
-def find_best_splits(
-    level_nodes_G: List[np.array],
-    level_nodes_H: List[np.array],
-    reg_lambda: float,
-    gamma: float,
-) -> Tuple[np.ndarray, np.ndarray]:
-    """find the best split buckets and if gains > gamma"""
+def calculate_gains(
+    level_nodes_G: List[np.ndarray], level_nodes_H: List[np.ndarray], reg_lambda: float
+) -> np.ndarray:
     GL = np.concatenate(level_nodes_G, axis=0)
     HL = np.concatenate(level_nodes_H, axis=0)
 
     # last buckets is the total gradient sum of all samples belong to current level nodes.
     GA = GL[:, -1].reshape(-1, 1)
     HA = HL[:, -1].reshape(-1, 1)
     # gradient sums of right child nodes after splitting by each bucket
@@ -80,11 +76,44 @@
     HR = HA - HL
     obj_l = compute_obj(GL, HL, reg_lambda)
     obj_r = compute_obj(GR, HR, reg_lambda)
 
     # last objective value means split all sample to left, equal to no split.
     obj = obj_l[:, -1].reshape(-1, 1)
     gain = obj_l + obj_r - obj
+    return gain
+
 
+def find_best_splits(
+    level_nodes_G: List[np.array],
+    level_nodes_H: List[np.array],
+    reg_lambda: float,
+    gamma: float,
+) -> Tuple[np.ndarray, np.ndarray]:
+    """find the best split buckets and if gains > gamma"""
+    gain = calculate_gains(level_nodes_G, level_nodes_H, reg_lambda)
     split_buckets = np.argmax(gain, 1)
-    should_split = (np.max(gain, 1) - gamma) > 0
+    should_split = (
+        (np.max(gain, 1) - gamma) > 0
+        if gamma > 0
+        else np.ones(split_buckets.shape).astype(bool)
+    )
     return (split_buckets, should_split)
+
+
+def find_best_splits_with_gains(
+    nodes_G: List[np.array], nodes_H: List[np.array], reg_lambda: float, gamma: float
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    gain = calculate_gains(nodes_G, nodes_H, reg_lambda)
+    split_buckets = np.argmax(gain, 1)
+    split_gains = np.max(gain, 1)
+    should_split = (split_gains - gamma) > 0
+    return (split_buckets, split_gains, should_split)
+
+
+def find_single_best_split(
+    node_indices: List[int],
+    split_buckets: np.ndarray,
+    split_gains: np.ndarray,
+) -> Tuple[int, int, float]:
+    index = np.argmax(split_gains)
+    return (node_indices[index], split_buckets[index], split_gains[index])
```

## secretflow/ml/boost/sgb_v/core/pure_numpy_ops/pred.py

```diff
@@ -41,9 +41,8 @@
         pred
     """
     # get final leaf selects based on collective information
     select = reduce(np.multiply, selects)
     assert (
         select.shape[1] == weights.shape[0]
     ), f"select {select.shape}, weights {weights.shape}"
-
     return np.matmul(select, weights).reshape((select.shape[0]), 1)
```

## secretflow/ml/boost/sgb_v/core/split_tree_trainer/order_map_context.py

```diff
@@ -9,16 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-import math
 from typing import List, Tuple
+from secretflow.ml.boost.core.order_map_tools import qcut
 
 import numpy as np
 
 
 # Deal with order map context of a single partition
 class OrderMapContext:
     """Manage context related to order map, and bucket and split point information derived from it."""
@@ -27,70 +27,15 @@
         self.order_map = None
         self.split_points = None
         self.feature_buckets = None
         self.features = None
         self.buckets = None
 
     def _qcut(self, x: np.ndarray) -> Tuple[np.ndarray, List]:
-        sorted_x = np.sort(x, axis=0)
-        remained_count = len(sorted_x)
-        assert remained_count > 0, 'can not qcut empty x'
-
-        value_category = list()
-        last_value = None
-
-        split_points = list()
-        expected_bin_count = math.ceil(remained_count / self.buckets)
-        current_bin_count = 0
-        for v in sorted_x:
-            if v != last_value:
-                if len(value_category) <= self.buckets:
-                    value_category.append(v)
-
-                if current_bin_count >= expected_bin_count:
-                    split_points.append(v)
-                    if len(split_points) == self.buckets - 1:
-                        break
-                    remained_count -= current_bin_count
-                    expected_bin_count = math.ceil(
-                        remained_count / (self.buckets - len(split_points))
-                    )
-                    current_bin_count = 0
-
-                last_value = v
-            current_bin_count += 1
-
-        if len(value_category) <= self.buckets:
-            # full dataset category count <= buckets
-            # use category as split point.
-            split_points = value_category[1:]
-        elif split_points[-1] != sorted_x[-1]:
-            # add max sample value into split_points like xgboost.
-            split_points.append(sorted_x[-1])
-
-        split_points = list(map(float, split_points))
-
-        def upper_bound_bin(x: float):
-            count = len(split_points)
-            pos = 0
-            while count > 0:
-                step = math.floor(count / 2)
-                v = split_points[pos + step]
-                if x == v:
-                    return pos + step + 1
-                elif x > v:
-                    pos = pos + step + 1
-                    count -= step + 1
-                else:
-                    count = step
-            return pos
-
-        bins = np.vectorize(upper_bound_bin)(x)
-
-        return bins, split_points
+        return qcut(x, self.buckets)
 
     def build_maps(self, x: np.ndarray, buckets: int) -> None:
         """
         split features into buckets and build maps use in train.
 
         Args:
             x: dataset from this partition.
```

## secretflow/ml/boost/sgb_v/core/split_tree_trainer/shuffler.py

```diff
@@ -9,16 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
-import numpy as np
+
 import jax.tree_util
+import numpy as np
+
 from ..pure_numpy_ops.random import create_permuation_with_last_number_fixed
 
 
 class Shuffler:
     def __init__(self):
         self.reindex_list_map = {}
 
@@ -28,15 +30,15 @@
         The random mask is a list of list of int.
         The random mask is private to each worker.
         It should be used to shuffle encrypted gh sum,
         before sending to label holder.
         It should also be applied to restore the correct split bucket,
         after receiving from label holder.
 
-        The key is the index of node in a fixed level.
+        The key is the index of node in a fixed level. (or node index for leaf wise mode)
         We will create one mask each for each fewer number child node selects at a level.
         Note when calculating bucket sums, we only do it for either left or right child.
         The other can be calculated
 
         Args:
             key: int. Each node select corresponds to one key.
             bucket_list: List[int]. List of number of buckets.
@@ -60,12 +62,16 @@
 
     def get_shuffling_indices(self, key: int) -> List[int]:
         return self.reindex_list_map[key]
 
     def reset_shuffle_mask(self):
         self.reindex_list_map = {}
 
+    def reset_shuffle_mask_with_keys(self, keys):
+        for key in keys:
+            self.reindex_list_map.pop(key)
+
     def is_shuffled(self) -> bool:
         return len(self.reindex_list_map) > 0
 
     def undo_shuffle_mask(self, key: int, index: int) -> int:
         return self.reindex_list_map[key][index]
```

## secretflow/ml/boost/sgb_v/factory/factory.py

```diff
@@ -19,15 +19,15 @@
 
 from secretflow.data import FedNdarray
 from secretflow.data.vertical import VDataFrame
 from secretflow.device import HEU
 
 from ..model import SgbModel
 from .booster import GlobalOrdermapBooster
-from .components import LevelWiseTreeTrainer
+from .components import LeafWiseTreeTrainer, LevelWiseTreeTrainer
 
 
 class TreeGrowingMethod(Enum):
     LEVEL = "level"
     LEAF = "leaf"
 
 
@@ -63,44 +63,44 @@
     def set_heu(self, heu: HEU):
         self.heu = heu
 
     def _produce(self) -> GlobalOrdermapBooster:
         assert self.heu is not None, "HEU must be set"
         if self.factory_params.tree_growing_method == TreeGrowingMethod.LEVEL:
             tree_trainer = LevelWiseTreeTrainer()
-            booster = GlobalOrdermapBooster(self.heu, tree_trainer)
-            # this line rectifies any conflicts in default settting of components
-            booster.set_params(booster.get_params())
-            # apply any custom settings
-            booster.set_params(self.params_dict)
-            return booster
         else:
-            assert False, "Feature not supported yet"
+            tree_trainer = LeafWiseTreeTrainer()
+        booster = GlobalOrdermapBooster(self.heu, tree_trainer)
+        # this line rectifies any conflicts in default settting of components
+        booster.set_params(booster.get_params())
+        # apply any custom settings
+        booster.set_params(self.params_dict)
+        return booster
 
     def get_params(self, detailed: bool = False) -> dict:
         """get the params set
 
         Args:
             detailed (bool, optional): If include default settings. Defaults to False.
 
         Returns:
             dict: current params.
         """
         if detailed:
             # detailed option will include all defaults
             if self.factory_params.tree_growing_method == TreeGrowingMethod.LEVEL:
                 tree_trainer = LevelWiseTreeTrainer()
-                booster = GlobalOrdermapBooster(self.heu, tree_trainer)
-                # this line rectifies any conflicts in default settting of components
-                booster.set_params(booster.get_params())
-                # apply any custom settings
-                booster.set_params(self.params_dict)
-                return booster.get_params()
             else:
-                assert False, "Feature not supported yet"
+                tree_trainer = LeafWiseTreeTrainer()
+            booster = GlobalOrdermapBooster(self.heu, tree_trainer)
+            # this line rectifies any conflicts in default settting of components
+            booster.set_params(booster.get_params())
+            # apply any custom settings
+            booster.set_params(self.params_dict)
+            return booster.get_params()
         else:
             # show only customized params
             return self.params_dict
 
     def fit(
         self,
         dataset: Union[FedNdarray, VDataFrame],
```

## secretflow/ml/boost/sgb_v/factory/booster/global_ordermap_booster.py

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
 import logging
 import time
 from dataclasses import dataclass
 from typing import Union
 
 from secretflow.data import FedNdarray
 from secretflow.data.vertical import VDataFrame
@@ -36,49 +37,61 @@
 @dataclass
 class GlobalOrdermapBoosterParams:
     """params specifically belonged to global ordermap booster, not its components.
 
     num_boost_round : int, default=10
                 Number of boosting iterations. Same as number of trees.
                 range: [1, 1024]
+    first_tree_with_label_holder_feature: bool, default=False
+                Whether to train the first tree with label holder's own features.
+                Can increase training speed and label security.
+                The training loss may increase.
     """
 
     num_boost_round: int = 10
+    first_tree_with_label_holder_feature: bool = False
 
 
 class GlobalOrdermapBooster(Composite):
     """
     This class provides both classification and regression tree boosting (also known as GBDT, GBM)
     for vertical split dataset setting by using level wise boost.
     """
 
     def __init__(self, heu: HEU, tree_trainer: TreeTrainer) -> None:
         self.components = GlobalOrdermapBoosterComponents()
         self.params = GlobalOrdermapBoosterParams()
+        self.user_config = {}
         self.heu = heu
         self.tree_trainer = tree_trainer
 
     def _set_booster_params(self, params: dict):
         trees = int(params.pop('num_boost_round', 10))
         assert 1 <= trees <= 1024, f"num_boost_round should in [1, 1024], got {trees}"
         self.params.num_boost_round = trees
+        self.params.first_tree_with_label_holder_feature = bool(
+            params.pop('first_tree_with_label_holder_feature', False)
+        )
 
     def _get_booster_params(self, params: dict):
         params['num_boost_round'] = self.params.num_boost_round
+        params[
+            'first_tree_with_label_holder_feature'
+        ] = self.params.first_tree_with_label_holder_feature
 
     def show_params(self):
         super().show_params()
         self.tree_trainer.show_params()
         print_params(self.params)
 
     def set_params(self, params: dict):
-        print("booster params", params)
         super().set_params(params)
         self.tree_trainer.set_params(params)
         self._set_booster_params(params)
+        self.user_config = params
 
     def get_params(self, params: dict = {}) -> dict:
         super().get_params(params)
         self.tree_trainer.get_params(params)
         self._get_booster_params(params)
         return params
 
@@ -97,17 +110,25 @@
 
         pred = self.components.model_builder.init_pred(x_shape[0])
         self.components.order_map_manager.build_order_map(x)
         self.components.model_builder.init_model()
 
         for tree_index in range(self.params.num_boost_round):
             start = time.perf_counter()
+            if self.params.first_tree_with_label_holder_feature and tree_index == 0:
+                # we are sure the config is small, so ok to copy
+                config = copy.deepcopy(self.user_config)
+                config['label_holder_feature_only'] = True
+                self.tree_trainer.set_params(config)
             tree = self.tree_trainer.train_tree(
                 tree_index, self.components.order_map_manager, y, pred, x_shape
             )
+            if self.params.first_tree_with_label_holder_feature and tree_index == 0:
+                config['label_holder_feature_only'] = False
+                self.tree_trainer.set_params(config)
             self.components.model_builder.insert_tree(tree)
             cur_tree_num = self.components.model_builder.get_tree_num()
 
             if cur_tree_num < self.params.num_boost_round:
                 pred = y.device(lambda x, y: x + y)(pred, tree.predict(x.partitions))
                 wait([pred])
             else:
```

## secretflow/ml/boost/sgb_v/factory/components/__init__.py

```diff
@@ -1,21 +1,21 @@
+from .bucket_sum_calculator import BucketSumCalculator
+from .cache import LevelWiseCache
 from .data_preprocessor import DataPreprocessor
-from .order_map_manager import OrderMapManager
 from .gradient_encryptor import GradientEncryptor
-from .sampler import Sampler
 from .leaf_manager import LeafManager
-from .model_builder import ModelBuilder
 from .loss_computer import LossComputer
-from .tree_trainer import TreeTrainer, LevelWiseTreeTrainer
+from .model_builder import ModelBuilder
 from .node_selector import NodeSelector
-from .cache import LevelWiseCache
+from .order_map_manager import OrderMapManager
+from .sampler import Sampler
 from .shuffler import Shuffler
-from .bucket_sum_calculator import BucketSumCalculator
 from .split_finder import SplitFinder
 from .split_tree_builder import SplitTreeBuilder
+from .tree_trainer import LeafWiseTreeTrainer, LevelWiseTreeTrainer, TreeTrainer
 
 __all__ = [
     'OrderMapManager',
     'GradientEncryptor',
     'Sampler',
     'LeafManager',
     'DataPreprocessor',
@@ -25,8 +25,9 @@
     'NodeSelector',
     'LevelWiseCache',
     'Shuffler',
     'BucketSumCalculator',
     'SplitFinder',
     'SplitTreeBuilder',
     'LevelWiseTreeTrainer',
+    'LeafWiseTreeTrainer',
 ]
```

## secretflow/ml/boost/sgb_v/factory/components/component.py

```diff
@@ -10,21 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import abc
-
+from dataclasses import dataclass, fields
 from typing import List
 
 from secretflow.device import HEU, PYU
 
-from dataclasses import dataclass, fields
-
 
 @dataclass
 class Devices:
     label_holder: PYU
     workers: List[PYU]
     heu: HEU
 
@@ -46,21 +44,19 @@
     def set_devices(self, devices: Devices):
         pass
 
 
 class Composite(Component):
     def __init__(self) -> None:
         self.components = None
-        self.params = None
 
     def show_params(self):
         for field in fields(self.components):
             print("showing the params of component", field.name)
             getattr(self.components, field.name).show_params()
-        print_params(self.params)
 
     def get_params_dict(self, params: dict = {}):
         for field in fields(self.components):
             getattr(self.components, field.name).get_params(params)
 
     def set_params(self, params: dict):
         for field in fields(self.components):
```

## secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/__init__.py

```diff
@@ -9,9 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .bucket_sum_calculator import BucketSumCalculator
+from .leaf_wise_bucket_sum_calculator import LeafWiseBucketSumCalculator
 
-__all__ = ['BucketSumCalculator']
+__all__ = ['BucketSumCalculator', 'LeafWiseBucketSumCalculator']
```

## secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/bucket_sum_calculator.py

```diff
@@ -17,43 +17,46 @@
 
 from secretflow.data import FedNdarray
 from secretflow.device import PYU, HEUObject, PYUObject
 
 from ....core.pure_numpy_ops.bucket_sum import batch_select_sum, regroup_bucket_sums
 from ....core.pure_numpy_ops.grad import split_GH
 from ..cache.level_wise_cache import LevelWiseCache
-from ..component import Composite, Devices
+from ..component import Composite, Devices, print_params
 from ..gradient_encryptor import GradientEncryptor
+from ..logging import LoggingParams, LoggingTools
 from ..shuffler import Shuffler
 
 
 @dataclass
 class BucketSumCalculatorComponents:
     level_wise_cache: LevelWiseCache = LevelWiseCache()
 
 
 class BucketSumCalculator(Composite):
     def __init__(self):
         self.components = BucketSumCalculatorComponents()
+        self.logging_params = LoggingParams()
 
     def show_params(self):
-        return
+        print_params(self.logging_params)
 
-    def set_params(self, _: dict):
-        return
+    def set_params(self, params: dict):
+        self.logging_params = LoggingTools.logging_params_from_dict(params)
 
-    def get_params(self, _: dict):
-        return
+    def get_params(self, params: dict):
+        LoggingTools.logging_params_write_dict(params, self.logging_params)
 
     def set_devices(self, devices: Devices):
         super().set_devices(devices)
         self.label_holder = devices.label_holder
         self.workers = devices.workers
         self.party_num = len(self.workers)
 
+    @LoggingTools.enable_logging
     def calculate_bucket_sum_level_wise(
         self,
         shuffler: Shuffler,
         encrypted_gh_dict: Dict[PYU, HEUObject],
         children_split_node_selects: List[PYUObject],
         is_lefts: List[bool],
         order_map_sub: FedNdarray,
```

## secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/data_preprocessor.py

```diff
@@ -7,54 +7,24 @@
 #   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import math
 
-from typing import Tuple, Union
+from typing import Tuple
+
+from secretflow.data import FedNdarray
 from secretflow.device import PYUObject
-from secretflow.data import FedNdarray, PartitionWay
-from secretflow.data.vertical import VDataFrame
+from secretflow.ml.boost.core.data_preprocess import validate
 
 from ..component import Component
 
 
-def prepare_dataset(
-    ds: Union[FedNdarray, VDataFrame]
-) -> Tuple[FedNdarray, Tuple[int, int]]:
-    """
-    check data setting and get total shape.
-
-    Args:
-        ds: input dataset
-
-    Return:
-        First: dataset in unified type
-        Second: shape concat all partition.
-    """
-    assert isinstance(
-        ds, (FedNdarray, VDataFrame)
-    ), f"ds should be FedNdarray or VDataFrame, got {type(ds)}"
-
-    ds = ds if isinstance(ds, FedNdarray) else ds.values
-
-    assert ds.partition_way == PartitionWay.VERTICAL, (
-        "Only support vertical dataset, "
-        "for horizontal dataset please use secreflow.ml.boost.homo_boost"
-    )
-
-    shape = ds.shape
-    assert math.prod(shape), f"not support empty dataset, shape {shape}"
-
-    return ds, shape
-
-
 class DataPreprocessor(Component):
     def __init__(self) -> None:
         super().__init__()
 
     def show_params(self):
         return
 
@@ -66,17 +36,8 @@
 
     def set_devices(self, _):
         return
 
     def validate(
         self, dataset, label
     ) -> Tuple[FedNdarray, Tuple[int, int], PYUObject, Tuple[int, int]]:
-        x, x_shape = prepare_dataset(dataset)
-        y, y_shape = prepare_dataset(label)
-        assert len(x_shape) == 2, "only support 2D-array on dtrain"
-        assert len(y_shape) == 1 or y_shape[1] == 1, "label only support one label col"
-        samples = y_shape[0]
-        assert samples == x_shape[0], "dtrain & label are not aligned"
-        assert len(y.partitions) == 1, "label only support one partition"
-        # get y as a PYUObject
-        y = list(y.partitions.values())[0]
-        return x, x_shape, y, y_shape
+        return validate(dataset, label)
```

## secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/gradient_encryptor.py

```diff
@@ -18,14 +18,15 @@
 import numpy as np
 from heu import phe
 
 from secretflow.device import PYU, HEUObject, PYUObject
 from secretflow.device.device.heu import HEUMoveConfig
 
 from ..component import Component, Devices, print_params
+from ..logging import LoggingParams, LoggingTools
 
 
 @dataclass
 class GradientEncryptorParams:
     """
     'fixed_point_parameter': int. Any floating point number encoded by heu,
              will multiply a scale and take the round,
@@ -55,70 +56,77 @@
 
 
 class GradientEncryptor(Component):
     """Manage all encryptions related to y, gradients, hessians"""
 
     def __init__(self):
         self.params = GradientEncryptorParams()
+        self.logging_params = LoggingParams()
         self.gh_encoder = define_encoder(self.params)
 
     def show_params(self):
         print_params(self.params)
+        print_params(self.logging_params)
 
     def set_devices(self, devices: Devices):
         self.label_holder = devices.label_holder
         self.workers = devices.workers
         self.heu = devices.heu
         label_holder_party_name = self.label_holder.party
         assert (
             label_holder_party_name == self.heu.sk_keeper_name()
         ), f"HEU sk keeper party {self.heu.sk_keeper_name()}, mismatch with label_holder device's party {label_holder_party_name}"
 
     def get_params(self, params: dict):
         params['fixed_point_parameter'] = self.params.fixed_point_parameter
         params['batch_encoding_enabled'] = self.params.batch_encoding_enabled
         params['audit_paths'] = self.params.audit_paths
+        LoggingTools.logging_params_write_dict(params, self.logging_params)
 
     def set_params(self, params: dict):
         # validation
         fxp_r = params.get('fixed_point_parameter', 20)
         assert (
-            fxp_r >= 20 and fxp_r <= 100
-        ), f"fixed_point_parameter should in [20, 100], got {fxp_r}"
+            fxp_r >= 10 and fxp_r <= 100
+        ), f"fixed_point_parameter should in [10, 100], got {fxp_r}"
 
         enable_batch_encoding = bool(params.get('batch_encoding_enabled', True))
 
         audit_paths = params.get('audit_paths', {})
+
         assert isinstance(audit_paths, dict), " audit paths must be a dict"
 
         # set params
         self.params.fixed_point_parameter = fxp_r
         self.params.batch_encoding_enabled = enable_batch_encoding
         self.params.audit_paths = audit_paths
 
         # calculate attributes
         self.gh_encoder = define_encoder(self.params)
+        self.logging_params = LoggingTools.logging_params_from_dict(params)
 
     def pack(self, g: PYUObject, h: PYUObject) -> PYUObject:
         return self.label_holder(lambda g, h: np.concatenate([g, h], axis=1))(g, h)
 
+    @LoggingTools.enable_logging
     def encrypt(self, gh: PYUObject, tree_index: int) -> HEUObject:
         if self.label_holder.party in self.params.audit_paths:
             path = (
                 self.params.audit_paths[self.label_holder.party]
                 + ".tree_"
                 + str(tree_index)
             )
         else:
             path = None
 
         return gh.to(self.heu, move_config(self.label_holder, self.gh_encoder)).encrypt(
             path
         )
 
+    @LoggingTools.enable_logging
     def cache_to_workers(
         self, encrypted_gh: HEUObject, gh: PYUObject
     ) -> Dict[PYU, Union[HEUObject, PYUObject]]:
         cache = {
             worker: encrypted_gh.to(self.heu, move_config(worker, self.gh_encoder))
             for worker in self.workers
             if worker != self.label_holder
```

## secretflow/ml/boost/sgb_v/factory/components/loss_computer/loss_computer.py

```diff
@@ -18,14 +18,15 @@
 import numpy as np
 
 from secretflow.device import PYUObject
 
 from ....core.preprocessing.params import RegType
 from ....core.pure_numpy_ops.grad import compute_gh_linear, compute_gh_logistic
 from ..component import Component, Devices, print_params
+from ..logging import LoggingParams, LoggingTools
 
 
 @dataclass
 class LossComputerParams:
     """
     'objective': Specify the learning objective.
         default: 'logistic'
@@ -36,32 +37,39 @@
 
 
 class LossComputer(Component):
     """Compute loss, gradients and hessians"""
 
     def __init__(self) -> None:
         self.params = LossComputerParams()
+        self.logging_params = LoggingParams()
 
     def show_params(self):
         print_params(self.params)
+        print_params(self.logging_params)
 
     def set_params(self, params: dict):
         obj = params.get('objective', 'logistic')
         assert obj in [
             e.value for e in RegType
         ], f"objective should in {[e.value for e in RegType]}, got {obj}"
         obj = RegType(obj)
         self.params.objective = obj
 
+        self.logging_params = LoggingTools.logging_params_from_dict(params)
+
     def get_params(self, params: dict):
         params['objective'] = self.params.objective
 
+        LoggingTools.logging_params_write_dict(params, self.logging_params)
+
     def set_devices(self, devices: Devices):
         self.label_holder = devices.label_holder
 
+    @LoggingTools.enable_logging
     def compute_gh(
         self, y: Union[PYUObject, np.ndarray], pred: Union[PYUObject, np.ndarray]
     ) -> Tuple[PYUObject, PYUObject]:
         obj = self.params.objective
         if obj == RegType.Linear:
             g, h = self.label_holder(compute_gh_linear, num_returns=2)(y, pred)
             return g, h
```

## secretflow/ml/boost/sgb_v/factory/components/node_selector/node_selector.py

```diff
@@ -39,14 +39,49 @@
 
     def root_select(self, sample_num):
         return root_select(samples=sample_num)
 
     def is_list_empty(self, any_list: Union[PYUObject, List]) -> PYUObject:
         return self.label_holder(lambda any_list: len(any_list) == 0)(any_list)
 
+    def get_child_indices(self, node_indices: List[int], is_lefts: List[bool]):
+        """node indices from the same level, in a [l_child, r_child, ...] fasion"""
+
+        def _inner(node_indices, is_lefts):
+            result = []
+            for i, is_left in enumerate(is_lefts):
+                is_left_offset = int(1 - is_left)
+                result.append(node_indices[2 * i + is_left_offset])
+            return result
+
+        return self.label_holder(_inner)(node_indices, is_lefts)
+
+    def get_pruned_indices_and_selects(
+        self,
+        node_indices: List[int],
+        node_selects: List[np.ndarray],
+        gain_is_cost_effective: List[bool],
+    ) -> Tuple[PYUObject, PYUObject]:
+        def _inner(
+            node_indices, node_selects, gain_is_cost_effective
+        ) -> Tuple[List[int], List[np.ndarray]]:
+            pruned_indices = []
+            pruned_node_selects = []
+            for node_index, node_select, gain in zip(
+                node_indices, node_selects, gain_is_cost_effective
+            ):
+                if not gain:
+                    pruned_indices.append(node_index)
+                    pruned_node_selects.append(node_select)
+            return pruned_indices, pruned_node_selects
+
+        return self.label_holder(_inner, num_returns=2)(
+            node_indices, node_selects, gain_is_cost_effective
+        )
+
     def pick_children_node_ss(
         self, node_select_list: PYUObject
     ) -> Tuple[List[PYUObject], List[bool], int]:
         return self.label_holder(pick_children_node_ss, num_returns=3)(node_select_list)
 
     def get_child_select(
         self,
```

## secretflow/ml/boost/sgb_v/factory/components/order_map_manager/order_map_manager.py

```diff
@@ -16,14 +16,15 @@
 from dataclasses import dataclass
 from typing import Dict, List, Union
 
 from secretflow.data import FedNdarray, PartitionWay
 from secretflow.device import PYUObject
 
 from ..component import Component, Devices, print_params
+from ..logging import LoggingParams, LoggingTools
 from .order_map_actor import OrderMapActor
 
 
 @dataclass
 class OrderMapBuilderParams:
     """
     'sketch_eps': This roughly translates into O(1 / sketch_eps) number of bins.
@@ -37,52 +38,60 @@
     sketch_eps: float = 0.1
     seed: int = 1212
 
 
 class OrderMapManager(Component):
     def __init__(self) -> None:
         self.params = OrderMapBuilderParams()
+        self.logging_params = LoggingParams()
         self.buckets = eps_inverse(self.params.sketch_eps)
         self.order_map_actors = []
 
     def show_params(self):
         print_params(self.params)
+        print_params(self.logging_params)
 
     def set_params(self, params: Dict):
         # validate
         sketch = params.get('sketch_eps', 0.1)
         assert (
             sketch > 0 and sketch <= 1
         ), f"sketch_eps should in (0, 1], got {sketch}"  # set
         self.params.sketch_eps = sketch
         # derive attributes
         self.buckets = eps_inverse(sketch)
         self.params.seed = int(params.get('seed', 1212))
 
+        self.logging_params = LoggingTools.logging_params_from_dict(params)
+
     def get_params(self, params: dict):
         params['sketch_eps'] = self.params.sketch_eps
         params['seed'] = self.params.seed
 
+        LoggingTools.logging_params_write_dict(params, self.logging_params)
+
     def set_devices(self, devices: Devices):
         self.order_map_actors = [
             OrderMapActor(idx, device=pyu) for idx, pyu in enumerate(devices.workers)
         ]
 
-    def build_order_map(self, x: FedNdarray):
+    @LoggingTools.enable_logging
+    def build_order_map(self, x: FedNdarray) -> FedNdarray:
         # we assumed x's devices match when setting up devices.
         buckets, seed = self.buckets, self.params.seed
         self.order_map = FedNdarray(
             {
                 order_map_actor.device: order_map_actor.build_order_map(
                     x.partitions[order_map_actor.device].data, buckets, seed
                 )
                 for order_map_actor in self.order_map_actors
             },
             partition_way=PartitionWay.VERTICAL,
         )
+        return self.order_map
 
     def get_order_map(self) -> FedNdarray:
         return self.order_map
 
     def get_feature_buckets(self) -> List[PYUObject]:
         return [
             order_map_actor.get_feature_buckets()
```

## secretflow/ml/boost/sgb_v/factory/components/sampler/sampler.py

```diff
@@ -23,27 +23,31 @@
 
 from ..component import Component, Devices, print_params
 
 
 @dataclass
 class SamplerParams:
     """
-    'row_sample_rate': Row sub sample ratio of the training instances.
+    'row_sample_rate': float. Row sub sample ratio of the training instances.
         default: 1
         range: (0, 1]
-    'col_sample_rate': Col sub sample ratio of columns when constructing each tree.
+    'col_sample_rate': float. Col sub sample ratio of columns when constructing each tree.
         default: 1
         range: (0, 1]
-    'seed': Pseudorandom number generator seed.
+    'seed': int. Pseudorandom number generator seed.
         default: 1212
+    'label_holder_feature_only': bool. affects col sampling.
+        default: False
+        if turned on, all non-label holder's col sample rate will be 0.
     """
 
     row_sample_rate: float = 1
     col_sample_rate: float = 1
     seed: int = 1212
+    label_holder_feature_only: bool = False
 
 
 class Sampler(Component):
     def __init__(self):
         self.params = SamplerParams()
 
     def show_params(self):
@@ -59,45 +63,64 @@
         assert (
             colsample > 0 and colsample <= 1
         ), f"col_sample_rate should in (0, 1], got {colsample}"
 
         self.params.row_sample_rate = subsample
         self.params.col_sample_rate = colsample
         self.params.seed = int(params.get('seed', 1212))
+        self.params.label_holder_feature_only = bool(
+            params.get('label_holder_feature_only', False)
+        )
 
         self.rng = np.random.default_rng(self.params.seed)
 
     def get_params(self, params: dict):
         params['seed'] = self.params.seed
         params['row_sample_rate'] = self.params.row_sample_rate
         params['col_sample_rate'] = self.params.col_sample_rate
+        params['label_holder_feature_only'] = self.params.label_holder_feature_only
 
-    def set_devices(self, _: Devices):
-        return
+    def set_devices(self, devices: Devices):
+        self.label_holder = devices.label_holder
 
     def generate_col_choices(
         self, feature_buckets: List[PYUObject]
     ) -> Tuple[List[PYUObject], List[PYUObject]]:
         """Generate column sample choices.
 
         Args:
             feature_buckets (List[PYUObject]): Behind PYUObject is List[int], bucket num for each feature.
 
         Returns:
             Tuple[List[PYUObject], List[PYUObject]]: first list is column choices, second is total number of buckets after sampling
         """
         colsample = self.params.col_sample_rate
-        col_choices, total_buckets = zip(
-            *[
-                fb.device(generate_one_partition_col_choices, num_returns=2)(
-                    colsample, fb
-                )
-                for fb in feature_buckets
-            ]
-        )
+
+        if self.params.label_holder_feature_only:
+            col_choices, total_buckets = zip(
+                *[
+                    fb.device(generate_one_partition_col_choices, num_returns=2)(
+                        colsample, fb
+                    )
+                    if fb.device == self.label_holder
+                    else fb.device(generate_one_partition_col_choices, num_returns=2)(
+                        0, fb
+                    )
+                    for fb in feature_buckets
+                ]
+            )
+        else:
+            col_choices, total_buckets = zip(
+                *[
+                    fb.device(generate_one_partition_col_choices, num_returns=2)(
+                        colsample, fb
+                    )
+                    for fb in feature_buckets
+                ]
+            )
         return col_choices, total_buckets
 
     def generate_row_choices(self, row_num) -> Union[None, np.ndarray]:
         if self.params.row_sample_rate == 1:
             return None
         sample_num_in_tree = math.ceil(row_num * self.params.row_sample_rate)
```

## secretflow/ml/boost/sgb_v/factory/components/shuffler/shuffler.py

```diff
@@ -8,21 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import List
-
 from dataclasses import dataclass
+from typing import List, Union
+
 from secretflow.device import PYUObject
 
-from .worker_shuffler import WorkerShuffler
 from ..component import Component, Devices, print_params
+from .worker_shuffler import WorkerShuffler
 
 
 @dataclass
 class ShufflerParams:
     """
     'seed': Pseudorandom number generator seed.
         default: 1212
@@ -74,7 +74,33 @@
         """
         return [
             worker_shuffler.undo_shuffle_mask_list_wise(split_buckets)
             for worker_shuffler, split_buckets in zip(
                 self.worker_shufflers, split_buckets_parition_wise
             )
         ]
+
+    def unshuffle_split_buckets_with_keys(
+        self,
+        split_buckets_parition_wise: List[PYUObject],
+        keys: Union[PYUObject, List[PYUObject]],
+    ) -> List[PYUObject]:
+        """unshuffle split buckets viewed by each parition
+
+        Args:
+            split_buckets_parition_wise (List[PYUObject]): PYUObject is List[int], split buckets viewed from this partition
+            keys (Union[PYUObject, List[PYUObject]]): Both cases are in fact List[int]. keys will be sent to all workers
+
+        Returns:
+            List[List[PYUObject]]: unshuffled split buckets
+        """
+        return [
+            worker_shuffler.undo_shuffle_mask_with_keys(
+                split_buckets,
+                keys.to(worker_shuffler.device)
+                if isinstance(keys, PYUObject)
+                else [k.to(worker_shuffler.device) for k in keys],
+            )
+            for worker_shuffler, split_buckets in zip(
+                self.worker_shufflers, split_buckets_parition_wise
+            )
+        ]
```

## secretflow/ml/boost/sgb_v/factory/components/shuffler/worker_shuffler.py

```diff
@@ -10,31 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 
+import numpy as np
 
 from secretflow.device import PYUObject, proxy
 
 from ....core.split_tree_trainer.shuffler import Shuffler
 
-import numpy as np
-
 
 @proxy(PYUObject)
 class WorkerShuffler:
     def __init__(self, seed: int):
         np.random.seed(seed)
         self.shuffler = Shuffler()
 
     def reset_shuffle_mask(self):
         self.shuffler.reset_shuffle_mask()
 
+    def reset_shuffle_mask_with_keys(self, keys: List[int]):
+        self.shuffler.reset_shuffle_mask_with_keys(keys)
+
     def create_shuffle_mask(self, key: int, bucket_list: List[PYUObject]) -> List[int]:
         self.shuffler.create_shuffle_mask(key, bucket_list)
         return self.shuffler.get_shuffling_indices(key)
 
     def is_shuffled(self) -> bool:
         return self.shuffler.is_shuffled()
 
@@ -48,7 +50,13 @@
             return index
 
     def undo_shuffle_mask_list_wise(self, split_buckets: List[int]) -> List[int]:
         return [
             self.undo_shuffle_mask(key, index)
             for key, index in enumerate(split_buckets)
         ]
+
+    def undo_shuffle_mask_with_keys(self, split_buckets: List[int], keys) -> List[int]:
+        return [
+            self.undo_shuffle_mask(key, index)
+            for key, index in zip(keys, split_buckets)
+        ]
```

## secretflow/ml/boost/sgb_v/factory/components/split_finder/split_finder.py

```diff
@@ -14,15 +14,15 @@
 
 import pickle
 from dataclasses import dataclass, field
 from typing import Tuple
 
 import numpy as np
 
-from ....core.pure_numpy_ops.boost import find_best_splits
+from ....core.pure_numpy_ops.boost import find_best_splits, find_best_splits_with_gains
 from ..component import Component, Devices, print_params
 
 
 @dataclass
 class SplitFinderParams:
     """
     'gamma': float. Greater than 0 means pre-pruning enabled.
@@ -68,15 +68,38 @@
         params['gamma'] = self.params.gamma
         params['reg_lambda'] = self.params.reg_lambda
         params['audit_path'] = self.params.audit_paths
 
     def set_devices(self, devices: Devices):
         self.label_holder = devices.label_holder
 
-    def find_best_splits(
+    def find_best_splits_with_gains(
+        self, G: np.ndarray, H: np.ndarray, tree_num: int, leaf: int
+    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        reg_lambda = self.params.reg_lambda
+        gamma = self.params.gamma
+        split_buckets, split_gains, should_split = self.label_holder(
+            find_best_splits_with_gains, num_returns=3
+        )(G, H, reg_lambda, gamma)
+
+        if self.label_holder.party in self.params.audit_paths:
+            # may change log later
+            split_info_path = (
+                self.params.audit_paths[self.label_holder.party]
+                + ".split_buckets.tree_"
+                + str(tree_num)
+                + ".leaf_"
+                + str(leaf)
+                + ".pickle"
+            )
+            # split info when considering the nth leaf
+            self.label_holder(write_log)(split_buckets, split_info_path)
+        return split_buckets, split_gains, should_split
+
+    def find_best_splits_level_wise(
         self, G: np.ndarray, H: np.ndarray, tree_num: int, level: int
     ) -> Tuple[np.ndarray, np.ndarray]:
         reg_lambda = self.params.reg_lambda
         gamma = self.params.gamma
         split_buckets, should_split = self.label_holder(
             find_best_splits, num_returns=2
         )(G, H, reg_lambda, gamma)
```

## secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_builder.py

```diff
@@ -59,25 +59,32 @@
             actor.set_col_choices(col_choice)
             actor.set_feature_bucket(feature_bucket)
             # total number buckets is broadcasted
             actor.set_buckets_count(
                 [buckets_count.to(actor.device) for buckets_count in total_buckets]
             )
 
-    def split_bucket_to_partition(self, split_buckets: PYUObject) -> List[PYUObject]:
+    def split_bucket_to_partition(
+        self, split_buckets: Union[PYUObject, List[PYUObject]]
+    ) -> List[PYUObject]:
         """map split bucket to position in the partition or -1 if not in partition
 
         Args:
-            split_buckets (PYUObject): PYUObject is in fact a List[int].
+            split_buckets (Union[PYUObject, List[PYUObject]]): Either is a PYUObject or List[PYUObject],
+                but in both cases it's in fact List[int].
 
         Returns:
             List[PYUObject]: each PYUObject is in fact a List[int]. split buckets viewed by each party
         """
         return [
-            actor.split_buckets_to_paritition(split_buckets.to(actor.device))
+            actor.split_buckets_to_paritition(
+                split_buckets.to(actor.device)
+                if isinstance(split_buckets, PYUObject)
+                else [sb.to(actor.device) for sb in split_buckets]
+            )
             for actor in self.split_tree_builder_actors
         ]
 
     def get_split_feature_list_wise_each_party(
         self, un_shuffled_split_buckets_each_party: List[PYUObject]
     ) -> List[PYUObject]:
         """map the unmasked split buckets to feature and split point
@@ -117,15 +124,18 @@
             left_child_selects: left child selects for the new split nodes.
         """
         lchild_selects = []
         for i, _ in enumerate(self.workers):
             split_node_indices_here = (
                 node_indices.to(self.workers[i])
                 if isinstance(node_indices, PYUObject)
-                else node_indices
+                else [
+                    node.to(self.workers[i]) if isinstance(node, PYUObject) else node
+                    for node in node_indices
+                ]
             )
             # split buckets is sent from label holder to workers
             selects = self.split_tree_builder_actors[i].do_split_list_wise(
                 split_features[i],
                 split_points[i],
                 left_child_selects[i],
                 gain_is_cost_effective,
```

## secretflow/ml/boost/sgb_v/factory/components/tree_trainer/__init__.py

```diff
@@ -1,4 +1,5 @@
-from .tree_trainer import TreeTrainer
+from .leaf_wise_tree_trainer import LeafWiseTreeTrainer
 from .level_wise_tree_trainer import LevelWiseTreeTrainer
+from .tree_trainer import TreeTrainer
 
-__all__ = ['TreeTrainer', 'LevelWiseTreeTrainer']
+__all__ = ['TreeTrainer', 'LevelWiseTreeTrainer', 'LeafWiseTreeTrainer']
```

## secretflow/ml/boost/sgb_v/factory/components/tree_trainer/level_wise_tree_trainer.py

```diff
@@ -17,17 +17,18 @@
 
 import numpy as np
 
 from secretflow.device import PYUObject, reveal
 
 from ....core.distributed_tree.distributed_tree import DistributedTree
 from ..bucket_sum_calculator import BucketSumCalculator
-from ..component import Devices
+from ..component import Devices, print_params
 from ..gradient_encryptor import GradientEncryptor
 from ..leaf_manager import LeafManager
+from ..logging import LoggingParams, LoggingTools
 from ..loss_computer import LossComputer
 from ..node_selector import NodeSelector
 from ..order_map_manager import OrderMapManager
 from ..sampler import Sampler
 from ..shuffler import Shuffler
 from ..split_finder import SplitFinder
 from ..split_tree_builder import SplitTreeBuilder
@@ -59,17 +60,20 @@
     max_depth: int = 5
 
 
 class LevelWiseTreeTrainer(TreeTrainer):
     def __init__(self) -> None:
         self.components = LevelWiseTreeTrainerComponents()
         self.params = LevelWiseTreeTrainerParams()
+        self.logging_params = LoggingParams()
 
     def show_params(self):
         super().show_params()
+        print_params(self.params)
+        print_params(self.logging_params)
 
     def set_params(self, params: dict):
         super().set_params(params)
         self._set_trainer_params(params)
 
     def get_params(self, params: dict):
         super().get_params(params)
@@ -79,21 +83,24 @@
         super().set_devices(devices)
         self.workers = devices.workers
         self.label_holder = devices.label_holder
         self.party_num = len(self.workers)
 
     def _get_trainer_params(self, params: dict):
         params['max_depth'] = self.params.max_depth
+        LoggingTools.logging_params_write_dict(params, self.logging_params)
 
     def _set_trainer_params(self, params: dict):
         depth = int(params.pop('max_depth', 5))
         assert depth > 0 and depth <= 16, f"max_depth should in [1, 16], got {depth}"
 
         self.params.max_depth = depth
+        self.logging_params = LoggingTools.logging_params_from_dict(params)
 
+    @LoggingTools.enable_logging
     def train_tree(
         self,
         cur_tree_num,
         order_map_manager: OrderMapManager,
         y: PYUObject,
         pred: Union[PYUObject, np.ndarray],
         x_shape: Tuple[int, int],
@@ -156,14 +163,15 @@
         tree = DistributedTree()
         self.components.split_tree_builder.insert_split_trees_into_distributed_tree(
             tree, leaf_node_indices
         )
         tree.set_leaf_weight(self.label_holder, weight)
         return tree
 
+    @LoggingTools.enable_logging
     def _train_level(
         self,
         split_node_selects: PYUObject,
         split_node_indices: Union[List[int], PYUObject],
         level: int,
         tree_num: int,
         order_map_manager: OrderMapManager,
@@ -264,15 +272,15 @@
             self.components.gradient_encryptor,
             node_num,
         )
 
         (
             split_buckets,
             gain_is_cost_effective,
-        ) = self.components.split_finder.find_best_splits(
+        ) = self.components.split_finder.find_best_splits_level_wise(
             level_nodes_G, level_nodes_H, tree_num, level
         )
         # all parties including driver know the shape of tree in each node
         # hence all parties including driver will know the pruning results.
         # hence we can reveal gain_is_cost_effective
         gain_is_cost_effective = reveal(gain_is_cost_effective)
         self.components.bucket_sum_calculator.update_level_cache(
```

## secretflow/ml/boost/sgb_v/factory/components/tree_trainer/tree_trainer.py

```diff
@@ -8,18 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from ....core.distributed_tree.distributed_tree import DistributedTree
-
 import abc
 
+from ....core.distributed_tree.distributed_tree import DistributedTree
 from ..component import Composite, Devices
 
 
 class TreeTrainer(Composite):
     def show_params(self):
         super().show_params()
```

## secretflow/ml/boost/ss_xgb_v/model.py

```diff
@@ -31,31 +31,30 @@
     SPUObject,
     wait,
 )
 
 from .core import node_split as split_fn
 from .core.node_split import RegType
 from .core.tree_worker import XgbTreeWorker as Worker
-from .core.utils import prepare_dataset
+from secretflow.ml.boost.core.data_preprocess import prepare_dataset, validate
 
 
 class XgbModel:
-    '''
+    """
     SS Xgb Model & predict.
-    '''
+    """
 
     def __init__(self, spu: SPU, objective: RegType, base: float) -> None:
         self.spu = spu
         self.objective = objective
         self.base = base
         # List[Dict[PYU, PYUObject of XgbTree]], owned by pyu, only knows split value if feature belong to this pyu.
         self.trees = list()
         # List[SPUObject of np.array], owned by spu and not reveal to any one
         self.weights = list()
-        # TODO how to ser/der ?
 
     def _tree_pred(self, tree: Dict[PYU, PYUObject], weight: SPUObject) -> SPUObject:
         assert len(tree) == len(self.x)
 
         weight_selects = list()
         for worker in self.workers:
             device = worker.device
@@ -68,33 +67,35 @@
         return pred
 
     def predict(
         self,
         dtrain: Union[FedNdarray, VDataFrame],
         to_pyu: PYU = None,
     ) -> Union[SPUObject, FedNdarray]:
-        '''
+        """
         predict on dtrain with this model.
 
         Args:
 
             dtrain : [FedNdarray, VDataFrame]
                 vertical split dataset.
 
             to: the prediction initiator
                 if not None predict result is reveal to to_pyu device and save as FedNdarray
                 otherwise, keep predict result in secret and save as SPUObject.
 
         Return:
             Pred values store in spu object or FedNdarray.
-        '''
+        """
         if len(self.trees) == 0:
             return None
         x, _ = prepare_dataset(dtrain)
-        assert len(x.partitions) == len(self.trees[0])
+        assert len(x.partitions) == len(
+            self.trees[0]
+        ), f"{len(x.partitions)}, {self.trees[0]}"
         self.workers = [Worker(0, device=pyu) for pyu in x.partitions]
         self.x = x.partitions
         preds = []
         for idx in range(len(self.trees)):
             pred = self._tree_pred(self.trees[idx], self.weights[idx])
             wait([pred])
             preds.append(pred)
@@ -117,25 +118,25 @@
                 partition_way=PartitionWay.VERTICAL,
             )
         else:
             return pred
 
 
 class Xgb:
-    '''
+    """
     This method provides both classification and regression tree boosting (also known as GBDT, GBM)
     for vertical split dataset setting by using secret sharing.
 
     SS-XGB is short for secret sharing XGB.
     more details: https://arxiv.org/pdf/2005.08479.pdf
 
     Args:
         spu: secret device running MPC protocols
 
-    '''
+    """
 
     def __init__(self, spu: Union[SPU, List[SPU]]) -> None:
         if not isinstance(spu, list):
             spu = [spu]
         self.spu = spu
 
     def _update_pred(self, tree: Dict[PYU, PYUObject], weight: SPUObject) -> None:
@@ -149,15 +150,15 @@
             weight_selects.append(s.to(self.spu[0]))
 
         current = self.spu[0](split_fn.predict_tree_weight)(weight_selects, weight)
         pred = self.spu[0](
             split_fn.update_train_pred,
             num_returns_policy=SPUCompilerNumReturnsPolicy.FROM_USER,
             user_specified_num_returns=self.fragment_count,
-            static_argnames=('fragments'),
+            static_argnames=("fragments"),
         )(self.pred, current, fragments=self.fragment_count)
 
         self.pred = pred if isinstance(pred, list) else [pred]
 
         for f_idx in range(self.fragment_count):
             spu_idx = f_idx % self.spus
             spu = self.spu[spu_idx]
@@ -168,83 +169,75 @@
         params: Dict,
         dataset: Union[FedNdarray, VDataFrame],
         label: Union[FedNdarray, VDataFrame],
     ) -> None:
         start = time.time()
         assert len(self.spu) > 0, "need at least one spu device"
         self.spus = len(self.spu)
-        x, x_shape = prepare_dataset(dataset)
-        y, y_shape = prepare_dataset(label)
-        assert len(x_shape) == 2, "only support 2D-array on dtrain"
-        assert len(y_shape) == 1 or y_shape[1] == 1, "label only support one col"
-        self.samples = y_shape[0]
-
-        assert self.samples == x_shape[0], "dtrain & label are not aligned"
-        assert len(y.partitions) == 1, "label only support one partition"
+        x, x_shape, y, y_shape = validate(dataset, label)
 
+        self.samples = y_shape[0]
         self.x = x.partitions
 
-        self.trees = int(params.pop('num_boost_round', 10))
+        self.trees = int(params.pop("num_boost_round", 10))
         assert (
             1 <= self.trees <= 1024
         ), f"num_boost_round should in [1, 1024], got {self.trees}"
 
-        self.depth = int(params.pop('max_depth', 5))
+        self.depth = int(params.pop("max_depth", 5))
         assert (
             self.depth > 0 and self.depth <= 16
         ), f"max_depth should in [1, 16], got {self.depth}"
 
-        self.lr = float(params.pop('learning_rate', 0.3))
+        self.lr = float(params.pop("learning_rate", 0.3))
         assert (
             self.lr > 0 and self.lr <= 1
         ), f"learning_rate should in (0, 1], got {self.lr}"
 
-        obj = params.pop('objective', 'logistic')
+        obj = params.pop("objective", "logistic")
         assert obj in [
             e.value for e in RegType
         ], f"objective should in {[e.value for e in RegType]}, got {obj}"
         self.obj = RegType(obj)
 
-        self.reg_lambda = float(params.pop('reg_lambda', 0.1))
+        self.reg_lambda = float(params.pop("reg_lambda", 0.1))
         assert (
             self.reg_lambda >= 0 and self.reg_lambda <= 10000
         ), f"reg_lambda should in [0, 10000], got {self.reg_lambda}"
 
-        self.subsample = float(params.pop('subsample', 1))
+        self.subsample = float(params.pop("subsample", 1))
         assert (
             self.subsample > 0 and self.subsample <= 1
         ), f"subsample should in (0, 1], got {self.subsample}"
 
-        self.colsample = float(params.pop('colsample_bytree', 1))
+        self.colsample = float(params.pop("colsample_by_tree", 1))
         assert (
             self.colsample > 0 and self.colsample <= 1
-        ), f"colsample_bytree should in (0, 1], got {self.colsample}"
+        ), f"colsample_by_tree should in (0, 1], got {self.colsample}"
 
-        self.base = float(params.pop('base_score', 0))
+        self.base = float(params.pop("base_score", 0))
 
-        sketch = params.pop('sketch_eps', 0.1)
+        sketch = params.pop("sketch_eps", 0.1)
         assert sketch > 0 and sketch <= 1, f"sketch_eps should in (0, 1], got {sketch}"
         self.buckets = math.ceil(1.0 / sketch)
-        self.seed = int(params.pop('seed', 42))
+        self.seed = int(params.pop("seed", 42))
 
         assert len(params) == 0, f"Unknown params {list(params.keys())}"
 
         all_features = x_shape[1]
         # split buckets_map into [256, 512]MB fragments. (for FM64 ABY3 or FM128 SEMI2K)
         rows_limit = 256 * (1024**2) / all_features / self.buckets / 16
         fragment_count = math.ceil(self.samples / rows_limit)
         fragment_count = math.ceil(fragment_count / self.spus) * self.spus
 
         self.workers = [Worker(idx, device=pyu) for idx, pyu in enumerate(x.partitions)]
         self.fragment_count = fragment_count
 
         logging.info(f"fragment_count {fragment_count}")
 
-        y = list(y.partitions.values())[0]
-
         if fragment_count == 1:
             y = y.device(lambda y: y.reshape((1, y.shape[0])))(y)
             y = [y]
         else:
             y = y.device(
                 lambda y: np.array_split(
                     y.reshape((1, y.shape[0])), fragment_count, axis=1
@@ -296,15 +289,15 @@
 
         start = time.time()
         self.pred = []
         for f_idx in range(self.fragment_count):
             f_samples = self.frag_samples[f_idx]
             spu_idx = f_idx % self.spus
             pred = self.spu[spu_idx](
-                split_fn.init_pred, static_argnames=('base', 'samples')
+                split_fn.init_pred, static_argnames=("base", "samples")
             )(base=self.base, samples=f_samples)
             self.pred.append(pred)
             if spu_idx == self.spus - 1:
                 wait(self.pred[-self.spus :])
         logging.info(f"init_pred time {time.time() - start}s")
 
     def _tree_setup(self) -> None:
@@ -322,15 +315,15 @@
             )
 
         assert len(self.y) == len(self.pred)
 
         if self.colsample < 1:
             self.col_choices = []
             for spu in self.spu:
-                choices = [c.to(spu, spu_vis='public') for c in col_buckets_choices]
+                choices = [c.to(spu, spu_vis="public") for c in col_buckets_choices]
                 spu_choices = spu(lambda c: jnp.concatenate(c, axis=None))(choices)
                 self.col_choices.append(spu_choices)
         else:
             self.col_choices = [None] * self.spus
 
         self.sub_choices = list()
         self.ghs = list()
@@ -345,19 +338,22 @@
             assert choices > 0, f"subsample {self.subsample} is too small"
 
             if choices < samples:
                 sub_choices = self.workers[0].device(
                     lambda s, c: np.sort(np.random.choice(s, c, replace=False))
                 )(samples, choices)
                 # same as colsample above, keep choices in public.
-                sub_choices = sub_choices.to(spu, spu_vis='public')
+                sub_choices = sub_choices.to(spu, spu_vis="public")
             else:
                 sub_choices = None
 
-            gh = spu(split_fn.tree_setup, static_argnames=("objective"),)(
+            gh = spu(
+                split_fn.tree_setup,
+                static_argnames=("objective"),
+            )(
                 pred,
                 y,
                 sub_choices,
                 objective=self.obj,
             )
 
             self.sub_choices.append(sub_choices)
@@ -368,15 +364,15 @@
 
     def train(
         self,
         params: Dict,
         dtrain: Union[FedNdarray, VDataFrame],
         label: Union[FedNdarray, VDataFrame],
     ) -> XgbModel:
-        '''train on dtrain and label.
+        """train on dtrain and label.
 
         Args:
             dtrain: {FedNdarray, VDataFrame}
                 vertical split dataset.
             label: {FedNdarray, VDataFrame}
                 label column.
             params: Dict
@@ -398,28 +394,28 @@
                 range: ['linear', 'logistic']
             'reg_lambda': L2 regularization term on weights.
                 default: 0.1
                 range: [0, 10000]
             'subsample': Subsample ratio of the training instances.
                 default: 1
                 range: (0, 1]
-            'colsample_bytree': Subsample ratio of columns when constructing each tree.
+            'colsample_by_tree': Subsample ratio of columns when constructing each tree.
                 default: 1
                 range: (0, 1]
             'sketch_eps': This roughly translates into O(1 / sketch_eps) number of bins.
                 default: 0.1
                 range: (0, 1]
             'base_score': The initial prediction score of all instances, global bias.
                 default: 0
             'seed': Pseudorandom number generator seed.
                 default: 42
 
         Return:
             XgbModel
-        '''
+        """
         self._prepare(params, dtrain, label)
         self._global_setup()
 
         model = XgbModel(self.spu[0], self.obj, self.base)
         while len(model.trees) < self.trees:
             start = time.time()
 
@@ -481,29 +477,29 @@
         self.cache = n_cache
 
         # merge GH to spu 0
         level_GHs = [GH.to(self.spu[0]) for GH in level_GHs]
 
         spu_split_buckets = self.spu[0](
             split_fn.find_best_split_bucket,
-            static_argnames='reg_lambda',
+            static_argnames="reg_lambda",
         )(level_GHs, reg_lambda=self.reg_lambda)
 
         lchild_ss = []
         for worker in self.workers:
             # In the final tree model, which party hold the split feature for tree nodes is public information.
             # so, we can reveal 'split_buckets' to each pyu.
             lchild_s = worker.do_split(spu_split_buckets.to(worker.device))
             lchild_ss.append(lchild_s.to(self.spu[0]))
 
         childs_s = self.spu[0](
             split_fn.get_child_select,
             num_returns_policy=SPUCompilerNumReturnsPolicy.FROM_USER,
             user_specified_num_returns=self.fragment_count,
-            static_argnames=('fragments'),
+            static_argnames=("fragments"),
         )(nodes_s, lchild_ss, fragments=self.fragment_count)
 
         childs_s = childs_s if isinstance(childs_s, list) else [childs_s]
 
         for f_idx in range(self.fragment_count):
             spu_idx = f_idx % self.spus
             spu = self.spu[spu_idx]
@@ -515,15 +511,15 @@
 
     def _init_root(self) -> List[SPUObject]:
         root_s = []
         for f_idx in range(self.fragment_count):
             spu_idx = f_idx % self.spus
             spu = self.spu[spu_idx]
             samples = self.frag_samples[f_idx]
-            s = spu(split_fn.root_select, static_argnames=('samples'))(samples=samples)
+            s = spu(split_fn.root_select, static_argnames=("samples"))(samples=samples)
             root_s.append(s)
         return root_s
 
     def _train_tree(self) -> Tuple[Dict[PYU, PYUObject], SPUObject]:
         nodes_s = self._init_root()
         self.cache = None
         for level in range(self.depth + 1):
```

## secretflow/ml/boost/ss_xgb_v/core/tree_worker.py

```diff
@@ -15,14 +15,15 @@
 import math
 from typing import List, Tuple
 
 import numpy as np
 from heu import numpy as hnp
 
 from secretflow.device import PYUObject, proxy
+from secretflow.ml.boost.core.order_map_tools import qcut
 
 from .xgb_tree import XgbTree
 
 
 @proxy(PYUObject)
 class XgbTreeWorker:
     '''
@@ -44,80 +45,15 @@
         Return:
             leaf nodes' selects
         '''
         x = x if isinstance(x, np.ndarray) else np.array(x)
         return hnp.tree_predict(x, tree.split_features, tree.split_values)
 
     def _qcut(self, x: np.ndarray) -> Tuple[np.ndarray, List]:
-        sorted_x = np.sort(x, axis=0)
-        samples = len(sorted_x)
-        remained_count = samples
-        assert remained_count > 0, 'can not qcut empty x'
-
-        value_category = list()
-        last_value = None
-
-        split_points = list()
-        idx = 0
-        expected_idx = math.ceil(remained_count / self.buckets)
-        fast_skip = False
-        while idx < samples:
-            v = sorted_x[idx]
-            value_diff = v != last_value
-            if not fast_skip and value_diff:
-                if len(value_category) <= self.buckets:
-                    value_category.append(v)
-                else:
-                    fast_skip = True
-                last_value = v
-
-            if idx >= expected_idx and value_diff:
-                split_points.append(v)
-                if len(split_points) == self.buckets - 1:
-                    break
-                remained_count = samples - idx
-                expected_bin_count = math.ceil(
-                    remained_count / (self.buckets - len(split_points))
-                )
-                expected_idx = idx + expected_bin_count
-                last_value = v
-
-            if not fast_skip or idx >= expected_idx:
-                idx += 1
-            else:
-                idx = expected_idx
-
-        if len(value_category) <= self.buckets:
-            # full dataset category count <= buckets
-            # use category as split point.
-            split_points = value_category[1:]
-        elif split_points[-1] != sorted_x[-1]:
-            # add max sample value into split_points like xgboost.
-            split_points.append(sorted_x[-1])
-
-        split_points = list(map(float, split_points))
-
-        def upper_bound_bin(x: float):
-            count = len(split_points)
-            pos = 0
-            while count > 0:
-                step = math.floor(count / 2)
-                v = split_points[pos + step]
-                if x == v:
-                    return pos + step + 1
-                elif x > v:
-                    pos = pos + step + 1
-                    count -= step + 1
-                else:
-                    count = step
-            return pos
-
-        bins = np.vectorize(upper_bound_bin)(x)
-
-        return bins, split_points
+        return qcut(x, self.buckets)
 
     def _build_maps(self, x: np.ndarray):
         '''
         split features into buckets and build maps use in train.
         '''
         # order_map: record sample belong to which bucket of all features.
         self.order_map = np.zeros((x.shape[0], x.shape[1]), dtype=np.int8, order='F')
```

## secretflow/ml/linear/fl_lr_mix.py

```diff
@@ -123,22 +123,25 @@
         batch_size: int,
     ):
         for ver_lr, x_part, y_part in zip(self.ver_lr_list, x.partitions, y.partitions):
             ver_lr.init_train_data(
                 x=x_part.values, y=y_part.values, epochs=epochs, batch_size=batch_size
             )
 
-    def _agg_weights(self):
+    def _agg_weights(self, aggr_hooks: List):
         weights_list = [
             list(ver_lr.get_weight().values()) for ver_lr in self.ver_lr_list
         ]
         agg_weight = [
             self.aggregators[i].average(weights, axis=0)
             for i, weights in enumerate(zip(*weights_list))
         ]
+
+        for hook in aggr_hooks:
+            agg_weight = hook.on_aggregate(agg_weight)
         for ver_lr in self.ver_lr_list:
             ver_lr.set_weight(dict(zip(ver_lr.workers.keys(), agg_weight)))
 
     def _compute_loss(
         self,
         x: MixDataFrame,
         y: MixDataFrame,
@@ -170,14 +173,15 @@
         aggregators: List[Aggregator],
         heus: List[HEU],
         fxp_bits: Optional[int] = spu_fxp_precision(spu.spu_pb2.FM64),
         tol: Optional[float] = 1e-4,
         learning_rate: Optional[float] = 0.1,
         agg_epochs: Optional[int] = 1,
         audit_log_dir: Dict[PYU, str] = None,
+        aggr_hooks: List = None,
     ):
         """Fit the model.
 
         Args:
             x: training vector. X should be a horizontal partitioned
                 :py:class:`~secretflow.data.mix.MixDataFrame`, which consists
                 of :py:class:`~secretflow.data.vertical.VDataFrame`s.
@@ -196,14 +200,15 @@
             learning_rate: optional, learning rate. Defaults to 0.1.
             agg_epochs: aggregate weights for every {agg_epochs} epochs.
                 Defaults to 1.
             audit_log_dir: a dict specifying the audit log directory for each
                 device. No audit log if is None. Default to None.
                 Please leave it None unless you are very sure what the audit
                 does and accept the risk.
+            aggr_hooks: The hooks called on each aggregation
         """
         assert isinstance(
             x, MixDataFrame
         ), f'X should be a MixDataFrame but got {type(x)}.'
         assert (
             x.partition_way == PartitionWay.HORIZONTAL
         ), 'X should be horizontal partitioned.'
@@ -222,14 +227,16 @@
             ), 'One and only one party should have y.'
         assert len(aggregators) == len(
             x.partitions
         ), 'Amount of aggregators should be same as `VDataFrame`s of X.'
         assert len(heus) == len(
             x.partitions
         ), 'Amount of heus should be same as `VDataFrame`s of X.'
+        aggr_hooks = aggr_hooks or []  # change None -> []
+        aggr_hooks = aggr_hooks if isinstance(aggr_hooks, List) else [aggr_hooks]
 
         devices_list = [list(part.partitions.keys()) for part in x.partitions]
         self.aggregators = []
         for ver_devices in zip(*devices_list):
             participants = list(set(ver_devices))
             participants.sort()
             self.aggregators.append(
@@ -254,23 +261,23 @@
             )
             for i in range(len(devices_list))
         ]
         self._init_train_data(x=x, y=y, epochs=epochs, batch_size=batch_size)
 
         for epoch in range(epochs):
             if epoch % agg_epochs == 0:
-                self._agg_weights()
+                self._agg_weights(aggr_hooks)
                 loss = self._compute_loss(x, y)
                 logging.info(f'MixLr epoch {epoch}: loss = {loss}')
                 if loss <= tol:
                     return
             self._fit_in_steps(
                 x, batch_size=batch_size, epoch=epoch, learning_rate=learning_rate
             )
-        self._agg_weights()
+        self._agg_weights(aggr_hooks)
         loss = self._compute_loss(x, y)
         logging.info(f'MixLr epoch {epoch + 1}: loss = {loss}')
 
     def _fit_in_steps(
         self,
         x: MixDataFrame,
         batch_size: int,
```

## secretflow/ml/linear/linear_model.py

```diff
@@ -10,40 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import dataclasses
-import os
 from enum import Enum, unique
-from typing import Dict, List, Union
+from typing import List, Union
 
-from secretflow.device import PYU, SPU, PYUObject, SPUObject
+from secretflow.device import PYUObject, SPUObject
 from secretflow.utils.sigmoid import SigType
 
 
 @unique
 class RegType(Enum):
-    Linear = 'linear'
-    Logistic = 'logistic'
-
-
-@dataclasses.dataclass
-class PartyPath:
-    party: str
-    path: str
-
-
-@dataclasses.dataclass
-class LinearModelRecord:
-    reg_type: RegType
-    sig_type: SigType
-    weights_spu: List[PartyPath]
-    weights_pyu: List[PartyPath]
+    Linear = "linear"
+    Logistic = "logistic"
 
 
 @dataclasses.dataclass
 class LinearModel:
     """
     Unified linear regression model.
 
@@ -56,51 +41,7 @@
         sig_type : SigType
             which sigmoid approximation should use, only use in mpc lr.
     """
 
     weights: Union[SPUObject, List[PYUObject]]
     reg_type: RegType
     sig_type: SigType
-
-    def dump(self, dir_path: Dict[str, str]) -> LinearModelRecord:
-        if isinstance(self.weights, SPUObject):
-            spu_paths = [
-                os.path.join(dir_path[name], 'weights')
-                for name in self.weights.device.actors.keys()
-            ]
-            self.weights.device.dump(self.weights, spu_paths)
-
-            weights_pyu = None
-            weights_spu = [
-                PartyPath(party, path)
-                for party, path in zip(self.weights.device.actors.keys(), spu_paths)
-            ]
-        else:
-            raise NotImplementedError("pyu weights are not supported")
-
-        return LinearModelRecord(
-            reg_type=self.reg_type,
-            sig_type=self.sig_type,
-            weights_pyu=weights_pyu,
-            weights_spu=weights_spu,
-        )
-
-    @classmethod
-    def load(
-        cls,
-        record: LinearModelRecord,
-        spu: SPU = None,
-        pyus: List[PYU] = None,
-    ) -> 'LinearModel':
-        assert len(record.weights_spu) or len(
-            record.weights_pyu
-        ), 'weights are not provided.'
-
-        if record.weights_spu:
-            assert spu, 'spu device is not provided'
-            path_dict = {t.party: t.path for t in record.weights_spu}
-            paths = [path_dict[party] for party in spu.actors.keys()]
-            weights = spu.load(paths)
-        else:
-            raise NotImplementedError("pyu weights are not supported")
-
-        return cls(weights, record.reg_type, record.sig_type)
```

## secretflow/ml/nn/metrics.py

```diff
@@ -52,15 +52,15 @@
         return Default(self.name, total, count)
 
     def __radd__(self, other):
         assert other == 0
         return Default(self.name, self.total, self.count)
 
     def result(self):
-        logging.warn(
+        logging.warning(
             "Please pay attention to local metrics, global only do naive aggregation "
         )
         import tensorflow as tf
 
         metric = tf.keras.metrics.Mean()
         metric.total = self.total
         metric.count = self.count
```

## secretflow/ml/nn/fl/fl_model.py

```diff
@@ -23,15 +23,15 @@
 import math
 import os
 from typing import Callable, Dict, List, Tuple, Union
 
 import numpy as np
 from tqdm import tqdm
 
-from secretflow.data.horizontal.dataframe import HDataFrame
+from secretflow.data.horizontal import HDataFrame
 from secretflow.data.ndarray import FedNdarray
 from secretflow.device import PYU, reveal, wait
 from secretflow.device.device.pyu import PYUObject
 from secretflow.ml.nn.fl.compress import COMPRESS_STRATEGY, do_compress
 from secretflow.ml.nn.fl.strategy_dispatcher import dispatch_strategy
 from secretflow.ml.nn.fl.utils import History
 from secretflow.ml.nn.metrics import Metric, aggregate_metrics
@@ -129,15 +129,14 @@
         stage="train",
         label_decoder=None,
         max_batch_size=20000,
         prefetch_buffer_size=None,
         dataset_builder=None,
     ):
         if dataset_builder:
-
             steps_per_epochs = []
             for device, worker in self._workers.items():
                 assert (
                     device in dataset_builder
                 ), f"party={device} does not provide dataset_builder, please check"
                 steps_per_epoch = worker.build_dataset_from_builder(
                     dataset_builder[device],
```

## secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_g.py

```diff
@@ -11,15 +11,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 import collections
 import copy
 from typing import Tuple
 
 import numpy as np
 import tensorflow as tf
 
@@ -102,15 +101,14 @@
         self.logs = logs
         self.epoch_logs = copy.deepcopy(self.logs)
 
         # DP operation
         if dp_strategy is not None:
             if dp_strategy.model_gdp is not None:
                 local_gradients_sum = dp_strategy.model_gdp(local_gradients_sum)
-
         return local_gradients_sum, num_sample
 
 
 @register_strategy(strategy_name='fed_avg_g', backend='tensorflow')
 @proxy(PYUObject)
 class PYUFedAvgG(FedAvgG):
     pass
```

## secretflow/ml/nn/fl/backend/torch/fl_base.py

```diff
@@ -7,31 +7,31 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+"""Torch model on worker side
+"""
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 import numpy as np
+import pandas as pd
 import torch
 import torchmetrics
-import pandas as pd
+
 from secretflow.ml.nn.fl.backend.torch.sampler import sampler_data
-from secretflow.ml.nn.fl.backend.torch.utils import TorchModel
+from secretflow.ml.nn.utils import TorchModel
 from secretflow.ml.nn.metrics import Default, Mean, Precision, Recall
 from secretflow.utils.io import rows_count
 
-# Torch model on worker side
-
 
 class BaseTorchModel(ABC):
     def __init__(
         self,
         builder_base: Callable[[], TorchModel],
         random_seed: int = None,
     ):
```

## secretflow/ml/nn/fl/backend/torch/sampler.py

```diff
@@ -42,15 +42,14 @@
         random_seed: Prg seed for shuffling
     Returns:
         data_set: tf.data.Dataset
     """
     batch_size = math.floor(x.shape[0] * sampling_rate)
     assert batch_size > 0, "Unvalid batch size"
     if random_seed is not None:
-
         random.seed(random_seed)
         torch.manual_seed(random_seed)  # set random seed for cpu
         torch.cuda.manual_seed(random_seed)  # set random seed for cuda
         torch.backends.cudnn.deterministic = True
     data_list = [torch.Tensor((x.astype(np.float64)).copy())]
     if y is not None and len(y.shape) > 0:
         data_list.append(torch.Tensor(y.copy()))
```

## secretflow/ml/nn/fl/backend/torch/strategy/fed_scr.py

```diff
@@ -19,15 +19,15 @@
 import copy
 from typing import Callable, Tuple
 
 import numpy as np
 
 from secretflow.device import PYUObject, proxy
 from secretflow.ml.nn.fl.backend.torch.fl_base import BaseTorchModel
-from secretflow.ml.nn.fl.backend.torch.utils import TorchModel
+from secretflow.ml.nn.utils import TorchModel
 from secretflow.ml.nn.fl.strategy_dispatcher import register_strategy
 from secretflow.utils.compressor import SCRSparse, sparse_encode
 
 
 class FedSCR(BaseTorchModel):
     """
     FedSCR: A structure-wise aggregation method to identify and remove redundant updates,
```

## secretflow/ml/nn/fl/backend/torch/strategy/fed_stc.py

```diff
@@ -19,15 +19,15 @@
 import copy
 from typing import Callable, Tuple
 
 import numpy as np
 
 from secretflow.device import PYUObject, proxy
 from secretflow.ml.nn.fl.backend.torch.fl_base import BaseTorchModel
-from secretflow.ml.nn.fl.backend.torch.utils import TorchModel
+from secretflow.ml.nn.utils import TorchModel
 from secretflow.ml.nn.fl.strategy_dispatcher import register_strategy
 from secretflow.utils.compressor import STCSparse, sparse_decode, sparse_encode
 
 
 class FedSTC(BaseTorchModel):
     """
     FedSTC: Sparse Ternary Compression (STC), a new compression framework that is speciﬁcally
```

## secretflow/ml/nn/sl/sl_model.py

```diff
@@ -15,80 +15,106 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """SLModel
 
 """
-
 import logging
 import math
 import os
 from typing import Callable, Dict, Iterable, List, Tuple, Union
 
 from multiprocess import cpu_count
 from tqdm import tqdm
 
 from secretflow.data.base import Partition
 from secretflow.data.horizontal import HDataFrame
 from secretflow.data.ndarray import FedNdarray
 from secretflow.data.vertical import VDataFrame
 from secretflow.device import PYU, Device, reveal, wait
 from secretflow.device.device.pyu import PYUObject
+from secretflow.ml.nn.sl.agglayer.agg_layer import AggLayer
+from secretflow.ml.nn.sl.agglayer.agg_method import AggMethod
 from secretflow.ml.nn.sl.strategy_dispatcher import dispatch_strategy
 from secretflow.security.privacy import DPStrategy
-from secretflow.utils.compressor import Compressor
 from secretflow.utils.random import global_random
 
 
 class SLModel:
     def __init__(
         self,
         base_model_dict: Dict[Device, Callable[[], 'tensorflow.keras.Model']] = {},
         device_y: PYU = None,
         model_fuse: Callable[[], 'tensorflow.keras.Model'] = None,
-        compressor: Compressor = None,
         dp_strategy_dict: Dict[Device, DPStrategy] = None,
         random_seed: int = None,
+        backend: str = "tensorflow",
         strategy='split_nn',
+        agg_method: AggMethod = None,
         **kwargs,
     ):
         """Interface for vertical split learning
         Attributes:
             base_model_dict: Basemodel dictionary, key is PYU, value is the Basemodel defined by party.
             device_y: Define which model have label.
             model_fuse:  Fuse model definition.
-            compressor: Define strategy tensor compression algorithms to speed up transmission.
             dp_strategy_dict: Dp strategy dictionary.
             random_seed: If specified, the initial value of the model will remain the same, which ensures reproducible.
+            backend: name of backend engine, tensorflow or torch, default tensorflow
             strategy: Strategy of split learning.
+            agg_method: agg method decide how to aggregate hiddens from each parties, default None(compatible with legacy mode)
+        Keyword Args
+            simulation: Only need when use simulation mode
+            base_local_steps: Only for 'split_async' strategy, Number of rounds for local base update process
+            fuse_local_steps: Only for 'split_async' strategy, Number of rounds for local fuse update process
+            bound_param: Only for 'split_async' strategy, Parameter for limiting local gradient change
+            loss_thres: Only for 'split_state_async' strategy, Loss threshold triggering switch state in splitStateAS strategy
+            split_steps: Only for 'split_state_async' strategy, Number of batches triggering switch state in splitStateAS strategy
+            max_fuse_local_steps: Only for 'split_state_async' strategy, Maximum number of rounds for fuse local update in splitStateAS strategy?
+            compressor: Define strategy tensor compression algorithms to speed up transmission.
+            device_agg: The party do aggregation,it can be a PYU,SPU,etc.
         """
 
         self.device_y = device_y
-        self.has_compressor = compressor is not None
         self.dp_strategy_dict = dp_strategy_dict
         self.simulation = kwargs.get('simulation', False)
+        self.device_agg = kwargs.get('device_agg', None)
+        self.compressor = kwargs.get('compressor', None)
+
+        self.backend = backend
         self.num_parties = len(base_model_dict)
+        self.agglayer = AggLayer(
+            device_agg=self.device_agg if self.device_agg else self.device_y,
+            parties=list(base_model_dict.keys()),
+            device_y=self.device_y,
+            agg_method=agg_method,
+            backend=backend,
+            compressor=self.compressor,
+        )
 
-        # TODO: add argument `backend`
-        import secretflow.ml.nn.sl.backend.tensorflow.strategy  # noqa
+        if backend.lower() == "tensorflow":
+            import secretflow.ml.nn.sl.backend.tensorflow.strategy  # noqa
+        elif backend.lower() == "torch":
+            import secretflow.ml.nn.sl.backend.torch.strategy  # noqa
+        else:
+            raise Exception(f"Invalid backend = {backend}")
 
         self._workers = {}
         for device, model in base_model_dict.items():
             self._workers[device], self.check_skip_grad = dispatch_strategy(
                 strategy,
-                backend=kwargs.get('backend', 'tensorflow'),
-                device=device,
+                backend=backend,
                 builder_base=model,
                 builder_fuse=None if device != device_y else model_fuse,
-                compressor=compressor,
                 random_seed=random_seed,
                 dp_strategy=dp_strategy_dict.get(device, None)
                 if dp_strategy_dict
                 else None,
+                device=device,
                 base_local_steps=kwargs.get('base_local_steps', 1),
                 fuse_local_steps=kwargs.get('fuse_local_steps', 1),
                 bound_param=kwargs.get('bound_param', 0.0),
                 loss_thres=kwargs.get('loss_thres', 0.01),
                 split_steps=kwargs.get('split_steps', 1),
                 max_fuse_local_steps=kwargs.get('max_fuse_local_steps', 1),
             )
@@ -138,14 +164,15 @@
                     device in dataset_builder
                 ), f"party={device} does not provide dataset_builder, please check"
                 ret = worker.build_dataset_from_builder(
                     *xs,
                     y=y_partitions,
                     s_w=s_w_partitions,
                     batch_size=batch_size,
+                    random_seed=random_seed,
                     stage=stage,
                     dataset_builder=dataset_builder[device],
                 )
                 worker_steps.append(ret)
 
             else:
                 worker.build_dataset_from_numeric(
@@ -238,15 +265,15 @@
             assert isinstance(dp_spent_step_freq, int) and dp_spent_step_freq >= 1
 
         # get basenet ouput num
         self.basenet_output_num = {
             device: reveal(worker.get_basenet_output_num())
             for device, worker in self._workers.items()
         }
-
+        self.agglayer.set_basenet_output_num(self.basenet_output_num)
         # build dataset
         train_x, train_y = x, y
         if validation_data is not None:
             logging.debug("validation_data provided")
             if len(validation_data) == 2:
                 valid_x, valid_y = validation_data
                 valid_sample_weight = None
@@ -276,62 +303,57 @@
                 batch_size=batch_size,
                 epochs=epochs,
                 stage="eval",
                 dataset_builder=dataset_builder,
             )
 
         self._workers[self.device_y].init_training(callbacks, epochs=epochs)
-        self._workers[self.device_y].on_train_begin()
-        fuse_net_num_returns = sum(self.basenet_output_num.values())
+        [worker.on_train_begin() for worker in self._workers.values()]
         wait_steps = min(min(self.get_cpus()) * 2, 100)
         for epoch in range(epochs):
             res = []
             report_list = []
             report_list.append(f"epoch: {epoch+1}/{epochs} - ")
             if verbose == 1:
                 pbar = tqdm(total=steps_per_epoch)
             self._workers[self.device_y].reset_metrics()
-            self._workers[self.device_y].on_epoch_begin(epoch)
-            fuse_net_num_returns = sum(self.basenet_output_num.values())
+            [worker.on_epoch_begin(epoch) for worker in self._workers.values()]
+
             for step in range(0, steps_per_epoch):
                 if verbose == 1:
                     pbar.update(1)
-                hiddens = []
+                hiddens = {}
                 self._workers[self.device_y].on_train_batch_begin(step=step)
                 for device, worker in self._workers.items():
-                    # enable compression in fit when model has compressor
-                    hidden = worker.base_forward(
-                        stage="train", compress=self.has_compressor
-                    )
-                    hiddens.append(hidden.to(self.device_y))
-
+                    # 1. Local calculation of basenet
+                    hidden = worker.base_forward(stage="train")
+                    # 2. The results of basenet are sent to fusenet
+                    hiddens[device] = hidden
+                # do agglayer forward
+                agg_hiddens = self.agglayer.forward(hiddens, axis=0)
+                if isinstance(agg_hiddens, PYUObject):
+                    agg_hiddens = [agg_hiddens]
+                # 3. Fusenet do local calculates and return gradients
                 gradients = self._workers[self.device_y].fuse_net(
-                    *hiddens,
-                    _num_returns=fuse_net_num_returns,
-                    compress=self.has_compressor,
+                    *agg_hiddens,
                 )
+
                 # In some strategies, we need to bypass the backpropagation step.
                 skip_gradient = False
                 if self.check_skip_grad:
                     skip_gradient = reveal(
                         self._workers[self.device_y].get_skip_gradient()
                     )
 
                 if not skip_gradient:
-                    idx = 0
+                    # do agglayer backward
+                    scatter_gradients = self.agglayer.backward(gradients)
                     for device, worker in self._workers.items():
-                        gradient_list = []
-                        for i in range(self.basenet_output_num[device]):
-                            gradient = gradients[idx + i].to(device)
-                            gradient_list.append(gradient)
-
-                        worker.base_backward(
-                            gradient_list, compress=self.has_compressor
-                        )
-                        idx += self.basenet_output_num[device]
+                        worker.base_backward(scatter_gradients[device])
+
                 r_count = self._workers[self.device_y].on_train_batch_end(step=step)
                 res.append(r_count)
                 if self.dp_strategy_dict is not None and dp_spent_step_freq is not None:
                     current_step = epoch * steps_per_epoch + step
                     if current_step % dp_spent_step_freq == 0:
                         privacy_device = {}
                         for device, dp_strategy in self.dp_strategy_dict.items():
@@ -341,19 +363,22 @@
                     wait(res)
                     res = []
             if validation and epoch % validation_freq == 0:
                 # validation
                 self._workers[self.device_y].reset_metrics()
                 res = []
                 for step in range(0, valid_steps):
-                    hiddens = []  # driver end
+                    hiddens = {}  # driver end
                     for device, worker in self._workers.items():
                         hidden = worker.base_forward("eval")
-                        hiddens.append(hidden.to(self.device_y))
-                    metrics = self._workers[self.device_y].evaluate(*hiddens)
+                        hiddens[device] = hidden
+                    agg_hiddens = self.agglayer.forward(hiddens, axis=0)
+                    if isinstance(agg_hiddens, PYUObject):
+                        agg_hiddens = [agg_hiddens]
+                    metrics = self._workers[self.device_y].evaluate(*agg_hiddens)
                     res.append(metrics)
                     if len(res) == wait_steps:
                         wait(res)
                         res = []
                 wait(res)
                 self._workers[self.device_y].on_validation(metrics)
 
@@ -394,37 +419,34 @@
             VDataFrame,
             FedNdarray,
             List[Union[HDataFrame, VDataFrame, FedNdarray]],
         ],
         batch_size=32,
         verbose=0,
         dataset_builder: Callable[[List], Tuple[int, Iterable]] = None,
-        compress: bool = False,
     ):
         """Vertical split learning offline prediction interface
 
         Args:
             x: Input data. It could be:
 
             - VDataFrame: a vertically aligned dataframe.
             - FedNdArray: a vertically aligned ndarray.
             - List[Union[HDataFrame, VDataFrame, FedNdarray]]: list of dataframe or ndarray.
 
             batch_size: Number of samples per gradient update, Int
             verbose: 0, 1. Verbosity mode
             dataset_builder: Callable function, its input is `x` or `[x, y]` if y is set, it should return
               steps_per_epoch and iterable dataset. Dataset builder is mainly for building graph dataset.
-            compress: Whether to use compressor to compress cross device data.
         """
 
         assert (
             isinstance(batch_size, int) and batch_size > 0
         ), f"batch_size should be integer > 0"
-        if compress:
-            assert self.has_compressor, "can not found compressor in model"
+
         predict_steps = self.handle_data(
             x,
             None,
             batch_size=batch_size,
             stage="eval",
             epochs=1,
             dataset_builder=dataset_builder,
@@ -432,21 +454,24 @@
         if verbose > 0:
             pbar = tqdm(total=predict_steps)
             pbar.set_description('Predict Processing:')
         result = []
         wait_steps = min(min(self.get_cpus()) * 2, 100)
         res = []
         for step in range(0, predict_steps):
-            hiddens = []
+            forward_data_dict = {}
             for device, worker in self._workers.items():
-                hidden = worker.base_forward(stage="eval", compress=compress)
-                hiddens.append(hidden.to(self.device_y))
+                f_data = worker.base_forward(stage="eval")
+                forward_data_dict[device] = f_data
+            agg_hiddens = self.agglayer.forward(forward_data_dict, axis=0)
+            if isinstance(agg_hiddens, PYUObject):
+                agg_hiddens = [agg_hiddens]
             if verbose > 0:
                 pbar.update(1)
-            y_pred = self._workers[self.device_y].predict(*hiddens, compress=compress)
+            y_pred = self._workers[self.device_y].predict(*agg_hiddens)
             result.append(y_pred)
 
             res.append(y_pred)
             if len(res) == wait_steps:
                 wait(res)
                 res = []
         wait(res)
@@ -462,15 +487,14 @@
         ],
         y: Union[VDataFrame, FedNdarray, PYUObject],
         batch_size: int = 32,
         sample_weight=None,
         verbose=1,
         dataset_builder: Dict = None,
         random_seed: int = None,
-        compress: bool = False,
     ):
         """Vertical split learning evaluate interface
 
         Args:
             x: Input data. It could be:
 
             - VDataFrame: a vertically aligned dataframe.
@@ -481,24 +505,22 @@
             batch_size: Integer or `Dict`. Number of samples per batch of
                 computation. If unspecified, `batch_size` will default to 32.
             sample_weight: Optional Numpy array of weights for the test samples,
                 used for weighting the loss function.
             verbose: Verbosity mode. 0 = silent, 1 = progress bar.
             dataset_builder: Callable function, its input is `x` or `[x, y]` if y is set, it should return dataset.
             random_seed: Seed for prgs, will only affect shuffle
-            compress: Whether to use compressor to compress cross device data.
         Returns:
             metrics: federate evaluate result
         """
 
         assert (
             isinstance(batch_size, int) and batch_size > 0
         ), f"batch_size should be integer > 0"
-        if compress:
-            assert self.has_compressor, "can not found compressor in model"
+
         if random_seed is None:
             random_seed = global_random(self.device_y, 100000)
         evaluate_steps = self.handle_data(
             x,
             y,
             sample_weight=sample_weight,
             batch_size=batch_size,
@@ -511,21 +533,24 @@
         self._workers[self.device_y].reset_metrics()
         if verbose > 0:
             pbar = tqdm(total=evaluate_steps)
             pbar.set_description('Evaluate Processing:')
 
         wait_steps = min(min(self.get_cpus()) * 2, 100)
         for step in range(0, evaluate_steps):
-            hiddens = []  # driver端
-            for worker in self._workers.values():
-                hidden = worker.base_forward(stage="eval", compress=compress)
-                hiddens.append(hidden.to(self.device_y))
+            hiddens = {}  # driver端
+            for device, worker in self._workers.items():
+                hidden = worker.base_forward(stage="eval")
+                hiddens[device] = hidden
             if verbose > 0:
                 pbar.update(1)
-            metrics = self._workers[self.device_y].evaluate(*hiddens, compress=compress)
+            agg_hiddens = self.agglayer.forward(hiddens, axis=0)
+            if isinstance(agg_hiddens, PYUObject):
+                agg_hiddens = [agg_hiddens]
+            metrics = self._workers[self.device_y].evaluate(*agg_hiddens)
             if (step + 1) % wait_steps == 0:
                 wait(metrics)
         report_list = [f"{k}:{v}" for k, v in reveal(metrics).items()]
         report = " ".join(report_list)
         if verbose == 1:
             pbar.set_postfix_str(report)
             pbar.close()
```

## secretflow/ml/nn/sl/backend/tensorflow/sl_base.py

```diff
@@ -17,33 +17,26 @@
 
 
 """sl model base
 """
 import copy
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Callable, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
-import torch
 from tensorflow.python.keras import callbacks as callbacks_module
-from torch import nn
-from torch.nn.modules.loss import _Loss as BaseTorchLoss
-from torch.optim import Optimizer
-from torch.utils.data import DataLoader
 
-import secretflow.device as ft
 from secretflow.device import PYUObject, proxy
 from secretflow.ml.nn.metrics import AUC, Mean, Precision, Recall
-from secretflow.ml.nn.sl.backend.tensorflow.utils import ForwardData
 from secretflow.ml.nn.sl.strategy_dispatcher import register_strategy
 from secretflow.security.privacy import DPStrategy
-from secretflow.utils.compressor import Compressor, SparseCompressor
+from secretflow.utils.communicate import ForwardData
 
 
 class SLBaseModel(ABC):
     def __init__(self, builder_base: Callable, builder_fuse: Callable = None):
         self.model_base = builder_base() if builder_base is not None else None
         self.model_fuse = builder_fuse() if builder_fuse is not None else None
 
@@ -56,62 +49,28 @@
         pass
 
     @abstractmethod
     def fuse_net(self, hiddens):
         pass
 
 
-class SLBaseModule(ABC, nn.Module):
-    @abstractmethod
-    def forward(self, x):
-        pass
-
-    def get_weights(self):
-        return {k: v.cpu() for k, v in self.state_dict().items()}
-
-    def set_weights(self, weights):
-        self.load_state_dict(weights)
-
-    def get_gradients(self, parameters=None):
-        if parameters is None:
-            parameters = self.parameters()
-        grads = []
-        for p in parameters:
-            grad = None if p.grad is None else p.grad.data.cpu().numpy()
-            grads.append(grad)
-        return grads
-
-    def set_gradients(
-        self,
-        gradients: List[Union[torch.Tensor, np.ndarray]],
-        parameters: Optional[List[torch.Tensor]] = None,
-    ):
-        if parameters is None:
-            parameters = self.parameters()
-        for g, p in zip(gradients, parameters):
-            if g is not None:
-                p.grad = torch.from_numpy(g.copy())
-
-
 class SLBaseTFModel(SLBaseModel):
     def __init__(
         self,
         builder_base: Callable[[], tf.keras.Model],
         builder_fuse: Callable[[], tf.keras.Model],
         dp_strategy: DPStrategy,
-        compressor: Compressor,
         random_seed: int = None,
         **kwargs,
     ):
         self.dp_strategy = dp_strategy
         self.embedding_dp = (
             self.dp_strategy.embedding_dp if dp_strategy is not None else None
         )
         self.label_dp = self.dp_strategy.label_dp if dp_strategy is not None else None
-        self.compressor = compressor
 
         self.train_set = None
         self.eval_set = None
         self.valid_set = None
         self.tape = None
         self.h = None
         self.train_x, self.train_y = None, None
@@ -150,15 +109,14 @@
     def set_steps_per_epoch(self, steps_per_epoch):
         self.steps_per_epoch = steps_per_epoch
 
     def get_basenet_output_num(self):
         if hasattr(self.model_base, 'outputs') and self.model_base.outputs is not None:
             return len(self.model_base.outputs)
         else:
-
             if hasattr(self.model_base, "output_num"):
                 return self.model_base.output_num()
             else:
                 raise Exception(
                     "Please define the output_num function in basemodel and return the number of basenet outputs, then try again"
                 )
 
@@ -227,14 +185,18 @@
     ):
         """build tf.data.Dataset
 
         Args:
             x: feature, FedNdArray or HDataFrame
             y: label, FedNdArray or HDataFrame
             s_w: sample weight, FedNdArray or HDataFrame
+            batch_size: Number of samples per gradient update.
+            shuffle: Whether to shuffle dataset
+            buffer_size: buffer size for shuffling
+            random_seed: Prg seed for shuffling
             stage: stage of this datset
             dataset_builder: dataset build callable function of worker
         """
         assert x and x[0] is not None, "X can not be None, please check"
         x = [xi for xi in x]
         has_y = False
         has_s_w = False
@@ -312,19 +274,18 @@
         if self.embedding_dp is not None:
             if isinstance(h, List):
                 h = [self.embedding_dp(hi) for hi in h]
             else:
                 h = self.embedding_dp(h)
         return h
 
-    def base_forward(self, stage="train", compress: bool = False) -> ForwardData:
+    def base_forward(self, stage="train") -> ForwardData:
         """compute hidden embedding
         Args:
             stage: Which stage of the base forward
-            compress: Whether to compress cross device data.
         Returns: hidden embedding
         """
 
         assert (
             self.model_base is not None
         ), "Base model cannot be none, please give model define or load a trained model"
 
@@ -378,50 +339,29 @@
                 data_x,
             )
         self.data_x = data_x
 
         forward_data = ForwardData()
         if len(self.model_base.losses) > 0:
             forward_data.losses = tf.add_n(self.model_base.losses)
-        # TODO: only vaild on no server mode, refactor when use agglayer or server mode.
-        # no need to compress data on model_fuse side
-        if compress and not self.model_fuse:
-            if self.compressor:
-                forward_data.hidden = self.compressor.compress(self.h.numpy())
-            else:
-                raise Exception(
-                    'can not find compressor when compress data in base_forward'
-                )
-        else:
-            forward_data.hidden = self.h
+        forward_data.hidden = self.h
         return forward_data
 
-    @tf.function
     def _base_backward_internal(self, gradients, trainable_vars):
         self.model_base.optimizer.apply_gradients(zip(gradients, trainable_vars))
 
-    def base_backward(self, gradient, compress: bool = False):
+    def base_backward(self, gradient):
         """backward on fusenet
 
         Args:
             gradient: gradient of fusenet hidden layer
-            compress: Whether to decompress gradient.
         """
 
         return_hiddens = []
 
-        # TODO: only vaild on no server mode, refactor when use agglayer or server mode.
-        # no need to decompress data on model_fuse side
-        if compress and not self.model_fuse:
-            if self.compressor:
-                gradient = self.compressor.decompress(gradient)
-            else:
-                raise Exception(
-                    'can not find compressor when decompress data in base_backward'
-                )
         with self.tape:
             if len(gradient) == len(self.h):
                 for i in range(len(gradient)):
                     return_hiddens.append(self.fuse_op(self.h[i], gradient[i]))
             else:
                 gradient = gradient[0]
                 return_hiddens.append(self.fuse_op(self.h, gradient))
@@ -462,103 +402,80 @@
         else:
             raise NotImplementedError
 
     def get_stop_training(self):
         return self.model_fuse.stop_training
 
     def on_train_begin(self):
-        self.fuse_callbacks.on_train_begin()
+        if self.fuse_callbacks:
+            self.fuse_callbacks.on_train_begin()
 
     def on_epoch_begin(self, epoch):
-        self.fuse_callbacks.on_epoch_begin(epoch)
+        if self.fuse_callbacks:
+            self.fuse_callbacks.on_epoch_begin(epoch)
 
     def on_train_batch_begin(self, step=None):
         assert step is not None, "Step cannot be none"
-        self.fuse_callbacks.on_train_batch_begin(step)
+        if self.fuse_callbacks:
+            self.fuse_callbacks.on_train_batch_begin(step)
 
     def on_train_batch_end(self, step=None):
         assert step is not None, "Step cannot be none"
         self.epoch_logs = copy.deepcopy(self.logs)
-        self.fuse_callbacks.on_train_batch_end(step, self.logs)
+        if self.fuse_callbacks:
+            self.fuse_callbacks.on_train_batch_end(step, self.logs)
 
     def on_validation(self, val_logs):
         val_logs = {'val_' + name: val for name, val in val_logs.items()}
         self.epoch_logs.update(val_logs)
 
     def on_epoch_end(self, epoch):
-
-        self.fuse_callbacks.on_epoch_end(epoch, self.epoch_logs)
+        if self.fuse_callbacks:
+            self.fuse_callbacks.on_epoch_end(epoch, self.epoch_logs)
         self.training_logs = self.epoch_logs
         return self.epoch_logs
 
     def on_train_end(self):
-        self.fuse_callbacks.on_train_end(logs=self.training_logs)
+        if self.fuse_callbacks:
+            self.fuse_callbacks.on_train_end(logs=self.training_logs)
         return self.model_fuse.history.history
 
     def set_sample_weight(self, sample_weight, stage="train"):
         if stage == "train":
             self.train_sample_weight = sample_weight
         elif stage == "eval":
             self.eval_sample_weight = sample_weight
         else:
             raise Exception("Illegal Argument")
 
     def fuse_net(
         self,
         *forward_data: List[ForwardData],
         _num_returns: int = 2,
-        compress: bool = False,
     ):
         """Fuses the hidden layer and calculates the reverse gradient
         only on the side with the label
 
         Args:
             forward_data: A list of ForwardData containing hidden layers, losses, etc.
                 that are uploaded by each party for computation.
-            compress: Whether to decompress/compress data.
         Returns:
             gradient Of hiddens
         """
         assert (
             self.model_fuse is not None
         ), "Fuse model cannot be none, please give model define"
+
         for i, h in enumerate(forward_data):
             assert h.hidden is not None, f"hidden cannot be found in forward_data[{i}]"
+            if isinstance(h.losses, List) and h.losses[0] is None:
+                h.losses = None
         # get reg losses:
         losses = [h.losses for h in forward_data if h.losses is not None]
         hidden_features = [h.hidden for h in forward_data]
-        if compress:
-            if self.compressor:
-                iscompressed = self.compressor.iscompressed(hidden_features)
-                # save fuse_sparse_masks to apply on gradients
-                if isinstance(self.compressor, SparseCompressor):
-                    fuse_sparse_masks = list(
-                        map(
-                            # Get a sparse matrix mask with dtype=bool.
-                            # Using <bool> as the dtype will ensure that the data type of gradients after applying the mask does not change.
-                            lambda d, compressed: (d != 0) if compressed else None,
-                            hidden_features,
-                            iscompressed,
-                        )
-                    )
-                # decompress
-                hidden_features = list(
-                    map(
-                        lambda d, compressed: self.compressor.decompress(d)
-                        if compressed
-                        else d,
-                        hidden_features,
-                        iscompressed,
-                    )
-                )
-            else:
-                raise Exception(
-                    'can not find compressor when decompress data in fuse_net'
-                )
-
         hiddens = []
         for h in hidden_features:
             # h will be list, if basenet is multi output
             if isinstance(h, List):
                 for i in range(len(h)):
                     hiddens.append(tf.convert_to_tensor(h[i]))
             else:
@@ -569,38 +486,14 @@
 
         for m in self.model_fuse.metrics:
             logs['train_' + m.name] = m.result().numpy()
         self.logs = logs
         # In some strategies, we don't need to return gradient.
         if self.skip_gradient:
             return [None] * _num_returns
-        if compress:
-            gradient = [g.numpy() for g in gradient]
-            # apply fuse_sparse_masks on gradients
-            if fuse_sparse_masks:
-                assert len(fuse_sparse_masks) == len(
-                    gradient
-                ), f'length of fuse_sparse_masks and gradient mismatch: {len(fuse_sparse_masks)} - {len(gradient)}'
-
-                def apply_mask(m, d):
-                    if m is not None:
-                        return m.multiply(d).tocsr()
-                    return d
-
-                gradient = list(map(apply_mask, fuse_sparse_masks, gradient))
-            else:
-                gradient = list(
-                    map(
-                        lambda d, compressed: self.compressor.compress(d)
-                        if compressed
-                        else d
-                    ),
-                    gradient,
-                    iscompressed,
-                )
         return gradient
 
     def _fuse_net_train(self, hiddens, losses=[]):
         return self._fuse_net_internal(
             hiddens,
             losses,
             self.train_y,
@@ -662,40 +555,34 @@
         )
 
         result = {}
         for m in self.model_fuse.metrics:
             result[m.name] = m.result()
         return result
 
-    def evaluate(self, *forward_data: List[ForwardData], compress: bool = False):
+    def evaluate(self, *forward_data: List[ForwardData]):
         """Returns the loss value & metrics values for the model in test mode.
 
         Args:
             forward_data: A list of data dictionaries containing hidden layers, losses, etc.
                 that are uploaded by each party for computation.
-            compress: Whether to decompress input data.
         Returns:
             map of model metrics.
         """
 
         assert (
             self.model_fuse is not None
         ), "model cannot be none, please give model define"
         for i, h in enumerate(forward_data):
             assert h.hidden is not None, f"hidden cannot be found in forward_data[{i}]"
+            if isinstance(h.losses, List) and h.losses[0] is None:
+                h.losses = None
         # get reg losses:
         losses = [h.losses for h in forward_data if h.losses is not None]
         hidden_features = [h.hidden for h in forward_data]
-        if compress:
-            if self.compressor:
-                hidden_features = self.compressor.decompress(hidden_features)
-            else:
-                raise Exception(
-                    'can not find compressor when decompress data in evaluate'
-                )
         hiddens = []
         for h in hidden_features:
             if isinstance(h, List):
                 for i in range(len(h)):
                     hiddens.append(tf.convert_to_tensor(h[i]))
             else:
                 hiddens.append(tf.convert_to_tensor(h))
@@ -755,37 +642,31 @@
         return self.wrap_local_metrics()
 
     @tf.function
     def _predict_internal(self, hiddens):
         y_pred = self.model_fuse(hiddens)
         return y_pred
 
-    def predict(self, *forward_data: List[ForwardData], compress: bool = False):
+    def predict(self, *forward_data: List[ForwardData]):
         """Generates output predictions for the input hidden layer features.
 
         Args:
             forward_data: A list of data dictionaries containing hidden layers,
                 that are uploaded by each party for computation.
-            compress: Whether to decompress input data.
         Returns:
             Array(s) of predictions.
         """
         assert (
             self.model_fuse is not None
         ), "Fuse model cannot be none, please give model define"
         for i, h in enumerate(forward_data):
             assert h.hidden is not None, f"hidden cannot be found in forward_data[{i}]"
+            if isinstance(h.losses, List) and h.losses[0] is None:
+                h.losses = None
         hidden_features = [h.hidden for h in forward_data]
-        if compress:
-            if self.compressor:
-                hidden_features = self.compressor.decompress(hidden_features)
-            else:
-                raise Exception(
-                    'can not find compressor when decompress data in predict'
-                )
 
         hiddens = []
         for h in hidden_features:
             if isinstance(h, List):
                 for i in range(len(h)):
                     hiddens.append(tf.convert_to_tensor(h[i]))
             else:
@@ -819,16 +700,15 @@
         return self._export_model(self.model_fuse, model_path, save_format, **kwargs)
 
     def _export_model(
         self, model, model_path: str, save_format: str = "onnx", **kwargs
     ):
         Path(model_path).parent.mkdir(parents=True, exist_ok=True)
         assert model_path is not None, "model path cannot be empty"
-        assert save_format in [
-            "onnx", "tf"], "save_format must be 'onnx' or 'tf'"
+        assert save_format in ["onnx", "tf"], "save_format must be 'onnx' or 'tf'"
         if save_format == "onnx":
             return self._export_onnx(model, model_path, **kwargs)
         elif save_format == "tf":
             return self._export_tf(model, model_path, **kwargs)
         else:
             raise Exception("invalid save_format")
 
@@ -851,16 +731,15 @@
 
         from tensorflow.python.tools import saved_model_utils
 
         from .utils import wrap_tf_input_output
 
         tag_set = 'serve'
         signature_def_key = 'serving_default'
-        meta_graph_def = saved_model_utils.get_meta_graph_def(
-            model_path, tag_set)
+        meta_graph_def = saved_model_utils.get_meta_graph_def(model_path, tag_set)
         if signature_def_key not in meta_graph_def.signature_def:
             raise ValueError(
                 f'Could not find signature "{signature_def_key}". Please choose from: '
                 f'{", ".join(meta_graph_def.signature_def.keys())}'
             )
         inputs = meta_graph_def.signature_def[signature_def_key].inputs
         outputs = meta_graph_def.signature_def[signature_def_key].outputs
@@ -879,79 +758,11 @@
         privacy_dict = self.dp_strategy.get_privacy_spent(step, orders)
         return privacy_dict
 
     def get_skip_gradient(self):
         return False
 
 
-class ModelPartition(object):
-    def __init__(self, model_fn, optim_fn, loss_fn, dataloader_fn):
-        self.model: SLBaseModule = model_fn()
-        self.optimizer: Optimizer = optim_fn(self.model.parameters())
-        self.loss: BaseTorchLoss = loss_fn()
-        self._dataloader: Dict[str, DataLoader] = {
-            k: dl_fn() for k, dl_fn in dataloader_fn.items()
-        }
-        self._dataiter: Dict[str, Iterator] = {
-            k: iter(_dl) for k, _dl in self._dataloader.items()
-        }
-
-    def get_one_batch(self, name='train'):
-        try:
-            x, y = next(self._dataiter[name])
-        except StopIteration:
-            self._dataiter = iter(self._dataloader[name])
-            x, y = next(self._dataiter)
-        return x, y
-
-    def forward(
-        self, used_name='train', external_input=None
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        if external_input is None:
-            external_input = {}
-        x, y = self.get_one_batch(used_name)
-        y_pred = self.model(x, **external_input)
-        return y_pred, y
-
-    def zero_grad(self):
-        self.optimizer.zero_grad()
-
-    def backward(self, used_name='train', gradients=None, external_input: Dict = None):
-        if gradients is not None:
-            self.model.set_gradients(gradients)
-        else:
-            if external_input is None:
-                external_input = {}
-            y_pred, y = self.forward(used_name, external_input)
-            loss = self.loss(y_pred, y)
-            loss.backward()
-        return self.model.get_gradients()
-
-    def apply_gradients(self, gradients=None):
-        if gradients is not None:
-            self.model.set_gradients(gradients)
-        self.optim_step()
-
-    def optim_step(self):
-        self.optimizer.step()
-        return self.model.get_weights()
-
-    def get_weights(self):
-        return self.model.get_weights()
-
-    def set_weights(self, weights):
-        self.model.set_weights(weights)
-
-    def call_model_fn(self, fn_name, *args, **kwargs):
-        # TODO: a temporary utils
-        return getattr(self.model, fn_name)(*args, **kwargs)
-
-
 @register_strategy(strategy_name='split_nn', backend='tensorflow')
 @proxy(PYUObject)
 class PYUSLTFModel(SLBaseTFModel):
     pass
-
-
-@proxy(ft.PYUObject)
-class PYUModel(ModelPartition):
-    pass
```

## secretflow/ml/nn/sl/backend/tensorflow/strategy/split_async.py

```diff
@@ -25,32 +25,34 @@
 
 import tensorflow as tf
 
 from secretflow.device import PYUObject, proxy
 from secretflow.ml.nn.sl.backend.tensorflow.sl_base import SLBaseTFModel
 from secretflow.ml.nn.sl.strategy_dispatcher import register_strategy
 from secretflow.security.privacy import DPStrategy
-from secretflow.utils.compressor import Compressor
 
 
 class SLAsyncTFModel(SLBaseTFModel):
     def __init__(
         self,
         builder_base: Callable[[], tf.keras.Model],
         builder_fuse: Callable[[], tf.keras.Model],
         dp_strategy: DPStrategy,
-        compressor: Compressor,
         base_local_steps: int,
         fuse_local_steps: int,
         bound_param: float,
         random_seed: int = None,
         **kwargs,
     ):
         super().__init__(
-            builder_base, builder_fuse, dp_strategy, compressor, random_seed, **kwargs
+            builder_base,
+            builder_fuse,
+            dp_strategy,
+            random_seed,
+            **kwargs,
         )
         self.base_local_steps = base_local_steps
         self.fuse_local_steps = fuse_local_steps
         self.bound_param = bound_param
 
     @tf.function
     def _base_forward_internal(self, data_x, use_dp: bool = True):
@@ -60,31 +62,21 @@
         if use_dp and self.embedding_dp is not None:
             if isinstance(h, List):
                 h = [self.embedding_dp(hi) for hi in h]
             else:
                 h = self.embedding_dp(h)
         return h
 
-    def base_backward(self, gradient, compress: bool = False):
+    def base_backward(self, gradient):
         """backward on fusenet
 
         Args:
             gradient: gradient of fusenet hidden layer
-            compress: Whether to decompress gradient.
         """
 
-        # TODO: only vaild on no server mode, refactor when use agglayer or server mode.
-        # no need to decompress data on model_fuse side
-        if compress and not self.model_fuse:
-            if self.compressor:
-                gradient = self.compressor.decompress(gradient)
-            else:
-                raise Exception(
-                    'can not find compressor when decompress data in base_backward'
-                )
         for local_step in range(self.base_local_steps):
             return_hiddens = []
             with self.tape:
                 if local_step == 0 and self.h is not None:
                     h = self.h
                 else:
                     h = self._base_forward_internal(self.data_x, use_dp=False)
```

## secretflow/ml/nn/sl/backend/tensorflow/strategy/split_state_async.py

```diff
@@ -25,34 +25,38 @@
 
 import tensorflow as tf
 
 from secretflow.device import PYUObject, proxy
 from secretflow.ml.nn.sl.backend.tensorflow.sl_base import SLBaseTFModel
 from secretflow.ml.nn.sl.strategy_dispatcher import register_strategy
 from secretflow.security.privacy import DPStrategy
-from secretflow.utils.compressor import Compressor
 
 
 class SLStateAsyncTFModel(SLBaseTFModel):
     def __init__(
         self,
         builder_base: Callable[[], tf.keras.Model],
         builder_fuse: Callable[[], tf.keras.Model],
         dp_strategy: DPStrategy,
-        compressor: Compressor,
         loss_thres: float = 0,
         split_steps: int = 1,
         max_fuse_local_steps: int = 1,
         random_seed: int = None,
         **kwargs,
     ):
         super().__init__(
-            builder_base, builder_fuse, dp_strategy, compressor, random_seed, **kwargs
+            builder_base,
+            builder_fuse,
+            dp_strategy,
+            random_seed,
+            **kwargs,
         )
-        assert max_fuse_local_steps > 0, f'state async max_fuse_local_steps should greater than 0'
+        assert (
+            max_fuse_local_steps > 0
+        ), f'state async max_fuse_local_steps should greater than 0'
         self.loss_thres = loss_thres
         self.split_steps = split_steps
         self.max_fuse_local_steps = max_fuse_local_steps
         # SplitAT state
         self.count = 0
         self.total_loss = 0
         self.last_update_loss = 0
```

## secretflow/ml/nn/sl/backend/torch/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Ant Group Co., Ltd.
+# Copyright 2023 Ant Group Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

## secretflow/preprocessing/binning/vert_woe_binning.py

```diff
@@ -42,37 +42,37 @@
         secure_device: HEU or SPU for secure bucket summation.
 
     """
 
     def __init__(self, secure_device: Union[SPU, HEU]):
         self.secure_device = secure_device
 
-    def _find_coordinator_device(self, vdata: VDataFrame, label_name) -> PYU:
+    def _find_label_holder_device(self, vdata: VDataFrame, label_name) -> PYU:
         """
         Find which holds the label column.
 
         Attributes:
             vdata: vertical slice datasets
             label_name: label column name.
 
         Return:
             PYU device
         """
         device_column_names = vdata.partition_columns
         label_count = 0
         for device in device_column_names:
             if np.isin(label_name, device_column_names[device]).all():
-                coordinator_device = device
+                label_holder_device = device
                 label_count += 1
 
         assert (
             label_count == 1
         ), f"One and only one party can have label, but found {label_count}"
 
-        return coordinator_device
+        return label_holder_device
 
     def binning(
         self,
         vdata: VDataFrame,
         binning_method: str = "quantile",
         bin_num: int = 10,
         bin_names: Dict[PYU, List[str]] = {},
@@ -82,14 +82,16 @@
         chimerge_target_bins: int = 10,
         chimerge_target_pvalue: float = 0.1,
         audit_log_path: Dict[str, str] = {},
     ):
         """
         Build woe substitution rules base on vdata.
         Only support binary classification label dataset.
+        The total sample numbers in each bin are not protected in current implementation.
+        The split points for bins and the number of postive samples in each bin are protected.
 
         Attributes:
             vdata: vertical slice datasets
                 use {binning_method} to bin all number type features.
                 for string type feature bin by it's categories.
                 else bin is count for np.nan samples
             binning_method: how to bin number type features.
@@ -127,20 +129,34 @@
                             "type": str, # "string" or "numeric", if feature is discrete or continuous
                             "categories": list[str], # categories for discrete feature
                             "split_points": list[float], # left-open right-close split points
                             "total_counts": list[int], # total samples count in each bins.
                             "else_counts": int, # np.nan samples count
                             "woes": list[float], # woe values for each bins.
                             "else_woe": float, # woe value for np.nan samples.
-                            "ivs": list[float], # iv values for each bins.
-                            "else_iv": float, # iv value for np.nan samples.
                         },
                         # ... others feature
+                    ],
+                    # label holder's PYUObject only
+                    # warning: giving bin_ivs to other party will leak positive samples in each bin.
+                    # it is up to label holder's will to give feature iv or bin ivs or all info to workers.
+                    # for more information, look at: https://github.com/secretflow/secretflow/issues/565
+
+                    # in the following comment, by safe we mean label distribution info is not leaked.
+                    "feature_iv_info" :[
+                        {
+                            "name": str, #feature name
+                            "ivs": list[float], #iv values for each bins, not safe to share with workers in any case.
+                            "else_iv": float, #iv for nan values, may share to with workers
+                            "feature_iv": float, #sum of bin_ivs, safe to share with workers when bin num > 2.
+                        }
                     ]
                 }
+
+
         """
         assert binning_method in (
             "quantile",
             "chimerge",
         ), f"binning_method only support ('quantile', 'chimerge'), got {binning_method}"
         assert bin_num > 0, f"bin_num range (0, ∞], got {bin_num}"
         assert (
@@ -152,74 +168,73 @@
         assert (
             chimerge_target_pvalue > 0 and chimerge_target_pvalue < 1
         ), f"chimerge_target_pvalue range (0, 1), got {chimerge_target_pvalue}"
 
         if audit_log_path:
             assert isinstance(self.secure_device, HEU), "only HEU support audit log"
 
-        coordinator_device = self._find_coordinator_device(vdata, label_name)
-        coordinator_audit_log_path = None
+        label_holder_device = self._find_label_holder_device(vdata, label_name)
+        label_holder_audit_log_path = None
 
         if isinstance(self.secure_device, HEU):
             assert len(bin_names) == 2, "only support two party binning in HEU mode"
-            assert self.secure_device.sk_keeper_name() == coordinator_device.party, (
+            assert self.secure_device.sk_keeper_name() == label_holder_device.party, (
                 f"HEU sk keeper party {self.secure_device.sk_keeper_name()} "
-                "mismatch with coordinator device's party {coordinator_device.party}"
+                "mismatch with label_holder device's party {label_holder_device.party}"
             )
             if audit_log_path:
                 assert (
-                    coordinator_device.party in audit_log_path
+                    label_holder_device.party in audit_log_path
                 ), "can not find sk keeper device's audit log path"
-                coordinator_audit_log_path = audit_log_path[coordinator_device.party]
+                label_holder_audit_log_path = audit_log_path[label_holder_device.party]
 
         workers: Dict[PYU, VertWoeBinningPyuWorker] = {}
-        if coordinator_device not in bin_names:
-            bin_names[coordinator_device] = list()
+        if label_holder_device not in bin_names:
+            bin_names[label_holder_device] = list()
 
         for device in bin_names:
             assert (
                 device in vdata.partitions.keys()
             ), f"device {device} in bin_names not exist in vdata"
             workers[device] = VertWoeBinningPyuWorker(
                 vdata.partitions[device].data.data,
                 binning_method,
                 bin_num,
                 bin_names[device],
-                label_name if coordinator_device == device else "",
+                label_name if label_holder_device == device else "",
                 positive_label,
                 chimerge_init_bins,
                 chimerge_target_bins,
                 chimerge_target_pvalue,
                 device=device,
             )
 
         woe_rules: Dict[PYU, PYUObject] = {}
 
-        # coordinator build woe rules
-        coordinator_worker = workers[coordinator_device]
-        label, coordinator_report = coordinator_worker.coordinator_work(
-            vdata.partitions[coordinator_device].data
+        # label_holder build woe rules
+        label_holder_worker = workers[label_holder_device]
+        label, label_holder_report = label_holder_worker.label_holder_work(
+            vdata.partitions[label_holder_device].data
         )
-        woe_rules[coordinator_device] = coordinator_report
 
         if isinstance(self.secure_device, SPU):
             secure_label = label.to(self.secure_device)
         elif isinstance(self.secure_device, HEU):
             secure_label = label.to(
                 self.secure_device,
-                HEUMoveConfig(heu_audit_log=coordinator_audit_log_path),
+                HEUMoveConfig(heu_audit_log=label_holder_audit_log_path),
             )
         else:
             raise NotImplementedError(
                 f'Secure device should be SPU or HEU, but got {type(self.secure_device)}.'
             )
 
         # all participants
         for device in workers:
-            if device == coordinator_device:
+            if device == label_holder_device:
                 continue
 
             worker = workers[device]
 
             if isinstance(self.secure_device, HEU):
                 if audit_log_path:
                     assert (
@@ -231,34 +246,46 @@
                         f'{worker_audit_path}.pk.pickle'
                     )
                 move_config = HEUMoveConfig()
                 move_config.heu_encoder = phe.BigintEncoderParams()
                 bin_indices = worker.participant_build_sum_indices(
                     vdata.partitions[device].data
                 )
-                bins_positive = (
-                    secure_label.batch_select_sum(bin_indices)
-                    .to(coordinator_device)
-                    .to(device)
+                bins_positive = secure_label.batch_select_sum(bin_indices).to(
+                    label_holder_device
                 )
-                bin_stats = worker.participant_sum_bin(bins_positive)
             else:
                 bin_select = worker.participant_build_sum_select(
                     vdata.partitions[device].data
                 )
 
                 def spu_work(label, select):
                     return jnp.matmul(label, select)
 
                 bins_positive = self.secure_device(spu_work)(
                     secure_label, bin_select.to(self.secure_device)
-                ).to(device)
+                ).to(label_holder_device)
 
-                bin_stats = worker.participant_sum_bin(bins_positive)
-
-            woe_ivs = coordinator_worker.coordinator_calc_woe_for_peer(
-                bin_stats.to(coordinator_device)
+            bim_sum_info = worker.get_bin_sum_info().to(label_holder_device)
+            (
+                bin_stats,
+                total_counts,
+                merged_split_point_indices,
+            ) = label_holder_worker.label_holder_sum_bin(bins_positive, bim_sum_info)
+            worker.participant_update_info(
+                total_counts.to(device), merged_split_point_indices.to(device)
+            )
+            woes, ivs = label_holder_worker.label_holder_calc_woe_for_peer(bin_stats)
+            # label_holder process and save the ivs, calculate the feature_ivs
+            label_holder_worker.label_holder_collect_iv_for_participant(
+                ivs, bim_sum_info
             )
-            report = worker.participant_build_report(woe_ivs.to(device))
+            report = worker.participant_build_report(woes.to(device))
             woe_rules[device] = report
 
+        # feature ivs are in label_holder report, which may be later shared to worker
+        label_holder_report = label_holder_worker.generate_iv_report(
+            label_holder_report
+        )
+        woe_rules[label_holder_device] = label_holder_report
+
         return woe_rules
```

## secretflow/preprocessing/binning/vert_woe_binning_pyu.py

```diff
@@ -8,23 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
 import math
+from dataclasses import dataclass
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import chi2
 
 from secretflow.device import PYUObject, proxy
 
+from .kernels.chi_merge import apply_chimerge, update_split_points
+
 
 @proxy(PYUObject)
 class VertWoeBinningPyuWorker:
     """
     PYU functions for woe binning
     Attributes: see VertWoeBinning
     """
@@ -38,14 +42,17 @@
         label_name: str,
         positive_label: str,
         chimerge_init_bins: int,
         chimerge_target_bins: int,
         chimerge_target_pvalue: float,
     ):
         data_columns = data.columns
+        assert isinstance(
+            bin_names, list
+        ), f"bin names should be a list of string but got {type(bin_names)}"
         assert np.isin(
             bin_names, data_columns
         ).all(), (
             f"bin_names[{bin_names}] not exist in input data columns[{data_columns}]"
         )
         self.bin_names = bin_names
         if label_name:
@@ -57,14 +64,16 @@
         else:
             self.label_name = ""
         self.bin_num = bin_num
         self.binning_method = binning_method
         self.chimerge_init_bins = chimerge_init_bins
         self.chimerge_target_bins = chimerge_target_bins
         self.chimerge_target_chi = chi2.ppf(1 - chimerge_target_pvalue, df=1)
+        # iv results
+        self.iv_results = []
 
     def _build_feature_bin(
         self, f_data: pd.DataFrame
     ) -> Tuple[List[np.ndarray], Union[np.ndarray, List[str]], np.ndarray]:
         '''
         split one feature column into {bin_num} bins.
 
@@ -177,30 +186,60 @@
                 raw_label[0], str
             ), f"only support str if dtype == np.obj, but got {type(raw_label[0])}"
             return np.array((raw_label == self.positive_label)).astype(np.float32)
         else:
             positive_value = float(self.positive_label)
             return np.array((raw_label == positive_value)).astype(np.float32)
 
+    def _build_iv_info_dict(
+        self,
+        f_name: str,
+        ivs: List[float],
+        else_iv: float,
+    ) -> Dict:
+        """
+        build iv info dict
+
+        Args:
+            f_name (str): feature name.
+            ivs (List[float]): bin ivs.
+            else_iv (float): else ivs.
+
+        Returns:
+            Dict:  with the following infomation:
+            {
+                "name": str, #feature name
+                "ivs": list[float], #iv values for each bins, not safe to share with workers in any case.
+                "else_iv": float, #iv for nan values, may share to with workers
+                "feature_iv": float, #sum of bin_ivs, safe to share with workers when bin num > 2.
+            }
+        """
+        ret = dict()
+        ret['name'] = f_name
+        ret['ivs'] = ivs
+        ret['else_iv'] = else_iv
+        ret['feature_iv'] = sum(ivs)
+        return ret
+
     def _build_report_dict(
         self,
-        woe_ivs: List[Tuple],
+        woes: List[float],
         f_name: str,
         split_points: Union[np.ndarray, List[str]],
-        else_woe_iv: Tuple,
+        else_woe: float,
         total_counts: List[int],
         else_counts: int,
     ) -> Dict:
         '''
         build report dict for one feature.
         Attributes:
-            woe_ivs: woe/iv values for each bins in feature.
+            woes: woe values for each bins in feature.
             f_name: feature name.
             split_points: see _build_feature_bin.
-            else_woe_iv: woe/iv for np.nan values in feature.
+            else_woe: woe for np.nan values in feature.
             total_counts: total samples in each bins.
             else_counts: total samples for np.nan values.
 
         Return:
             Dict report.
         '''
         ret = dict()
@@ -209,26 +248,23 @@
             ret['type'] = "string"
             ret['categories'] = split_points
         else:
             ret['type'] = "numeric"
             ret['split_points'] = list(split_points)
 
         ret['woes'] = list()
-        ret['ivs'] = list()
         ret['total_counts'] = list()
-        assert len(total_counts) == len(woe_ivs), (
-            f"len(total_counts) {len(total_counts)}," f" len(woe_ivs) {len(woe_ivs)}"
+        assert len(total_counts) == len(woes), (
+            f"len(total_counts) {len(total_counts)}," f" len(woes) {len(woes)}"
         )
-        for i in range(len(woe_ivs)):
+        for i in range(len(woes)):
             ret['total_counts'].append(total_counts[i])
-            ret['woes'].append(woe_ivs[i][0])
-            ret['ivs'].append(woe_ivs[i][1])
+            ret['woes'].append(woes[i])
 
-        ret['else_woe'] = else_woe_iv[0]
-        ret['else_iv'] = else_woe_iv[1]
+        ret['else_woe'] = else_woe
         ret['else_counts'] = else_counts
 
         return ret
 
     def _calc_bin_woe_iv(
         self, bin_total: int, bin_positives: int
     ) -> Tuple[float, float]:
@@ -260,186 +296,109 @@
             positive_distrib = bin_positives * 1.0 / total_positives
             negative_distrib = bin_negatives * 1.0 / total_negatives
 
         woe = math.log(positive_distrib / negative_distrib)
         iv = (positive_distrib - negative_distrib) * woe
         return (woe, iv)
 
+    def accumulate_iv_info(
+        self,
+        ivs: List[float],
+        bin_names: List[str],
+        else_ivs: List[float],
+        split_point_sizes: List[int],
+    ):
+        """accumulate iv info in results.
+
+        Args:
+            ivs (List[float]): bin ivs
+            bin_names (List[str]): bin names
+            else_iv (List[float]): nan iv.
+            split_point_sizes (List[int]): _description_
+
+        """
+        pos = 0
+        for f_idx in range(len(bin_names)):
+            f_bin_size = split_point_sizes[f_idx]
+            self.iv_results.append(
+                self._build_iv_info_dict(
+                    bin_names[f_idx],
+                    ivs[pos : pos + f_bin_size],
+                    else_ivs[f_idx],
+                )
+            )
+            pos += f_bin_size
+        return
+
     def _build_report(
         self,
-        woe_ivs: List[Tuple[float]],
+        woes: Tuple[float],
         split_points: List[Union[np.ndarray, List[str]]],
-        else_woe_ivs: List[Tuple],
+        else_woes: List[Tuple],
         total_counts: List[int],
         else_counts: List[int],
     ) -> Dict:
         '''
         Attributes:
-            woe_ivs: woe/iv values for all features' bins.
+            woes: woe values for all features' bins.
             split_points: see _build_feature_bin.
-            else_woe_iv: woe/iv values for all features' np.nan bin.
+            else_woe: woe values for all features' np.nan bin.
             total_counts: total samples all features' bins.
             else_counts: np.nan samples in all features.
 
         Return:
             Dict report
         '''
-        assert len(else_woe_ivs) == len(self.bin_names), (
-            f"len(else_woe_ivs) {len(else_woe_ivs)},"
+        assert len(else_woes) == len(self.bin_names), (
+            f"len(else_woes) {len(else_woes)},"
             f" len(self.bin_names) {len(self.bin_names)}"
         )
         assert len(split_points) == len(self.bin_names), (
             f"len(split_points) {len(split_points)},"
             f" len(self.bin_names) {len(self.bin_names)}"
         )
-        assert len(woe_ivs) == len(total_counts), (
-            f"len(woe_ivs) {len(woe_ivs)}," f" len(total_counts) {len(total_counts)}"
+        assert len(woes) == len(total_counts), (
+            f"len(woes) {len(woes)}," f" len(total_counts) {len(total_counts)}"
         )
-        assert len(else_woe_ivs) == len(else_counts), (
-            f"len(else_woe_ivs) {len(else_woe_ivs)},"
-            f" len(else_counts) {len(else_counts)}"
+        assert len(else_woes) == len(else_counts), (
+            f"len(else_woes) {len(else_woes)}," f" len(else_counts) {len(else_counts)}"
         )
         pos = 0
         variables = list()
         for f_idx in range(len(split_points)):
             split_point = split_points[f_idx]
             f_bin_size = 0
             if isinstance(split_point, list):
                 f_bin_size = len(split_point)
             else:
                 f_bin_size = split_point.size + 1
 
             assert pos + f_bin_size <= len(
-                woe_ivs
-            ), f"pos {pos}, f_bin_size {f_bin_size}, len(woe_ivs) {len(woe_ivs)}"
+                woes
+            ), f"pos {pos}, f_bin_size {f_bin_size}, len(woes) {len(woes)}"
             variables.append(
                 self._build_report_dict(
-                    woe_ivs[pos : pos + f_bin_size],
+                    woes[pos : pos + f_bin_size],
                     self.bin_names[f_idx],
                     split_points[f_idx],
-                    else_woe_ivs[f_idx],
+                    else_woes[f_idx],
                     total_counts[pos : pos + f_bin_size],
                     else_counts[f_idx],
                 )
             )
             pos += f_bin_size
 
-        assert pos == len(woe_ivs), f"pos {pos}, len(woe_ivs) {len(woe_ivs)}"
+        assert pos == len(woes), f"pos {pos}, len(woes) {len(woes)}"
         assert len(variables) == len(self.bin_names), (
             f"len(variables) {len(variables)}, "
             f"len(self.bin_names) {len(self.bin_names)}"
         )
         return {"variables": variables}
 
-    def _chi_merge(
-        self, bins: List[Tuple[float, float]]
-    ) -> Tuple[List[Tuple[float, float]], List[int]]:
-        '''
-        apply ChiMerge on one feature. ChiMerge proposed by paper AAAI92-019.
-        merge adjacent bins by their samples' Chi-Square Statistic.
-        Attributes:
-            bins: bins in feature build by initialization cut.
-
-        Return:
-            Tuple[bins after merge, removed bin indices in input bins]
-        '''
-
-        def get_chi(bin1: Tuple[float, float], bin2: Tuple[float, float]):
-            total = bin1[0] + bin2[0]
-            total_positive = bin1[1] + bin2[1]
-            positive_rate = float(total_positive) / float(total)
-
-            if positive_rate == 0 or positive_rate == 1:
-                # two bins has same label distribution
-                return 0.0
-
-            bin1_positive = bin1[1]
-            bin1_expt_positive = positive_rate * float(bin1[0])
-            bin1_negative = bin1[0] - bin1[1]
-            bin1_expt_negative = float(bin1[0]) - bin1_expt_positive
-
-            bin2_positive = bin2[1]
-            bin2_expt_positive = positive_rate * float(bin2[0])
-            bin2_negative = bin2[0] - bin2[1]
-            bin2_expt_negative = float(bin2[0]) - bin2_expt_positive
-
-            return (
-                math.pow(bin1_positive - bin1_expt_positive, 2) / bin1_expt_positive
-                + math.pow(bin1_negative - bin1_expt_negative, 2) / bin1_expt_negative
-                + math.pow(bin2_positive - bin2_expt_positive, 2) / bin2_expt_positive
-                + math.pow(bin2_negative - bin2_expt_negative, 2) / bin2_expt_negative
-            )
-
-        chis = [get_chi(bins[i], bins[i + 1]) for i in range(len(bins) - 1)]
-
-        def get_min(chis):
-            min_idx = np.argmin(chis)
-            return chis[min_idx], min_idx
-
-        orig_idx = [i for i in range(len(bins))]
-        removed_idx = list()
-        while True:
-            if len(bins) <= self.chimerge_target_bins:
-                # chi_merge stop by bin size
-                return bins, removed_idx
-
-            min_chi, min_idx = get_min(chis)
-            if min_chi > self.chimerge_target_chi:
-                # chi_merge stop by chi value3333333
-                return bins, removed_idx
-
-            # merge bins[min_idx] & bins[min_idx + 1]
-            new_stat = (
-                bins[min_idx][0] + bins[min_idx + 1][0],
-                bins[min_idx][1] + bins[min_idx + 1][1],
-            )
-            bins.pop(min_idx + 1)
-            bins[min_idx] = new_stat
-            removed_idx.append(orig_idx.pop(min_idx))
-            # update chis
-            chis.pop(min_idx)
-            if min_idx > 0:
-                chis[min_idx - 1] = get_chi(bins[min_idx - 1], bins[min_idx])
-            if min_idx < len(bins) - 1:
-                chis[min_idx] = get_chi(bins[min_idx], bins[min_idx + 1])
-
-    def _apply_chimerge(
-        self,
-        bins_stat: List[Tuple[float, float]],
-        split_points: List[Union[np.ndarray, List[str]]],
-    ) -> Tuple[List[Tuple[float, float]], List[Union[np.ndarray, List[str]]]]:
-        '''
-        apply ChiMerge on all number type features.
-        Attributes:
-            bins_stat: bins for all features build by initialization cut.
-            split_points: see _build_feature_bin
-
-        Return:
-            Tuple[bins after merge, split points after merge]
-        '''
-        pos = 0
-        merged_bins_stat = list()
-        merged_split_points = list()
-        for f_idx in range(len(split_points)):
-            if isinstance(split_points[f_idx], list):
-                # can not apple chimerge on string type feature. skip and forward values into result.
-                f_size = len(split_points[f_idx])
-                merged_bins_stat += bins_stat[pos : pos + f_size]
-                merged_split_points.append(split_points[f_idx])
-                pos += f_size
-            else:
-                f_size = split_points[f_idx].size + 1
-                mbs, merged_idx = self._chi_merge(bins_stat[pos : pos + f_size])
-                merged_split_points.append(np.delete(split_points[f_idx], merged_idx))
-                merged_bins_stat += mbs
-                pos += f_size
-
-        return merged_bins_stat, merged_split_points
-
-    def coordinator_work(self, data: pd.DataFrame) -> Tuple[np.ndarray, Dict]:
+    def label_holder_work(self, data: pd.DataFrame) -> Tuple[np.ndarray, Dict]:
         '''
         Label holder build report for it's own feature, and provide label to driver.
         Attributes:
             data: full dataset for this party.
 
         Return:
             Tuple[label, report for this party]
@@ -456,26 +415,42 @@
             total_count = bin.size
             positive_count = round(label[bin].sum())
             return (total_count, positive_count)
 
         bins_stat = [sum_bin(b) for b in bins_idx]
 
         if self.binning_method == "chimerge":
-            bins_stat, split_points = self._apply_chimerge(bins_stat, split_points)
+            bins_stat, merged_split_point_indices = apply_chimerge(
+                bins_stat,
+                self.is_string_features(split_points),
+                self.get_split_points_sizes(split_points),
+                self.chimerge_target_bins,
+                self.chimerge_target_chi,
+            )
+            split_points = update_split_points(
+                split_points,
+                merged_split_point_indices,
+                self.is_string_features(split_points),
+            )
 
-        woe_ivs = [self._calc_bin_woe_iv(*s) for s in bins_stat]
+        woes, bin_ivs = tuple(zip(*[self._calc_bin_woe_iv(*b) for b in bins_stat]))
         total_counts = [b[0] for b in bins_stat]
 
-        else_woe_ivs = [self._calc_bin_woe_iv(*sum_bin(b)) for b in else_bins]
+        else_woes, else_ivs = tuple(
+            zip(*[self._calc_bin_woe_iv(*sum_bin(b)) for b in else_bins])
+        )
         else_counts = [b.size for b in else_bins]
 
+        self.accumulate_iv_info(
+            bin_ivs, self.bin_names, else_ivs, self.get_split_points_sizes(split_points)
+        )
         return (
             label,
             self._build_report(
-                woe_ivs, split_points, else_woe_ivs, total_counts, else_counts
+                woes, split_points, else_woes, total_counts, else_counts
             ),
         )
 
     def participant_build_sum_indices(self, data: pd.DataFrame) -> List[List[int]]:
         '''
         build sum indices for driver to calculate positive samples by HE.
         Attributes:
@@ -512,96 +487,196 @@
             if else_bins_idx[i].size:
                 s = np.zeros((samples, 1), np.float32)
                 s[else_bins_idx[i]] = 1.0
                 else_select.append(s)
 
         return np.concatenate((select, *else_select), axis=1)
 
-    def participant_sum_bin(
-        self, bins_positive: Union[List, np.ndarray]
-    ) -> List[Tuple[int, int]]:
-        '''
-        build bins stat tuple.
-        Attributes:
-            bins_positive: positive counts in all not empty bins.
+    def _is_string_features(self):
+        return self.is_string_features(self.split_points)
 
-        Return:
-            List[Tuple[total, positive]]
-        '''
-        else_bin_count = len([x for x in self.else_counts if x > 0])
+    def is_string_features(self, split_points):
+        return [isinstance(sp, list) for sp in split_points]
+
+    def _get_split_points_sizes(self):
+        return self.get_split_points_sizes(self.split_points)
+
+    def get_split_points_sizes(self, split_points):
+        return [len(sp) if isinstance(sp, list) else sp.size + 1 for sp in split_points]
+
+    def get_bin_sum_info(self) -> 'ParticipantTransactionInfo':
+        return ParticipantTransactionInfo(
+            self.else_counts,
+            self.total_counts,
+            self.bin_names,
+            self.binning_method,
+            self._is_string_features(),
+            self._get_split_points_sizes(),
+            self.chimerge_target_bins,
+            self.chimerge_target_chi,
+        )
+
+    def label_holder_sum_bin(
+        self,
+        bins_positive: Union[List, np.ndarray],
+        bin_sum_info: 'ParticipantTransactionInfo',
+    ) -> Tuple[List[Tuple[int, int]], List[int], List[Union[None, int]]]:
+        """build bins stat tuple and information for participant to update
+
+        Args:
+            bins_positive (Union[List, np.ndarray]): number of positive samples in bins
+            bin_sum_info ParticipantTransactionInfo: information participant give to label_holder.
+        Returns:
+            List[Tuple[int, int]: bin stats
+            List[int]: updated total counts
+            List[Union[None, int]]]: merged indices for split points
+        """
+        else_bin_count = len([x for x in bin_sum_info.else_counts if x > 0])
         if len(bins_positive) == 1 and isinstance(bins_positive[0], np.ndarray):
             bins_positive = list(bins_positive[0])
         else:
             bins_positive = list(bins_positive)
 
         if else_bin_count:
             else_positive = bins_positive[-else_bin_count:]
             bins_positive = bins_positive[:-else_bin_count]
         else:
             else_positive = list()
 
-        assert len(bins_positive) == len(self.total_counts), (
+        assert len(bins_positive) == len(bin_sum_info.total_counts), (
             f"len(bins_positive) {len(bins_positive)}, "
-            f"len(self.total_counts) {len(self.total_counts)}"
+            f"len(total_counts) {len(bin_sum_info.total_counts)}"
         )
-
         bins_positive = [round(float(p)) for p in bins_positive]
-        bins_stat = [b for b in zip(self.total_counts, bins_positive)]
+        bins_stat = [b for b in zip(bin_sum_info.total_counts, bins_positive)]
+        total_counts = bin_sum_info.total_counts
+        merged_split_point_indices = None
+        if bin_sum_info.binning_method == "chimerge":
+            bins_stat, merged_split_point_indices = apply_chimerge(
+                bins_stat,
+                bin_sum_info.is_string_features,
+                bin_sum_info.split_points_sizes,
+                bin_sum_info.chimerge_target_bins,
+                bin_sum_info.chimerge_target_chi,
+            )
+            total_counts = [b[0] for b in bins_stat]
+
+        else_stats = self._label_holder_build_else_stats(
+            else_positive, bin_sum_info.bin_names, bin_sum_info.else_counts
+        )
+        bins_stat += else_stats
+
+        return bins_stat, total_counts, merged_split_point_indices
 
+    def participant_update_info(self, total_counts, merged_split_point_indices):
         if self.binning_method == "chimerge":
-            bins_stat, self.split_points = self._apply_chimerge(
-                bins_stat, self.split_points
+            self.total_counts = total_counts
+            self.split_points = update_split_points(
+                self.split_points,
+                merged_split_point_indices,
+                self._is_string_features(),
             )
-            self.total_counts = [b[0] for b in bins_stat]
 
-        assert len(self.bin_names) == len(self.else_counts), (
-            f"len(self.bin_names) {len(self.bin_names)}, "
-            f"len(self.else_counts) {len(self.else_counts)}"
+    def _label_holder_build_else_stats(self, else_positive, bin_names, else_counts):
+        assert len(bin_names) == len(else_counts), (
+            f"len(bin_names) {len(bin_names)}, " f"len(else_counts) {len(else_counts)}"
         )
 
         else_stat = list()
-        for i in range(len(self.else_counts)):
-            count = self.else_counts[i]
+        for i in range(len(else_counts)):
+            count = else_counts[i]
             if count > 0:
                 assert (
                     len(else_positive) > 0
                 ), f"len(else_positive) {len(else_positive)}"
                 p = else_positive.pop(0)
                 else_stat.append((count, round(float(p))))
             else:
                 else_stat.append((0, 0))
         assert len(else_positive) == 0, f"len(else_positive) {len(else_positive)}"
 
-        bins_stat += else_stat
+        return else_stat
 
-        return bins_stat
-
-    def coordinator_calc_woe_for_peer(
+    def label_holder_calc_woe_for_peer(
         self, bins_stat: List[Tuple[int, int]]
-    ) -> List[Tuple[float, float]]:
+    ) -> Tuple[Tuple[float], Tuple[float]]:
         '''
         calculate woe/iv for participant party.
         Attributes:
             bins_stat: bins stat tuple from participant party.
 
         Return:
-           List[Tuple[woe, iv]]
+           woes : woe for each bin
+           ivs : iv for each bin
         '''
-        return [self._calc_bin_woe_iv(*b) for b in bins_stat]
+        woe_iv = tuple(zip(*[self._calc_bin_woe_iv(*b) for b in bins_stat]))
+        # empty case
+        if len(woe_iv) != 2:
+            return [], []
+        woes, bin_ivs = woe_iv[0], woe_iv[1]
+        return woes, bin_ivs
+
+    def label_holder_collect_iv_for_participant(
+        self, ivs: Tuple[float], transaction_info: 'ParticipantTransactionInfo'
+    ):
+        f_count = len(transaction_info.bin_names)
+        self.accumulate_iv_info(
+            ivs[:-f_count],
+            transaction_info.bin_names,
+            ivs[-f_count:],
+            transaction_info.split_points_sizes,
+        )
+
+    def generate_iv_report(self, report_dict: Dict) -> Dict:
+        iv_results = copy.deepcopy(self.iv_results)
+        self.iv_results = []
+        report_dict["feature_iv_info"] = iv_results
+        return report_dict
 
-    def participant_build_report(self, woe_ivs: List[Tuple[float, float]]) -> Dict:
+    def participant_build_report(self, woes: Tuple[float]) -> Dict:
         '''
-        build report based on coordinator party's woe/iv values.
+        build report based on label_holder party's woe values.
         Attributes:
-            woe_ivs: woe/iv values for all features' bins.
+            woes: woe values for all features' bins.
 
         Return:
             Dict
         '''
         f_count = len(self.bin_names)
         return self._build_report(
-            woe_ivs[:-f_count],
+            woes[:-f_count],
             self.split_points,
-            woe_ivs[-f_count:],
+            woes[-f_count:],
             self.total_counts,
             self.else_counts,
         )
+
+
+@dataclass
+class ParticipantTransactionInfo:
+    """The information participant give to label_holder in order to calculate woe.
+
+    All these information are public any ways or can be inferred from public information,
+    except for total counts and else counts: these are revealed due to the approach of calculating woe,
+    and yet we consider them ok to give to label_holder.
+
+    Note that split point values are protected.
+
+
+    else_counts (List[int]): number of nan values in bins
+    total_counts (List[int]): total number of samples in bins
+    bin_names (List[str]): bin names
+    binning_method (str): binning method. 'chimerge' or else.
+    is_string_features (List[bool]): if features are string type
+    split_points_sizes (List[int]): size of split points
+    chimerge_target_bins (int): chimerge parameter: target bin num
+    chimerge_target_chi (float): chimerge parameter: chi
+    """
+
+    else_counts: List[int]
+    total_counts: List[int]
+    bin_names: List[str]
+    binning_method: str
+    is_string_features: List[bool]
+    split_points_sizes: List[int]
+    chimerge_target_bins: int
+    chimerge_target_chi: float
```

## secretflow/protos/component/cluster_pb2.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: secretflow/protos/component/cluster.proto
-"""Generated protocol buffer code."""
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
@@ -15,15 +15,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='secretflow/protos/component/cluster.proto',
   package='secretflow.component',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n)secretflow/protos/component/cluster.proto\x12\x14secretflow.component\"\xd4\x01\n\rSFClusterDesc\x12\x12\n\nsf_version\x18\x01 \x01(\t\x12\x12\n\npy_version\x18\x02 \x01(\t\x12\x0f\n\x07parties\x18\x03 \x03(\t\x12?\n\x07\x64\x65vices\x18\x04 \x03(\x0b\x32..secretflow.component.SFClusterDesc.DeviceDesc\x1aI\n\nDeviceDesc\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07parties\x18\x03 \x03(\t\x12\x0e\n\x06\x63onfig\x18\x04 \x01(\t\"`\n\x10SPUAddressConfig\x12\x0e\n\x06spu_id\x18\x01 \x01(\t\x12\x0f\n\x07parties\x18\x02 \x03(\t\x12\x11\n\taddresses\x18\x03 \x03(\t\x12\x18\n\x10listen_addresses\x18\x04 \x03(\t\">\n\x0fSFAddressConfig\x12\x11\n\taddresses\x18\x03 \x03(\t\x12\x18\n\x10listen_addresses\x18\x04 \x03(\t\"\x1b\n\rLocalFsConfig\x12\n\n\x02wd\x18\x01 \x01(\t\"T\n\rStorageConfig\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x35\n\x08local_fs\x18\x02 \x01(\x0b\x32#.secretflow.component.LocalFsConfig\"\xa1\x02\n\x0fSFClusterConfig\x12\x31\n\x04\x64\x65sc\x18\x01 \x01(\x0b\x32#.secretflow.component.SFClusterDesc\x12\x12\n\nself_party\x18\x02 \x01(\t\x12\x34\n\x07storage\x18\x03 \x01(\x0b\x32#.secretflow.component.StorageConfig\x12\x15\n\rray_head_addr\x18\x04 \x01(\t\x12;\n\x0csf_addresses\x18\x05 \x01(\x0b\x32%.secretflow.component.SFAddressConfig\x12=\n\rspu_addresses\x18\x06 \x03(\x0b\x32&.secretflow.component.SPUAddressConfigb\x06proto3'
+  serialized_pb=b'\n)secretflow/protos/component/cluster.proto\x12\x14secretflow.component\"\xd4\x01\n\rSFClusterDesc\x12\x12\n\nsf_version\x18\x01 \x01(\t\x12\x12\n\npy_version\x18\x02 \x01(\t\x12\x0f\n\x07parties\x18\x03 \x03(\t\x12?\n\x07\x64\x65vices\x18\x04 \x03(\x0b\x32..secretflow.component.SFClusterDesc.DeviceDesc\x1aI\n\nDeviceDesc\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07parties\x18\x03 \x03(\t\x12\x0e\n\x06\x63onfig\x18\x04 \x01(\t\"\x7f\n\rStorageConfig\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x43\n\x08local_fs\x18\x02 \x01(\x0b\x32\x31.secretflow.component.StorageConfig.LocalFSConfig\x1a\x1b\n\rLocalFSConfig\x12\n\n\x02wd\x18\x01 \x01(\t\"\x9e\x05\n\x0fSFClusterConfig\x12\x31\n\x04\x64\x65sc\x18\x01 \x01(\x0b\x32#.secretflow.component.SFClusterDesc\x12I\n\rpublic_config\x18\x02 \x01(\x0b\x32\x32.secretflow.component.SFClusterConfig.PublicConfig\x12K\n\x0eprivate_config\x18\x03 \x01(\x0b\x32\x33.secretflow.component.SFClusterConfig.PrivateConfig\x1aL\n\x0cRayFedConfig\x12\x0f\n\x07parties\x18\x01 \x03(\t\x12\x11\n\taddresses\x18\x02 \x03(\t\x12\x18\n\x10listen_addresses\x18\x03 \x03(\t\x1aW\n\tSPUConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07parties\x18\x02 \x03(\t\x12\x11\n\taddresses\x18\x03 \x03(\t\x12\x18\n\x10listen_addresses\x18\x04 \x03(\t\x1a\x9f\x01\n\x0cPublicConfig\x12I\n\rrayfed_config\x18\x01 \x01(\x0b\x32\x32.secretflow.component.SFClusterConfig.RayFedConfig\x12\x44\n\x0bspu_configs\x18\x02 \x03(\x0b\x32/.secretflow.component.SFClusterConfig.SPUConfig\x1aw\n\rPrivateConfig\x12\x12\n\nself_party\x18\x01 \x01(\t\x12\x15\n\rray_head_addr\x18\x02 \x01(\t\x12;\n\x0estorage_config\x18\x03 \x01(\x0b\x32#.secretflow.component.StorageConfigb\x06proto3'
 )
 
 
 
 
 _SFCLUSTERDESC_DEVICEDESC = _descriptor.Descriptor(
   name='DeviceDesc',
@@ -126,85 +126,109 @@
   oneofs=[
   ],
   serialized_start=68,
   serialized_end=280,
 )
 
 
-_SPUADDRESSCONFIG = _descriptor.Descriptor(
-  name='SPUAddressConfig',
-  full_name='secretflow.component.SPUAddressConfig',
+_STORAGECONFIG_LOCALFSCONFIG = _descriptor.Descriptor(
+  name='LocalFSConfig',
+  full_name='secretflow.component.StorageConfig.LocalFSConfig',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='spu_id', full_name='secretflow.component.SPUAddressConfig.spu_id', index=0,
+      name='wd', full_name='secretflow.component.StorageConfig.LocalFSConfig.wd', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=382,
+  serialized_end=409,
+)
+
+_STORAGECONFIG = _descriptor.Descriptor(
+  name='StorageConfig',
+  full_name='secretflow.component.StorageConfig',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='parties', full_name='secretflow.component.SPUAddressConfig.parties', index=1,
-      number=2, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='addresses', full_name='secretflow.component.SPUAddressConfig.addresses', index=2,
-      number=3, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
+      name='type', full_name='secretflow.component.StorageConfig.type', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='listen_addresses', full_name='secretflow.component.SPUAddressConfig.listen_addresses', index=3,
-      number=4, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
+      name='local_fs', full_name='secretflow.component.StorageConfig.local_fs', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_STORAGECONFIG_LOCALFSCONFIG, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=282,
-  serialized_end=378,
+  serialized_end=409,
 )
 
 
-_SFADDRESSCONFIG = _descriptor.Descriptor(
-  name='SFAddressConfig',
-  full_name='secretflow.component.SFAddressConfig',
+_SFCLUSTERCONFIG_RAYFEDCONFIG = _descriptor.Descriptor(
+  name='RayFedConfig',
+  full_name='secretflow.component.SFClusterConfig.RayFedConfig',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='addresses', full_name='secretflow.component.SFAddressConfig.addresses', index=0,
-      number=3, type=9, cpp_type=9, label=3,
+      name='parties', full_name='secretflow.component.SFClusterConfig.RayFedConfig.parties', index=0,
+      number=1, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='listen_addresses', full_name='secretflow.component.SFAddressConfig.listen_addresses', index=1,
-      number=4, type=9, cpp_type=9, label=3,
+      name='addresses', full_name='secretflow.component.SFClusterConfig.RayFedConfig.addresses', index=1,
+      number=2, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='listen_addresses', full_name='secretflow.component.SFClusterConfig.RayFedConfig.listen_addresses', index=2,
+      number=3, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -213,70 +237,89 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=380,
-  serialized_end=442,
+  serialized_start=634,
+  serialized_end=710,
 )
 
-
-_LOCALFSCONFIG = _descriptor.Descriptor(
-  name='LocalFsConfig',
-  full_name='secretflow.component.LocalFsConfig',
+_SFCLUSTERCONFIG_SPUCONFIG = _descriptor.Descriptor(
+  name='SPUConfig',
+  full_name='secretflow.component.SFClusterConfig.SPUConfig',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='wd', full_name='secretflow.component.LocalFsConfig.wd', index=0,
+      name='name', full_name='secretflow.component.SFClusterConfig.SPUConfig.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='parties', full_name='secretflow.component.SFClusterConfig.SPUConfig.parties', index=1,
+      number=2, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='addresses', full_name='secretflow.component.SFClusterConfig.SPUConfig.addresses', index=2,
+      number=3, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='listen_addresses', full_name='secretflow.component.SFClusterConfig.SPUConfig.listen_addresses', index=3,
+      number=4, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=444,
-  serialized_end=471,
+  serialized_start=712,
+  serialized_end=799,
 )
 
-
-_STORAGECONFIG = _descriptor.Descriptor(
-  name='StorageConfig',
-  full_name='secretflow.component.StorageConfig',
+_SFCLUSTERCONFIG_PUBLICCONFIG = _descriptor.Descriptor(
+  name='PublicConfig',
+  full_name='secretflow.component.SFClusterConfig.PublicConfig',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='type', full_name='secretflow.component.StorageConfig.type', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='rayfed_config', full_name='secretflow.component.SFClusterConfig.PublicConfig.rayfed_config', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='local_fs', full_name='secretflow.component.StorageConfig.local_fs', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='spu_configs', full_name='secretflow.component.SFClusterConfig.PublicConfig.spu_configs', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -284,96 +327,123 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=473,
-  serialized_end=557,
+  serialized_start=802,
+  serialized_end=961,
 )
 
-
-_SFCLUSTERCONFIG = _descriptor.Descriptor(
-  name='SFClusterConfig',
-  full_name='secretflow.component.SFClusterConfig',
+_SFCLUSTERCONFIG_PRIVATECONFIG = _descriptor.Descriptor(
+  name='PrivateConfig',
+  full_name='secretflow.component.SFClusterConfig.PrivateConfig',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='desc', full_name='secretflow.component.SFClusterConfig.desc', index=0,
-      number=1, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='self_party', full_name='secretflow.component.SFClusterConfig.PrivateConfig.self_party', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='self_party', full_name='secretflow.component.SFClusterConfig.self_party', index=1,
+      name='ray_head_addr', full_name='secretflow.component.SFClusterConfig.PrivateConfig.ray_head_addr', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='storage', full_name='secretflow.component.SFClusterConfig.storage', index=2,
+      name='storage_config', full_name='secretflow.component.SFClusterConfig.PrivateConfig.storage_config', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=963,
+  serialized_end=1082,
+)
+
+_SFCLUSTERCONFIG = _descriptor.Descriptor(
+  name='SFClusterConfig',
+  full_name='secretflow.component.SFClusterConfig',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='ray_head_addr', full_name='secretflow.component.SFClusterConfig.ray_head_addr', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='desc', full_name='secretflow.component.SFClusterConfig.desc', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='sf_addresses', full_name='secretflow.component.SFClusterConfig.sf_addresses', index=4,
-      number=5, type=11, cpp_type=10, label=1,
+      name='public_config', full_name='secretflow.component.SFClusterConfig.public_config', index=1,
+      number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='spu_addresses', full_name='secretflow.component.SFClusterConfig.spu_addresses', index=5,
-      number=6, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
+      name='private_config', full_name='secretflow.component.SFClusterConfig.private_config', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_SFCLUSTERCONFIG_RAYFEDCONFIG, _SFCLUSTERCONFIG_SPUCONFIG, _SFCLUSTERCONFIG_PUBLICCONFIG, _SFCLUSTERCONFIG_PRIVATECONFIG, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=560,
-  serialized_end=849,
+  serialized_start=412,
+  serialized_end=1082,
 )
 
 _SFCLUSTERDESC_DEVICEDESC.containing_type = _SFCLUSTERDESC
 _SFCLUSTERDESC.fields_by_name['devices'].message_type = _SFCLUSTERDESC_DEVICEDESC
-_STORAGECONFIG.fields_by_name['local_fs'].message_type = _LOCALFSCONFIG
+_STORAGECONFIG_LOCALFSCONFIG.containing_type = _STORAGECONFIG
+_STORAGECONFIG.fields_by_name['local_fs'].message_type = _STORAGECONFIG_LOCALFSCONFIG
+_SFCLUSTERCONFIG_RAYFEDCONFIG.containing_type = _SFCLUSTERCONFIG
+_SFCLUSTERCONFIG_SPUCONFIG.containing_type = _SFCLUSTERCONFIG
+_SFCLUSTERCONFIG_PUBLICCONFIG.fields_by_name['rayfed_config'].message_type = _SFCLUSTERCONFIG_RAYFEDCONFIG
+_SFCLUSTERCONFIG_PUBLICCONFIG.fields_by_name['spu_configs'].message_type = _SFCLUSTERCONFIG_SPUCONFIG
+_SFCLUSTERCONFIG_PUBLICCONFIG.containing_type = _SFCLUSTERCONFIG
+_SFCLUSTERCONFIG_PRIVATECONFIG.fields_by_name['storage_config'].message_type = _STORAGECONFIG
+_SFCLUSTERCONFIG_PRIVATECONFIG.containing_type = _SFCLUSTERCONFIG
 _SFCLUSTERCONFIG.fields_by_name['desc'].message_type = _SFCLUSTERDESC
-_SFCLUSTERCONFIG.fields_by_name['storage'].message_type = _STORAGECONFIG
-_SFCLUSTERCONFIG.fields_by_name['sf_addresses'].message_type = _SFADDRESSCONFIG
-_SFCLUSTERCONFIG.fields_by_name['spu_addresses'].message_type = _SPUADDRESSCONFIG
+_SFCLUSTERCONFIG.fields_by_name['public_config'].message_type = _SFCLUSTERCONFIG_PUBLICCONFIG
+_SFCLUSTERCONFIG.fields_by_name['private_config'].message_type = _SFCLUSTERCONFIG_PRIVATECONFIG
 DESCRIPTOR.message_types_by_name['SFClusterDesc'] = _SFCLUSTERDESC
-DESCRIPTOR.message_types_by_name['SPUAddressConfig'] = _SPUADDRESSCONFIG
-DESCRIPTOR.message_types_by_name['SFAddressConfig'] = _SFADDRESSCONFIG
-DESCRIPTOR.message_types_by_name['LocalFsConfig'] = _LOCALFSCONFIG
 DESCRIPTOR.message_types_by_name['StorageConfig'] = _STORAGECONFIG
 DESCRIPTOR.message_types_by_name['SFClusterConfig'] = _SFCLUSTERCONFIG
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 SFClusterDesc = _reflection.GeneratedProtocolMessageType('SFClusterDesc', (_message.Message,), {
 
   'DeviceDesc' : _reflection.GeneratedProtocolMessageType('DeviceDesc', (_message.Message,), {
@@ -385,44 +455,63 @@
   'DESCRIPTOR' : _SFCLUSTERDESC,
   '__module__' : 'secretflow.protos.component.cluster_pb2'
   # @@protoc_insertion_point(class_scope:secretflow.component.SFClusterDesc)
   })
 _sym_db.RegisterMessage(SFClusterDesc)
 _sym_db.RegisterMessage(SFClusterDesc.DeviceDesc)
 
-SPUAddressConfig = _reflection.GeneratedProtocolMessageType('SPUAddressConfig', (_message.Message,), {
-  'DESCRIPTOR' : _SPUADDRESSCONFIG,
-  '__module__' : 'secretflow.protos.component.cluster_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.SPUAddressConfig)
-  })
-_sym_db.RegisterMessage(SPUAddressConfig)
-
-SFAddressConfig = _reflection.GeneratedProtocolMessageType('SFAddressConfig', (_message.Message,), {
-  'DESCRIPTOR' : _SFADDRESSCONFIG,
-  '__module__' : 'secretflow.protos.component.cluster_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.SFAddressConfig)
-  })
-_sym_db.RegisterMessage(SFAddressConfig)
-
-LocalFsConfig = _reflection.GeneratedProtocolMessageType('LocalFsConfig', (_message.Message,), {
-  'DESCRIPTOR' : _LOCALFSCONFIG,
-  '__module__' : 'secretflow.protos.component.cluster_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.LocalFsConfig)
-  })
-_sym_db.RegisterMessage(LocalFsConfig)
-
 StorageConfig = _reflection.GeneratedProtocolMessageType('StorageConfig', (_message.Message,), {
+
+  'LocalFSConfig' : _reflection.GeneratedProtocolMessageType('LocalFSConfig', (_message.Message,), {
+    'DESCRIPTOR' : _STORAGECONFIG_LOCALFSCONFIG,
+    '__module__' : 'secretflow.protos.component.cluster_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.StorageConfig.LocalFSConfig)
+    })
+  ,
   'DESCRIPTOR' : _STORAGECONFIG,
   '__module__' : 'secretflow.protos.component.cluster_pb2'
   # @@protoc_insertion_point(class_scope:secretflow.component.StorageConfig)
   })
 _sym_db.RegisterMessage(StorageConfig)
+_sym_db.RegisterMessage(StorageConfig.LocalFSConfig)
 
 SFClusterConfig = _reflection.GeneratedProtocolMessageType('SFClusterConfig', (_message.Message,), {
+
+  'RayFedConfig' : _reflection.GeneratedProtocolMessageType('RayFedConfig', (_message.Message,), {
+    'DESCRIPTOR' : _SFCLUSTERCONFIG_RAYFEDCONFIG,
+    '__module__' : 'secretflow.protos.component.cluster_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.SFClusterConfig.RayFedConfig)
+    })
+  ,
+
+  'SPUConfig' : _reflection.GeneratedProtocolMessageType('SPUConfig', (_message.Message,), {
+    'DESCRIPTOR' : _SFCLUSTERCONFIG_SPUCONFIG,
+    '__module__' : 'secretflow.protos.component.cluster_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.SFClusterConfig.SPUConfig)
+    })
+  ,
+
+  'PublicConfig' : _reflection.GeneratedProtocolMessageType('PublicConfig', (_message.Message,), {
+    'DESCRIPTOR' : _SFCLUSTERCONFIG_PUBLICCONFIG,
+    '__module__' : 'secretflow.protos.component.cluster_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.SFClusterConfig.PublicConfig)
+    })
+  ,
+
+  'PrivateConfig' : _reflection.GeneratedProtocolMessageType('PrivateConfig', (_message.Message,), {
+    'DESCRIPTOR' : _SFCLUSTERCONFIG_PRIVATECONFIG,
+    '__module__' : 'secretflow.protos.component.cluster_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.SFClusterConfig.PrivateConfig)
+    })
+  ,
   'DESCRIPTOR' : _SFCLUSTERCONFIG,
   '__module__' : 'secretflow.protos.component.cluster_pb2'
   # @@protoc_insertion_point(class_scope:secretflow.component.SFClusterConfig)
   })
 _sym_db.RegisterMessage(SFClusterConfig)
+_sym_db.RegisterMessage(SFClusterConfig.RayFedConfig)
+_sym_db.RegisterMessage(SFClusterConfig.SPUConfig)
+_sym_db.RegisterMessage(SFClusterConfig.PublicConfig)
+_sym_db.RegisterMessage(SFClusterConfig.PrivateConfig)
 
 
 # @@protoc_insertion_point(module_scope)
```

## secretflow/protos/component/evaluation_pb2.py

```diff
@@ -1,145 +1,91 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: secretflow/protos/component/evaluation.proto
-"""Generated protocol buffer code."""
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from secretflow.protos.component import comp_def_pb2 as secretflow_dot_protos_dot_component_dot_comp__def__pb2
-from secretflow.protos.component import data_def_pb2 as secretflow_dot_protos_dot_component_dot_data__def__pb2
-from secretflow.protos.component import cluster_pb2 as secretflow_dot_protos_dot_component_dot_cluster__pb2
+from secretflow.protos.component import comp_pb2 as secretflow_dot_protos_dot_component_dot_comp__pb2
+from secretflow.protos.component import data_pb2 as secretflow_dot_protos_dot_component_dot_data__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='secretflow/protos/component/evaluation.proto',
   package='secretflow.component',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n,secretflow/protos/component/evaluation.proto\x12\x14secretflow.component\x1a*secretflow/protos/component/comp_def.proto\x1a*secretflow/protos/component/data_def.proto\x1a)secretflow/protos/component/cluster.proto\"{\n\tAttrValue\x12\x10\n\x08prefixes\x18\x01 \x03(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x35\n\x06\x61tomic\x18\x03 \x01(\x0b\x32%.secretflow.component.AtomicParameter\x12\x17\n\x0funion_selection\x18\x04 \x01(\t\"\xf9\x01\n\rNodeEvalParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x63omp_id\x18\x02 \x01(\t\x12.\n\x05\x61ttrs\x18\x03 \x03(\x0b\x32\x1f.secretflow.component.AttrValue\x12.\n\x06inputs\x18\x04 \x03(\x0b\x32\x1e.secretflow.component.DistData\x12\x14\n\x0coutput_names\x18\x05 \x03(\t\x12\x14\n\x0creport_names\x18\x06 \x03(\t\x12=\n\x0e\x63luster_config\x18\x07 \x01(\x0b\x32%.secretflow.component.SFClusterConfig\"r\n\x0eNodeEvalResult\x12/\n\x07outputs\x18\x01 \x03(\x0b\x32\x1e.secretflow.component.DistData\x12/\n\x07reports\x18\x02 \x03(\x0b\x32\x1e.secretflow.component.DistDatab\x06proto3'
+  serialized_pb=b'\n,secretflow/protos/component/evaluation.proto\x12\x14secretflow.component\x1a&secretflow/protos/component/comp.proto\x1a&secretflow/protos/component/data.proto\"\xc7\x01\n\rNodeEvalParam\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x12\n\nattr_paths\x18\x04 \x03(\t\x12.\n\x05\x61ttrs\x18\x05 \x03(\x0b\x32\x1f.secretflow.component.Attribute\x12.\n\x06inputs\x18\x06 \x03(\x0b\x32\x1e.secretflow.component.DistData\x12\x13\n\x0boutput_uris\x18\x07 \x03(\t\"A\n\x0eNodeEvalResult\x12/\n\x07outputs\x18\x01 \x03(\x0b\x32\x1e.secretflow.component.DistDatab\x06proto3'
   ,
-  dependencies=[secretflow_dot_protos_dot_component_dot_comp__def__pb2.DESCRIPTOR,secretflow_dot_protos_dot_component_dot_data__def__pb2.DESCRIPTOR,secretflow_dot_protos_dot_component_dot_cluster__pb2.DESCRIPTOR,])
-
+  dependencies=[secretflow_dot_protos_dot_component_dot_comp__pb2.DESCRIPTOR,secretflow_dot_protos_dot_component_dot_data__pb2.DESCRIPTOR,])
 
 
 
-_ATTRVALUE = _descriptor.Descriptor(
-  name='AttrValue',
-  full_name='secretflow.component.AttrValue',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='prefixes', full_name='secretflow.component.AttrValue.prefixes', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.AttrValue.name', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='atomic', full_name='secretflow.component.AttrValue.atomic', index=2,
-      number=3, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='union_selection', full_name='secretflow.component.AttrValue.union_selection', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=201,
-  serialized_end=324,
-)
-
 
 _NODEEVALPARAM = _descriptor.Descriptor(
   name='NodeEvalParam',
   full_name='secretflow.component.NodeEvalParam',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.NodeEvalParam.name', index=0,
+      name='domain', full_name='secretflow.component.NodeEvalParam.domain', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='comp_id', full_name='secretflow.component.NodeEvalParam.comp_id', index=1,
+      name='name', full_name='secretflow.component.NodeEvalParam.name', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='attrs', full_name='secretflow.component.NodeEvalParam.attrs', index=2,
-      number=3, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
+      name='version', full_name='secretflow.component.NodeEvalParam.version', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='inputs', full_name='secretflow.component.NodeEvalParam.inputs', index=3,
-      number=4, type=11, cpp_type=10, label=3,
+      name='attr_paths', full_name='secretflow.component.NodeEvalParam.attr_paths', index=3,
+      number=4, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='output_names', full_name='secretflow.component.NodeEvalParam.output_names', index=4,
-      number=5, type=9, cpp_type=9, label=3,
+      name='attrs', full_name='secretflow.component.NodeEvalParam.attrs', index=4,
+      number=5, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='report_names', full_name='secretflow.component.NodeEvalParam.report_names', index=5,
-      number=6, type=9, cpp_type=9, label=3,
+      name='inputs', full_name='secretflow.component.NodeEvalParam.inputs', index=5,
+      number=6, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='cluster_config', full_name='secretflow.component.NodeEvalParam.cluster_config', index=6,
-      number=7, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='output_uris', full_name='secretflow.component.NodeEvalParam.output_uris', index=6,
+      number=7, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -147,16 +93,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=327,
-  serialized_end=576,
+  serialized_start=151,
+  serialized_end=350,
 )
 
 
 _NODEEVALRESULT = _descriptor.Descriptor(
   name='NodeEvalResult',
   full_name='secretflow.component.NodeEvalResult',
   filename=None,
@@ -167,55 +113,37 @@
     _descriptor.FieldDescriptor(
       name='outputs', full_name='secretflow.component.NodeEvalResult.outputs', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='reports', full_name='secretflow.component.NodeEvalResult.reports', index=1,
-      number=2, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=578,
-  serialized_end=692,
+  serialized_start=352,
+  serialized_end=417,
 )
 
-_ATTRVALUE.fields_by_name['atomic'].message_type = secretflow_dot_protos_dot_component_dot_comp__def__pb2._ATOMICPARAMETER
-_NODEEVALPARAM.fields_by_name['attrs'].message_type = _ATTRVALUE
-_NODEEVALPARAM.fields_by_name['inputs'].message_type = secretflow_dot_protos_dot_component_dot_data__def__pb2._DISTDATA
-_NODEEVALPARAM.fields_by_name['cluster_config'].message_type = secretflow_dot_protos_dot_component_dot_cluster__pb2._SFCLUSTERCONFIG
-_NODEEVALRESULT.fields_by_name['outputs'].message_type = secretflow_dot_protos_dot_component_dot_data__def__pb2._DISTDATA
-_NODEEVALRESULT.fields_by_name['reports'].message_type = secretflow_dot_protos_dot_component_dot_data__def__pb2._DISTDATA
-DESCRIPTOR.message_types_by_name['AttrValue'] = _ATTRVALUE
+_NODEEVALPARAM.fields_by_name['attrs'].message_type = secretflow_dot_protos_dot_component_dot_comp__pb2._ATTRIBUTE
+_NODEEVALPARAM.fields_by_name['inputs'].message_type = secretflow_dot_protos_dot_component_dot_data__pb2._DISTDATA
+_NODEEVALRESULT.fields_by_name['outputs'].message_type = secretflow_dot_protos_dot_component_dot_data__pb2._DISTDATA
 DESCRIPTOR.message_types_by_name['NodeEvalParam'] = _NODEEVALPARAM
 DESCRIPTOR.message_types_by_name['NodeEvalResult'] = _NODEEVALRESULT
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-AttrValue = _reflection.GeneratedProtocolMessageType('AttrValue', (_message.Message,), {
-  'DESCRIPTOR' : _ATTRVALUE,
-  '__module__' : 'secretflow.protos.component.evaluation_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.AttrValue)
-  })
-_sym_db.RegisterMessage(AttrValue)
-
 NodeEvalParam = _reflection.GeneratedProtocolMessageType('NodeEvalParam', (_message.Message,), {
   'DESCRIPTOR' : _NODEEVALPARAM,
   '__module__' : 'secretflow.protos.component.evaluation_pb2'
   # @@protoc_insertion_point(class_scope:secretflow.component.NodeEvalParam)
   })
 _sym_db.RegisterMessage(NodeEvalParam)
```

## secretflow/security/aggregation/plain_aggregator.py

```diff
@@ -56,14 +56,15 @@
     @staticmethod
     def _get_dtype(arr):
         if isinstance(arr, np.ndarray):
             return arr.dtype
         else:
             try:
                 import tensorflow as tf
+
                 if isinstance(arr, tf.Tensor):
                     return arr.numpy().dtype
             except ImportError:
                 return None
 
     def sum(self, data: List[DeviceObject], axis=None) -> PYUObject:
         """Sum of array elements over a given axis.
```

## secretflow/security/privacy/__init__.py

```diff
@@ -8,20 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .mechanism.tensorflow.layers import GaussianEmbeddingDP, LabelDP
-from .mechanism.tensorflow.mechanism_fl import GaussianModelDP
-from .strategy import DPStrategy
-from .strategy_fl import DPStrategyFL
+from secretflow.security.privacy.mechanism.mechanism_fl import GaussianModelDP
+from secretflow.security.privacy.strategy import DPStrategy
+from secretflow.security.privacy.strategy_fl import DPStrategyFL
+from secretflow.security.privacy.mechanism.label_dp import LabelDP
 
 __all__ = [
-    'GaussianEmbeddingDP',
     'GaussianModelDP',
-    'LabelDP',
-    'GaussianModelGsDP',
     'DPStrategy',
     'DPStrategyFL',
+    'LabelDP',
 ]
```

## secretflow/security/privacy/strategy.py

```diff
@@ -7,22 +7,28 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from secretflow.security.privacy.mechanism.tensorflow.layers import EmbeddingDP, LabelDP
+from typing import Union
+from secretflow.security.privacy.mechanism.tensorflow.layers import (
+    GaussianEmbeddingDP as tf_embedding_dp,
+)
+from secretflow.security.privacy.mechanism.torch.layers import (
+    GaussianEmbeddingDP as torch_embedding_dp,
+)
+from secretflow.security.privacy.mechanism.label_dp import LabelDP
 
 
 class DPStrategy:
     def __init__(
         self,
-        embedding_dp: EmbeddingDP = None,
+        embedding_dp: Union[tf_embedding_dp, torch_embedding_dp] = None,
         label_dp: LabelDP = None,
         accountant_type='rdp',
         sampling_type=None,
     ):
         """
         Args:
             embedding_dp: Embedding dp layer.
```

## secretflow/security/privacy/strategy_fl.py

```diff
@@ -8,17 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from secretflow.security.privacy.mechanism.tensorflow.mechanism_fl import (
-    GaussianModelDP,
-)
+from secretflow.security.privacy.mechanism.mechanism_fl import GaussianModelDP
 
 
 class DPStrategyFL:
     def __init__(
         self,
         model_gdp: GaussianModelDP = None,
         accountant_type='rdp',
```

## secretflow/security/privacy/mechanism/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Ant Group Co., Ltd.
+# Copyright 2023 Ant Group Co., Ltd.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
```

## secretflow/security/privacy/mechanism/tensorflow/__init__.py

```diff
@@ -7,7 +7,13 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from .layers import GaussianEmbeddingDP
+
+__all__ = [
+    'GaussianEmbeddingDP',
+]
```

## secretflow/security/privacy/mechanism/tensorflow/layers.py

```diff
@@ -8,41 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from abc import ABC, abstractmethod
-from typing import List
-
-import numpy as np
 import tensorflow as tf
 
-from secretflow.security.privacy.accounting.gdp_accountant import (
-    cal_mu_poisson,
-    cal_mu_uniform,
-    get_eps_from_mu,
-)
-from secretflow.security.privacy.accounting.rdp_accountant import (
-    get_privacy_spent_rdp,
-    get_rdp,
-)
-
-
-class EmbeddingDP(tf.keras.layers.Layer, ABC):
-    def __init__(self) -> None:
-        super().__init__()
-
-    @abstractmethod
-    def call(self, inputs):
-        pass
+from secretflow.security.privacy.accounting.budget_accountant import BudgetAccountant
 
 
-class GaussianEmbeddingDP(EmbeddingDP):
+class GaussianEmbeddingDP(BudgetAccountant, tf.keras.layers.Layer):
     """Embedding differential privacy perturbation using gaussian noise"""
 
     def __init__(
         self,
         noise_multiplier: float,
         batch_size: int,
         num_samples: int,
@@ -90,95 +69,7 @@
             )
         else:
             noise = tf.random.normal(
                 inputs.shape, stddev=self.noise_multiplier * self.l2_norm_clip
             )
 
         return tf.add(embed_clipped, noise)
-
-    def privacy_spent_rdp(self, step: int, orders: List = None):
-        """Get accountant using RDP.
-
-        Args:
-            step: The current step of model training or prediction.
-            orders: An array (or a scalar) of RDP orders.
-        """
-
-        if orders is None:
-            orders = [1 + x / 10.0 for x in range(1, 100)] + list(range(12, 64))
-
-        q = self.batch_size / self.num_samples
-        rdp = get_rdp(q, self.noise_multiplier, step, orders)
-        eps, _, opt_order = get_privacy_spent_rdp(orders, rdp, target_delta=self.delta)
-        return eps, self.delta, opt_order
-
-    def privacy_spent_gdp(
-        self,
-        step: int,
-        sampling_type: str,
-    ):
-        """Get accountant using GDP.
-
-        Args:
-            step: The current step of model training or prediction.
-            sampling_type: Sampling type, which must be "poisson" or "uniform".
-        """
-
-        if sampling_type == 'poisson':
-            mu_ideal = cal_mu_poisson(
-                step, self.noise_multiplier, self.num_samples, self.batch_size
-            )
-        elif sampling_type == 'uniform':
-            mu_ideal = cal_mu_uniform(
-                step, self.noise_multiplier, self.num_samples, self.batch_size
-            )
-        else:
-            raise ValueError('the sampling_type must be "poisson" or "uniform".')
-
-        eps = get_eps_from_mu(mu_ideal, self.delta)
-        return eps, self.delta
-
-
-class LabelDP:
-    """Label differential privacy perturbation"""
-
-    def __init__(self, eps: float) -> None:
-        """
-        Args:
-            eps: epsilon for pure DP.
-        """
-        self._eps = eps
-
-    def __call__(self, inputs: np.ndarray):
-        """Random Response. Except for binary classification, inputs only support onehot form.
-
-        Args:
-            inputs: the label.
-        """
-        if not np.sum((inputs == 0) + (inputs == 1)) == inputs.size:
-            raise ValueError(
-                'Except for binary classification, inputs only support onehot form.'
-            )
-
-        if inputs.ndim == 1:
-            p_ori = np.exp(self._eps) / (np.exp(self._eps) + 1)
-            choice_ori = np.random.binomial(1, p_ori, size=inputs.shape[0])
-            outputs = np.abs(1 - choice_ori - inputs)
-        elif inputs.ndim == 2:
-            p_ori = np.exp(self._eps) / (np.exp(self._eps) + inputs.shape[-1] - 1)
-            p_oth = (1 - p_ori) / (inputs.shape[-1] - 1)
-            p_array = inputs * (p_ori - p_oth) + np.ones(inputs.shape) * p_oth
-            index_rr = np.array(
-                [
-                    np.random.choice(inputs.shape[-1], p=p_array[i])
-                    for i in range(inputs.shape[0])
-                ]
-            )
-            outputs = np.eye(inputs.shape[-1])[index_rr]
-        else:
-            raise ValueError('the dim of inputs in LabelDP must be less than 2.')
-
-        # TODO(@yushi): Support regression.
-        return outputs
-
-    def privacy_spent(self):
-        return self._eps
```

## secretflow/stats/pva_eval.py

```diff
@@ -22,15 +22,17 @@
 
 from .core import pva
 
 
 def pva_eval(
     actual: Union[FedNdarray, VDataFrame],
     prediction: Union[FedNdarray, VDataFrame],
-    target,
+    target: float,
+    rtol: float = 1e-05,
+    atol: float = 1e-08,
 ) -> PYUObject:
     """Compute Prediction Vs Actual score.
 
     Args:
         actual: Union[FedNdarray, VDataFrame]
 
         prediction: Union[FedNdarray, VDataFrame]
@@ -74,8 +76,8 @@
         actual = ([*actual.partitions.values()][0]).data
 
     if isinstance(prediction, FedNdarray):
         prediction = [*prediction.partitions.values()][0]
     else:
         prediction = ([*prediction.partitions.values()][0]).data
 
-    return device(pva)(actual, prediction, target)
+    return device(pva)(actual, prediction, target, rtol, atol)
```

## secretflow/stats/table_statistics.py

```diff
@@ -37,48 +37,48 @@
             sum_2 means sum(X^2).
     """
     assert isinstance(
         table, (pd.DataFrame, VDataFrame)
     ), "table must be a pd.DataFrame or VDataFrame"
     index = table.columns
     result = pd.DataFrame(index=index)
-    result['datatype'] = table.dtypes
-    result['total_count'] = table.shape[0]
-    result['count'] = table.count()
-    result['count_na'] = table.isna().sum()
-    result['min'] = table.min(numeric_only=True)
-    result['max'] = table.max(numeric_only=True)
-    result['mean'] = table.mean(numeric_only=True)
-    result['var'] = table.var(numeric_only=True)
-    result['std'] = table.std(numeric_only=True)
-    result['sem'] = table.sem(numeric_only=True)
-    result['skew'] = table.skew(numeric_only=True)
-    result['kurtosis'] = table.kurtosis(numeric_only=True)
-    result['q1'] = table.quantile(0.25)
-    result['q2'] = table.quantile(0.5)
-    result['q3'] = table.quantile(0.75)
-    result['moment_2'] = table.select_dtypes('number').pow(2).mean(numeric_only=True)
-    result['moment_3'] = table.select_dtypes('number').pow(3).mean(numeric_only=True)
-    result['moment_4'] = table.select_dtypes('number').pow(4).mean(numeric_only=True)
-    result['central_moment_2'] = (
-        table.subtract(result['mean'])
-        .select_dtypes('number')
+    result["datatype"] = table.dtypes
+    result["total_count"] = table.shape[0]
+    result["count"] = table.count()
+    result["count_na"] = table.isna().sum()
+    result["min"] = table.min(numeric_only=True)
+    result["max"] = table.max(numeric_only=True)
+    result["mean"] = table.mean(numeric_only=True)
+    result["var"] = table.var(numeric_only=True)
+    result["std"] = table.std(numeric_only=True)
+    result["sem"] = table.sem(numeric_only=True)
+    result["skew"] = table.skew(numeric_only=True)
+    result["kurtosis"] = table.kurtosis(numeric_only=True)
+    result["q1"] = table.quantile(0.25)
+    result["q2"] = table.quantile(0.5)
+    result["q3"] = table.quantile(0.75)
+    result["moment_2"] = table.select_dtypes("number").pow(2).mean(numeric_only=True)
+    result["moment_3"] = table.select_dtypes("number").pow(3).mean(numeric_only=True)
+    result["moment_4"] = table.select_dtypes("number").pow(4).mean(numeric_only=True)
+    result["central_moment_2"] = (
+        table.subtract(result["mean"])
+        .select_dtypes("number")
         .pow(2)
         .mean(numeric_only=True)
     )
-    result['central_moment_3'] = (
-        table.subtract(result['mean'])
-        .select_dtypes('number')
+    result["central_moment_3"] = (
+        table.subtract(result["mean"])
+        .select_dtypes("number")
         .pow(3)
         .mean(numeric_only=True)
     )
-    result['central_moment_4'] = (
-        table.subtract(result['mean'])
-        .select_dtypes('number')
+    result["central_moment_4"] = (
+        table.subtract(result["mean"])
+        .select_dtypes("number")
         .pow(4)
         .mean(numeric_only=True)
     )
-    result['sum'] = table.sum(numeric_only=True)
-    result['sum_2'] = table.select_dtypes('number').pow(2).sum(numeric_only=True)
-    result['sum_3'] = table.select_dtypes('number').pow(3).sum(numeric_only=True)
-    result['sum_4'] = table.select_dtypes('number').pow(4).sum(numeric_only=True)
+    result["sum"] = table.sum(numeric_only=True)
+    result["sum_2"] = table.select_dtypes("number").pow(2).sum(numeric_only=True)
+    result["sum_3"] = table.select_dtypes("number").pow(3).sum(numeric_only=True)
+    result["sum_4"] = table.select_dtypes("number").pow(4).sum(numeric_only=True)
     return result
```

## secretflow/stats/core/biclassification_eval_core.py

```diff
@@ -44,17 +44,15 @@
         eq_range_result_arr_list,
         summary_report_arr,
         head_prs,
     ):
         self.eq_frequent_bin_report = [
             EqBinReport(a) for a in eq_frequent_result_arr_list
         ]
-        self.eq_range_bin_report = [
-            EqBinReport(a) for a in eq_range_result_arr_list
-        ]
+        self.eq_range_bin_report = [EqBinReport(a) for a in eq_range_result_arr_list]
         self.summary_report = SummaryReport(summary_report_arr)
         self.head_report = [PrReport(a) for a in head_prs]
 
 
 class PrReport:
     """Precision Related statistics Report.
 
@@ -163,15 +161,15 @@
         self.negative = arr[3]
         self.total = arr[4]
         self.precision = arr[5]
         self.recall = arr[6]
         self.false_positive_rate = arr[7]
         self.f1_score = arr[8]
         self.Lift = arr[9]
-        self.predicted_negative_ratio = arr[10]
+        self.predicted_positive_ratio = arr[10]
         self.predicted_negative_ratio = arr[11]
         self.cumulative_percent_of_positive = arr[12]
         self.cumulative_percent_of_negative = arr[13]
         self.total_cumulative_percent = arr[14]
         self.ks = arr[15]
         self.avg_score = arr[16]
```

## secretflow/stats/core/pva_core.py

```diff
@@ -19,15 +19,17 @@
 import jax.numpy as jnp
 import pandas as pd
 
 
 def pva(
     actual: Union[pd.DataFrame, jnp.array],
     prediction: Union[pd.DataFrame, jnp.array],
-    target,
+    target: float,
+    rtol: float = 1e-05,
+    atol: float = 1e-08,
 ):
     """Compute Prediction Vs Actual score.
 
     Args:
         actual: Union[pd.DataFrame, jnp.array]
 
         prediction: Union[pd.DataFrame, jnp.array]
@@ -44,9 +46,9 @@
     if isinstance(prediction, pd.DataFrame):
         prediction = prediction.to_numpy()
     assert actual.size > 1, "there must be at least one actual"
     assert (
         prediction.size == actual.size
     ), "there must be at equal number of actuals and predictions"
     score_p = jnp.mean(prediction)
-    score_a = jnp.sum(actual == target) / actual.size
+    score_a = jnp.sum(jnp.isclose(actual, target, rtol=rtol, atol=atol)) / actual.size
     return jnp.abs(score_p - score_a)
```

## secretflow/utils/compressor.py

```diff
@@ -11,17 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABC, abstractmethod
 from typing import Any, List, Union
 
+import jax.numpy as jnp
 import numpy as np
 from scipy import sparse
 
+from secretflow.utils.communicate import ForwardData
+
 
 class Compressor(ABC):
     """Abstract base class for cross device data compressor"""
 
     @abstractmethod
     def compress(
         self, data: Union[np.ndarray, List[np.ndarray]]
@@ -86,54 +89,75 @@
             sparse.spmatrix: compressed sparse matrix.
         """
         raise NotImplementedError()
 
     # sample random element from original List[np.ndarray]
     def compress(
         self,
-        data: Union[np.ndarray, List[np.ndarray]],
+        data: Union[ForwardData, np.ndarray, List[np.ndarray]],
     ) -> Union[sparse.spmatrix, List[sparse.spmatrix]]:
         """Compress data to sparse matrix before send.
 
         Args:
             data (Union[np.ndarray, List[np.ndarray]]): data need to compress.
 
         Returns:
             Union[sparse.spmatrix, List[sparse.spmatrix]]: compressed data.
         """
         # there is no need for sparsification in evaluate/predict.
         is_list = True
-        if isinstance(data, np.ndarray):
+
+        if isinstance(data, ForwardData):
+            hidden = data.hidden
+        else:
+            hidden = data
+
+        if isinstance(hidden, (np.ndarray, jnp.ndarray)):
             is_list = False
-            data = [data]
-        elif not isinstance(data, (list, tuple)):
-            assert False, f'invalid data: {type(data)}'
-        out = list(map(lambda d: self._compress_one(d), data))
-        return out if is_list else out[0]
+            hidden = [hidden]
+        elif not isinstance(hidden, (list, tuple)):
+            assert False, f'invalid data: {type(hidden)}'
+        out = list(map(lambda d: self._compress_one(d), hidden))
+        out = out if is_list else out[0]
+        if isinstance(data, ForwardData):
+            data.hidden = out
+        else:
+            data = out
+        return data
 
     def decompress(
-        self, data: Union[sparse.spmatrix, List[sparse.spmatrix]]
+        self, data: Union[ForwardData, sparse.spmatrix, List[sparse.spmatrix]]
     ) -> Union[np.ndarray, List[np.ndarray]]:
         """Decompress data from sparse matrix to dense after received.
 
         Args:
             data (Union[sparse.spmatrix, List[sparse.spmatrix]]): data need to decompress.
 
         Returns:
             Union[np.ndarray, List[np.ndarray]]: decompressed data.
         """
         # there is no need for sparsification in evaluate/predict.
         is_list = True
-        if sparse.issparse(data):
+        if isinstance(data, ForwardData):
+            sparse_hidden = data.hidden
+        else:
+            sparse_hidden = data
+
+        if sparse.issparse(sparse_hidden):
             is_list = False
-            data = [data]
-        elif not isinstance(data, (list, tuple)):
-            assert False, f'invalid data: {type(data)}'
-        data = list(map(lambda d: d.todense(), data))
-        return data if is_list else data[0]
+            sparse_hidden = [sparse_hidden]
+        elif not isinstance(sparse_hidden, (list, tuple)):
+            assert False, f'invalid data: {type(sparse_hidden)}'
+        sparse_hidden = list(map(lambda d: d.todense(), sparse_hidden))
+        sparse_hidden = sparse_hidden if is_list else sparse_hidden[0]
+        if isinstance(data, ForwardData):
+            data.hidden = sparse_hidden
+        else:
+            data = sparse_hidden
+        return data
 
     def iscompressed(
         self, data: Union[sparse.spmatrix, List[sparse.spmatrix]]
     ) -> Union[bool, List[bool]]:
         """Checks whether data or data array has been compressed.
 
         Args:
```

## secretflow/utils/simulation/datasets.py

```diff
@@ -314,15 +314,15 @@
             dict {PYU: value}, the value shall be one of the followings.
             1) a float
             2) an interval in tuple closed on the left-side and open on the right-side.
         normalized_x: optional, normalize x if True. Default to True.
         categorical_y: optional, do one hot encoding to y if True. Default to True.
 
     Returns:
-        A tuple consists of two tuples, (x_train, y_train) and (x_train, y_train).
+        A tuple consists of two tuples, (x_train, y_train) and (x_test, y_test).
     """
     filepath = _get_dataset(_DATASETS['mnist'])
     with np.load(filepath) as f:
         x_train, y_train = f['x_train'], f['y_train']
         x_test, y_test = f['x_test'], f['y_test']
 
     if normalized_x:
```

## Comparing `secretflow/ml/nn/fl/backend/torch/utils.py` & `secretflow/ml/nn/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,21 +67,35 @@
         if parameters is None:
             parameters = self.parameters()
         for g, p in zip(gradients, parameters):
             if g is not None:
                 p.grad = torch.from_numpy(np.array(g.copy()))
 
 
-# @dataclass
 class TorchModel:
     def __init__(
         self,
         model_fn: BaseModule = None,
         loss_fn: BaseTorchLoss = None,
         optim_fn: optim.Optimizer = None,
         metrics: List[Metric] = [],
+        **kwargs,
     ):
-
         self.model_fn = model_fn
         self.loss_fn: BaseTorchLoss = loss_fn
         self.optim_fn: optim.Optimizer = optim_fn
         self.metrics: List[Metric] = metrics
+        self.kwargs = kwargs
+
+
+def metric_wrapper(func, *args, **kwargs):
+    def wrapped_func():
+        return func(*args, **kwargs)
+
+    return wrapped_func
+
+
+def optim_wrapper(func, *args, **kwargs):
+    def wrapped_func(params):
+        return func(params, *args, **kwargs)
+
+    return wrapped_func
```

## Comparing `secretflow/protos/component/comp_def_pb2.py` & `secretflow/protos/component/comp_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,446 +1,292 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: secretflow/protos/component/comp_def.proto
-"""Generated protocol buffer code."""
+# source: secretflow/protos/component/comp.proto
+
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='secretflow/protos/component/comp_def.proto',
+  name='secretflow/protos/component/comp.proto',
   package='secretflow.component',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n*secretflow/protos/component/comp_def.proto\x12\x14secretflow.component\"q\n\x0f\x41tomicParameter\x12\t\n\x01\x66\x18\x01 \x01(\x02\x12\x0b\n\x03i64\x18\x02 \x01(\x03\x12\t\n\x01s\x18\x03 \x01(\t\x12\t\n\x01\x62\x18\x04 \x01(\x08\x12\n\n\x02\x66s\x18\x05 \x03(\x02\x12\x0c\n\x04i64s\x18\x06 \x03(\x03\x12\n\n\x02ss\x18\x07 \x03(\t\x12\n\n\x02\x62s\x18\x08 \x03(\x08\"\x8c\x04\n\x12\x41tomicParameterDef\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).secretflow.component.AtomicParameterType\x12 \n\x18list_min_lenth_inclusive\x18\x02 \x01(\x03\x12!\n\x19list_max_length_inclusive\x18\x03 \x01(\x03\x12\x13\n\x0bis_optional\x18\x04 \x01(\x08\x12<\n\rdefault_value\x18\x05 \x01(\x0b\x32%.secretflow.component.AtomicParameter\x12=\n\x0e\x61llowed_values\x18\x06 \x01(\x0b\x32%.secretflow.component.AtomicParameter\x12\x17\n\x0fhas_lower_bound\x18\x07 \x01(\x08\x12:\n\x0blower_bound\x18\x08 \x01(\x0b\x32%.secretflow.component.AtomicParameter\x12\x1d\n\x15lower_bound_inclusive\x18\t \x01(\x08\x12\x17\n\x0fhas_upper_bound\x18\n \x01(\x08\x12:\n\x0bupper_bound\x18\x0b \x01(\x0b\x32%.secretflow.component.AtomicParameter\x12\x1d\n\x15upper_bound_inclusive\x18\x0c \x01(\x08\".\n\x11ParameterUnionDef\x12\x19\n\x11\x64\x65\x66\x61ult_selection\x18\x01 \x01(\t\"\xec\x01\n\rParameterNode\x12\x10\n\x08prefixes\x18\x01 \x03(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ndoc_string\x18\x03 \x01(\t\x12\x35\n\x04type\x18\x04 \x01(\x0e\x32\'.secretflow.component.ParameterNodeType\x12\x38\n\x06\x61tomic\x18\x05 \x01(\x0b\x32(.secretflow.component.AtomicParameterDef\x12\x36\n\x05union\x18\x06 \x01(\x0b\x32\'.secretflow.component.ParameterUnionDef\"\xce\x02\n\x08TableDef\x12<\n\x04\x63ols\x18\x01 \x03(\x0b\x32..secretflow.component.TableDef.ColParameterDef\x12.\n\x05types\x18\x02 \x03(\x0e\x32\x1f.secretflow.component.TableType\x1a\xd3\x01\n\x0f\x43olParameterDef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ndoc_string\x18\x02 \x01(\t\x12\x35\n\ndata_types\x18\x03 \x03(\x0e\x32!.secretflow.component.ColDataType\x12\x18\n\x10\x63ol_list_min_cnt\x18\x04 \x01(\x03\x12\x18\n\x10\x63ol_list_max_cnt\x18\x05 \x01(\x03\x12\x33\n\x06params\x18\x06 \x01(\x0b\x32#.secretflow.component.ParameterNode\"\x19\n\x08ModelDef\x12\r\n\x05types\x18\x02 \x03(\t\"\x18\n\x07RuleDef\x12\r\n\x05types\x18\x02 \x03(\t\"\xa7\x02\n\x05IoDef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ndoc_string\x18\x02 \x01(\t\x12\x33\n\x04\x64\x61ta\x18\x03 \x03(\x0b\x32%.secretflow.component.IoDef.SFDataDef\x1a\xc6\x01\n\tSFDataDef\x12.\n\x04type\x18\x01 \x01(\x0e\x32 .secretflow.component.SFDataType\x12-\n\x05table\x18\x02 \x01(\x0b\x32\x1e.secretflow.component.TableDef\x12-\n\x05model\x18\x03 \x01(\x0b\x32\x1e.secretflow.component.ModelDef\x12+\n\x04rule\x18\x04 \x01(\x0b\x32\x1d.secretflow.component.RuleDef\"\xe1\x01\n\x0c\x43omponentDef\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\ndoc_string\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x33\n\x06params\x18\x05 \x03(\x0b\x32#.secretflow.component.ParameterNode\x12+\n\x06inputs\x18\x06 \x03(\x0b\x32\x1b.secretflow.component.IoDef\x12,\n\x07outputs\x18\x07 \x03(\x0b\x32\x1b.secretflow.component.IoDef\"s\n\x0b\x43ompListDef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ndoc_string\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x31\n\x05\x63omps\x18\x04 \x03(\x0b\x32\".secretflow.component.ComponentDef*\xa0\x01\n\x13\x41tomicParameterType\x12\x11\n\rAPT_UNDEFINED\x10\x00\x12\r\n\tAPT_FLOAT\x10\x01\x12\x0b\n\x07\x41PT_INT\x10\x02\x12\x0e\n\nAPT_STRING\x10\x03\x12\x0c\n\x08\x41PT_BOOL\x10\x04\x12\x0e\n\nAPT_FLOATS\x10\x05\x12\x0c\n\x08\x41PT_INTS\x10\x06\x12\x0f\n\x0b\x41PT_STRINGS\x10\x07\x12\r\n\tAPT_BOOLS\x10\x08*I\n\x11ParameterNodeType\x12\x11\n\rPNT_UNDEFINED\x10\x00\x12\n\n\x06\x41TOMIC\x10\x01\x12\t\n\x05UNION\x10\x02\x12\n\n\x06STRUCT\x10\x03*}\n\tTableType\x12\x16\n\x12TABLE_TYPE_INVALID\x10\x00\x12\x14\n\x10INDIVIDUAL_TABLE\x10\x01\x12\x1f\n\x1bVERTICAL_PARTITIONING_TABLE\x10\x02\x12!\n\x1dHORIZONTAL_PARTITIONING_TABLE\x10\x03*Z\n\x0b\x43olDataType\x12\x11\n\rCDT_UNDEFINED\x10\x00\x12\r\n\tCDT_FLOAT\x10\x01\x12\x0b\n\x07\x43\x44T_INT\x10\x02\x12\x0e\n\nCDT_STRING\x10\x03\x12\x0c\n\x08\x43\x44T_BOOL\x10\x04*J\n\nSFDataType\x12\x10\n\x0c\x44T_UNDEFINED\x10\x00\x12\t\n\x05TABLE\x10\x01\x12\t\n\x05MODEL\x10\x02\x12\x08\n\x04RULE\x10\x03\x12\n\n\x06REPORT\x10\x04\x62\x06proto3'
-)
-
-_ATOMICPARAMETERTYPE = _descriptor.EnumDescriptor(
-  name='AtomicParameterType',
-  full_name='secretflow.component.AtomicParameterType',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
-    _descriptor.EnumValueDescriptor(
-      name='APT_UNDEFINED', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='APT_FLOAT', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='APT_INT', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='APT_STRING', index=3, number=3,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='APT_BOOL', index=4, number=4,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='APT_FLOATS', index=5, number=5,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='APT_INTS', index=6, number=6,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='APT_STRINGS', index=7, number=7,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='APT_BOOLS', index=8, number=8,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=2031,
-  serialized_end=2191,
-)
-_sym_db.RegisterEnumDescriptor(_ATOMICPARAMETERTYPE)
-
-AtomicParameterType = enum_type_wrapper.EnumTypeWrapper(_ATOMICPARAMETERTYPE)
-_PARAMETERNODETYPE = _descriptor.EnumDescriptor(
-  name='ParameterNodeType',
-  full_name='secretflow.component.ParameterNodeType',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
-    _descriptor.EnumValueDescriptor(
-      name='PNT_UNDEFINED', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='ATOMIC', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='UNION', index=2, number=2,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='STRUCT', index=3, number=3,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=2193,
-  serialized_end=2266,
+  serialized_pb=b'\n&secretflow/protos/component/comp.proto\x12\x14secretflow.component\"z\n\tAttribute\x12\t\n\x01\x66\x18\x01 \x01(\x02\x12\x0b\n\x03i64\x18\x02 \x01(\x03\x12\t\n\x01s\x18\x03 \x01(\t\x12\t\n\x01\x62\x18\x04 \x01(\x08\x12\n\n\x02\x66s\x18\x05 \x03(\x02\x12\x0c\n\x04i64s\x18\x06 \x03(\x03\x12\n\n\x02ss\x18\x07 \x03(\t\x12\n\n\x02\x62s\x18\x08 \x03(\x08\x12\r\n\x05is_na\x18\t \x01(\x08\"\xdf\x05\n\x0c\x41ttributeDef\x12\x10\n\x08prefixes\x18\x01 \x03(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12,\n\x04type\x18\x04 \x01(\x0e\x32\x1e.secretflow.component.AttrType\x12\x41\n\x06\x61tomic\x18\x05 \x01(\x0b\x32\x31.secretflow.component.AttributeDef.AtomicAttrDesc\x12\x44\n\x05union\x18\x06 \x01(\x0b\x32\x35.secretflow.component.AttributeDef.UnionAttrGroupDesc\x1a\xb8\x03\n\x0e\x41tomicAttrDesc\x12!\n\x19list_min_length_inclusive\x18\x01 \x01(\x03\x12!\n\x19list_max_length_inclusive\x18\x02 \x01(\x03\x12\x13\n\x0bis_optional\x18\x03 \x01(\x08\x12\x36\n\rdefault_value\x18\x04 \x01(\x0b\x32\x1f.secretflow.component.Attribute\x12\x37\n\x0e\x61llowed_values\x18\x05 \x01(\x0b\x32\x1f.secretflow.component.Attribute\x12\x17\n\x0fhas_lower_bound\x18\x06 \x01(\x08\x12\x34\n\x0blower_bound\x18\x07 \x01(\x0b\x32\x1f.secretflow.component.Attribute\x12\x1d\n\x15lower_bound_inclusive\x18\x08 \x01(\x08\x12\x17\n\x0fhas_upper_bound\x18\t \x01(\x08\x12\x34\n\x0bupper_bound\x18\n \x01(\x0b\x32\x1f.secretflow.component.Attribute\x12\x1d\n\x15upper_bound_inclusive\x18\x0b \x01(\x08\x1a/\n\x12UnionAttrGroupDesc\x12\x19\n\x11\x64\x65\x66\x61ult_selection\x18\x01 \x01(\t\"\x98\x02\n\x05IoDef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\r\n\x05types\x18\x03 \x03(\t\x12\x37\n\x05\x61ttrs\x18\x04 \x03(\x0b\x32(.secretflow.component.IoDef.TableAttrDef\x1a\xaa\x01\n\x0cTableAttrDef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\r\n\x05types\x18\x03 \x03(\t\x12\x1d\n\x15\x63ol_min_cnt_inclusive\x18\x04 \x01(\x03\x12\x1d\n\x15\x63ol_max_cnt_inclusive\x18\x05 \x01(\x03\x12\x31\n\x05\x61ttrs\x18\x06 \x03(\x0b\x32\".secretflow.component.AttributeDef\"\xd9\x01\n\x0c\x43omponentDef\x12\x0e\n\x06\x64omain\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x31\n\x05\x61ttrs\x18\x05 \x03(\x0b\x32\".secretflow.component.AttributeDef\x12+\n\x06inputs\x18\x06 \x03(\x0b\x32\x1b.secretflow.component.IoDef\x12,\n\x07outputs\x18\x07 \x03(\x0b\x32\x1b.secretflow.component.IoDef\"m\n\x0b\x43ompListDef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x31\n\x05\x63omps\x18\x04 \x03(\x0b\x32\".secretflow.component.ComponentDef*\xca\x01\n\x08\x41ttrType\x12\x10\n\x0c\x41T_UNDEFINED\x10\x00\x12\x0c\n\x08\x41T_FLOAT\x10\x01\x12\n\n\x06\x41T_INT\x10\x02\x12\r\n\tAT_STRING\x10\x03\x12\x0b\n\x07\x41T_BOOL\x10\x04\x12\r\n\tAT_FLOATS\x10\x05\x12\x0b\n\x07\x41T_INTS\x10\x06\x12\x0e\n\nAT_STRINGS\x10\x07\x12\x0c\n\x08\x41T_BOOLS\x10\x08\x12\x13\n\x0f\x41T_STRUCT_GROUP\x10\t\x12\x12\n\x0e\x41T_UNION_GROUP\x10\n\x12\x13\n\x0f\x41T_SF_TABLE_COL\x10\x0b\x62\x06proto3'
 )
-_sym_db.RegisterEnumDescriptor(_PARAMETERNODETYPE)
 
-ParameterNodeType = enum_type_wrapper.EnumTypeWrapper(_PARAMETERNODETYPE)
-_TABLETYPE = _descriptor.EnumDescriptor(
-  name='TableType',
-  full_name='secretflow.component.TableType',
+_ATTRTYPE = _descriptor.EnumDescriptor(
+  name='AttrType',
+  full_name='secretflow.component.AttrType',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='TABLE_TYPE_INVALID', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='INDIVIDUAL_TABLE', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='VERTICAL_PARTITIONING_TABLE', index=2, number=2,
+      name='AT_UNDEFINED', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='HORIZONTAL_PARTITIONING_TABLE', index=3, number=3,
+      name='AT_FLOAT', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=2268,
-  serialized_end=2393,
-)
-_sym_db.RegisterEnumDescriptor(_TABLETYPE)
-
-TableType = enum_type_wrapper.EnumTypeWrapper(_TABLETYPE)
-_COLDATATYPE = _descriptor.EnumDescriptor(
-  name='ColDataType',
-  full_name='secretflow.component.ColDataType',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
     _descriptor.EnumValueDescriptor(
-      name='CDT_UNDEFINED', index=0, number=0,
+      name='AT_INT', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CDT_FLOAT', index=1, number=1,
+      name='AT_STRING', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CDT_INT', index=2, number=2,
+      name='AT_BOOL', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CDT_STRING', index=3, number=3,
+      name='AT_FLOATS', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CDT_BOOL', index=4, number=4,
+      name='AT_INTS', index=6, number=6,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
-  ],
-  containing_type=None,
-  serialized_options=None,
-  serialized_start=2395,
-  serialized_end=2485,
-)
-_sym_db.RegisterEnumDescriptor(_COLDATATYPE)
-
-ColDataType = enum_type_wrapper.EnumTypeWrapper(_COLDATATYPE)
-_SFDATATYPE = _descriptor.EnumDescriptor(
-  name='SFDataType',
-  full_name='secretflow.component.SFDataType',
-  filename=None,
-  file=DESCRIPTOR,
-  create_key=_descriptor._internal_create_key,
-  values=[
     _descriptor.EnumValueDescriptor(
-      name='DT_UNDEFINED', index=0, number=0,
+      name='AT_STRINGS', index=7, number=7,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='TABLE', index=1, number=1,
+      name='AT_BOOLS', index=8, number=8,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='MODEL', index=2, number=2,
+      name='AT_STRUCT_GROUP', index=9, number=9,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='RULE', index=3, number=3,
+      name='AT_UNION_GROUP', index=10, number=10,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPORT', index=4, number=4,
+      name='AT_SF_TABLE_COL', index=11, number=11,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2487,
-  serialized_end=2561,
+  serialized_start=1541,
+  serialized_end=1743,
 )
-_sym_db.RegisterEnumDescriptor(_SFDATATYPE)
+_sym_db.RegisterEnumDescriptor(_ATTRTYPE)
 
-SFDataType = enum_type_wrapper.EnumTypeWrapper(_SFDATATYPE)
-APT_UNDEFINED = 0
-APT_FLOAT = 1
-APT_INT = 2
-APT_STRING = 3
-APT_BOOL = 4
-APT_FLOATS = 5
-APT_INTS = 6
-APT_STRINGS = 7
-APT_BOOLS = 8
-PNT_UNDEFINED = 0
-ATOMIC = 1
-UNION = 2
-STRUCT = 3
-TABLE_TYPE_INVALID = 0
-INDIVIDUAL_TABLE = 1
-VERTICAL_PARTITIONING_TABLE = 2
-HORIZONTAL_PARTITIONING_TABLE = 3
-CDT_UNDEFINED = 0
-CDT_FLOAT = 1
-CDT_INT = 2
-CDT_STRING = 3
-CDT_BOOL = 4
-DT_UNDEFINED = 0
-TABLE = 1
-MODEL = 2
-RULE = 3
-REPORT = 4
+AttrType = enum_type_wrapper.EnumTypeWrapper(_ATTRTYPE)
+AT_UNDEFINED = 0
+AT_FLOAT = 1
+AT_INT = 2
+AT_STRING = 3
+AT_BOOL = 4
+AT_FLOATS = 5
+AT_INTS = 6
+AT_STRINGS = 7
+AT_BOOLS = 8
+AT_STRUCT_GROUP = 9
+AT_UNION_GROUP = 10
+AT_SF_TABLE_COL = 11
 
 
 
-_ATOMICPARAMETER = _descriptor.Descriptor(
-  name='AtomicParameter',
-  full_name='secretflow.component.AtomicParameter',
+_ATTRIBUTE = _descriptor.Descriptor(
+  name='Attribute',
+  full_name='secretflow.component.Attribute',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='f', full_name='secretflow.component.AtomicParameter.f', index=0,
+      name='f', full_name='secretflow.component.Attribute.f', index=0,
       number=1, type=2, cpp_type=6, label=1,
       has_default_value=False, default_value=float(0),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='i64', full_name='secretflow.component.AtomicParameter.i64', index=1,
+      name='i64', full_name='secretflow.component.Attribute.i64', index=1,
       number=2, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='s', full_name='secretflow.component.AtomicParameter.s', index=2,
+      name='s', full_name='secretflow.component.Attribute.s', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='b', full_name='secretflow.component.AtomicParameter.b', index=3,
+      name='b', full_name='secretflow.component.Attribute.b', index=3,
       number=4, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='fs', full_name='secretflow.component.AtomicParameter.fs', index=4,
+      name='fs', full_name='secretflow.component.Attribute.fs', index=4,
       number=5, type=2, cpp_type=6, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='i64s', full_name='secretflow.component.AtomicParameter.i64s', index=5,
+      name='i64s', full_name='secretflow.component.Attribute.i64s', index=5,
       number=6, type=3, cpp_type=2, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='ss', full_name='secretflow.component.AtomicParameter.ss', index=6,
+      name='ss', full_name='secretflow.component.Attribute.ss', index=6,
       number=7, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='bs', full_name='secretflow.component.AtomicParameter.bs', index=7,
+      name='bs', full_name='secretflow.component.Attribute.bs', index=7,
       number=8, type=8, cpp_type=7, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='is_na', full_name='secretflow.component.Attribute.is_na', index=8,
+      number=9, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=68,
-  serialized_end=181,
+  serialized_start=64,
+  serialized_end=186,
 )
 
 
-_ATOMICPARAMETERDEF = _descriptor.Descriptor(
-  name='AtomicParameterDef',
-  full_name='secretflow.component.AtomicParameterDef',
+_ATTRIBUTEDEF_ATOMICATTRDESC = _descriptor.Descriptor(
+  name='AtomicAttrDesc',
+  full_name='secretflow.component.AttributeDef.AtomicAttrDesc',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='type', full_name='secretflow.component.AtomicParameterDef.type', index=0,
-      number=1, type=14, cpp_type=8, label=1,
+      name='list_min_length_inclusive', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.list_min_length_inclusive', index=0,
+      number=1, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='list_min_lenth_inclusive', full_name='secretflow.component.AtomicParameterDef.list_min_lenth_inclusive', index=1,
+      name='list_max_length_inclusive', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.list_max_length_inclusive', index=1,
       number=2, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='list_max_length_inclusive', full_name='secretflow.component.AtomicParameterDef.list_max_length_inclusive', index=2,
-      number=3, type=3, cpp_type=2, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='is_optional', full_name='secretflow.component.AtomicParameterDef.is_optional', index=3,
-      number=4, type=8, cpp_type=7, label=1,
+      name='is_optional', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.is_optional', index=2,
+      number=3, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='default_value', full_name='secretflow.component.AtomicParameterDef.default_value', index=4,
-      number=5, type=11, cpp_type=10, label=1,
+      name='default_value', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.default_value', index=3,
+      number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='allowed_values', full_name='secretflow.component.AtomicParameterDef.allowed_values', index=5,
-      number=6, type=11, cpp_type=10, label=1,
+      name='allowed_values', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.allowed_values', index=4,
+      number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='has_lower_bound', full_name='secretflow.component.AtomicParameterDef.has_lower_bound', index=6,
-      number=7, type=8, cpp_type=7, label=1,
+      name='has_lower_bound', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.has_lower_bound', index=5,
+      number=6, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='lower_bound', full_name='secretflow.component.AtomicParameterDef.lower_bound', index=7,
-      number=8, type=11, cpp_type=10, label=1,
+      name='lower_bound', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.lower_bound', index=6,
+      number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='lower_bound_inclusive', full_name='secretflow.component.AtomicParameterDef.lower_bound_inclusive', index=8,
-      number=9, type=8, cpp_type=7, label=1,
+      name='lower_bound_inclusive', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.lower_bound_inclusive', index=7,
+      number=8, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='has_upper_bound', full_name='secretflow.component.AtomicParameterDef.has_upper_bound', index=9,
-      number=10, type=8, cpp_type=7, label=1,
+      name='has_upper_bound', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.has_upper_bound', index=8,
+      number=9, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='upper_bound', full_name='secretflow.component.AtomicParameterDef.upper_bound', index=10,
-      number=11, type=11, cpp_type=10, label=1,
+      name='upper_bound', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.upper_bound', index=9,
+      number=10, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='upper_bound_inclusive', full_name='secretflow.component.AtomicParameterDef.upper_bound_inclusive', index=11,
-      number=12, type=8, cpp_type=7, label=1,
+      name='upper_bound_inclusive', full_name='secretflow.component.AttributeDef.AtomicAttrDesc.upper_bound_inclusive', index=10,
+      number=11, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -449,29 +295,28 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=184,
-  serialized_end=708,
+  serialized_start=435,
+  serialized_end=875,
 )
 
-
-_PARAMETERUNIONDEF = _descriptor.Descriptor(
-  name='ParameterUnionDef',
-  full_name='secretflow.component.ParameterUnionDef',
+_ATTRIBUTEDEF_UNIONATTRGROUPDESC = _descriptor.Descriptor(
+  name='UnionAttrGroupDesc',
+  full_name='secretflow.component.AttributeDef.UnionAttrGroupDesc',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='default_selection', full_name='secretflow.component.ParameterUnionDef.default_selection', index=0,
+      name='default_selection', full_name='secretflow.component.AttributeDef.UnionAttrGroupDesc.default_selection', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -481,234 +326,131 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=710,
-  serialized_end=756,
+  serialized_start=877,
+  serialized_end=924,
 )
 
-
-_PARAMETERNODE = _descriptor.Descriptor(
-  name='ParameterNode',
-  full_name='secretflow.component.ParameterNode',
+_ATTRIBUTEDEF = _descriptor.Descriptor(
+  name='AttributeDef',
+  full_name='secretflow.component.AttributeDef',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='prefixes', full_name='secretflow.component.ParameterNode.prefixes', index=0,
+      name='prefixes', full_name='secretflow.component.AttributeDef.prefixes', index=0,
       number=1, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.ParameterNode.name', index=1,
+      name='name', full_name='secretflow.component.AttributeDef.name', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='doc_string', full_name='secretflow.component.ParameterNode.doc_string', index=2,
+      name='desc', full_name='secretflow.component.AttributeDef.desc', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='type', full_name='secretflow.component.ParameterNode.type', index=3,
+      name='type', full_name='secretflow.component.AttributeDef.type', index=3,
       number=4, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='atomic', full_name='secretflow.component.ParameterNode.atomic', index=4,
+      name='atomic', full_name='secretflow.component.AttributeDef.atomic', index=4,
       number=5, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='union', full_name='secretflow.component.ParameterNode.union', index=5,
+      name='union', full_name='secretflow.component.AttributeDef.union', index=5,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_ATTRIBUTEDEF_ATOMICATTRDESC, _ATTRIBUTEDEF_UNIONATTRGROUPDESC, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=759,
-  serialized_end=995,
+  serialized_start=189,
+  serialized_end=924,
 )
 
 
-_TABLEDEF_COLPARAMETERDEF = _descriptor.Descriptor(
-  name='ColParameterDef',
-  full_name='secretflow.component.TableDef.ColParameterDef',
+_IODEF_TABLEATTRDEF = _descriptor.Descriptor(
+  name='TableAttrDef',
+  full_name='secretflow.component.IoDef.TableAttrDef',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.TableDef.ColParameterDef.name', index=0,
+      name='name', full_name='secretflow.component.IoDef.TableAttrDef.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='doc_string', full_name='secretflow.component.TableDef.ColParameterDef.doc_string', index=1,
+      name='desc', full_name='secretflow.component.IoDef.TableAttrDef.desc', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='data_types', full_name='secretflow.component.TableDef.ColParameterDef.data_types', index=2,
-      number=3, type=14, cpp_type=8, label=3,
+      name='types', full_name='secretflow.component.IoDef.TableAttrDef.types', index=2,
+      number=3, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='col_list_min_cnt', full_name='secretflow.component.TableDef.ColParameterDef.col_list_min_cnt', index=3,
+      name='col_min_cnt_inclusive', full_name='secretflow.component.IoDef.TableAttrDef.col_min_cnt_inclusive', index=3,
       number=4, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='col_list_max_cnt', full_name='secretflow.component.TableDef.ColParameterDef.col_list_max_cnt', index=4,
+      name='col_max_cnt_inclusive', full_name='secretflow.component.IoDef.TableAttrDef.col_max_cnt_inclusive', index=4,
       number=5, type=3, cpp_type=2, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='params', full_name='secretflow.component.TableDef.ColParameterDef.params', index=5,
-      number=6, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=1121,
-  serialized_end=1332,
-)
-
-_TABLEDEF = _descriptor.Descriptor(
-  name='TableDef',
-  full_name='secretflow.component.TableDef',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='cols', full_name='secretflow.component.TableDef.cols', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='types', full_name='secretflow.component.TableDef.types', index=1,
-      number=2, type=14, cpp_type=8, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[_TABLEDEF_COLPARAMETERDEF, ],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=998,
-  serialized_end=1332,
-)
-
-
-_MODELDEF = _descriptor.Descriptor(
-  name='ModelDef',
-  full_name='secretflow.component.ModelDef',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='types', full_name='secretflow.component.ModelDef.types', index=0,
-      number=2, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=1334,
-  serialized_end=1359,
-)
-
-
-_RULEDEF = _descriptor.Descriptor(
-  name='RuleDef',
-  full_name='secretflow.component.RuleDef',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='types', full_name='secretflow.component.RuleDef.types', index=0,
-      number=2, type=9, cpp_type=9, label=3,
+      name='attrs', full_name='secretflow.component.IoDef.TableAttrDef.attrs', index=5,
+      number=6, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -717,69 +459,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1361,
-  serialized_end=1385,
-)
-
-
-_IODEF_SFDATADEF = _descriptor.Descriptor(
-  name='SFDataDef',
-  full_name='secretflow.component.IoDef.SFDataDef',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='type', full_name='secretflow.component.IoDef.SFDataDef.type', index=0,
-      number=1, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='table', full_name='secretflow.component.IoDef.SFDataDef.table', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='model', full_name='secretflow.component.IoDef.SFDataDef.model', index=2,
-      number=3, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='rule', full_name='secretflow.component.IoDef.SFDataDef.rule', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=1485,
-  serialized_end=1683,
+  serialized_start=1037,
+  serialized_end=1207,
 )
 
 _IODEF = _descriptor.Descriptor(
   name='IoDef',
   full_name='secretflow.component.IoDef',
   filename=None,
   file=DESCRIPTOR,
@@ -790,41 +479,48 @@
       name='name', full_name='secretflow.component.IoDef.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='doc_string', full_name='secretflow.component.IoDef.doc_string', index=1,
+      name='desc', full_name='secretflow.component.IoDef.desc', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='data', full_name='secretflow.component.IoDef.data', index=2,
-      number=3, type=11, cpp_type=10, label=3,
+      name='types', full_name='secretflow.component.IoDef.types', index=2,
+      number=3, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='attrs', full_name='secretflow.component.IoDef.attrs', index=3,
+      number=4, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_IODEF_SFDATADEF, ],
+  nested_types=[_IODEF_TABLEATTRDEF, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1388,
-  serialized_end=1683,
+  serialized_start=927,
+  serialized_end=1207,
 )
 
 
 _COMPONENTDEF = _descriptor.Descriptor(
   name='ComponentDef',
   full_name='secretflow.component.ComponentDef',
   filename=None,
@@ -843,29 +539,29 @@
       name='name', full_name='secretflow.component.ComponentDef.name', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='doc_string', full_name='secretflow.component.ComponentDef.doc_string', index=2,
+      name='desc', full_name='secretflow.component.ComponentDef.desc', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='version', full_name='secretflow.component.ComponentDef.version', index=3,
       number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='params', full_name='secretflow.component.ComponentDef.params', index=4,
+      name='attrs', full_name='secretflow.component.ComponentDef.attrs', index=4,
       number=5, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='inputs', full_name='secretflow.component.ComponentDef.inputs', index=5,
@@ -889,16 +585,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1686,
-  serialized_end=1911,
+  serialized_start=1210,
+  serialized_end=1427,
 )
 
 
 _COMPLISTDEF = _descriptor.Descriptor(
   name='CompListDef',
   full_name='secretflow.component.CompListDef',
   filename=None,
@@ -910,15 +606,15 @@
       name='name', full_name='secretflow.component.CompListDef.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='doc_string', full_name='secretflow.component.CompListDef.doc_string', index=1,
+      name='desc', full_name='secretflow.component.CompListDef.desc', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='version', full_name='secretflow.component.CompListDef.version', index=2,
@@ -942,139 +638,96 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1913,
-  serialized_end=2028,
+  serialized_start=1429,
+  serialized_end=1538,
 )
 
-_ATOMICPARAMETERDEF.fields_by_name['type'].enum_type = _ATOMICPARAMETERTYPE
-_ATOMICPARAMETERDEF.fields_by_name['default_value'].message_type = _ATOMICPARAMETER
-_ATOMICPARAMETERDEF.fields_by_name['allowed_values'].message_type = _ATOMICPARAMETER
-_ATOMICPARAMETERDEF.fields_by_name['lower_bound'].message_type = _ATOMICPARAMETER
-_ATOMICPARAMETERDEF.fields_by_name['upper_bound'].message_type = _ATOMICPARAMETER
-_PARAMETERNODE.fields_by_name['type'].enum_type = _PARAMETERNODETYPE
-_PARAMETERNODE.fields_by_name['atomic'].message_type = _ATOMICPARAMETERDEF
-_PARAMETERNODE.fields_by_name['union'].message_type = _PARAMETERUNIONDEF
-_TABLEDEF_COLPARAMETERDEF.fields_by_name['data_types'].enum_type = _COLDATATYPE
-_TABLEDEF_COLPARAMETERDEF.fields_by_name['params'].message_type = _PARAMETERNODE
-_TABLEDEF_COLPARAMETERDEF.containing_type = _TABLEDEF
-_TABLEDEF.fields_by_name['cols'].message_type = _TABLEDEF_COLPARAMETERDEF
-_TABLEDEF.fields_by_name['types'].enum_type = _TABLETYPE
-_IODEF_SFDATADEF.fields_by_name['type'].enum_type = _SFDATATYPE
-_IODEF_SFDATADEF.fields_by_name['table'].message_type = _TABLEDEF
-_IODEF_SFDATADEF.fields_by_name['model'].message_type = _MODELDEF
-_IODEF_SFDATADEF.fields_by_name['rule'].message_type = _RULEDEF
-_IODEF_SFDATADEF.containing_type = _IODEF
-_IODEF.fields_by_name['data'].message_type = _IODEF_SFDATADEF
-_COMPONENTDEF.fields_by_name['params'].message_type = _PARAMETERNODE
+_ATTRIBUTEDEF_ATOMICATTRDESC.fields_by_name['default_value'].message_type = _ATTRIBUTE
+_ATTRIBUTEDEF_ATOMICATTRDESC.fields_by_name['allowed_values'].message_type = _ATTRIBUTE
+_ATTRIBUTEDEF_ATOMICATTRDESC.fields_by_name['lower_bound'].message_type = _ATTRIBUTE
+_ATTRIBUTEDEF_ATOMICATTRDESC.fields_by_name['upper_bound'].message_type = _ATTRIBUTE
+_ATTRIBUTEDEF_ATOMICATTRDESC.containing_type = _ATTRIBUTEDEF
+_ATTRIBUTEDEF_UNIONATTRGROUPDESC.containing_type = _ATTRIBUTEDEF
+_ATTRIBUTEDEF.fields_by_name['type'].enum_type = _ATTRTYPE
+_ATTRIBUTEDEF.fields_by_name['atomic'].message_type = _ATTRIBUTEDEF_ATOMICATTRDESC
+_ATTRIBUTEDEF.fields_by_name['union'].message_type = _ATTRIBUTEDEF_UNIONATTRGROUPDESC
+_IODEF_TABLEATTRDEF.fields_by_name['attrs'].message_type = _ATTRIBUTEDEF
+_IODEF_TABLEATTRDEF.containing_type = _IODEF
+_IODEF.fields_by_name['attrs'].message_type = _IODEF_TABLEATTRDEF
+_COMPONENTDEF.fields_by_name['attrs'].message_type = _ATTRIBUTEDEF
 _COMPONENTDEF.fields_by_name['inputs'].message_type = _IODEF
 _COMPONENTDEF.fields_by_name['outputs'].message_type = _IODEF
 _COMPLISTDEF.fields_by_name['comps'].message_type = _COMPONENTDEF
-DESCRIPTOR.message_types_by_name['AtomicParameter'] = _ATOMICPARAMETER
-DESCRIPTOR.message_types_by_name['AtomicParameterDef'] = _ATOMICPARAMETERDEF
-DESCRIPTOR.message_types_by_name['ParameterUnionDef'] = _PARAMETERUNIONDEF
-DESCRIPTOR.message_types_by_name['ParameterNode'] = _PARAMETERNODE
-DESCRIPTOR.message_types_by_name['TableDef'] = _TABLEDEF
-DESCRIPTOR.message_types_by_name['ModelDef'] = _MODELDEF
-DESCRIPTOR.message_types_by_name['RuleDef'] = _RULEDEF
+DESCRIPTOR.message_types_by_name['Attribute'] = _ATTRIBUTE
+DESCRIPTOR.message_types_by_name['AttributeDef'] = _ATTRIBUTEDEF
 DESCRIPTOR.message_types_by_name['IoDef'] = _IODEF
 DESCRIPTOR.message_types_by_name['ComponentDef'] = _COMPONENTDEF
 DESCRIPTOR.message_types_by_name['CompListDef'] = _COMPLISTDEF
-DESCRIPTOR.enum_types_by_name['AtomicParameterType'] = _ATOMICPARAMETERTYPE
-DESCRIPTOR.enum_types_by_name['ParameterNodeType'] = _PARAMETERNODETYPE
-DESCRIPTOR.enum_types_by_name['TableType'] = _TABLETYPE
-DESCRIPTOR.enum_types_by_name['ColDataType'] = _COLDATATYPE
-DESCRIPTOR.enum_types_by_name['SFDataType'] = _SFDATATYPE
+DESCRIPTOR.enum_types_by_name['AttrType'] = _ATTRTYPE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-AtomicParameter = _reflection.GeneratedProtocolMessageType('AtomicParameter', (_message.Message,), {
-  'DESCRIPTOR' : _ATOMICPARAMETER,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.AtomicParameter)
-  })
-_sym_db.RegisterMessage(AtomicParameter)
-
-AtomicParameterDef = _reflection.GeneratedProtocolMessageType('AtomicParameterDef', (_message.Message,), {
-  'DESCRIPTOR' : _ATOMICPARAMETERDEF,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.AtomicParameterDef)
-  })
-_sym_db.RegisterMessage(AtomicParameterDef)
-
-ParameterUnionDef = _reflection.GeneratedProtocolMessageType('ParameterUnionDef', (_message.Message,), {
-  'DESCRIPTOR' : _PARAMETERUNIONDEF,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.ParameterUnionDef)
-  })
-_sym_db.RegisterMessage(ParameterUnionDef)
-
-ParameterNode = _reflection.GeneratedProtocolMessageType('ParameterNode', (_message.Message,), {
-  'DESCRIPTOR' : _PARAMETERNODE,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.ParameterNode)
+Attribute = _reflection.GeneratedProtocolMessageType('Attribute', (_message.Message,), {
+  'DESCRIPTOR' : _ATTRIBUTE,
+  '__module__' : 'secretflow.protos.component.comp_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.component.Attribute)
   })
-_sym_db.RegisterMessage(ParameterNode)
+_sym_db.RegisterMessage(Attribute)
 
-TableDef = _reflection.GeneratedProtocolMessageType('TableDef', (_message.Message,), {
+AttributeDef = _reflection.GeneratedProtocolMessageType('AttributeDef', (_message.Message,), {
 
-  'ColParameterDef' : _reflection.GeneratedProtocolMessageType('ColParameterDef', (_message.Message,), {
-    'DESCRIPTOR' : _TABLEDEF_COLPARAMETERDEF,
-    '__module__' : 'secretflow.protos.component.comp_def_pb2'
-    # @@protoc_insertion_point(class_scope:secretflow.component.TableDef.ColParameterDef)
+  'AtomicAttrDesc' : _reflection.GeneratedProtocolMessageType('AtomicAttrDesc', (_message.Message,), {
+    'DESCRIPTOR' : _ATTRIBUTEDEF_ATOMICATTRDESC,
+    '__module__' : 'secretflow.protos.component.comp_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.AttributeDef.AtomicAttrDesc)
     })
   ,
-  'DESCRIPTOR' : _TABLEDEF,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.TableDef)
-  })
-_sym_db.RegisterMessage(TableDef)
-_sym_db.RegisterMessage(TableDef.ColParameterDef)
 
-ModelDef = _reflection.GeneratedProtocolMessageType('ModelDef', (_message.Message,), {
-  'DESCRIPTOR' : _MODELDEF,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.ModelDef)
-  })
-_sym_db.RegisterMessage(ModelDef)
-
-RuleDef = _reflection.GeneratedProtocolMessageType('RuleDef', (_message.Message,), {
-  'DESCRIPTOR' : _RULEDEF,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.RuleDef)
+  'UnionAttrGroupDesc' : _reflection.GeneratedProtocolMessageType('UnionAttrGroupDesc', (_message.Message,), {
+    'DESCRIPTOR' : _ATTRIBUTEDEF_UNIONATTRGROUPDESC,
+    '__module__' : 'secretflow.protos.component.comp_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.AttributeDef.UnionAttrGroupDesc)
+    })
+  ,
+  'DESCRIPTOR' : _ATTRIBUTEDEF,
+  '__module__' : 'secretflow.protos.component.comp_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.component.AttributeDef)
   })
-_sym_db.RegisterMessage(RuleDef)
+_sym_db.RegisterMessage(AttributeDef)
+_sym_db.RegisterMessage(AttributeDef.AtomicAttrDesc)
+_sym_db.RegisterMessage(AttributeDef.UnionAttrGroupDesc)
 
 IoDef = _reflection.GeneratedProtocolMessageType('IoDef', (_message.Message,), {
 
-  'SFDataDef' : _reflection.GeneratedProtocolMessageType('SFDataDef', (_message.Message,), {
-    'DESCRIPTOR' : _IODEF_SFDATADEF,
-    '__module__' : 'secretflow.protos.component.comp_def_pb2'
-    # @@protoc_insertion_point(class_scope:secretflow.component.IoDef.SFDataDef)
+  'TableAttrDef' : _reflection.GeneratedProtocolMessageType('TableAttrDef', (_message.Message,), {
+    'DESCRIPTOR' : _IODEF_TABLEATTRDEF,
+    '__module__' : 'secretflow.protos.component.comp_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.IoDef.TableAttrDef)
     })
   ,
   'DESCRIPTOR' : _IODEF,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
+  '__module__' : 'secretflow.protos.component.comp_pb2'
   # @@protoc_insertion_point(class_scope:secretflow.component.IoDef)
   })
 _sym_db.RegisterMessage(IoDef)
-_sym_db.RegisterMessage(IoDef.SFDataDef)
+_sym_db.RegisterMessage(IoDef.TableAttrDef)
 
 ComponentDef = _reflection.GeneratedProtocolMessageType('ComponentDef', (_message.Message,), {
   'DESCRIPTOR' : _COMPONENTDEF,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
+  '__module__' : 'secretflow.protos.component.comp_pb2'
   # @@protoc_insertion_point(class_scope:secretflow.component.ComponentDef)
   })
 _sym_db.RegisterMessage(ComponentDef)
 
 CompListDef = _reflection.GeneratedProtocolMessageType('CompListDef', (_message.Message,), {
   'DESCRIPTOR' : _COMPLISTDEF,
-  '__module__' : 'secretflow.protos.component.comp_def_pb2'
+  '__module__' : 'secretflow.protos.component.comp_pb2'
   # @@protoc_insertion_point(class_scope:secretflow.component.CompListDef)
   })
 _sym_db.RegisterMessage(CompListDef)
 
 
 # @@protoc_insertion_point(module_scope)
```

## Comparing `secretflow/protos/component/data_def_pb2.py` & `secretflow/kuscia/proto/api/v1alpha1/kusciatask/kuscia_task_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: secretflow/protos/component/data_def.proto
+# source: kuscia/proto/api/v1alpha1/kusciatask/kuscia_task.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
-from secretflow.protos.component import cluster_pb2 as secretflow_dot_protos_dot_component_dot_cluster__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='secretflow/protos/component/data_def.proto',
-  package='secretflow.component',
+  name='kuscia/proto/api/v1alpha1/kusciatask/kuscia_task.proto',
+  package='kuscia.proto.api.v1alpha1.kusciatask',
   syntax='proto3',
-  serialized_options=None,
+  serialized_options=b'\n\"com.secretflow.v1alpha1.kusciataskZ:github.com/secretflow/kuscia/proto/api/v1alpha1/kusciatask',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n*secretflow/protos/component/data_def.proto\x12\x14secretflow.component\x1a\x19google/protobuf/any.proto\x1a)secretflow/protos/component/cluster.proto\"W\n\nSystemInfo\x12\x10\n\x08\x61pp_name\x18\x01 \x01(\t\x12\x37\n\nsecretflow\x18\x02 \x01(\x0b\x32#.secretflow.component.SFClusterDesc\"\xdf\x01\n\x08\x44istData\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x31\n\x07sysinfo\x18\x03 \x01(\x0b\x32 .secretflow.component.SystemInfo\x12\"\n\x04meta\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x39\n\tdata_refs\x18\x05 \x03(\x0b\x32&.secretflow.component.DistData.DataRef\x1a%\n\x07\x44\x61taRef\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\r\n\x05party\x18\x02 \x01(\t\"\x88\x01\n\x06VTable\x12\x32\n\x06slices\x18\x01 \x03(\x0b\x32\".secretflow.component.VTable.Slice\x12\x11\n\tnum_lines\x18\x02 \x01(\x03\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\t\x1a\'\n\x05Slice\x12\r\n\x05types\x18\x01 \x03(\t\x12\x0f\n\x07headers\x18\x02 \x03(\tb\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_any__pb2.DESCRIPTOR,secretflow_dot_protos_dot_component_dot_cluster__pb2.DESCRIPTOR,])
+  serialized_pb=b'\n6kuscia/proto/api/v1alpha1/kusciatask/kuscia_task.proto\x12$kuscia.proto.api.v1alpha1.kusciatask\"/\n\x07Service\x12\x11\n\tport_name\x18\x01 \x01(\t\x12\x11\n\tendpoints\x18\x02 \x03(\t\"d\n\x05Party\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04role\x18\x02 \x01(\t\x12?\n\x08services\x18\x03 \x03(\x0b\x32-.kuscia.proto.api.v1alpha1.kusciatask.Service\"\x80\x01\n\rClusterDefine\x12<\n\x07parties\x18\x01 \x03(\x0b\x32+.kuscia.proto.api.v1alpha1.kusciatask.Party\x12\x16\n\x0eself_party_idx\x18\x02 \x01(\x05\x12\x19\n\x11self_endpoint_idx\x18\x03 \x01(\x05\"C\n\x04Port\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\r\n\x05scope\x18\x03 \x01(\t\x12\x10\n\x08protocol\x18\x04 \x01(\t\"K\n\x0e\x41llocatedPorts\x12\x39\n\x05ports\x18\x01 \x03(\x0b\x32*.kuscia.proto.api.v1alpha1.kusciatask.PortB`\n\"com.secretflow.v1alpha1.kusciataskZ:github.com/secretflow/kuscia/proto/api/v1alpha1/kusciataskb\x06proto3'
+)
 
 
 
 
-_SYSTEMINFO = _descriptor.Descriptor(
-  name='SystemInfo',
-  full_name='secretflow.component.SystemInfo',
+_SERVICE = _descriptor.Descriptor(
+  name='Service',
+  full_name='kuscia.proto.api.v1alpha1.kusciatask.Service',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='app_name', full_name='secretflow.component.SystemInfo.app_name', index=0,
+      name='port_name', full_name='kuscia.proto.api.v1alpha1.kusciatask.Service.port_name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='secretflow', full_name='secretflow.component.SystemInfo.secretflow', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='endpoints', full_name='kuscia.proto.api.v1alpha1.kusciatask.Service.endpoints', index=1,
+      number=2, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -58,136 +55,144 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=138,
-  serialized_end=225,
+  serialized_start=96,
+  serialized_end=143,
 )
 
 
-_DISTDATA_DATAREF = _descriptor.Descriptor(
-  name='DataRef',
-  full_name='secretflow.component.DistData.DataRef',
+_PARTY = _descriptor.Descriptor(
+  name='Party',
+  full_name='kuscia.proto.api.v1alpha1.kusciatask.Party',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='uri', full_name='secretflow.component.DistData.DataRef.uri', index=0,
+      name='name', full_name='kuscia.proto.api.v1alpha1.kusciatask.Party.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='party', full_name='secretflow.component.DistData.DataRef.party', index=1,
+      name='role', full_name='kuscia.proto.api.v1alpha1.kusciatask.Party.role', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='services', full_name='kuscia.proto.api.v1alpha1.kusciatask.Party.services', index=2,
+      number=3, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=414,
-  serialized_end=451,
+  serialized_start=145,
+  serialized_end=245,
 )
 
-_DISTDATA = _descriptor.Descriptor(
-  name='DistData',
-  full_name='secretflow.component.DistData',
+
+_CLUSTERDEFINE = _descriptor.Descriptor(
+  name='ClusterDefine',
+  full_name='kuscia.proto.api.v1alpha1.kusciatask.ClusterDefine',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.DistData.name', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='type', full_name='secretflow.component.DistData.type', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='sysinfo', full_name='secretflow.component.DistData.sysinfo', index=2,
-      number=3, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='parties', full_name='kuscia.proto.api.v1alpha1.kusciatask.ClusterDefine.parties', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='meta', full_name='secretflow.component.DistData.meta', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='self_party_idx', full_name='kuscia.proto.api.v1alpha1.kusciatask.ClusterDefine.self_party_idx', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='data_refs', full_name='secretflow.component.DistData.data_refs', index=4,
-      number=5, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
+      name='self_endpoint_idx', full_name='kuscia.proto.api.v1alpha1.kusciatask.ClusterDefine.self_endpoint_idx', index=2,
+      number=3, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_DISTDATA_DATAREF, ],
+  nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=228,
-  serialized_end=451,
+  serialized_start=248,
+  serialized_end=376,
 )
 
 
-_VTABLE_SLICE = _descriptor.Descriptor(
-  name='Slice',
-  full_name='secretflow.component.VTable.Slice',
+_PORT = _descriptor.Descriptor(
+  name='Port',
+  full_name='kuscia.proto.api.v1alpha1.kusciatask.Port',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='types', full_name='secretflow.component.VTable.Slice.types', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
+      name='name', full_name='kuscia.proto.api.v1alpha1.kusciatask.Port.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='headers', full_name='secretflow.component.VTable.Slice.headers', index=1,
-      number=2, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
+      name='port', full_name='kuscia.proto.api.v1alpha1.kusciatask.Port.port', index=1,
+      number=2, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='scope', full_name='kuscia.proto.api.v1alpha1.kusciatask.Port.scope', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='protocol', full_name='kuscia.proto.api.v1alpha1.kusciatask.Port.protocol', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -195,107 +200,91 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=551,
-  serialized_end=590,
+  serialized_start=378,
+  serialized_end=445,
 )
 
-_VTABLE = _descriptor.Descriptor(
-  name='VTable',
-  full_name='secretflow.component.VTable',
+
+_ALLOCATEDPORTS = _descriptor.Descriptor(
+  name='AllocatedPorts',
+  full_name='kuscia.proto.api.v1alpha1.kusciatask.AllocatedPorts',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='slices', full_name='secretflow.component.VTable.slices', index=0,
+      name='ports', full_name='kuscia.proto.api.v1alpha1.kusciatask.AllocatedPorts.ports', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='num_lines', full_name='secretflow.component.VTable.num_lines', index=1,
-      number=2, type=3, cpp_type=2, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='format', full_name='secretflow.component.VTable.format', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_VTABLE_SLICE, ],
+  nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=454,
-  serialized_end=590,
+  serialized_start=447,
+  serialized_end=522,
 )
 
-_SYSTEMINFO.fields_by_name['secretflow'].message_type = secretflow_dot_protos_dot_component_dot_cluster__pb2._SFCLUSTERDESC
-_DISTDATA_DATAREF.containing_type = _DISTDATA
-_DISTDATA.fields_by_name['sysinfo'].message_type = _SYSTEMINFO
-_DISTDATA.fields_by_name['meta'].message_type = google_dot_protobuf_dot_any__pb2._ANY
-_DISTDATA.fields_by_name['data_refs'].message_type = _DISTDATA_DATAREF
-_VTABLE_SLICE.containing_type = _VTABLE
-_VTABLE.fields_by_name['slices'].message_type = _VTABLE_SLICE
-DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
-DESCRIPTOR.message_types_by_name['DistData'] = _DISTDATA
-DESCRIPTOR.message_types_by_name['VTable'] = _VTABLE
+_PARTY.fields_by_name['services'].message_type = _SERVICE
+_CLUSTERDEFINE.fields_by_name['parties'].message_type = _PARTY
+_ALLOCATEDPORTS.fields_by_name['ports'].message_type = _PORT
+DESCRIPTOR.message_types_by_name['Service'] = _SERVICE
+DESCRIPTOR.message_types_by_name['Party'] = _PARTY
+DESCRIPTOR.message_types_by_name['ClusterDefine'] = _CLUSTERDEFINE
+DESCRIPTOR.message_types_by_name['Port'] = _PORT
+DESCRIPTOR.message_types_by_name['AllocatedPorts'] = _ALLOCATEDPORTS
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
-  'DESCRIPTOR' : _SYSTEMINFO,
-  '__module__' : 'secretflow.protos.component.data_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.SystemInfo)
+Service = _reflection.GeneratedProtocolMessageType('Service', (_message.Message,), {
+  'DESCRIPTOR' : _SERVICE,
+  '__module__' : 'kuscia.proto.api.v1alpha1.kusciatask.kuscia_task_pb2'
+  # @@protoc_insertion_point(class_scope:kuscia.proto.api.v1alpha1.kusciatask.Service)
   })
-_sym_db.RegisterMessage(SystemInfo)
+_sym_db.RegisterMessage(Service)
 
-DistData = _reflection.GeneratedProtocolMessageType('DistData', (_message.Message,), {
+Party = _reflection.GeneratedProtocolMessageType('Party', (_message.Message,), {
+  'DESCRIPTOR' : _PARTY,
+  '__module__' : 'kuscia.proto.api.v1alpha1.kusciatask.kuscia_task_pb2'
+  # @@protoc_insertion_point(class_scope:kuscia.proto.api.v1alpha1.kusciatask.Party)
+  })
+_sym_db.RegisterMessage(Party)
 
-  'DataRef' : _reflection.GeneratedProtocolMessageType('DataRef', (_message.Message,), {
-    'DESCRIPTOR' : _DISTDATA_DATAREF,
-    '__module__' : 'secretflow.protos.component.data_def_pb2'
-    # @@protoc_insertion_point(class_scope:secretflow.component.DistData.DataRef)
-    })
-  ,
-  'DESCRIPTOR' : _DISTDATA,
-  '__module__' : 'secretflow.protos.component.data_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.DistData)
+ClusterDefine = _reflection.GeneratedProtocolMessageType('ClusterDefine', (_message.Message,), {
+  'DESCRIPTOR' : _CLUSTERDEFINE,
+  '__module__' : 'kuscia.proto.api.v1alpha1.kusciatask.kuscia_task_pb2'
+  # @@protoc_insertion_point(class_scope:kuscia.proto.api.v1alpha1.kusciatask.ClusterDefine)
   })
-_sym_db.RegisterMessage(DistData)
-_sym_db.RegisterMessage(DistData.DataRef)
+_sym_db.RegisterMessage(ClusterDefine)
 
-VTable = _reflection.GeneratedProtocolMessageType('VTable', (_message.Message,), {
+Port = _reflection.GeneratedProtocolMessageType('Port', (_message.Message,), {
+  'DESCRIPTOR' : _PORT,
+  '__module__' : 'kuscia.proto.api.v1alpha1.kusciatask.kuscia_task_pb2'
+  # @@protoc_insertion_point(class_scope:kuscia.proto.api.v1alpha1.kusciatask.Port)
+  })
+_sym_db.RegisterMessage(Port)
 
-  'Slice' : _reflection.GeneratedProtocolMessageType('Slice', (_message.Message,), {
-    'DESCRIPTOR' : _VTABLE_SLICE,
-    '__module__' : 'secretflow.protos.component.data_def_pb2'
-    # @@protoc_insertion_point(class_scope:secretflow.component.VTable.Slice)
-    })
-  ,
-  'DESCRIPTOR' : _VTABLE,
-  '__module__' : 'secretflow.protos.component.data_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.VTable)
+AllocatedPorts = _reflection.GeneratedProtocolMessageType('AllocatedPorts', (_message.Message,), {
+  'DESCRIPTOR' : _ALLOCATEDPORTS,
+  '__module__' : 'kuscia.proto.api.v1alpha1.kusciatask.kuscia_task_pb2'
+  # @@protoc_insertion_point(class_scope:kuscia.proto.api.v1alpha1.kusciatask.AllocatedPorts)
   })
-_sym_db.RegisterMessage(VTable)
-_sym_db.RegisterMessage(VTable.Slice)
+_sym_db.RegisterMessage(AllocatedPorts)
 
 
+DESCRIPTOR._options = None
 # @@protoc_insertion_point(module_scope)
```

## Comparing `secretflow/protos/component/node_def_pb2.py` & `secretflow/protos/component/data_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,146 +1,108 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: secretflow/protos/component/node_def.proto
-"""Generated protocol buffer code."""
+# source: secretflow/protos/component/data.proto
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from secretflow.protos.component import comp_def_pb2 as secretflow_dot_protos_dot_component_dot_comp__def__pb2
+from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
+from secretflow.protos.component import cluster_pb2 as secretflow_dot_protos_dot_component_dot_cluster__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='secretflow/protos/component/node_def.proto',
+  name='secretflow/protos/component/data.proto',
   package='secretflow.component',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n*secretflow/protos/component/node_def.proto\x12\x14secretflow.component\x1a*secretflow/protos/component/comp_def.proto\"\x7f\n\rNodeParameter\x12\x10\n\x08prefixes\x18\x01 \x03(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x35\n\x06\x61tomic\x18\x03 \x01(\x0b\x32%.secretflow.component.AtomicParameter\x12\x17\n\x0funion_selection\x18\x04 \x01(\t\"4\n\x15IndivialTableMetadata\x12\r\n\x05party\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"D\n\"VeriticalPartitioningTableMetaData\x12\x0f\n\x07parties\x18\x01 \x03(\t\x12\r\n\x05paths\x18\x02 \x03(\t\"\xd6\x01\n\rTableMetadata\x12-\n\x04type\x18\x01 \x01(\x0e\x32\x1f.secretflow.component.TableType\x12=\n\x08indivial\x18\x02 \x01(\x0b\x32+.secretflow.component.IndivialTableMetadata\x12W\n\x15vertical_partitioning\x18\x03 \x01(\x0b\x32\x38.secretflow.component.VeriticalPartitioningTableMetaData\"S\n\rModelMetadata\x12\x18\n\x10public_file_path\x18\x01 \x01(\t\x12\x0f\n\x07parties\x18\x02 \x03(\t\x12\x17\n\x0fparty_dir_paths\x18\x03 \x03(\t\"\x0e\n\x0cRuleMetadata\"\x10\n\x0eReportMetadata\"\xf6\x01\n\x0bTableParams\x12\x42\n\ncol_params\x18\x01 \x03(\x0b\x32..secretflow.component.TableParams.ColParameter\x1a=\n\x06Params\x12\x33\n\x06values\x18\x01 \x03(\x0b\x32#.secretflow.component.NodeParameter\x1a\x64\n\x0c\x43olParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ols\x18\x02 \x03(\t\x12\x38\n\x06params\x18\x03 \x03(\x0b\x32(.secretflow.component.TableParams.Params\"\xf3\x02\n\x06NodeIo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x04type\x18\x02 \x01(\x0e\x32 .secretflow.component.SFDataType\x12\x37\n\x0ctable_params\x18\x03 \x01(\x0b\x32!.secretflow.component.TableParams\x12;\n\x0etable_metadata\x18\x04 \x01(\x0b\x32#.secretflow.component.TableMetadata\x12;\n\x0emodel_metadata\x18\x05 \x01(\x0b\x32#.secretflow.component.ModelMetadata\x12\x39\n\rrule_metadata\x18\x06 \x01(\x0b\x32\".secretflow.component.RuleMetadata\x12=\n\x0freport_metadata\x18\x07 \x01(\x0b\x32$.secretflow.component.ReportMetadata\"\xd6\x01\n\x07NodeDef\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x64omain\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x33\n\x06params\x18\x05 \x03(\x0b\x32#.secretflow.component.NodeParameter\x12,\n\x06inputs\x18\x06 \x03(\x0b\x32\x1c.secretflow.component.NodeIo\x12-\n\x07outputs\x18\x07 \x03(\x0b\x32\x1c.secretflow.component.NodeIob\x06proto3'
+  serialized_pb=b'\n&secretflow/protos/component/data.proto\x12\x14secretflow.component\x1a\x19google/protobuf/any.proto\x1a)secretflow/protos/component/cluster.proto\"W\n\nSystemInfo\x12\x10\n\x08\x61pp_name\x18\x01 \x01(\t\x12\x37\n\nsecretflow\x18\x02 \x01(\x0b\x32#.secretflow.component.SFClusterDesc\"K\n\x0bTableSchema\x12\x0b\n\x03ids\x18\x01 \x03(\t\x12\x10\n\x08\x66\x65\x61tures\x18\x02 \x03(\t\x12\r\n\x05types\x18\x03 \x03(\t\x12\x0e\n\x06labels\x18\x04 \x03(\t\"V\n\rVerticalTable\x12\x32\n\x07schemas\x18\x01 \x03(\x0b\x32!.secretflow.component.TableSchema\x12\x11\n\tnum_lines\x18\x02 \x01(\x03\"W\n\x0fIndividualTable\x12\x31\n\x06schema\x18\x01 \x01(\x0b\x32!.secretflow.component.TableSchema\x12\x11\n\tnum_lines\x18\x02 \x01(\x03\"\xab\x01\n\x16\x44\x65viceObjectCollection\x12G\n\x04objs\x18\x01 \x03(\x0b\x32\x39.secretflow.component.DeviceObjectCollection.DeviceObject\x12\x13\n\x0bpublic_info\x18\x02 \x01(\t\x1a\x33\n\x0c\x44\x65viceObject\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x15\n\rdata_ref_idxs\x18\x02 \x03(\x05\"\xf0\x01\n\x08\x44istData\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x32\n\x08sys_info\x18\x03 \x01(\x0b\x32 .secretflow.component.SystemInfo\x12\"\n\x04meta\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x39\n\tdata_refs\x18\x05 \x03(\x0b\x32&.secretflow.component.DistData.DataRef\x1a\x35\n\x07\x44\x61taRef\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\r\n\x05party\x18\x02 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x03 \x01(\tb\x06proto3'
   ,
-  dependencies=[secretflow_dot_protos_dot_component_dot_comp__def__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_protobuf_dot_any__pb2.DESCRIPTOR,secretflow_dot_protos_dot_component_dot_cluster__pb2.DESCRIPTOR,])
 
 
 
 
-_NODEPARAMETER = _descriptor.Descriptor(
-  name='NodeParameter',
-  full_name='secretflow.component.NodeParameter',
+_SYSTEMINFO = _descriptor.Descriptor(
+  name='SystemInfo',
+  full_name='secretflow.component.SystemInfo',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='prefixes', full_name='secretflow.component.NodeParameter.prefixes', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.NodeParameter.name', index=1,
-      number=2, type=9, cpp_type=9, label=1,
+      name='app_name', full_name='secretflow.component.SystemInfo.app_name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='atomic', full_name='secretflow.component.NodeParameter.atomic', index=2,
-      number=3, type=11, cpp_type=10, label=1,
+      name='secretflow', full_name='secretflow.component.SystemInfo.secretflow', index=1,
+      number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='union_selection', full_name='secretflow.component.NodeParameter.union_selection', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=112,
-  serialized_end=239,
+  serialized_start=134,
+  serialized_end=221,
 )
 
 
-_INDIVIALTABLEMETADATA = _descriptor.Descriptor(
-  name='IndivialTableMetadata',
-  full_name='secretflow.component.IndivialTableMetadata',
+_TABLESCHEMA = _descriptor.Descriptor(
+  name='TableSchema',
+  full_name='secretflow.component.TableSchema',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='party', full_name='secretflow.component.IndivialTableMetadata.party', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='ids', full_name='secretflow.component.TableSchema.ids', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='path', full_name='secretflow.component.IndivialTableMetadata.path', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='features', full_name='secretflow.component.TableSchema.features', index=1,
+      number=2, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=241,
-  serialized_end=293,
-)
-
-
-_VERITICALPARTITIONINGTABLEMETADATA = _descriptor.Descriptor(
-  name='VeriticalPartitioningTableMetaData',
-  full_name='secretflow.component.VeriticalPartitioningTableMetaData',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
     _descriptor.FieldDescriptor(
-      name='parties', full_name='secretflow.component.VeriticalPartitioningTableMetaData.parties', index=0,
-      number=1, type=9, cpp_type=9, label=3,
+      name='types', full_name='secretflow.component.TableSchema.types', index=2,
+      number=3, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='paths', full_name='secretflow.component.VeriticalPartitioningTableMetaData.paths', index=1,
-      number=2, type=9, cpp_type=9, label=3,
+      name='labels', full_name='secretflow.component.TableSchema.labels', index=3,
+      number=4, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -149,45 +111,38 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=295,
-  serialized_end=363,
+  serialized_start=223,
+  serialized_end=298,
 )
 
 
-_TABLEMETADATA = _descriptor.Descriptor(
-  name='TableMetadata',
-  full_name='secretflow.component.TableMetadata',
+_VERTICALTABLE = _descriptor.Descriptor(
+  name='VerticalTable',
+  full_name='secretflow.component.VerticalTable',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='type', full_name='secretflow.component.TableMetadata.type', index=0,
-      number=1, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='indivial', full_name='secretflow.component.TableMetadata.indivial', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='schemas', full_name='secretflow.component.VerticalTable.schemas', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='vertical_partitioning', full_name='secretflow.component.TableMetadata.vertical_partitioning', index=2,
-      number=3, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='num_lines', full_name='secretflow.component.VerticalTable.num_lines', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -195,45 +150,38 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=366,
-  serialized_end=580,
+  serialized_start=300,
+  serialized_end=386,
 )
 
 
-_MODELMETADATA = _descriptor.Descriptor(
-  name='ModelMetadata',
-  full_name='secretflow.component.ModelMetadata',
+_INDIVIDUALTABLE = _descriptor.Descriptor(
+  name='IndividualTable',
+  full_name='secretflow.component.IndividualTable',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='public_file_path', full_name='secretflow.component.ModelMetadata.public_file_path', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='parties', full_name='secretflow.component.ModelMetadata.parties', index=1,
-      number=2, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
+      name='schema', full_name='secretflow.component.IndividualTable.schema', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='party_dir_paths', full_name='secretflow.component.ModelMetadata.party_dir_paths', index=2,
-      number=3, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
+      name='num_lines', full_name='secretflow.component.IndividualTable.num_lines', index=1,
+      number=2, type=3, cpp_type=2, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -241,125 +189,37 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=582,
-  serialized_end=665,
-)
-
-
-_RULEMETADATA = _descriptor.Descriptor(
-  name='RuleMetadata',
-  full_name='secretflow.component.RuleMetadata',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=667,
-  serialized_end=681,
-)
-
-
-_REPORTMETADATA = _descriptor.Descriptor(
-  name='ReportMetadata',
-  full_name='secretflow.component.ReportMetadata',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=683,
-  serialized_end=699,
+  serialized_start=388,
+  serialized_end=475,
 )
 
 
-_TABLEPARAMS_PARAMS = _descriptor.Descriptor(
-  name='Params',
-  full_name='secretflow.component.TableParams.Params',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='values', full_name='secretflow.component.TableParams.Params.values', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=785,
-  serialized_end=846,
-)
-
-_TABLEPARAMS_COLPARAMETER = _descriptor.Descriptor(
-  name='ColParameter',
-  full_name='secretflow.component.TableParams.ColParameter',
+_DEVICEOBJECTCOLLECTION_DEVICEOBJECT = _descriptor.Descriptor(
+  name='DeviceObject',
+  full_name='secretflow.component.DeviceObjectCollection.DeviceObject',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.TableParams.ColParameter.name', index=0,
+      name='type', full_name='secretflow.component.DeviceObjectCollection.DeviceObject.type', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='cols', full_name='secretflow.component.TableParams.ColParameter.cols', index=1,
-      number=2, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='params', full_name='secretflow.component.TableParams.ColParameter.params', index=2,
-      number=3, type=11, cpp_type=10, label=3,
+      name='data_ref_idxs', full_name='secretflow.component.DeviceObjectCollection.DeviceObject.data_ref_idxs', index=1,
+      number=2, type=5, cpp_type=1, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -368,104 +228,83 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=848,
-  serialized_end=948,
+  serialized_start=598,
+  serialized_end=649,
 )
 
-_TABLEPARAMS = _descriptor.Descriptor(
-  name='TableParams',
-  full_name='secretflow.component.TableParams',
+_DEVICEOBJECTCOLLECTION = _descriptor.Descriptor(
+  name='DeviceObjectCollection',
+  full_name='secretflow.component.DeviceObjectCollection',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='col_params', full_name='secretflow.component.TableParams.col_params', index=0,
+      name='objs', full_name='secretflow.component.DeviceObjectCollection.objs', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='public_info', full_name='secretflow.component.DeviceObjectCollection.public_info', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_TABLEPARAMS_PARAMS, _TABLEPARAMS_COLPARAMETER, ],
+  nested_types=[_DEVICEOBJECTCOLLECTION_DEVICEOBJECT, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=702,
-  serialized_end=948,
+  serialized_start=478,
+  serialized_end=649,
 )
 
 
-_NODEIO = _descriptor.Descriptor(
-  name='NodeIo',
-  full_name='secretflow.component.NodeIo',
+_DISTDATA_DATAREF = _descriptor.Descriptor(
+  name='DataRef',
+  full_name='secretflow.component.DistData.DataRef',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.NodeIo.name', index=0,
+      name='uri', full_name='secretflow.component.DistData.DataRef.uri', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='type', full_name='secretflow.component.NodeIo.type', index=1,
-      number=2, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='table_params', full_name='secretflow.component.NodeIo.table_params', index=2,
-      number=3, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='table_metadata', full_name='secretflow.component.NodeIo.table_metadata', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='model_metadata', full_name='secretflow.component.NodeIo.model_metadata', index=4,
-      number=5, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='rule_metadata', full_name='secretflow.component.NodeIo.rule_metadata', index=5,
-      number=6, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='party', full_name='secretflow.component.DistData.DataRef.party', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='report_metadata', full_name='secretflow.component.NodeIo.report_metadata', index=6,
-      number=7, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='format', full_name='secretflow.component.DistData.DataRef.format', index=2,
+      number=3, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -473,203 +312,147 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=951,
-  serialized_end=1322,
+  serialized_start=839,
+  serialized_end=892,
 )
 
-
-_NODEDEF = _descriptor.Descriptor(
-  name='NodeDef',
-  full_name='secretflow.component.NodeDef',
+_DISTDATA = _descriptor.Descriptor(
+  name='DistData',
+  full_name='secretflow.component.DistData',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='secretflow.component.NodeDef.id', index=0,
+      name='name', full_name='secretflow.component.DistData.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='domain', full_name='secretflow.component.NodeDef.domain', index=1,
+      name='type', full_name='secretflow.component.DistData.type', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.component.NodeDef.name', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='sys_info', full_name='secretflow.component.DistData.sys_info', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='version', full_name='secretflow.component.NodeDef.version', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='meta', full_name='secretflow.component.DistData.meta', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='params', full_name='secretflow.component.NodeDef.params', index=4,
+      name='data_refs', full_name='secretflow.component.DistData.data_refs', index=4,
       number=5, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='inputs', full_name='secretflow.component.NodeDef.inputs', index=5,
-      number=6, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='outputs', full_name='secretflow.component.NodeDef.outputs', index=6,
-      number=7, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[],
+  nested_types=[_DISTDATA_DATAREF, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1325,
-  serialized_end=1539,
+  serialized_start=652,
+  serialized_end=892,
 )
 
-_NODEPARAMETER.fields_by_name['atomic'].message_type = secretflow_dot_protos_dot_component_dot_comp__def__pb2._ATOMICPARAMETER
-_TABLEMETADATA.fields_by_name['type'].enum_type = secretflow_dot_protos_dot_component_dot_comp__def__pb2._TABLETYPE
-_TABLEMETADATA.fields_by_name['indivial'].message_type = _INDIVIALTABLEMETADATA
-_TABLEMETADATA.fields_by_name['vertical_partitioning'].message_type = _VERITICALPARTITIONINGTABLEMETADATA
-_TABLEPARAMS_PARAMS.fields_by_name['values'].message_type = _NODEPARAMETER
-_TABLEPARAMS_PARAMS.containing_type = _TABLEPARAMS
-_TABLEPARAMS_COLPARAMETER.fields_by_name['params'].message_type = _TABLEPARAMS_PARAMS
-_TABLEPARAMS_COLPARAMETER.containing_type = _TABLEPARAMS
-_TABLEPARAMS.fields_by_name['col_params'].message_type = _TABLEPARAMS_COLPARAMETER
-_NODEIO.fields_by_name['type'].enum_type = secretflow_dot_protos_dot_component_dot_comp__def__pb2._SFDATATYPE
-_NODEIO.fields_by_name['table_params'].message_type = _TABLEPARAMS
-_NODEIO.fields_by_name['table_metadata'].message_type = _TABLEMETADATA
-_NODEIO.fields_by_name['model_metadata'].message_type = _MODELMETADATA
-_NODEIO.fields_by_name['rule_metadata'].message_type = _RULEMETADATA
-_NODEIO.fields_by_name['report_metadata'].message_type = _REPORTMETADATA
-_NODEDEF.fields_by_name['params'].message_type = _NODEPARAMETER
-_NODEDEF.fields_by_name['inputs'].message_type = _NODEIO
-_NODEDEF.fields_by_name['outputs'].message_type = _NODEIO
-DESCRIPTOR.message_types_by_name['NodeParameter'] = _NODEPARAMETER
-DESCRIPTOR.message_types_by_name['IndivialTableMetadata'] = _INDIVIALTABLEMETADATA
-DESCRIPTOR.message_types_by_name['VeriticalPartitioningTableMetaData'] = _VERITICALPARTITIONINGTABLEMETADATA
-DESCRIPTOR.message_types_by_name['TableMetadata'] = _TABLEMETADATA
-DESCRIPTOR.message_types_by_name['ModelMetadata'] = _MODELMETADATA
-DESCRIPTOR.message_types_by_name['RuleMetadata'] = _RULEMETADATA
-DESCRIPTOR.message_types_by_name['ReportMetadata'] = _REPORTMETADATA
-DESCRIPTOR.message_types_by_name['TableParams'] = _TABLEPARAMS
-DESCRIPTOR.message_types_by_name['NodeIo'] = _NODEIO
-DESCRIPTOR.message_types_by_name['NodeDef'] = _NODEDEF
+_SYSTEMINFO.fields_by_name['secretflow'].message_type = secretflow_dot_protos_dot_component_dot_cluster__pb2._SFCLUSTERDESC
+_VERTICALTABLE.fields_by_name['schemas'].message_type = _TABLESCHEMA
+_INDIVIDUALTABLE.fields_by_name['schema'].message_type = _TABLESCHEMA
+_DEVICEOBJECTCOLLECTION_DEVICEOBJECT.containing_type = _DEVICEOBJECTCOLLECTION
+_DEVICEOBJECTCOLLECTION.fields_by_name['objs'].message_type = _DEVICEOBJECTCOLLECTION_DEVICEOBJECT
+_DISTDATA_DATAREF.containing_type = _DISTDATA
+_DISTDATA.fields_by_name['sys_info'].message_type = _SYSTEMINFO
+_DISTDATA.fields_by_name['meta'].message_type = google_dot_protobuf_dot_any__pb2._ANY
+_DISTDATA.fields_by_name['data_refs'].message_type = _DISTDATA_DATAREF
+DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
+DESCRIPTOR.message_types_by_name['TableSchema'] = _TABLESCHEMA
+DESCRIPTOR.message_types_by_name['VerticalTable'] = _VERTICALTABLE
+DESCRIPTOR.message_types_by_name['IndividualTable'] = _INDIVIDUALTABLE
+DESCRIPTOR.message_types_by_name['DeviceObjectCollection'] = _DEVICEOBJECTCOLLECTION
+DESCRIPTOR.message_types_by_name['DistData'] = _DISTDATA
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-NodeParameter = _reflection.GeneratedProtocolMessageType('NodeParameter', (_message.Message,), {
-  'DESCRIPTOR' : _NODEPARAMETER,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.NodeParameter)
-  })
-_sym_db.RegisterMessage(NodeParameter)
-
-IndivialTableMetadata = _reflection.GeneratedProtocolMessageType('IndivialTableMetadata', (_message.Message,), {
-  'DESCRIPTOR' : _INDIVIALTABLEMETADATA,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.IndivialTableMetadata)
-  })
-_sym_db.RegisterMessage(IndivialTableMetadata)
-
-VeriticalPartitioningTableMetaData = _reflection.GeneratedProtocolMessageType('VeriticalPartitioningTableMetaData', (_message.Message,), {
-  'DESCRIPTOR' : _VERITICALPARTITIONINGTABLEMETADATA,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.VeriticalPartitioningTableMetaData)
-  })
-_sym_db.RegisterMessage(VeriticalPartitioningTableMetaData)
-
-TableMetadata = _reflection.GeneratedProtocolMessageType('TableMetadata', (_message.Message,), {
-  'DESCRIPTOR' : _TABLEMETADATA,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.TableMetadata)
+SystemInfo = _reflection.GeneratedProtocolMessageType('SystemInfo', (_message.Message,), {
+  'DESCRIPTOR' : _SYSTEMINFO,
+  '__module__' : 'secretflow.protos.component.data_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.component.SystemInfo)
   })
-_sym_db.RegisterMessage(TableMetadata)
+_sym_db.RegisterMessage(SystemInfo)
 
-ModelMetadata = _reflection.GeneratedProtocolMessageType('ModelMetadata', (_message.Message,), {
-  'DESCRIPTOR' : _MODELMETADATA,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.ModelMetadata)
+TableSchema = _reflection.GeneratedProtocolMessageType('TableSchema', (_message.Message,), {
+  'DESCRIPTOR' : _TABLESCHEMA,
+  '__module__' : 'secretflow.protos.component.data_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.component.TableSchema)
   })
-_sym_db.RegisterMessage(ModelMetadata)
+_sym_db.RegisterMessage(TableSchema)
 
-RuleMetadata = _reflection.GeneratedProtocolMessageType('RuleMetadata', (_message.Message,), {
-  'DESCRIPTOR' : _RULEMETADATA,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.RuleMetadata)
+VerticalTable = _reflection.GeneratedProtocolMessageType('VerticalTable', (_message.Message,), {
+  'DESCRIPTOR' : _VERTICALTABLE,
+  '__module__' : 'secretflow.protos.component.data_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.component.VerticalTable)
   })
-_sym_db.RegisterMessage(RuleMetadata)
+_sym_db.RegisterMessage(VerticalTable)
 
-ReportMetadata = _reflection.GeneratedProtocolMessageType('ReportMetadata', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTMETADATA,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.ReportMetadata)
+IndividualTable = _reflection.GeneratedProtocolMessageType('IndividualTable', (_message.Message,), {
+  'DESCRIPTOR' : _INDIVIDUALTABLE,
+  '__module__' : 'secretflow.protos.component.data_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.component.IndividualTable)
   })
-_sym_db.RegisterMessage(ReportMetadata)
+_sym_db.RegisterMessage(IndividualTable)
 
-TableParams = _reflection.GeneratedProtocolMessageType('TableParams', (_message.Message,), {
+DeviceObjectCollection = _reflection.GeneratedProtocolMessageType('DeviceObjectCollection', (_message.Message,), {
 
-  'Params' : _reflection.GeneratedProtocolMessageType('Params', (_message.Message,), {
-    'DESCRIPTOR' : _TABLEPARAMS_PARAMS,
-    '__module__' : 'secretflow.protos.component.node_def_pb2'
-    # @@protoc_insertion_point(class_scope:secretflow.component.TableParams.Params)
+  'DeviceObject' : _reflection.GeneratedProtocolMessageType('DeviceObject', (_message.Message,), {
+    'DESCRIPTOR' : _DEVICEOBJECTCOLLECTION_DEVICEOBJECT,
+    '__module__' : 'secretflow.protos.component.data_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.DeviceObjectCollection.DeviceObject)
     })
   ,
+  'DESCRIPTOR' : _DEVICEOBJECTCOLLECTION,
+  '__module__' : 'secretflow.protos.component.data_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.component.DeviceObjectCollection)
+  })
+_sym_db.RegisterMessage(DeviceObjectCollection)
+_sym_db.RegisterMessage(DeviceObjectCollection.DeviceObject)
+
+DistData = _reflection.GeneratedProtocolMessageType('DistData', (_message.Message,), {
 
-  'ColParameter' : _reflection.GeneratedProtocolMessageType('ColParameter', (_message.Message,), {
-    'DESCRIPTOR' : _TABLEPARAMS_COLPARAMETER,
-    '__module__' : 'secretflow.protos.component.node_def_pb2'
-    # @@protoc_insertion_point(class_scope:secretflow.component.TableParams.ColParameter)
+  'DataRef' : _reflection.GeneratedProtocolMessageType('DataRef', (_message.Message,), {
+    'DESCRIPTOR' : _DISTDATA_DATAREF,
+    '__module__' : 'secretflow.protos.component.data_pb2'
+    # @@protoc_insertion_point(class_scope:secretflow.component.DistData.DataRef)
     })
   ,
-  'DESCRIPTOR' : _TABLEPARAMS,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.TableParams)
-  })
-_sym_db.RegisterMessage(TableParams)
-_sym_db.RegisterMessage(TableParams.Params)
-_sym_db.RegisterMessage(TableParams.ColParameter)
-
-NodeIo = _reflection.GeneratedProtocolMessageType('NodeIo', (_message.Message,), {
-  'DESCRIPTOR' : _NODEIO,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.NodeIo)
-  })
-_sym_db.RegisterMessage(NodeIo)
-
-NodeDef = _reflection.GeneratedProtocolMessageType('NodeDef', (_message.Message,), {
-  'DESCRIPTOR' : _NODEDEF,
-  '__module__' : 'secretflow.protos.component.node_def_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.component.NodeDef)
+  'DESCRIPTOR' : _DISTDATA,
+  '__module__' : 'secretflow.protos.component.data_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.component.DistData)
   })
-_sym_db.RegisterMessage(NodeDef)
+_sym_db.RegisterMessage(DistData)
+_sym_db.RegisterMessage(DistData.DataRef)
 
 
 # @@protoc_insertion_point(module_scope)
```

## Comparing `secretflow/protos/kuscia/__init__.py` & `secretflow/component/ml/boost/__init__.py`

 * *Files identical despite different names*

## Comparing `secretflow/protos/kuscia/kuscia_task_pb2.py` & `secretflow/protos/pipeline/pipeline_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,98 +1,143 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: secretflow/protos/kuscia/kuscia_task.proto
-"""Generated protocol buffer code."""
+# source: secretflow/protos/pipeline/pipeline.proto
+
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from secretflow.protos.component import comp_pb2 as secretflow_dot_protos_dot_component_dot_comp__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
-  name='secretflow/protos/kuscia/kuscia_task.proto',
-  package='secretflow.kuscia',
+  name='secretflow/protos/pipeline/pipeline.proto',
+  package='secretflow.pipeline',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n*secretflow/protos/kuscia/kuscia_task.proto\x12\x11secretflow.kuscia\"/\n\x07Service\x12\x11\n\tport_name\x18\x01 \x01(\t\x12\x11\n\tendpoints\x18\x02 \x03(\t\"Q\n\x05Party\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04role\x18\x02 \x01(\t\x12,\n\x08services\x18\x03 \x03(\x0b\x32\x1a.secretflow.kuscia.Service\"m\n\rClusterDefine\x12)\n\x07parties\x18\x01 \x03(\x0b\x32\x18.secretflow.kuscia.Party\x12\x16\n\x0eself_party_idx\x18\x02 \x01(\x05\x12\x19\n\x11self_endpoint_idx\x18\x03 \x01(\x05\"C\n\x04Port\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\r\n\x05scope\x18\x03 \x01(\t\x12\x10\n\x08protocol\x18\x04 \x01(\t\"8\n\x0e\x41llocatedPorts\x12&\n\x05ports\x18\x01 \x03(\x0b\x32\x17.secretflow.kuscia.Portb\x06proto3'
+  serialized_pb=b'\n)secretflow/protos/pipeline/pipeline.proto\x12\x13secretflow.pipeline\x1a&secretflow/protos/component/comp.proto\"\xa9\x01\n\x07NodeDef\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x64omain\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x12\n\nattr_paths\x18\x05 \x03(\t\x12.\n\x05\x61ttrs\x18\x06 \x03(\x0b\x32\x1f.secretflow.component.Attribute\x12\x0e\n\x06inputs\x18\x07 \x03(\t\x12\x0f\n\x07outputs\x18\x08 \x03(\t\"F\n\x0bPipelineDef\x12\n\n\x02id\x18\x01 \x01(\t\x12+\n\x05nodes\x18\x02 \x03(\x0b\x32\x1c.secretflow.pipeline.NodeDef\"B\n\tNodeState\x12\n\n\x02id\x18\x01 \x01(\t\x12)\n\x05state\x18\x02 \x01(\x0e\x32\x1a.secretflow.pipeline.State\"u\n\rPipelineState\x12\n\n\x02id\x18\x01 \x01(\t\x12)\n\x05state\x18\x02 \x01(\x0e\x32\x1a.secretflow.pipeline.State\x12-\n\x05nodes\x18\x03 \x03(\x0b\x32\x1e.secretflow.pipeline.NodeState*K\n\x05State\x12\x0b\n\x07Staging\x10\x00\x12\x0f\n\x0bInitialized\x10\x01\x12\x0b\n\x07Running\x10\x02\x12\x0b\n\x07Succeed\x10\x03\x12\n\n\x06\x46\x61iled\x10\x04\x62\x06proto3'
+  ,
+  dependencies=[secretflow_dot_protos_dot_component_dot_comp__pb2.DESCRIPTOR,])
+
+_STATE = _descriptor.EnumDescriptor(
+  name='State',
+  full_name='secretflow.pipeline.State',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='Staging', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Initialized', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Running', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Succeed', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='Failed', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=537,
+  serialized_end=612,
 )
+_sym_db.RegisterEnumDescriptor(_STATE)
 
+State = enum_type_wrapper.EnumTypeWrapper(_STATE)
+Staging = 0
+Initialized = 1
+Running = 2
+Succeed = 3
+Failed = 4
 
 
 
-_SERVICE = _descriptor.Descriptor(
-  name='Service',
-  full_name='secretflow.kuscia.Service',
+_NODEDEF = _descriptor.Descriptor(
+  name='NodeDef',
+  full_name='secretflow.pipeline.NodeDef',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='port_name', full_name='secretflow.kuscia.Service.port_name', index=0,
+      name='id', full_name='secretflow.pipeline.NodeDef.id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='endpoints', full_name='secretflow.kuscia.Service.endpoints', index=1,
-      number=2, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
+      name='domain', full_name='secretflow.pipeline.NodeDef.domain', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=65,
-  serialized_end=112,
-)
-
-
-_PARTY = _descriptor.Descriptor(
-  name='Party',
-  full_name='secretflow.kuscia.Party',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.kuscia.Party.name', index=0,
-      number=1, type=9, cpp_type=9, label=1,
+      name='name', full_name='secretflow.pipeline.NodeDef.name', index=2,
+      number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='role', full_name='secretflow.kuscia.Party.role', index=1,
-      number=2, type=9, cpp_type=9, label=1,
+      name='version', full_name='secretflow.pipeline.NodeDef.version', index=3,
+      number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='services', full_name='secretflow.kuscia.Party.services', index=2,
-      number=3, type=11, cpp_type=10, label=3,
+      name='attr_paths', full_name='secretflow.pipeline.NodeDef.attr_paths', index=4,
+      number=5, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='attrs', full_name='secretflow.pipeline.NodeDef.attrs', index=5,
+      number=6, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='inputs', full_name='secretflow.pipeline.NodeDef.inputs', index=6,
+      number=7, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='outputs', full_name='secretflow.pipeline.NodeDef.outputs', index=7,
+      number=8, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -101,45 +146,38 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=114,
-  serialized_end=195,
+  serialized_start=107,
+  serialized_end=276,
 )
 
 
-_CLUSTERDEFINE = _descriptor.Descriptor(
-  name='ClusterDefine',
-  full_name='secretflow.kuscia.ClusterDefine',
+_PIPELINEDEF = _descriptor.Descriptor(
+  name='PipelineDef',
+  full_name='secretflow.pipeline.PipelineDef',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='parties', full_name='secretflow.kuscia.ClusterDefine.parties', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='self_party_idx', full_name='secretflow.kuscia.ClusterDefine.self_party_idx', index=1,
-      number=2, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
+      name='id', full_name='secretflow.pipeline.PipelineDef.id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='self_endpoint_idx', full_name='secretflow.kuscia.ClusterDefine.self_endpoint_idx', index=2,
-      number=3, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
+      name='nodes', full_name='secretflow.pipeline.PipelineDef.nodes', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -147,83 +185,83 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=197,
-  serialized_end=306,
+  serialized_start=278,
+  serialized_end=348,
 )
 
 
-_PORT = _descriptor.Descriptor(
-  name='Port',
-  full_name='secretflow.kuscia.Port',
+_NODESTATE = _descriptor.Descriptor(
+  name='NodeState',
+  full_name='secretflow.pipeline.NodeState',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='name', full_name='secretflow.kuscia.Port.name', index=0,
+      name='id', full_name='secretflow.pipeline.NodeState.id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='port', full_name='secretflow.kuscia.Port.port', index=1,
-      number=2, type=5, cpp_type=1, label=1,
+      name='state', full_name='secretflow.pipeline.NodeState.state', index=1,
+      number=2, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='scope', full_name='secretflow.kuscia.Port.scope', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='protocol', full_name='secretflow.kuscia.Port.protocol', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=308,
-  serialized_end=375,
+  serialized_start=350,
+  serialized_end=416,
 )
 
 
-_ALLOCATEDPORTS = _descriptor.Descriptor(
-  name='AllocatedPorts',
-  full_name='secretflow.kuscia.AllocatedPorts',
+_PIPELINESTATE = _descriptor.Descriptor(
+  name='PipelineState',
+  full_name='secretflow.pipeline.PipelineState',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='ports', full_name='secretflow.kuscia.AllocatedPorts.ports', index=0,
-      number=1, type=11, cpp_type=10, label=3,
+      name='id', full_name='secretflow.pipeline.PipelineState.id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='state', full_name='secretflow.pipeline.PipelineState.state', index=1,
+      number=2, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='nodes', full_name='secretflow.pipeline.PipelineState.nodes', index=2,
+      number=3, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -232,58 +270,53 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=377,
-  serialized_end=433,
+  serialized_start=418,
+  serialized_end=535,
 )
 
-_PARTY.fields_by_name['services'].message_type = _SERVICE
-_CLUSTERDEFINE.fields_by_name['parties'].message_type = _PARTY
-_ALLOCATEDPORTS.fields_by_name['ports'].message_type = _PORT
-DESCRIPTOR.message_types_by_name['Service'] = _SERVICE
-DESCRIPTOR.message_types_by_name['Party'] = _PARTY
-DESCRIPTOR.message_types_by_name['ClusterDefine'] = _CLUSTERDEFINE
-DESCRIPTOR.message_types_by_name['Port'] = _PORT
-DESCRIPTOR.message_types_by_name['AllocatedPorts'] = _ALLOCATEDPORTS
+_NODEDEF.fields_by_name['attrs'].message_type = secretflow_dot_protos_dot_component_dot_comp__pb2._ATTRIBUTE
+_PIPELINEDEF.fields_by_name['nodes'].message_type = _NODEDEF
+_NODESTATE.fields_by_name['state'].enum_type = _STATE
+_PIPELINESTATE.fields_by_name['state'].enum_type = _STATE
+_PIPELINESTATE.fields_by_name['nodes'].message_type = _NODESTATE
+DESCRIPTOR.message_types_by_name['NodeDef'] = _NODEDEF
+DESCRIPTOR.message_types_by_name['PipelineDef'] = _PIPELINEDEF
+DESCRIPTOR.message_types_by_name['NodeState'] = _NODESTATE
+DESCRIPTOR.message_types_by_name['PipelineState'] = _PIPELINESTATE
+DESCRIPTOR.enum_types_by_name['State'] = _STATE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
-Service = _reflection.GeneratedProtocolMessageType('Service', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICE,
-  '__module__' : 'secretflow.protos.kuscia.kuscia_task_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.kuscia.Service)
-  })
-_sym_db.RegisterMessage(Service)
-
-Party = _reflection.GeneratedProtocolMessageType('Party', (_message.Message,), {
-  'DESCRIPTOR' : _PARTY,
-  '__module__' : 'secretflow.protos.kuscia.kuscia_task_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.kuscia.Party)
+NodeDef = _reflection.GeneratedProtocolMessageType('NodeDef', (_message.Message,), {
+  'DESCRIPTOR' : _NODEDEF,
+  '__module__' : 'secretflow.protos.pipeline.pipeline_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.pipeline.NodeDef)
   })
-_sym_db.RegisterMessage(Party)
+_sym_db.RegisterMessage(NodeDef)
 
-ClusterDefine = _reflection.GeneratedProtocolMessageType('ClusterDefine', (_message.Message,), {
-  'DESCRIPTOR' : _CLUSTERDEFINE,
-  '__module__' : 'secretflow.protos.kuscia.kuscia_task_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.kuscia.ClusterDefine)
+PipelineDef = _reflection.GeneratedProtocolMessageType('PipelineDef', (_message.Message,), {
+  'DESCRIPTOR' : _PIPELINEDEF,
+  '__module__' : 'secretflow.protos.pipeline.pipeline_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.pipeline.PipelineDef)
   })
-_sym_db.RegisterMessage(ClusterDefine)
+_sym_db.RegisterMessage(PipelineDef)
 
-Port = _reflection.GeneratedProtocolMessageType('Port', (_message.Message,), {
-  'DESCRIPTOR' : _PORT,
-  '__module__' : 'secretflow.protos.kuscia.kuscia_task_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.kuscia.Port)
+NodeState = _reflection.GeneratedProtocolMessageType('NodeState', (_message.Message,), {
+  'DESCRIPTOR' : _NODESTATE,
+  '__module__' : 'secretflow.protos.pipeline.pipeline_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.pipeline.NodeState)
   })
-_sym_db.RegisterMessage(Port)
+_sym_db.RegisterMessage(NodeState)
 
-AllocatedPorts = _reflection.GeneratedProtocolMessageType('AllocatedPorts', (_message.Message,), {
-  'DESCRIPTOR' : _ALLOCATEDPORTS,
-  '__module__' : 'secretflow.protos.kuscia.kuscia_task_pb2'
-  # @@protoc_insertion_point(class_scope:secretflow.kuscia.AllocatedPorts)
+PipelineState = _reflection.GeneratedProtocolMessageType('PipelineState', (_message.Message,), {
+  'DESCRIPTOR' : _PIPELINESTATE,
+  '__module__' : 'secretflow.protos.pipeline.pipeline_pb2'
+  # @@protoc_insertion_point(class_scope:secretflow.pipeline.PipelineState)
   })
-_sym_db.RegisterMessage(AllocatedPorts)
+_sym_db.RegisterMessage(PipelineState)
 
 
 # @@protoc_insertion_point(module_scope)
```

## Comparing `secretflow/security/privacy/mechanism/tensorflow/mechanism_fl.py` & `secretflow/security/privacy/mechanism/mechanism_fl.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
 
 import numpy as np
-import tensorflow as tf
-
 from secretflow.security.privacy.accounting.rdp_accountant import (
     get_privacy_spent_rdp,
     get_rdp,
 )
 
 
 class GaussianModelDP:
@@ -58,21 +56,20 @@
 
         Args:
             inputs: Model parameters.
         """
         assert inputs, 'the inputs of GaussianModelDP should not be empty!'
 
         model_weights_noised = []
-        gradient_norm_all = tf.linalg.global_norm(inputs)
+        gradient_norm_all = self.global_norm(inputs)
 
         if self.is_clip_each_layer:
             for i in range(len(inputs)):
-
                 # clipping
-                gradient_norm = tf.linalg.global_norm([inputs[i]])
+                gradient_norm = self.global_norm([inputs[i]])
                 gradient_clipped = inputs[i] * min(
                     1,
                     (self.l2_norm_clip / np.sqrt(gradient_norm * gradient_norm_all)),
                 )
 
                 # add noise
                 if self.is_secure_generator:
@@ -80,49 +77,54 @@
 
                     noise = random.secure_normal_real(
                         0,
                         self.noise_multiplier * self.l2_norm_clip,
                         size=inputs[i].shape,
                     )
                 else:
-                    noise = tf.random.normal(
+                    noise = np.random.normal(
                         inputs[i].shape,
                         stddev=self.noise_multiplier * self.l2_norm_clip,
                     )
 
                 model_weights_noised.append(
-                    tf.add(gradient_clipped, noise / np.sqrt(self.num_updates))
+                    np.add(gradient_clipped, noise / np.sqrt(self.num_updates))
                 )
         else:
             scale = min(1, self.l2_norm_clip / gradient_norm_all)
             for i in range(len(inputs)):
-
                 # clipping
                 gradient_clipped = inputs[i] * scale
 
                 # add noise
                 if self.is_secure_generator:
                     import secretflow.security.privacy._lib.random as random
 
                     noise = random.secure_normal_real(
                         0,
                         self.noise_multiplier * self.l2_norm_clip,
                         size=inputs[i].shape,
-                    )
+                    ).astype(np.float32)
                 else:
-                    noise = tf.random.normal(
-                        inputs[i].shape,
-                        stddev=self.noise_multiplier * self.l2_norm_clip,
-                    )
+                    noise = np.random.normal(
+                        loc=0.0,
+                        scale=self.noise_multiplier * self.l2_norm_clip,
+                        size=inputs[i].shape,
+                    ).astype(np.float32)
 
                 model_weights_noised.append(
                     np.add(gradient_clipped, noise / np.sqrt(self.num_updates))
                 )
         return model_weights_noised
 
+    def global_norm(self, inputs):
+        inputs = [np.linalg.norm(i) ** 2 for i in inputs]
+
+        return np.sqrt(sum(inputs))
+
     def privacy_spent_rdp(self, step: int, orders: List = None):
         """Get accountant using RDP.
 
         Args:
             step: The dp current step of model training or prediction.
             orders: An array (or a scalar) of RDP orders.
         """
```

## Comparing `secretflow-0.8.2b3.dist-info/LICENSE` & `secretflow-0.8.3b0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `secretflow-0.8.2b3.dist-info/METADATA` & `secretflow-0.8.3b0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: secretflow
-Version: 0.8.2b3
-Summary: Secret Flow
+Version: 0.8.3b0
+Summary: SecretFlow
 Home-page: https://github.com/secretflow/secretflow
 Author: SCI Center
 Author-email: secretflow-contact@service.alipay.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: clean-text
+Requires-Dist: click
 Requires-Dist: grpcio (<=1.49.1)
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: multiprocess
 Requires-Dist: networkx (==2.8.8)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: protobuf (==3.19.6)
 Requires-Dist: pyarrow (==11.0.0)
 Requires-Dist: s3fs (==2022.1.0)
 Requires-Dist: scikit-learn (==1.1.3)
 Requires-Dist: secretflow-rayfed (==0.1.1a3)
 Requires-Dist: setuptools (>=65.5.1)
 Requires-Dist: sparse (>=0.14.0)
-Requires-Dist: spu (==0.3.3b2)
+Requires-Dist: spu (==0.4.0b1)
 Requires-Dist: sf-heu (==0.4.3b3)
 Requires-Dist: tf2onnx (>=1.13.0)
 Requires-Dist: tqdm
 Requires-Dist: validator.py (==1.3.0)
 Requires-Dist: xgboost (==1.7.5)
 Requires-Dist: wheel (>=0.38.1)
 Requires-Dist: torch (==2.0.0)
 Requires-Dist: torchmetrics (==0.11.4)
 Requires-Dist: torchvision (==0.15.1)
 Requires-Dist: torchaudio (==2.0.1)
-Requires-Dist: click
 Requires-Dist: tensorflow (==2.11.1) ; platform_machine != "arm64"
 Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64" and platform_system == "Darwin"
 Requires-Dist: sdc-apis (==0.1.0b0) ; platform_system != "Darwin"
 Requires-Dist: sdc-sdk (==0.1.0b0) ; platform_system != "Darwin"
 Provides-Extra: dev
 Requires-Dist: pylint ; extra == 'dev'
```

### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: secretflow Version: 0.8.2b3 Summary: Secret Flow
+Metadata-Version: 2.1 Name: secretflow Version: 0.8.3b0 Summary: SecretFlow
 Home-page: https://github.com/secretflow/secretflow Author: SCI Center Author-
 email: secretflow-contact@service.alipay.com License: Apache 2.0 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist: grpcio
-(<=1.49.1) Requires-Dist: jax Requires-Dist: jaxlib Requires-Dist: multiprocess
-Requires-Dist: networkx (==2.8.8) Requires-Dist: numpy (==1.23.5) Requires-
-Dist: pandas (==1.5.3) Requires-Dist: protobuf (==3.19.6) Requires-Dist:
-pyarrow (==11.0.0) Requires-Dist: s3fs (==2022.1.0) Requires-Dist: scikit-learn
-(==1.1.3) Requires-Dist: secretflow-rayfed (==0.1.1a3) Requires-Dist:
-setuptools (>=65.5.1) Requires-Dist: sparse (>=0.14.0) Requires-Dist: spu
-(==0.3.3b2) Requires-Dist: sf-heu (==0.4.3b3) Requires-Dist: tf2onnx (>=1.13.0)
-Requires-Dist: tqdm Requires-Dist: validator.py (==1.3.0) Requires-Dist:
-xgboost (==1.7.5) Requires-Dist: wheel (>=0.38.1) Requires-Dist: torch
-(==2.0.0) Requires-Dist: torchmetrics (==0.11.4) Requires-Dist: torchvision
-(==0.15.1) Requires-Dist: torchaudio (==2.0.1) Requires-Dist: click Requires-
-Dist: tensorflow (==2.11.1) ; platform_machine != "arm64" Requires-Dist:
-tensorflow-macos (==2.11.0) ; platform_machine == "arm64" and platform_system
-== "Darwin" Requires-Dist: sdc-apis (==0.1.0b0) ; platform_system != "Darwin"
-Requires-Dist: sdc-sdk (==0.1.0b0) ; platform_system != "Darwin" Provides-
-Extra: dev Requires-Dist: pylint ; extra == 'dev'
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: clean-text
+Requires-Dist: click Requires-Dist: grpcio (<=1.49.1) Requires-Dist: jax
+Requires-Dist: jaxlib Requires-Dist: multiprocess Requires-Dist: networkx
+(==2.8.8) Requires-Dist: numpy (==1.23.5) Requires-Dist: pandas (==1.5.3)
+Requires-Dist: protobuf (==3.19.6) Requires-Dist: pyarrow (==11.0.0) Requires-
+Dist: s3fs (==2022.1.0) Requires-Dist: scikit-learn (==1.1.3) Requires-Dist:
+secretflow-rayfed (==0.1.1a3) Requires-Dist: setuptools (>=65.5.1) Requires-
+Dist: sparse (>=0.14.0) Requires-Dist: spu (==0.4.0b1) Requires-Dist: sf-heu
+(==0.4.3b3) Requires-Dist: tf2onnx (>=1.13.0) Requires-Dist: tqdm Requires-
+Dist: validator.py (==1.3.0) Requires-Dist: xgboost (==1.7.5) Requires-Dist:
+wheel (>=0.38.1) Requires-Dist: torch (==2.0.0) Requires-Dist: torchmetrics
+(==0.11.4) Requires-Dist: torchvision (==0.15.1) Requires-Dist: torchaudio
+(==2.0.1) Requires-Dist: tensorflow (==2.11.1) ; platform_machine != "arm64"
+Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64" and
+platform_system == "Darwin" Requires-Dist: sdc-apis (==0.1.0b0) ;
+platform_system != "Darwin" Requires-Dist: sdc-sdk (==0.1.0b0) ;
+platform_system != "Darwin" Provides-Extra: dev Requires-Dist: pylint ; extra
+== 'dev'
                          [docs/_static/logo-light.png]
 --- [![CircleCI](https://dl.circleci.com/status-badge/img/gh/secretflow/
 secretflow/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/
 redirect/gh/secretflow/secretflow/tree/main)
                             ç®ä½ä¸­æï½English
 SecretFlow is a unified framework for privacy-preserving data intelligence and
 machine learning. To achieve this goal, it provides: - An abstract device layer
```

## Comparing `secretflow-0.8.2b3.dist-info/RECORD` & `secretflow-0.8.3b0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,295 +1,341 @@
 secretflow/__init__.py,sha256=hNYxuX4jqzIoRuUxKl9OMp9UcbvdsvwROS6i7pHmqJQ,1321
-secretflow/cli.py,sha256=2VBlLJ4JYtZZnekOQe8hLhx1MzZwGyozPZKgPQ3Tb74,3229
-secretflow/version.py,sha256=2I6PFftmySLNfb9s4IDrRIMvJeDXDGgzYfTFrSiiJ_c,607
-secretflow/component/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/component/component.py,sha256=4pOG6XaMRD9ws334jtdTHdb4WwR-eMFzyPlU-hXLARg,21958
-secretflow/component/entry.py,sha256=20Ia1Xa-UWLVIvBXpj5_-fZg6o32rCfsBoMLFqTPrKA,2235
-secretflow/component/node_reader.py,sha256=rKEPIXyXutGHto-14JhL4Y2K543S96AkCUgBH5cIM0w,7339
+secretflow/cli.py,sha256=EMNzikFKsXnyK1e5nUhblYF_fqYNc5vgnYWmnJB0sYU,6478
+secretflow/version.py,sha256=v8UL9oQ1sxV9vBVZJLVDlKZiKhcFBXt9lhPdLgj1r6c,607
+secretflow/component/__init__.py,sha256=smAVmCDFaBfCKUTTcKqRNiG58NQk1xBAXdv25DST2FQ,635
+secretflow/component/__main__.py,sha256=wYrFQT-Q1RJpZ1F_iKN5Mk-5idUIVZn9pSwiiktKtUY,628
+secretflow/component/component.py,sha256=pHoFdjyZV-xwE4cNIcqmLjxq0Vm3dwvUlr4HEhmPjx0,30621
+secretflow/component/data_utils.py,sha256=tc8ydG7XUHppc6tN085pjRlzJCqEPigCsRQBpVPH0Xs,16205
+secretflow/component/entry.py,sha256=yzocwj5745VkA5_G0PPVpnYwf_9oXZB8oCaciMTlDvg,3791
+secretflow/component/eval_param_reader.py,sha256=9ui4Cy4G8IWEAfdX3DpZjVgCvxvTlQbelQO2J2YvB5k,9676
+secretflow/component/i18n.py,sha256=T2hYTTN08ueC_-knKzL4SFzkf5WkijVGuvhcQu8wGwA,3377
 secretflow/component/ml/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/component/ml/boost/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/component/ml/boost/sgb/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/component/ml/boost/sgb/sgb.py,sha256=SyGbpamLYTV28-yFS5mtkSHdpBbaeuBzRLjfohvxvcA,12463
+secretflow/component/ml/boost/ss_xgb/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/component/ml/boost/ss_xgb/ss_xgb.py,sha256=uiV7RA6Y-v6JqypclTu1TBEUZZkg4RNCfJmTMHk-z9I,11692
 secretflow/component/ml/linear/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/component/ml/linear/ss_sgd.py,sha256=K33kCaz8vwAkWfWQfW2U2tRqZPuy-PljDtx4E4hLT3s,7573
+secretflow/component/ml/linear/ss_sgd.py,sha256=Tr_ZRo8BvA-eTQhO7wUYGhRbGyDaULFu4Hlv0KcWQUs,10564
 secretflow/component/preprocessing/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/component/preprocessing/train_test_split.py,sha256=Exz3dOHd4POgYeX9PJ65R9q1Xa_0SbKqQrhkGmfSUBk,3938
+secretflow/component/preprocessing/feature_filter.py,sha256=YHhW5RC1wDajNJxwzS7ppDVE2F9WfxgXxfLbWeEqsaY,2640
+secretflow/component/preprocessing/train_test_split.py,sha256=qRqGSBe1f4lYuywRfWiVj7hFgL2mR5rOoSZP3nL2-5Y,3652
+secretflow/component/preprocessing/vert_woe_binning.py,sha256=xC5uvIyf26w2re7zSr1dcZlIxXN4WFEQaYSR_qgPwgU,8532
 secretflow/component/psi/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/component/psi/two_party_balanced.py,sha256=57hhJ7bZyGPUpKHb2bzoIqwr34tU1_Me1PAXcErbDoU,5605
+secretflow/component/psi/two_party_balanced.py,sha256=R4Xsv-f06qNZn06owjyPkql9xStiN1FMl_MTrxe7irQ,7598
+secretflow/component/stats/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/component/stats/biclassification_eval.py,sha256=yjJV2CUZ8vtNuXr4_HWXQWccsfVINN0ACGkB6DNFilo,13594
+secretflow/component/stats/pva_eval.py,sha256=iRwv62SVGI4f-TLIUPyBTxYeja4nA-gmjx8p3iNL2ns,2137
+secretflow/component/stats/ss_pearsonr.py,sha256=qhUurEpX-qh1Ot1HC9XLZ4b_cbLQtkEwy5E2Mf-u5xI,3843
+secretflow/component/stats/ss_pvalue.py,sha256=8Y5r31A6c0qu1pu4QgRRi-vWomHUyOz2iYWZP0LW4JY,3750
+secretflow/component/stats/ss_vif.py,sha256=9IPaD83Jyv5LfVHPRhTbJ5eKnEvvPHYfZDRKX-RNXKk,3626
+secretflow/component/stats/table_statistics.py,sha256=TQED9AiLzj8B7wpmzWhcCYvHOBBdeePsMvMmH8xRXPk,2035
 secretflow/data/__init__.py,sha256=dfSoOj_BQ2QEMiFZXgitx2IHrpJ2qyN4hGfgpKbeKcI,754
 secretflow/data/base.py,sha256=qDwucRS3FHJ0kYYMatUuS_1HL67UxJ2IjKi6UvFBfSw,14806
 secretflow/data/math_utils.py,sha256=wLVcz6eJC7LAYdTXfxERZmwtmxVfchpUkTNKVEW86HA,1108
 secretflow/data/ndarray.py,sha256=DN3GXtz2MAbbohNPvnJvYvSs9Eyy6a2kBJekTNElgh4,24878
 secretflow/data/split.py,sha256=s8HV00DaVKulNvP2-BkH_Y8cWrrnqSc_ANPgKtOQBlY,5420
-secretflow/data/horizontal/__init__.py,sha256=_2-VKz4GGygJrut0AqnLa4qvWQGztgzHkFIcoLMYhmk,716
+secretflow/data/horizontal/__init__.py,sha256=449NmBfIAOGZJO30s-l2ip6Xmzif3PJGdyaTtyEE0Ys,694
 secretflow/data/horizontal/dataframe.py,sha256=Vbc_GmHbDE6o54qEdYSQ12FVRPTc5TPzCdorO5nMZcQ,15042
-secretflow/data/horizontal/io.py,sha256=qIkzQLT8kMBq-PLU1M3OfS7-fXug61AbdzItvaNySsY,2557
+secretflow/data/horizontal/io.py,sha256=6IAoI3ggWlBhG0U7u6le7eLW4XvHCXEtKn1I8xivPTw,2135
 secretflow/data/horizontal/sampler.py,sha256=wTkHd8A_C4bLSm380P2Lg0e6LBeLXplAQdHDrXDNz1M,1555
 secretflow/data/io/__init__.py,sha256=GiNwroIs5A3LY5nKf5KR32Gay8e-zoVHo8_qKdVZEd4,627
 secretflow/data/io/oss.py,sha256=ma0WzVSQO37GBDI7AmHQByM1eUtXRMMBL1z3CxoM6ag,2112
 secretflow/data/io/util.py,sha256=fJ0Onq_8Hs8i19MeV1bZgwcLG80OnqCmXUaTHdubEnI,2501
 secretflow/data/mix/__init__.py,sha256=h2bB-DvEkqUeUINstjjMvNzTEOxrwDpp3DML2oD2RoU,691
 secretflow/data/mix/dataframe.py,sha256=vAuf-CVuCrG6U5qUtbcwdv-N2I6ORLzGdHgna7-oRuY,15054
-secretflow/data/vertical/__init__.py,sha256=lvsakfHAkSdOtxQ88zhVftq5opqHQbKWs_3avYr5-xc,716
+secretflow/data/vertical/__init__.py,sha256=2ebdxD1yKTCQu5kEZGeQTjCM7t6G-oERwM5bK-rwOiQ,694
 secretflow/data/vertical/dataframe.py,sha256=EAzfauTNycPHfZHteBf-FLVOqiBS0VuLkpzf7mtjF5Q,22944
-secretflow/data/vertical/io.py,sha256=DNJCLONTIQx66Vg4UhzFl2pSzokApKtG-cjDhI-c81U,6972
+secretflow/data/vertical/io.py,sha256=3OFeKanrbIv_BM4j6drGV_WTa8Vo-kYsY_MuzyvIf04,6550
 secretflow/device/__init__.py,sha256=BEn43Wg3C8Pr9-f1ynF-L1HJ4IVKC8R2tU-SqnOOpp4,745
-secretflow/device/driver.py,sha256=9Xqp_Z-jqVH76V7m83jqbtgy3o7uG5ihKALq0lpFj-U,21823
+secretflow/device/driver.py,sha256=ZsK2Re8-AM9qz9oOhgnM7PF_ffA9ssKG825_Qt8DrCM,22241
 secretflow/device/global_state.py,sha256=5C6cysrgRG56oB93sBYHr2afkTMjlM3rL1VlD6sBuvw,2981
 secretflow/device/link.py,sha256=s8Dsx-UQ2XcbByFauiix2TXUWIosXhZCvB2T1dtPRJ0,10795
 secretflow/device/proxy.py,sha256=DZTukc-c3-PmdJwpTgoUY7HqaxNWkdGYIepts87akDI,8100
 secretflow/device/device/__init__.py,sha256=WI_jmQfWPY5VQu-b-cUbqK8SqjXHYdRG-NF4iIFTEgc,939
 secretflow/device/device/_utils.py,sha256=H6q--hVRw7lQYzSbIenVM1vcGheQY8kNVK-KOEg-13w,889
 secretflow/device/device/base.py,sha256=kvlkLFmZ0fmAsGQOTR5NC3X6YAnc9NecAPSS_UNoSGQ,2264
-secretflow/device/device/heu.py,sha256=V9d15fladVqHq3GUccbGLKnfY6Ow7VHzUC_aOMbxXc4,22932
-secretflow/device/device/heu_object.py,sha256=gPd3ZEKWxDFcWTNLwKDycl66-7fZXWKT9c3bq1wnB9Y,6096
-secretflow/device/device/pyu.py,sha256=T8SoyTiNIUQWj4OmBgqV7EFZxFkS-q-OxV54Zo0eRkU,4693
+secretflow/device/device/heu.py,sha256=G7qc2I8-IaWS0tXwCrRHbTHZ0NUWsuFi3xUWnMPlB80,23141
+secretflow/device/device/heu_object.py,sha256=VS1hEcb8NDV1jW_mn7Wh249BBjEJX14mkNnlshP4ixg,6881
+secretflow/device/device/pyu.py,sha256=Xo3ioCVvB4w8pFdmKGPToTitvUy2uA_f-PvIGj1iVYE,4706
 secretflow/device/device/register.py,sha256=-2PA4a01mX5Rlh-bbNEgto73P_3c4EtaFd1gbdUVICc,3589
-secretflow/device/device/spu.py,sha256=-rajnMqufgh8QjfO3Fykx2wvcBLytV0-rCH3EMYbF9U,67451
+secretflow/device/device/spu.py,sha256=qw8skajQE8lpBe2GUSwOITxqy-VSitjH_zHM8W3p1F8,76168
 secretflow/device/device/teeu.py,sha256=uUUehACeu-pzEl8zFIcgnzlmv6CC2xG2VbQcDKeoavE,7667
-secretflow/device/device/type_traits.py,sha256=5jU1LTot9DrQl2meNc5c3mt-_NSnpKnLrHsTUZ-azUI,2410
+secretflow/device/device/type_traits.py,sha256=etV0qPB4-4ermenT2y1BPkmey1VW8CZx8v7El0B_H_c,2410
 secretflow/device/kernels/__init__.py,sha256=gWgvZx-2t6_XfGQoVdC9TQNyF-Jm9I9hnn-iVUcNKlE,638
 secretflow/device/kernels/heu.py,sha256=OEVnoebeKU6Jxua1yOCsEPQlhHUlYiQkvpwvvElGkrk,5716
 secretflow/device/kernels/pyu.py,sha256=ftF1UKfABWR84ZjpgvRw5Jnc689SZnOivrpQ4-UQ77c,6842
-secretflow/device/kernels/spu.py,sha256=i6hwS7-3cx0conMPn8OsEdP1H3ohobdD-4ESaWiiI1U,16767
+secretflow/device/kernels/spu.py,sha256=3pMYiRBntss8wlq4Zad8ryKdWEtSEblVibdKewDULlo,17619
 secretflow/device/kernels/teeu.py,sha256=o6T8NLSpE9skxJ8eQAqcA4Dk00kC0mMjCzcmkcM1dQc,923
 secretflow/distributed/__init__.py,sha256=lemgXRrzin237GO_Srg0VjaXv0PeJ0daxPVLJT78Qns,784
 secretflow/distributed/primitive.py,sha256=3cSCX6kwIjnB38zzO7TRk9EACZamOhe-NeBg66Yy6p4,6373
 secretflow/kuscia/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/kuscia/entry.py,sha256=Q813urkkdh9-fIgoDMoM21B3lPtSynCnWmB3zwFeGLI,3722
-secretflow/kuscia/task_config.py,sha256=KV-SjDQmkKPxfsWEP25iwFQCYgHXKTn3grKojI874Ic,5912
+secretflow/kuscia/entry.py,sha256=IBj2lsQ6nBTPFXvmnw2Hyx0CWLQoqsKT0ayVy6V-BCE,2380
+secretflow/kuscia/ray_config.py,sha256=KVW4VPXLEk2iZBBJf6ZQmHVoYrOn-F2IG1-Y72ARvis,3651
+secretflow/kuscia/sf_config.py,sha256=Ac_U_7u1L2JJw4DOq1kYCYgjThbHeIzpM0p_caQ0nfQ,4495
+secretflow/kuscia/task_config.py,sha256=IyQGi1gHyu354S9Zld-H29_oCRFEJKk0kEeqPFBEbhU,3229
+secretflow/kuscia/proto/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/kuscia/proto/api/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/kuscia/proto/api/v1alpha1/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/kuscia/proto/api/v1alpha1/kusciatask/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/kuscia/proto/api/v1alpha1/kusciatask/kuscia_task_pb2.py,sha256=eGrFApnlcfpDcZgNgDZqsRMDZt7kBRGEYz-Kbhyyp5Q,11973
 secretflow/ml/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
-secretflow/ml/boost/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
+secretflow/ml/boost/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/ml/boost/core/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/ml/boost/core/data_preprocess.py,sha256=QI0bhtPvJP271H0nx-tJxbUpAehOMHF1cPCmNnIX6D8,2827
+secretflow/ml/boost/core/order_map_tools.py,sha256=2pvIriLrSQlsi-lC-R6Av_2mv8C8GkCHdvrWh9Sk27M,3161
 secretflow/ml/boost/homo_boost/__init__.py,sha256=MWOYs8dgKs5CBSGS6V95PYd3_j5QGxRvota2xXDXjfk,654
 secretflow/ml/boost/homo_boost/homo_booster.py,sha256=QSmPBfQy6zh0w7ImjApumrKsHMvED2mB8AILtFroQpk,9580
 secretflow/ml/boost/homo_boost/homo_booster_worker.py,sha256=BRW8t729QXx3mhd-BhMlDAWDNsSDfVnBoMit1F5jGXg,7462
-secretflow/ml/boost/homo_boost/homo_decision_tree.py,sha256=tL9ZNnCzEtItkBcm2IOzvyld1oso0z0FUHIa6XF-uZI,11166
+secretflow/ml/boost/homo_boost/homo_decision_tree.py,sha256=Ka_E8lf7PAJamy6Sfa27_L18KOt68SE5P8E7w7RuAHo,11134
 secretflow/ml/boost/homo_boost/tree_param.py,sha256=y7-5wrirBUU0qTiARbf3UMPTFHtVeawXVOblX9NTb7o,3043
 secretflow/ml/boost/homo_boost/boost_core/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/ml/boost/homo_boost/boost_core/callback.py,sha256=VMFBtZA0Kxny-X_QwwMSX4QDSMkIqjtq6jn_tNQe_ik,4365
-secretflow/ml/boost/homo_boost/boost_core/core.py,sha256=scOVjAq3w-wIadR7BkdcwA0YsXyscVqpXeMTJObJPw0,7200
+secretflow/ml/boost/homo_boost/boost_core/core.py,sha256=s4z5Cw4pxAnPg6PIoKr4TCE_MxbYdIE9FDEyYn9RI_o,7248
 secretflow/ml/boost/homo_boost/boost_core/training.py,sha256=dOpDWB2anPL0PCLn5GyFO15Eu1xYKzxVA04gYplESuc,9292
 secretflow/ml/boost/homo_boost/tree_core/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/ml/boost/homo_boost/tree_core/criterion.py,sha256=4JERxTXcVG_Ad_bJP7OgqyOnCkh7H3RN-6gPVtX7rS4,4429
-secretflow/ml/boost/homo_boost/tree_core/decision_tree.py,sha256=ceRTiHzizRqtj8cfCsHIpv4Jumo7QsT4Gju2GuW7F2c,18577
+secretflow/ml/boost/homo_boost/tree_core/decision_tree.py,sha256=1TzZJ8oFAJG8QbkeHHm5tGClrhqN8mRU7yvC0TyIWhU,18576
 secretflow/ml/boost/homo_boost/tree_core/feature_histogram.py,sha256=365Zuy8Y9PczRYMHYbR1QrmxDUBWZ68wca1aQJWBxi0,9371
 secretflow/ml/boost/homo_boost/tree_core/feature_importance.py,sha256=RtYMeKZ4aA8FnihFaTGTfvaeOh0098kvwahY9aj3bY4,2535
 secretflow/ml/boost/homo_boost/tree_core/loss_function.py,sha256=DGW0AuQuZe64a-SQPfr8XKEknMeW3HW-cK4K-ivc_m4,4218
 secretflow/ml/boost/homo_boost/tree_core/node.py,sha256=oogyME57SuPl08PcXtUXtK37Wqsbb7LFSuQ0gp52n-M,2060
 secretflow/ml/boost/homo_boost/tree_core/splitter.py,sha256=pK0qK3Ia5LMziazmdBHTRtum0VjcyohXbCq_nm-qDHA,9846
 secretflow/ml/boost/sgb_v/__init__.py,sha256=8_0WO_-Pu_j0TzFvQVVYgqp74T1mdDtOSQVYOUJPnRY,712
-secretflow/ml/boost/sgb_v/model.py,sha256=xS7ZP8JQUi7AVW1t7F4sC7Mn982Oj70VnY1q-qvyWJQ,7826
-secretflow/ml/boost/sgb_v/sgb.py,sha256=EvC4RL98OpY8Mk9REhp5RDXBfedohkgah3xRkTL1b2k,19839
-secretflow/ml/boost/sgb_v/core/__init__.py,sha256=-4CUOQrpg8PEoHg-xqdm8R3kCTLSzrH_HFOB8evjdHo,584
-secretflow/ml/boost/sgb_v/core/cache/__init__.py,sha256=-4CUOQrpg8PEoHg-xqdm8R3kCTLSzrH_HFOB8evjdHo,584
-secretflow/ml/boost/sgb_v/core/cache/level_cache.py,sha256=5atsIrrJMigAFODeTScRGuG3ngdl_rrcVZ3zKbEAGxg,2561
+secretflow/ml/boost/sgb_v/model.py,sha256=B3ikfm8PlnNWAv0zkQv2qoRddUoUSAALMdeiaXK5zU0,7830
+secretflow/ml/boost/sgb_v/sgb.py,sha256=5cgaLRBMh6lasLLKT0U7r-rMKmnVgr3a_Bu51TJYA6c,19455
+secretflow/ml/boost/sgb_v/core/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/ml/boost/sgb_v/core/cache/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/ml/boost/sgb_v/core/cache/level_cache.py,sha256=ZgUQVfqg1X-BSnFrJY9R21olyMwjo6tg-ImwgmXJYL4,2642
 secretflow/ml/boost/sgb_v/core/distributed_tree/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
 secretflow/ml/boost/sgb_v/core/distributed_tree/distributed_tree.py,sha256=MIzNQfoqHovdlYahLWNeHjAMkYQXdrFIwCgZizg9-PA,3817
-secretflow/ml/boost/sgb_v/core/distributed_tree/split_tree.py,sha256=A-JKUcdwaxmTS5VpT1LYIC7g54F2AAU1T4K_4p3gJF8,2767
+secretflow/ml/boost/sgb_v/core/distributed_tree/split_tree.py,sha256=mCzz7kCLoreK7U8x3EKzIVLm_DgbmlUTYpj5aRWXOAA,2768
 secretflow/ml/boost/sgb_v/core/label_holder/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/ml/boost/sgb_v/core/label_holder/label_holder.py,sha256=xyhkZpZlxEfU54qhgR7qO3lXijvfw56P5QAYOFL39dY,9416
+secretflow/ml/boost/sgb_v/core/label_holder/label_holder.py,sha256=LL99fjyacO-8GdBtnX5l9FQbaFM4yqGHS7E6a23zzhY,9642
 secretflow/ml/boost/sgb_v/core/preprocessing/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
 secretflow/ml/boost/sgb_v/core/preprocessing/params.py,sha256=sX4DS4DPxFF3QsyJBfUuucnlkoMu4pZ6UqfKvnKD9XY,1238
-secretflow/ml/boost/sgb_v/core/preprocessing/preprocessing.py,sha256=of8cB_3GEHWzszCDKFgxQVv5Vt3rQaliLtKKzLLf9TI,3355
+secretflow/ml/boost/sgb_v/core/preprocessing/preprocessing.py,sha256=lfe99BlRlVBvjz7pvP7DDcgmWZ1XFpQig4IwCuis6rs,2432
 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/ml/boost/sgb_v/core/pure_numpy_ops/boost.py,sha256=4w7YpOgCE4pEERYqTFFpQlSRwoj2yzMZXR_CX2V_QPw,2746
+secretflow/ml/boost/sgb_v/core/pure_numpy_ops/boost.py,sha256=yrHE8bJRhML0YQcr0suAJu3FlHATZwPyuUfqzGpKWEw,3706
 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/bucket_sum.py,sha256=oYgjkq2LEL4BPcIGFqYToA8kU8fgNVv-5IFi4kKwocU,1724
 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/grad.py,sha256=nfNO70mw3ccB-HfwBjhNp12QNg2b4PRS8aqSKJwZM-M,988
 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/node_select.py,sha256=8PoaQTt78nSHhZGaFTHlz4Yd6NSSQLKpXKy3Nebi6pI,2807
-secretflow/ml/boost/sgb_v/core/pure_numpy_ops/pred.py,sha256=H2exNOfvxuLpGgYPVUI0YwkF1unXYF9H0ooo7YBAg9k,1466
+secretflow/ml/boost/sgb_v/core/pure_numpy_ops/pred.py,sha256=Wtk00mM3P4D98_sxTEXs3y1gLamgu4w0uwBDhmtAqM4,1465
 secretflow/ml/boost/sgb_v/core/pure_numpy_ops/random.py,sha256=VgcOd9rmziLBxcBEIEtQMHjEV_uJAEWiUSZErKZaEvM,765
 secretflow/ml/boost/sgb_v/core/split_tree_trainer/__init__.py,sha256=-4CUOQrpg8PEoHg-xqdm8R3kCTLSzrH_HFOB8evjdHo,584
-secretflow/ml/boost/sgb_v/core/split_tree_trainer/order_map_context.py,sha256=s4gzLsaeFphTNRcCV5dejTG_B92Cs2yX1SFy3R_st1k,4714
-secretflow/ml/boost/sgb_v/core/split_tree_trainer/shuffler.py,sha256=dQRuKJ39V1tNfTHuIvvwae8fL8F1XbPu4CwAKLgfo7w,2631
+secretflow/ml/boost/sgb_v/core/split_tree_trainer/order_map_context.py,sha256=PjAWIsJa1FdrRDd8WOna7jpwccomJR9kCJX49iAwZ2c,2840
+secretflow/ml/boost/sgb_v/core/split_tree_trainer/shuffler.py,sha256=OeBZeRYLc1CTbFjeqhlsrs9ZgQDKlygztICVfxuVudg,2787
 secretflow/ml/boost/sgb_v/core/split_tree_trainer/split_tree_trainer.py,sha256=sxe3hJp9CBp2Ah5QQorTV9uTIWxk8_ncaScURkh37N4,4166
 secretflow/ml/boost/sgb_v/core/split_tree_trainer/splitter.py,sha256=be8BquAywE7IH4WUnALuWudtaX6OuTHq1oXRBK91cCQ,5057
 secretflow/ml/boost/sgb_v/factory/__init__.py,sha256=t7GyTozDqc-rZwm3_gwO4I9LMSoU9SHCnQX9Ku37y8Q,644
-secretflow/ml/boost/sgb_v/factory/factory.py,sha256=1wYcFqOhmcsSNi9vkjZ6hcLmbXvP3TbZL27Nhfk2kyo,4366
+secretflow/ml/boost/sgb_v/factory/factory.py,sha256=MIkOgbE9WTEwTHKHURRzjzH87i0QZ9sFVUwzlQPirVs,4329
 secretflow/ml/boost/sgb_v/factory/booster/__init__.py,sha256=MibEqwWWVnUZ4l99himNUDQPAvsfUFtA1LYMjdUK0sk,683
-secretflow/ml/boost/sgb_v/factory/booster/global_ordermap_booster.py,sha256=fvgJB-kEdSAo3aAG0dhtqonXcjrYPYGaeZr0MxVvkc0,4272
-secretflow/ml/boost/sgb_v/factory/components/__init__.py,sha256=nhERkbGWDgGNVM22IOxaA30LB93qSSr0FaFJkwHiWoI,935
-secretflow/ml/boost/sgb_v/factory/components/component.py,sha256=3R0iP7UoWEucjZJGoqehwkfI4OQ0kYwytTWnELkBtqs,2073
-secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/__init__.py,sha256=5D7NvxhKH-mTqrTnyvkHuFmmnL4kTgkmqV92sY_3VQ8,676
-secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/bucket_sum_calculator.py,sha256=yd6pARPlLoW10rqWjBqvekFEmXFuqer_pF1bivLZEOM,4658
+secretflow/ml/boost/sgb_v/factory/booster/global_ordermap_booster.py,sha256=7GFABQlEoJ05SAv5WMGGQQYqSUdAruaXVTirZeFtMV4,5409
+secretflow/ml/boost/sgb_v/factory/components/__init__.py,sha256=E0pZSZuufbw_IGmbgPktgBNtWFBFvOLjMDhGbYF5xOA,983
+secretflow/ml/boost/sgb_v/factory/components/component.py,sha256=uV54Z455BzSdeZ8bZ-ME6TB3TtImBSE4v5ho090ViKw,2010
+secretflow/ml/boost/sgb_v/factory/components/logging.py,sha256=DX-jo3_4iIOTNbtNUr9Z6Z9EcYZfmmUtjFURU2ADc_c,3194
+secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/__init__.py,sha256=gcSn648-zTb9QY9WnwAmObWxG2E8DXEwMo8rh4ZI_zw,780
+secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/bucket_sum_calculator.py,sha256=jYFXRKKwKVokPaUZcg6dd7uFG6SVKQBRRYMQPW-YDdc,4960
+secretflow/ml/boost/sgb_v/factory/components/bucket_sum_calculator/leaf_wise_bucket_sum_calculator.py,sha256=YCv8WWsxrr-SA73quhOMPDKiWmnjXU16aDFxIpGNTTo,5176
 secretflow/ml/boost/sgb_v/factory/components/cache/__init__.py,sha256=viINyNfu1NuwaOpD2B6jCm8JWlGPcpVf6kKCKaoADf0,661
 secretflow/ml/boost/sgb_v/factory/components/cache/level_wise_cache.py,sha256=ejglgBW52epHFc_Nq5UDTEs8w_oRVE7w6zrHKGVY8Y0,2051
+secretflow/ml/boost/sgb_v/factory/components/cache/node_bucket_sum_cache_internal.py,sha256=B6DAeWfsYkjoI8I1A035fFzKfoRPCGRJlWxDd5TvfAQ,1893
+secretflow/ml/boost/sgb_v/factory/components/cache/node_wise_bucket_sum_cache.py,sha256=rFQqCSKZnbhKKHKbn9-zoAEUV0t0BLVOEmrPmOjOTXQ,2583
 secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/__init__.py,sha256=pDTKnLq4lXZ9HcnFW_KbUDWttVyTyNl5Co8EL-Md-5I,666
-secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/data_preprocessor.py,sha256=8psvitOMrvgatVN_05M--PCFiklVBNixIM1iNg1Fb_s,2503
+secretflow/ml/boost/sgb_v/factory/components/data_preprocessor/data_preprocessor.py,sha256=yIFrktSuAmHXUDbGdN6LLgyj-2OMPoavDyknSgTonX0,1220
 secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/__init__.py,sha256=mJHnt6biEkZ1MRDSoMnP_ScuOVx4WNAkznK7vA5Tnjk,669
-secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/gradient_encryptor.py,sha256=GxGp8x70iP3fnIg7iNkRr5ZsPPIy8zX-NRtFrOlKWA0,4833
+secretflow/ml/boost/sgb_v/factory/components/gradient_encryptor/gradient_encryptor.py,sha256=w0xMa3dhomTGDwdxEiLApVAPM3clRvRGXADtNPQ_eNs,5190
 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/__init__.py,sha256=htivChBgoisIQ9radijKCiLE5RrYPxqb-6m7ch8oxNg,651
 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/leaf_actor.py,sha256=15D0j6h7CS0sC2lRr1_xrcwvOpQhxqklbVdMK090Kys,1633
 secretflow/ml/boost/sgb_v/factory/components/leaf_manager/leaf_manager.py,sha256=BJXnm5gTCiHwcpTUX6xZJLtRKBl1HBOUnjOdvWWhdA0,2588
 secretflow/ml/boost/sgb_v/factory/components/loss_computer/__init__.py,sha256=CQI2V2HnuYGKVDFPW18PFtTrCIr_OeIcDs_sUb18910,654
-secretflow/ml/boost/sgb_v/factory/components/loss_computer/loss_computer.py,sha256=n4a7ZEl15HwkXlf3QBpCEeaj5nyOIvxU_BuJZLrRTgg,2326
+secretflow/ml/boost/sgb_v/factory/components/loss_computer/loss_computer.py,sha256=qH0Kus8gGYXVozE-V5LlA_KiUfMzAR_t3ivfTaqRuRI,2651
 secretflow/ml/boost/sgb_v/factory/components/model_builder/__init__.py,sha256=q5AXXsaXtCXvySlnPclrK7-fQL4JrCO_ZMpFRm-hcP4,654
 secretflow/ml/boost/sgb_v/factory/components/model_builder/model_builder.py,sha256=1QlpCqCvpat0X6RtpoaYgfNLAYF6ojv2WOWUupzH85M,2655
 secretflow/ml/boost/sgb_v/factory/components/node_selector/__init__.py,sha256=Qv8b-_-bm0Ozfrz7WVCyYrEHl8Pbz_RcFD7FzoHWnBE,654
-secretflow/ml/boost/sgb_v/factory/components/node_selector/node_selector.py,sha256=-YOxdz3HHo0kM61Pw8lOjz5D8K-X2IplLzB2SyQIGUQ,4494
+secretflow/ml/boost/sgb_v/factory/components/node_selector/node_selector.py,sha256=vSTiPHPIJen-JQDXW1I3Zdqjb6z1xnCuKEkoPpM_Kwo,5865
 secretflow/ml/boost/sgb_v/factory/components/order_map_manager/__init__.py,sha256=m8_ADmhhYfJfwX3M6cEf8XUT0QI4GO5zf5jxwgbjuy0,664
 secretflow/ml/boost/sgb_v/factory/components/order_map_manager/order_map_actor.py,sha256=a2hsyM2KhfLOWL6Fsn7WA53vHGAOfLOpA6tEkvjUXQU,4121
-secretflow/ml/boost/sgb_v/factory/components/order_map_manager/order_map_manager.py,sha256=RnU-ZYV4nN079UTgw7RXyGMHtn7hB4-p2e2TxTaCKSg,4280
+secretflow/ml/boost/sgb_v/factory/components/order_map_manager/order_map_manager.py,sha256=lq1UngIpmcyzzre2T4SSTTAOR-t_ySh9IHC4e1vtpVc,4649
 secretflow/ml/boost/sgb_v/factory/components/sampler/__init__.py,sha256=pLaIVelZVEwQc6Xow_BauIPmmZFiD0BZdSA3UO5b6fA,638
-secretflow/ml/boost/sgb_v/factory/components/sampler/sampler.py,sha256=bf28U_-JQfEXPJ7-RJMMKtE8lZfpHTcJIp9Qhq6xatI,7180
+secretflow/ml/boost/sgb_v/factory/components/sampler/sampler.py,sha256=1oCC0xBQ-KUHcfZ9W4dmgwwXbZoCxlDGtNMJI1Kzce8,8221
 secretflow/ml/boost/sgb_v/factory/components/shuffler/__init__.py,sha256=8nV_hO0YjzMQDF3zmf9M6I8LNt_FU28DH_pnFBS2aRI,641
-secretflow/ml/boost/sgb_v/factory/components/shuffler/shuffler.py,sha256=S7zZlQJOZXvdJeA0ojjppLFoiHc2XVD4FlDCR7A3s-M,2468
-secretflow/ml/boost/sgb_v/factory/components/shuffler/worker_shuffler.py,sha256=fOD07fj03ESN74pzTMpxz1yY2kLX2XFO5C9tvMslKZU,1721
+secretflow/ml/boost/sgb_v/factory/components/shuffler/shuffler.py,sha256=PsNimg2eXDwguWy3i_auFD9BHu8Tn9TzIQpOmgNbnck,3498
+secretflow/ml/boost/sgb_v/factory/components/shuffler/worker_shuffler.py,sha256=4zjzO2eKpj8OGmIFbZh390-lvDeZE0zrSHMwcjgs_ag,2057
+secretflow/ml/boost/sgb_v/factory/components/split_candidate_manager/__init__.py,sha256=BQ88VjxxZuWHApalbkl3gR3Ix17OtRyVUGzcTBtylOY,716
+secretflow/ml/boost/sgb_v/factory/components/split_candidate_manager/split_candidate_manager.py,sha256=U_HhoRTNss_KnarkI01cQgZB9EaC1sBcahgYsdKsr3k,5248
 secretflow/ml/boost/sgb_v/factory/components/split_finder/__init__.py,sha256=UqJLiIcJs-7gyrYTfAPlKMpnGEsuiky1dmkhlrncucM,651
-secretflow/ml/boost/sgb_v/factory/components/split_finder/split_finder.py,sha256=_f9_4yPzNNwbKmUYpKYow3HSrMt5mHwwuRzwkmnj9gQ,3265
+secretflow/ml/boost/sgb_v/factory/components/split_finder/leaf_wise_split_finder.py,sha256=YJlthUGjjjhyHPzQkn5qjiyBDqr2TT0eVEynv7vPaM8,3339
+secretflow/ml/boost/sgb_v/factory/components/split_finder/split_finder.py,sha256=U22rTBbHk2V7xyFmleNMaQP_bRYIBtF3_sRByYTZhHk,4252
 secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/__init__.py,sha256=8zWMI0KJjM_qVg8hlKQrPuIB8rL64mSSv3Zsawwl414,667
 secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_actor.py,sha256=ctrBWbE-Ra2Isn02l8IlNZgNhWH3BcpemsDp1tgx64Q,6171
-secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_builder.py,sha256=7JxfNmKzq-G3ayuVBXUWkk1A037-wf463u8G_gDChJQ,6550
-secretflow/ml/boost/sgb_v/factory/components/tree_trainer/__init__.py,sha256=tjAfTRmJ8XYZ-hr8hNYoGwQeIdVwyjghaUdLO50dnwI,147
-secretflow/ml/boost/sgb_v/factory/components/tree_trainer/level_wise_tree_trainer.py,sha256=7iB2nrGTy5rPhaTm-qaF3jVONMQqEmf3ty48Cc1fUAE,10486
-secretflow/ml/boost/sgb_v/factory/components/tree_trainer/tree_trainer.py,sha256=ykeYkehW1doUS4o1alx07019siyyD-Z_qJq68DasSXg,1142
+secretflow/ml/boost/sgb_v/factory/components/split_tree_builder/split_tree_builder.py,sha256=yzW_eKVdsrqVUu7s4c3diFV8Algoz_yZom_gJRuU4qQ,6969
+secretflow/ml/boost/sgb_v/factory/components/tree_trainer/__init__.py,sha256=IlYcQbsoiejlqAmOMSd-l0CCRlUI7nmjgqTZfq1YCIc,226
+secretflow/ml/boost/sgb_v/factory/components/tree_trainer/leaf_wise_tree_trainer.py,sha256=hlJnKSaJWhtsVglNx9XYO_C-ZTRzWj9f06A_PrMayfg,12111
+secretflow/ml/boost/sgb_v/factory/components/tree_trainer/level_wise_tree_trainer.py,sha256=WioZFdkbVU0ogkxHUkki69Y-4KaRslZ3KWPgoDC_qHQ,10901
+secretflow/ml/boost/sgb_v/factory/components/tree_trainer/tree_trainer.py,sha256=py3_1yD4wP3PEeypwcZPONO0vBg_u-AWBbSLsD_ub7o,1141
 secretflow/ml/boost/ss_xgb_v/__init__.py,sha256=mWFWnNM-indGXq7-H80y9KisAWayUQtH0MV0nVG0ymE,661
-secretflow/ml/boost/ss_xgb_v/model.py,sha256=-ZKihB60XDRPbn2tqXRwQdZhKY_-RBboves8Dmpa6LY,19885
+secretflow/ml/boost/ss_xgb_v/model.py,sha256=SfdnjIjCWukpb90zF2QXCy3zSoeLyaFprnZROmpmHas,19627
 secretflow/ml/boost/ss_xgb_v/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 secretflow/ml/boost/ss_xgb_v/core/node_split.py,sha256=_DQ01D3dn-SKpJAwS6NNDKJXNp1Cro41Fpip_AzKO1U,8801
-secretflow/ml/boost/ss_xgb_v/core/tree_worker.py,sha256=CW9JWpwmCLdpNjxXOvChgLIM8MVoxVjW4PvdFwMqJdI,9885
-secretflow/ml/boost/ss_xgb_v/core/utils.py,sha256=DQZ4xkE_6UhQIM0Wh8gfVDFG7wPlfsNV6mGtdyOu76s,1513
+secretflow/ml/boost/ss_xgb_v/core/tree_worker.py,sha256=lUBxaNang_IdoCWwr5ryWE9WOEyMcuiWxAW6iu1tjQM,7747
 secretflow/ml/boost/ss_xgb_v/core/xgb_tree.py,sha256=JNeEdH_Boe7mJ8hNjCu0nnuNm2LIfIdiNHBWmDIPF_w,980
 secretflow/ml/linear/__init__.py,sha256=S6Te5j_pKa2N860u3hrjDaxnN2hiW3c_On6JDidhxQM,1013
-secretflow/ml/linear/fl_lr_mix.py,sha256=0rrB_ZOLwqNIOEloWJe7upjqd-JOARW0VaAAklBJXaI,11993
+secretflow/ml/linear/fl_lr_mix.py,sha256=FN6S7Gmvjgm2mENI_HCC5nQSNwCPaUIpty2pq5by2ps,12354
 secretflow/ml/linear/fl_lr_v.py,sha256=VVcwXkpAVDuU_sVocRiLb_QhLN3m-Kv75UPrP-hMw2o,19143
-secretflow/ml/linear/linear_model.py,sha256=UX7sn9dj60-YVkI7POpiaRbFphntrtje099rOFFZHFE,3129
+secretflow/ml/linear/linear_model.py,sha256=RV-X8PJ9mh1GlZQCNv_-oBhSolMRpFgl5Tlj-cNNEJA,1373
 secretflow/ml/linear/hess_sgd/__init__.py,sha256=tqLher8w0NHhOe5pb7Erfdg8Woa6793desVvSkKRJCU,673
 secretflow/ml/linear/hess_sgd/model.py,sha256=2XUnobMXen7SKvai1eC410l-WdWjD9mMS3a3I-Mr1oQ,13354
 secretflow/ml/linear/ss_glm/__init__.py,sha256=SXmD8shOQpUA5Dp89bX5yNSDThcsWbeVTKMhtLuxRJw,639
 secretflow/ml/linear/ss_glm/model.py,sha256=znhxnxq5e0k3bLctH3WegAz6E418Z-vS-J1D3DSEKuw,23754
 secretflow/ml/linear/ss_glm/core/__init__.py,sha256=Hz7_m2Fjd5Efyq_PWbvAAGFaM33blcDFMGURY1v0Fq4,233
 secretflow/ml/linear/ss_glm/core/distribution.py,sha256=fUizQ1UYW8OyF6Vs5X6Wu3Ue3_7NPaU4MDFRCfGWwQo,5287
 secretflow/ml/linear/ss_glm/core/link.py,sha256=DXNbYAyxUzheTplGMtqjOOYclhlol0wWqC5iDH_yQTM,2950
 secretflow/ml/linear/ss_sgd/__init__.py,sha256=hdNmisOmrvblwF4XbF2v8Ddv3ldHzbkYjW2f5rhkM5o,653
 secretflow/ml/linear/ss_sgd/model.py,sha256=JSlUpHLBNeniq04TRIDuHRJ3WzFBB6kGSKzysej-pp4,21895
 secretflow/ml/nn/__init__.py,sha256=iOeB3Fi78uSNTBvlkmcpgkRLo1IPw7ipn1yj6rQrXu4,698
-secretflow/ml/nn/metrics.py,sha256=gBobUmtRhk3ZKUAqG1ahKpSe68pOCTQq7KdQiqOKN2g,8064
+secretflow/ml/nn/metrics.py,sha256=ad-02DE5ljcDYVosAjcH6P4WK2_2nWFmav0JY-9XRbI,8067
+secretflow/ml/nn/utils.py,sha256=h7P7qh8GBCMI0BSR-8vAazY42kPLnB6A_oL2Qj2Hono,3018
 secretflow/ml/nn/applications/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/ml/nn/applications/sl_deep_fm.py,sha256=w252NcasCrQwgiO1pPOjZ4kh9Yrld2HW3-Q9I14-7eE,5261
 secretflow/ml/nn/fl/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/ml/nn/fl/compress.py,sha256=Vuhbq4PCfEy0rsuLEEQNAshlr6Qxl14MBRgQO7h2pLg,1743
-secretflow/ml/nn/fl/fl_model.py,sha256=At5sXpxFcykejqb1TTWAOkjzhgL8yOJhNNqwJa43SE0,30837
+secretflow/ml/nn/fl/fl_model.py,sha256=xAjHm8Y5X1OmJQL6of9MN3NFPmFfHcmZWkh8xz79L3g,30826
 secretflow/ml/nn/fl/strategy_dispatcher.py,sha256=C2uR__I-aepXfC8RlOKue9Y_YBo7wnR5JISWegEZkJE,2152
 secretflow/ml/nn/fl/utils.py,sha256=ZzX_JJqba9f7O7cuc7OhoAksWM7jyfmYD1tFlkLjJMo,3279
 secretflow/ml/nn/fl/backend/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/ml/nn/fl/backend/tensorflow/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/ml/nn/fl/backend/tensorflow/fl_base.py,sha256=TAwxMXhX5euL4jU7PrDXdKAYz5ce3NkTZ4_tQKQ-oYA,12678
 secretflow/ml/nn/fl/backend/tensorflow/sampler.py,sha256=noozDHkSAhHRWyui5YFrwEO9hAtn9mtQyESsF8Ooy7o,4369
 secretflow/ml/nn/fl/backend/tensorflow/strategy/__init__.py,sha256=HkHwvlJJEqZUA1kQ_TtPXDhfRu7cygrdG4X4R9pp6mg,904
-secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_g.py,sha256=uCTNkOEQHhQ5l3mz6RHz5nhUfyBni3TS4czgQPhHkH8,4073
+secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_g.py,sha256=YicDbuRGbnBtWn8KyElIMjP8SqKHY8MZOH_cAIx7TyM,4071
 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_u.py,sha256=I8pNc5zYvg-mExDfuI5FprvUze5lwSzHdCxJQc5lsgg,4105
 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_avg_w.py,sha256=0-3BwO1Eb7Ewd5WXITiEfnTGjTkTTcyjBbeIHGUe5DU,3834
 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_prox.py,sha256=2IqdzPwyYETf7SfBUbpWaEqCKxVL7_qQAjMK7R5Wk28,4677
 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_scr.py,sha256=fJJSAhBDBwhYEL3nnRamOkI-CgSm533BXqfkUbHSdmM,5579
 secretflow/ml/nn/fl/backend/tensorflow/strategy/fed_stc.py,sha256=986SjH0AH1y9_1VogzDm_4VPM74nkUFVPc8kWbxN840,5453
 secretflow/ml/nn/fl/backend/torch/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
-secretflow/ml/nn/fl/backend/torch/fl_base.py,sha256=Zpr8WQGLzQEo8it5de8-p22w2Zc0SfbSfVg9suliG3c,13406
-secretflow/ml/nn/fl/backend/torch/sampler.py,sha256=r6Wkw3LdkfcHo_cv8iop220ZlugCH25_0Yyj7mCnby0,3606
-secretflow/ml/nn/fl/backend/torch/utils.py,sha256=2kL3E9kEoAGUV05-ntG_3iujuQ0gy8-C_9kYwr0q_aU,2710
+secretflow/ml/nn/fl/backend/torch/fl_base.py,sha256=u18Uas3uEMtMBFmEYGKJ7uZ6J6cA0tkAgHj1oTT2694,13393
+secretflow/ml/nn/fl/backend/torch/sampler.py,sha256=arMJpmuMAV5wUsk-faqcKZ0y2Vb_pmCt888HCGkEUTs,3605
 secretflow/ml/nn/fl/backend/torch/strategy/__init__.py,sha256=RgjI2iZFjusgZ25_8-s2iNIyUsAbUjK3SaUJGoiDPhc,904
 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_g.py,sha256=9WkDVZ69S8jm6w1KHMbCSYu5w0ddFiE1xekDo6FSzp4,3482
 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_u.py,sha256=7oSPq97gpMYJ6QgC-UVk3YkW5j21MOseXOzr0X2PMt0,3324
 secretflow/ml/nn/fl/backend/torch/strategy/fed_avg_w.py,sha256=LpJBwjb6r8QGVbu48ook0DUrqTh2OMNFRkI9aBFYjlA,3381
 secretflow/ml/nn/fl/backend/torch/strategy/fed_prox.py,sha256=DBIdG6LQo3ZXM4YkbSzG3hpUM0TILORyhfi2wF4KF7U,3838
-secretflow/ml/nn/fl/backend/torch/strategy/fed_scr.py,sha256=zo8ZtKnOLj9QeI9utApthejtcvIxs_Il-oK9u7w-bds,5266
-secretflow/ml/nn/fl/backend/torch/strategy/fed_stc.py,sha256=MqV42jJewc5_zB6kogIOYr4VYckTu_NTlDHkerZv0R4,5275
+secretflow/ml/nn/fl/backend/torch/strategy/fed_scr.py,sha256=UMNem1LWcHk8yb0Rx90fMCmIm-LD9GbsnEwVh1LQz3g,5249
+secretflow/ml/nn/fl/backend/torch/strategy/fed_stc.py,sha256=12vUMonxNQxUmcPNYKlfAFfARE94nTifrfxeE0rm9yU,5258
 secretflow/ml/nn/sl/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
-secretflow/ml/nn/sl/sl_model.py,sha256=uC1CKI8Nyasov0I8ShtaNtauw9nD1kdO7k6q6w-qwqU,28640
+secretflow/ml/nn/sl/sl_model.py,sha256=0o699QDpNWuDWifC0S-ds0WGiITlPRQE4fQoHJBddhI,30239
 secretflow/ml/nn/sl/strategy_dispatcher.py,sha256=1Sac34P5sXSlZKJqYM2OvuJcQNt9KHjcOZ5A74QzJ-0,2395
+secretflow/ml/nn/sl/agglayer/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/ml/nn/sl/agglayer/agg_layer.py,sha256=TmEdjoLX_sFzeg4lITEIppWzEiCOUIw8IRNA0GGD0CE,15812
+secretflow/ml/nn/sl/agglayer/agg_method.py,sha256=MTkZbyLUkauDbkE95Vtf6iW6uxA1IH6gV6uPeiv3wyI,3432
 secretflow/ml/nn/sl/backend/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/ml/nn/sl/backend/tensorflow/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
-secretflow/ml/nn/sl/backend/tensorflow/sl_base.py,sha256=z276tkAdillmuyHCL6GuT3iM7cggh8_umVrHc8G7eXc,34424
+secretflow/ml/nn/sl/backend/tensorflow/sl_base.py,sha256=FnzSET-yTvnN11FaiB-FWRlMhKBf6IMWAisipjmXKOw,27575
 secretflow/ml/nn/sl/backend/tensorflow/utils.py,sha256=My5jPf99yW11QGgp-XRAwMv7TdfsnxL8JOnMorcwiUc,4487
 secretflow/ml/nn/sl/backend/tensorflow/strategy/__init__.py,sha256=Wiv8YukYUdZMHtdjpFdBD7tPt0yiodlUiMkgEdpqWnc,753
-secretflow/ml/nn/sl/backend/tensorflow/strategy/split_async.py,sha256=lbgw7N3HjDWqMKBd7SryJuvJQ4cQDlN3IhGqMsGyGLo,6773
-secretflow/ml/nn/sl/backend/tensorflow/strategy/split_state_async.py,sha256=7TGyI9oUDNTXuUBJKHGJiK9DyLd3chpEF-udkIKvVrw,5162
-secretflow/ml/nn/sl/backend/torch/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
+secretflow/ml/nn/sl/backend/tensorflow/strategy/split_async.py,sha256=IsBY3J7mq1vRCXhSBDktMXeLb6OI-OKtsgIDmT1Rvis,6210
+secretflow/ml/nn/sl/backend/tensorflow/strategy/split_state_async.py,sha256=Vbqc5EhsDkkVpIYOUlWi0Q4YL6MnixctBB2I_Y7A_0s,5140
+secretflow/ml/nn/sl/backend/torch/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/ml/nn/sl/backend/torch/sl_base.py,sha256=_uyh5AKRBvw2_R9IhIJYWqLTBjkGuxphx9phJhp2UhE,24467
+secretflow/ml/nn/sl/backend/torch/strategy/__init__.py,sha256=4XLIiLitj8RCWQiQrBuqO5vN4lrZ1z1smdPgaOb-Ky0,652
+secretflow/ml/nn/sl/backend/torch/strategy/split_nn.py,sha256=UAwQZhxlSdahr2QrBAi0tJ9aAzSFOrRWh1A7Xps6v3k,3569
 secretflow/preprocessing/__init__.py,sha256=WArCKEUzlmqFHl08W4XvmFNSR24fShDAmUH3uF_cexk,923
 secretflow/preprocessing/base.py,sha256=hi3nD9aE7c4gNyfdhrOdHVoZ6KKugP8GgUqziEM2ddI,1231
 secretflow/preprocessing/discretization.py,sha256=U5iTyPDKc13_-ZiaNxXCmImUs4h_DKhR3cSRbobSkh8,11845
 secretflow/preprocessing/encoder.py,sha256=uUPDtydfMUh2gGmx1ZQyQBH5moMTsuvIpkYJEVUOQ8c,13154
 secretflow/preprocessing/scaler.py,sha256=-8xLo-suvMmiDbAONdRR9kbKv9BGTX28UQ1pCooHXlU,14116
 secretflow/preprocessing/transformer.py,sha256=1dlC3DVSoARXphMa2x2_sxbhkiVczRlElsDaAN7-aT8,5162
 secretflow/preprocessing/binning/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/preprocessing/binning/homo_binning.py,sha256=0lsDRvj4vUavSajUZgt5TJh__q-MIt6zkAYyo6fkVnk,7218
 secretflow/preprocessing/binning/homo_binning_base.py,sha256=wHcPdvgbPTrVMUP4ajYviFybnuixYi2gxwmkjJikHxs,11274
-secretflow/preprocessing/binning/vert_woe_binning.py,sha256=fzuKZRpaZMIRjmXhW91cUKjKkil-ocCe_2OB6rJ_vjg,10841
-secretflow/preprocessing/binning/vert_woe_binning_pyu.py,sha256=Qqcdg6CcmHKDSGs6vgmsJH1HxYwgZiKMMK-sNMtkevc,22492
+secretflow/preprocessing/binning/vert_woe_binning.py,sha256=JDzW2x0MmDIQxghfQiZXmR8ONL3lN_7xOmBaoqa_kvM,12444
+secretflow/preprocessing/binning/vert_woe_binning_pyu.py,sha256=byQxZEADI6syOvLTT4rZ8BheYkYfnL27VSgEKidK5w4,24664
 secretflow/preprocessing/binning/vert_woe_substitution.py,sha256=1wSHMFMUYIHHAR84Bsnrpw2t7zTuikQ5rgfRxacV2SI,3503
 secretflow/preprocessing/binning/kernels/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
 secretflow/preprocessing/binning/kernels/base_binning.py,sha256=_0whbDbFJ4wL5lxtacAIQTikDcmCKIhHk9p2ku65shs,2524
+secretflow/preprocessing/binning/kernels/chi_merge.py,sha256=MtsKkYLkt1KCyW48qyh384zO5V65lGRHP0H2M9YD-i0,5281
 secretflow/preprocessing/binning/kernels/quantile_binning.py,sha256=ZZqP7k4vSxyY1eQUvcNZccjda_eFsVWjVddZhACF0aE,5291
 secretflow/preprocessing/binning/kernels/quantile_summaries.py,sha256=wIzrTEr8goAn9sMOdFdhVrSq3npChJrpOXlyQpkzc7E,6517
 secretflow/protos/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
 secretflow/protos/component/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/protos/component/cluster_pb2.py,sha256=cVdEeDflPMU-h-UJVnBjhra9g5leEA7tDkVI9k7s774,18614
-secretflow/protos/component/comp_def_pb2.py,sha256=8qcyLO8wDEgQNxKNk3Cs3FPfnHnHD_e3TSS3oAXaTRQ,48160
-secretflow/protos/component/data_def_pb2.py,sha256=Gi-h1PnHWo_f9oHcQjG0gR5X_LDcxMNbnQgG3NZyT8o,12421
-secretflow/protos/component/evaluation_pb2.py,sha256=KIL-55tCQND61w77GxRVkbF6KaWMBWzQtBDTdwVaHm0,11115
-secretflow/protos/component/node_def_pb2.py,sha256=DWEVii3uIZ_NyaLHWk067Y03OGnOMHAPN_YlNAl8dHo,29124
-secretflow/protos/kuscia/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
-secretflow/protos/kuscia/kuscia_task_pb2.py,sha256=7pWQeYp9iOcKPlsF_70UOXU2X93f7abv7G2a0JBWBcs,11123
+secretflow/protos/component/cluster_pb2.py,sha256=hAnomp8SrO7KidUKLw8p_6NZPlZxBiRkH-FnkPwg5z0,22818
+secretflow/protos/component/comp_pb2.py,sha256=TWLYL0sh2sr7j8_K9OwemQohf1VDG-Am8lyi_SuopXk,35269
+secretflow/protos/component/data_pb2.py,sha256=mwiv07BXkRN56lReNQvewmR-GCQ9HJ7uHuDva9oZa7c,19380
+secretflow/protos/component/evaluation_pb2.py,sha256=DfZVEckVDotWkgAoCAYnejAXDyorZI7gmYAPfLZndDY,7199
+secretflow/protos/component/report_pb2.py,sha256=JIihz1WbDKX9HDn7NE97_mlOJpTsBm-_ADlxQZdZTI8,24482
+secretflow/protos/pipeline/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/protos/pipeline/pipeline_pb2.py,sha256=48DoQ64TrgjcCTTQzX3N6dDyr_Sjdotnzy8YK0sHjdU,13293
 secretflow/security/__init__.py,sha256=XSa8vQ3YNjHEWbHVXrM9MwxonaxndtCOi50CipzrU90,941
 secretflow/security/diffie_hellman.py,sha256=uIAICEjHJZKNYP2A50R6nWU6qGkVGSgGNIV9CXn48z0,11579
 secretflow/security/aggregation/__init__.py,sha256=QLB9vulzN399OMy9T_S6ZA0iaeKuVbRS9L61Hpz2F8o,946
 secretflow/security/aggregation/_utils.py,sha256=KgXRCCxr9PQsinDALN4a5Dn0jycSF3x3qYqq2kcTMv4,1039
 secretflow/security/aggregation/aggregator.py,sha256=smdPapUc9I3LdAuneIIbdKOWcGvWKOUeLxTlN47o85g,1072
-secretflow/security/aggregation/plain_aggregator.py,sha256=h2FEQgiyU77zW6qisJnJURiX0_S1guRGmNMgQ2gnsT4,4473
+secretflow/security/aggregation/plain_aggregator.py,sha256=ETwarnTPe_NTYvCx61SF3lHDEfJOr_-xoc0qtuwWWJM,4474
 secretflow/security/aggregation/secure_aggregator.py,sha256=HiSf8dostWXMxA2N46NpCU2icr23cAsEUWTNK94yfCk,12148
 secretflow/security/aggregation/sparse_plain_aggregator.py,sha256=KWiNrMX1HEfTorGyGDWjqqI651jaquxU90cwMSwoNcc,5009
 secretflow/security/aggregation/spu_aggregator.py,sha256=KYUUmwf99bXamZ2CVxTZGvKtnOCEoBJ262ehdiKegfQ,4179
 secretflow/security/compare/__init__.py,sha256=yVG0XmROdF0Qq3LYeXJb8SzVuXtu-Ii8yoCCWNahoRY,858
 secretflow/security/compare/comparator.py,sha256=3L4W9SKlWi9FDKOidGfOjlPb0SB5XogJWdKbDnBB2mw,1066
 secretflow/security/compare/device_comparator.py,sha256=e5P0yTEqRFTmr1a8fOJtRt-NurXb5pJ-d8bT9BY-Rhk,2220
 secretflow/security/compare/plain_comparator.py,sha256=wpn4UusUHkFeCAUTvUw_SIhQB-7GClaD50z7QcCCMwg,1871
 secretflow/security/compare/spu_comparator.py,sha256=iQCd8z0UpkKD3h5AhPklQ9oP-8KAGkTUNyyRyJ2qvDg,1762
-secretflow/security/privacy/__init__.py,sha256=5kkF46VCKxJmsPoutJ2b22FA3xYpdp9itV1zCbJJR2s,933
-secretflow/security/privacy/_lib.cpython-38-x86_64-linux-gnu.so,sha256=s2DwZHX7rVfv8GXxhaQi_hf4rl_aEUoAOL5CLQFtRCs,2221784
-secretflow/security/privacy/strategy.py,sha256=-H8riGuYZEuuEDmRzwO1HvDCGK89TjWpknXUv2bm3yQ,2749
-secretflow/security/privacy/strategy_fl.py,sha256=WAUGSRS1ZRW2XxAqeQwMVe2Tgyab_AOOYspUcXBWxl8,1875
+secretflow/security/privacy/__init__.py,sha256=KSR4jJRon2SyKyMpwLIcmfssZA4vqLIqbrsXpVGhgPQ,948
+secretflow/security/privacy/_lib.cpython-38-darwin.so,sha256=nhcUCXtn8OZ2869QJcvA6QAZuDnLne_I7zkvlFu00Y4,2208676
+secretflow/security/privacy/strategy.py,sha256=ojMMuNe-Ciq3QBhBEa-Kig8G5nGrwXeX-d04-sqHXBg,3012
+secretflow/security/privacy/strategy_fl.py,sha256=P4G0f1UVFe7EHt6sVeDPmedX2DWPvh2tIYHUsCKgpzY,1855
 secretflow/security/privacy/accounting/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
+secretflow/security/privacy/accounting/budget_accountant.py,sha256=0rprsewY4wQcbkLSuh4cEOG37O7vnam9FZ2zjGEn-yk,1814
 secretflow/security/privacy/accounting/gdp_accountant.py,sha256=J7pOwbiStkOuX37pIGkx7RnEdH7DwGRgUXE3duskRPk,2508
 secretflow/security/privacy/accounting/log_utils.py,sha256=cbyOYkWMuJxJgdL8zT7DidWHuA-RPl-W77CQJ1aLmVQ,3670
 secretflow/security/privacy/accounting/rdp_accountant.py,sha256=QAowmFm3Vyd-cOH_i0y1mI3YnagbthHtq-Nwnv7yEEo,5702
-secretflow/security/privacy/mechanism/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
-secretflow/security/privacy/mechanism/tensorflow/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
-secretflow/security/privacy/mechanism/tensorflow/layers.py,sha256=NetuDiA6icc5jXKs0SRjVwyOj3mJmBXdo3-kT5-GQDQ,6127
-secretflow/security/privacy/mechanism/tensorflow/mechanism_fl.py,sha256=aA54csKBRrpBSQ7MwIR0JQwxWzjl9fqckHJbSsU2fkI,5251
+secretflow/security/privacy/mechanism/__init__.py,sha256=ZUqwQZnz9z36XuNKu6t6TmLqDv7UOsGXmST0SKjZ6hI,585
+secretflow/security/privacy/mechanism/label_dp.py,sha256=SCcPCLJxpKp4ECzyYSI7rw1c1hha4VEXRvYWsDWUsvI,2167
+secretflow/security/privacy/mechanism/mechanism_fl.py,sha256=BPkkaEAGnkpDLTgz9BNSqEOrSB2K77bgmPPrdULNHfo,5420
+secretflow/security/privacy/mechanism/tensorflow/__init__.py,sha256=u6T9L2TljKVn26sCrg4gek8Z8H4mHsor6A5pwSMsy4k,668
+secretflow/security/privacy/mechanism/tensorflow/layers.py,sha256=yavu1GS4XxyeVcSngBSV_-sM_9mNJh1rzJHpK3KbM_8,2750
+secretflow/security/privacy/mechanism/torch/__init__.py,sha256=08fKvSZRIawpQwSXjiZLSvD0PRwI-hrUSfvhIEvCdMQ,668
+secretflow/security/privacy/mechanism/torch/layers.py,sha256=XTWd4fJJjBdzT_vnrYm6y1A-WV8hZwSxUrUdoOBzFp0,2115
 secretflow/stats/__init__.py,sha256=31yDkVpNZ9Xa3bwohM_3JiEk1hzTIjdE5n0Foys3kJk,1159
 secretflow/stats/biclassification_eval.py,sha256=Teu4hKYJKYzTlWBo9BkA-8K1STBorfLPXiyNGkDtMvk,4042
 secretflow/stats/psi_eval.py,sha256=2ACH222UQj5RtOz4fbCE-gMIbd7SvCuyWv4AgZoOnP8,2386
-secretflow/stats/pva_eval.py,sha256=Z1WkfUg6-Ca5i7cpG9PLtd9O31T5g_PfhazWqhSFPTs,2751
+secretflow/stats/pva_eval.py,sha256=_C8o0YsY4Fa765GOyMw4dBZ-DCra1QG9hvAt3Q0R_bk,2820
 secretflow/stats/regression_eval.py,sha256=YdmfF2L5RExr5Yr_UeHT7CMvT-F5AXpiYy8pFUvcSlQ,2995
 secretflow/stats/score_card.py,sha256=P8MyXGvVU1aV11f_Vkd57mEtLVZ3Yz5OFlq3BRekTYA,4421
 secretflow/stats/ss_pearsonr_v.py,sha256=MS5ASr1P_5OoiC5vL2rPGnazA7iFsG1N4CsS6MdybIQ,2421
 secretflow/stats/ss_pvalue_v.py,sha256=PQD1ZNujpZVUhEMnK7C4IVj92PD7JSotaUU_k1XX1Ds,7265
 secretflow/stats/ss_vif_v.py,sha256=jN0M-1TTpjK10TEjgkdI1NGvAIM_kiVDdmDIUyWAA-s,3631
-secretflow/stats/table_statistics.py,sha256=PS-wrfFqcza9vjI_W48mq3B1A45gj4SOcWC21vVlMPM,3262
+secretflow/stats/table_statistics.py,sha256=qKgGnC0JuZ32N5_u5c1jvqgbceQlSe3MmHnFeGZ3mKc,3262
 secretflow/stats/core/__init__.py,sha256=FCobL1hK9wpgG3MpMSZRojYPUOJEwgZwYcYnLbsPTS0,726
-secretflow/stats/core/biclassification_eval_core.py,sha256=NZ-gkw80aMAyX6Pll8-DphWRaQoiW0i8M40mV0KqzH0,20039
+secretflow/stats/core/biclassification_eval_core.py,sha256=xU5I7ZcXzHaMGin7BoTj51werAimqmPQd_CDfczPdls,20017
 secretflow/stats/core/psi_core.py,sha256=gYMoHQfNpWh5VFgNv-aA6H6bWIeXIFxtcrZePNLfVuM,2802
-secretflow/stats/core/pva_core.py,sha256=CLSvM35Bag8nGsGvjUeL4lFsAv0lCANClHArZsOtC_w,1665
+secretflow/stats/core/pva_core.py,sha256=aVlG6jFBJeTHHgX0WC_IhoHLWVfYcJ_ADVV5k7V0wLU,1755
 secretflow/stats/core/utils.py,sha256=VL6W4gR6ciggEoRYLEUutViWql5cnsjyjQtSYqdkA24,1776
 secretflow/utils/__init__.py,sha256=LsaruislCBOGxAxIhzEQEuRvZP0bW9-M3OgabZQiwRA,662
 secretflow/utils/cloudpickle.py,sha256=D9Lf_I_I4iJFmahoM2OOBvfQPLcs2McBHbMuMgqr-nk,13370
-secretflow/utils/compressor.py,sha256=qWydSrBqDzBjEs2yv40Q5EgnwCa95eeH-QfrAM8DpgM,11236
+secretflow/utils/communicate.py,sha256=hOVwTsAXK2KEeKbnhEg9wKLhyLd0f00DwzkqUuAK5uQ,400
+secretflow/utils/compressor.py,sha256=-3gHp5r6SJ6yMHGWwC9ey1uA268INttkenL_xRxrzCQ,11981
 secretflow/utils/errors.py,sha256=rRnEwSIU-ewJ4JXNBkbn_bk_ifGGaWS2CeeiAbYpGHg,1084
 secretflow/utils/hash.py,sha256=aWbXLTdmXc_xOl5FlXQW7Yw93iujdqu2X_01t6LF8cU,870
 secretflow/utils/io.py,sha256=vDesPaH9sKe8X7qdVDEaFhF4RksVzowNIJ-YuvYZ-TY,978
 secretflow/utils/logging.py,sha256=OZHkbOTsiN17do3t1iT6lbjW9JrdqJyBPEx4CCskF-8,964
 secretflow/utils/ndarray_bigint.py,sha256=awneTcQwL2SCMsE5dnv3WXGg9ZIWGM6MrEHteTldCgA,2842
 secretflow/utils/ndarray_encoding.py,sha256=Fs-q-409SG7Jh2mgBy64uDv7F2kJygrRpgZKFgP9l4A,2489
 secretflow/utils/random.py,sha256=YR5ZysYl6AyOMV0qV0qMxQYzsZ8O7YqYrRnCBseMWIg,803
 secretflow/utils/ray_compatibility.py,sha256=gVO78f_ZzuH0yaZGMtjn5v0NP00p_cZ_BdmRNgZ6XeI,1330
 secretflow/utils/sigmoid.py,sha256=cMw5zBMeJ9yYT4TrJdfsMr6PowQyxkNftCOIgMaSMHY,3930
 secretflow/utils/testing.py,sha256=JsZrw5PMsyeBJp1h-fWQHpzGcNHn13NYxdoHhFCGE8w,3308
 secretflow/utils/simulation/__init__.py,sha256=Wd00rjlQJKH-aY2LbPoVGjBo932U5pCSy9wAKN9ekjw,585
-secretflow/utils/simulation/datasets.py,sha256=Zv870-32nMLtRVRycdG7FY9nK9b8PyCxMRtRU75xDOo,30745
+secretflow/utils/simulation/datasets.py,sha256=RplOCPT9bHwxTDXbyIWwKSXVt67G8wcjypyF-1ntCiU,30743
 secretflow/utils/simulation/tf_gnn_model.py,sha256=385s0qZEOACN97MYQEPJX-vSVNEeQq8xb-nVYHEV7ls,8941
 secretflow/utils/simulation/data/__init__.py,sha256=KD77PGi-0ECpneFzilAxvo-N9fknaBc9CgiB2qlfuZU,769
 secretflow/utils/simulation/data/_utils.py,sha256=YauA2ujZLhodRrVGF1xMLVIHqSrLSbXLB5iOrxxO45I,2548
 secretflow/utils/simulation/data/dataframe.py,sha256=CRcnioLLM0o2bwy8SoLmx21S0icW6GG5yqfnlxkzAvY,5389
 secretflow/utils/simulation/data/ndarray.py,sha256=YkH4ZkIJYd9sKIB0YAueGlgb77iGQ9xEGs_mQTKHCbQ,4093
-secretflow-0.8.2b3.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-secretflow-0.8.2b3.dist-info/METADATA,sha256=jW4BKH8MP4F-ZJq6vEcfiFh3ygS5b2mlBzO0KdcU3RU,4171
-secretflow-0.8.2b3.dist-info/WHEEL,sha256=Q7wC2KUfz4qeyN-PnIiRDulJuXUHOlLP5Wm9pL_uT7s,111
-secretflow-0.8.2b3.dist-info/dependency_links.txt,sha256=LI4hT0fA00A7twyfHB-RG2dlg3JwhnHCi7lOWmSjA3E,55
-secretflow-0.8.2b3.dist-info/entry_points.txt,sha256=SHNAJtXkknDpzavWGYDfIpmBVdlRgeJElng358N3cvg,50
-secretflow-0.8.2b3.dist-info/top_level.txt,sha256=gnx5PWbIu_7IpkW_zzqjwN5TFcosT0RCQGqKRUlVt7I,44
-secretflow-0.8.2b3.dist-info/RECORD,,
+secretflow-0.8.3b0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+secretflow-0.8.3b0.dist-info/METADATA,sha256=-_lIoDVeF3SkVMBPVVaHJq5EfR5lRGRzmSsZUcyP0Co,4196
+secretflow-0.8.3b0.dist-info/WHEEL,sha256=lbCZQl32rz70_Iou4S1h8sUmNh5Rak_YxaqmnmkwnjQ,108
+secretflow-0.8.3b0.dist-info/dependency_links.txt,sha256=LI4hT0fA00A7twyfHB-RG2dlg3JwhnHCi7lOWmSjA3E,55
+secretflow-0.8.3b0.dist-info/entry_points.txt,sha256=SHNAJtXkknDpzavWGYDfIpmBVdlRgeJElng358N3cvg,50
+secretflow-0.8.3b0.dist-info/top_level.txt,sha256=gnx5PWbIu_7IpkW_zzqjwN5TFcosT0RCQGqKRUlVt7I,44
+secretflow-0.8.3b0.dist-info/RECORD,,
```

