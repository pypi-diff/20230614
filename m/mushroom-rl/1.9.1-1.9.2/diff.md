# Comparing `tmp/mushroom-rl-1.9.1.tar.gz` & `tmp/mushroom-rl-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mushroom-rl-1.9.1.tar", last modified: Tue Feb 14 17:19:40 2023, max compression
+gzip compressed data, was "mushroom-rl-1.9.2.tar", last modified: Wed Jun 14 08:53:39 2023, max compression
```

## Comparing `mushroom-rl-1.9.1.tar` & `mushroom-rl-1.9.2.tar`

### file list

```diff
@@ -1,316 +1,315 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.042842 mushroom-rl-1.9.1/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1106 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)       42 2020-01-10 10:25:29.000000 mushroom-rl-1.9.1/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1091 2023-02-14 17:19:40.042842 mushroom-rl-1.9.1/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)    10691 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.018842 mushroom-rl-1.9.1/mushroom_rl/
--rw-rw-r--   0 dave      (1000) dave      (1000)       22 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.018842 mushroom-rl-1.9.1/mushroom_rl/algorithms/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.018842 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/
--rw-rw-r--   0 dave      (1000) dave      (1000)      270 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.018842 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/classic_actor_critic/
--rw-rw-r--   0 dave      (1000) dave      (1000)      148 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/classic_actor_critic/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3780 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/classic_actor_critic/copdac_q.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4610 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/classic_actor_critic/stochastic_ac.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.018842 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/
--rw-rw-r--   0 dave      (1000) dave      (1000)      233 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3326 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/a2c.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6467 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/ddpg.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2795 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/deep_actor_critic.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5663 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/ppo.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    13654 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/sac.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3958 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/td3.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8518 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/trpo.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/
--rw-rw-r--   0 dave      (1000) dave      (1000)      222 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/
--rw-rw-r--   0 dave      (1000) dave      (1000)      254 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1843 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/black_box_optimization.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2270 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/constrained_reps.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5380 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/more.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1902 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/pgpe.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1977 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/reps.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      909 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/rwr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/
--rw-rw-r--   0 dave      (1000) dave      (1000)      169 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1721 2022-07-05 08:54:00.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/enac.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3178 2021-08-10 15:42:27.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/gpomdp.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3984 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/policy_gradient.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1910 2021-08-10 15:42:27.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/reinforce.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/
--rw-rw-r--   0 dave      (1000) dave      (1000)      523 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/
--rw-rw-r--   0 dave      (1000) dave      (1000)      198 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1223 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/batch_td.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1830 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/boosted_fqi.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2023 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/double_fqi.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1724 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/fqi.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2230 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/lspi.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/
--rw-rw-r--   0 dave      (1000) dave      (1000)      501 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6596 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/abstract_dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2111 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/averaged_dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5595 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/categorical_dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      572 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/double_dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      476 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2215 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/dueling_dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1684 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/maxmin_dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3849 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/noisy_dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4301 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/quantile_dqn.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7049 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/rainbow.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/
--rw-rw-r--   0 dave      (1000) dave      (1000)      834 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1427 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/double_q_learning.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      796 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/expected_sarsa.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1374 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/maxmin_q_learning.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1471 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/q_lambda.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      712 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/q_learning.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1258 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/r_learning.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2749 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/rq_learning.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      685 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/sarsa.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1483 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/sarsa_lambda.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1804 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/sarsa_lambda_continuous.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1116 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/speedy_q_learning.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1891 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/td.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2477 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/true_online_sarsa_lambda.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3521 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/weighted_q_learning.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/approximators/
--rw-rw-r--   0 dave      (1000) dave      (1000)      118 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.022842 mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4147 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/action_regressor.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4227 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/ensemble.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2081 2021-05-18 15:51:34.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/generic_regressor.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2770 2020-08-24 09:07:25.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/q_regressor.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/approximators/parametric/
--rw-rw-r--   0 dave      (1000) dave      (1000)      175 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/parametric/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2870 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/parametric/cmac.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3641 2020-08-24 09:07:25.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/parametric/linear.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    12055 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/parametric/torch_approximator.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8310 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/approximators/regressor.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/core/
--rw-rw-r--   0 dave      (1000) dave      (1000)      275 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/core/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2962 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/core/agent.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8927 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/core/core.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5637 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/core/environment.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/core/logger/
--rw-rw-r--   0 dave      (1000) dave      (1000)      159 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/core/logger/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4030 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/core/logger/console_logger.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4085 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/core/logger/data_logger.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2076 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/core/logger/logger.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     9482 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/core/serialization.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/distributions/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/distributions/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3958 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/distributions/distribution.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    14862 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/distributions/gaussian.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/environments/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1574 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5216 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/atari.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3686 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/car_on_hill.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3865 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/environments/cart_pole.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4808 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/dm_control_env.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1777 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/environments/finite_mdp.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/environments/generators/
--rw-rw-r--   0 dave      (1000) dave      (1000)      124 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/generators/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4869 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/generators/grid_world.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1990 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/generators/simple_chain.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8411 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/generators/taxi.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4990 2022-11-11 10:38:22.000000 mushroom-rl-1.9.1/mushroom_rl/environments/grid_world.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4481 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/gym_env.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11453 2022-11-11 10:38:22.000000 mushroom-rl-1.9.1/mushroom_rl/environments/habitat_env.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4786 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/igibson_env.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3850 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/inverted_pendulum.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5507 2022-11-11 10:38:22.000000 mushroom-rl-1.9.1/mushroom_rl/environments/lqr.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3592 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/minigrid_env.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    17073 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      254 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/
--rw-rw-r--   0 dave      (1000) dave      (1000)      137 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7569 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/base.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4968 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/defend.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7267 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/double.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4932 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/hit.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5874 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/prepare.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4619 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/repel.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5382 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/single.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5099 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/ball_in_a_cup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.026842 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.030842 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1588 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/double.xml
--rw-rw-r--   0 dave      (1000) dave      (1000)     3144 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/planar_robot_1.xml
--rw-rw-r--   0 dave      (1000) dave      (1000)     2888 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/planar_robot_2.xml
--rw-rw-r--   0 dave      (1000) dave      (1000)     1168 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/single.xml
--rw-rw-r--   0 dave      (1000) dave      (1000)     1929 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/table.xml
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.030842 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.034842 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/__init__.py
--rwxrwxr-x   0 dave      (1000) dave      (1000)    16584 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/base_link_convex.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   720584 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/base_link_fine.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     2484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split1.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1684 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split10.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1884 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split11.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     2084 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split12.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1684 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split13.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split14.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1584 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split15.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1684 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split16.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split17.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1784 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split18.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split2.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1884 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split3.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1584 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split4.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split5.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1184 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split6.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split7.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1884 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split8.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)     1584 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split9.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    16484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/elbow_link_convex.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   141384 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/elbow_link_fine.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    33484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_convex_decomposition_p1.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   205484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_convex_decomposition_p2.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   154484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_fine.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    23284 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p1.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    60284 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p2.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    56284 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p3.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   362984 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_fine.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    24284 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_pitch_link_convex.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   146084 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_pitch_link_fine.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   104884 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_convex_decomposition_p1.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    13484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_convex_decomposition_p2.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   615684 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_fine.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)     7684 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_palm_link_convex.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    44484 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_palm_link_fine.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    35284 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p1.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    34284 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p2.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    33284 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p3.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)   563684 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_fine.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    19284 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_convex_decomposition_p1.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)    63684 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_convex_decomposition_p2.stl
--rwxrwxr-x   0 dave      (1000) dave      (1000)  1316784 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_fine.stl
--rw-rw-r--   0 dave      (1000) dave      (1000)    16060 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/model.xml
--rw-rw-r--   0 dave      (1000) dave      (1000)     4695 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/environments/puddle_world.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11249 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.034842 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/
--rw-rw-r--   0 dave      (1000) dave      (1000)       26 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.034842 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/
--rw-rw-r--   0 dave      (1000) dave      (1000)      294 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     9988 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/base.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8883 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/defend.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7205 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/double.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8599 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/hit.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     9611 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/prepare.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8328 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/repel.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6404 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/single.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/
--rw-rw-r--   0 dave      (1000) dave      (1000)     9661 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/air_hockey_table.urdf
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/
--rw-rw-r--   0 dave      (1000) dave      (1000)     6474 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/planar_robot_1.urdf
--rw-rw-r--   0 dave      (1000) dave      (1000)     6474 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/planar_robot_2.urdf
--rw-rw-r--   0 dave      (1000) dave      (1000)     2799 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/puck.urdf
--rw-rw-r--   0 dave      (1000) dave      (1000)     4188 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/environments/segway.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4584 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/environments/ship_steering.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/features/
--rw-rw-r--   0 dave      (1000) dave      (1000)       99 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/features/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/features/_implementations/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/features/_implementations/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      643 2020-01-10 10:25:29.000000 mushroom-rl-1.9.1/mushroom_rl/features/_implementations/basis_features.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      776 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/_implementations/features_implementation.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      485 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/features/_implementations/functional_features.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1467 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/_implementations/tiles_features.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      704 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/_implementations/torch_features.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/features/basis/
--rw-rw-r--   0 dave      (1000) dave      (1000)      174 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/features/basis/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2353 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/features/basis/fourier.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2486 2020-06-30 09:38:24.000000 mushroom-rl-1.9.1/mushroom_rl/features/basis/gaussian_rbf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3330 2022-11-11 10:39:03.000000 mushroom-rl-1.9.1/mushroom_rl/features/basis/polynomial.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3996 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/features.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/features/tensors/
--rw-rw-r--   0 dave      (1000) dave      (1000)      216 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/tensors/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      273 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/tensors/constant_tensor.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2669 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/tensors/gaussian_tensor.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2751 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/tensors/random_fourier_tensor.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/features/tiles/
--rw-rw-r--   0 dave      (1000) dave      (1000)       96 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/features/tiles/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4309 2022-05-02 11:50:53.000000 mushroom-rl-1.9.1/mushroom_rl/features/tiles/tiles.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3102 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/features/tiles/voronoi.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/policy/
--rw-rw-r--   0 dave      (1000) dave      (1000)      935 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/policy/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1518 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/policy/deterministic_policy.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11334 2022-11-11 10:39:40.000000 mushroom-rl-1.9.1/mushroom_rl/policy/gaussian_policy.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4365 2022-11-11 10:39:40.000000 mushroom-rl-1.9.1/mushroom_rl/policy/noise_policy.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3609 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/policy/policy.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6772 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/policy/td_policy.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     9419 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/policy/torch_policy.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/solvers/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/solvers/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2127 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/solvers/car_on_hill.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2572 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/solvers/dynamic_programming.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6979 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/solvers/lqr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.038842 mushroom-rl-1.9.1/mushroom_rl/utils/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3576 2022-11-11 10:39:21.000000 mushroom-rl-1.9.1/mushroom_rl/utils/angles.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.042842 mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/
--rw-rw-r--   0 dave      (1000) dave      (1000)      468 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      783 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/callback.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      264 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/collect_dataset.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      712 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/collect_max_q.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      843 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/collect_parameters.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      936 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/collect_q.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6812 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/plot_dataset.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6705 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/utils/dataset.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      991 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/eligibility_trace.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1625 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/features.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1005 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/folder.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1405 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/utils/frames.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1095 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/minibatches.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.042842 mushroom-rl-1.9.1/mushroom_rl/utils/mujoco/
--rw-rw-r--   0 dave      (1000) dave      (1000)      147 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/utils/mujoco/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      749 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/utils/mujoco/kinematics.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8482 2023-02-14 17:15:29.000000 mushroom-rl-1.9.1/mushroom_rl/utils/mujoco/observation_helper.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5381 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/utils/mujoco/viewer.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2574 2020-08-24 09:07:25.000000 mushroom-rl-1.9.1/mushroom_rl/utils/numerical_gradient.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7074 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/utils/optimizers.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4314 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/utils/parameters.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1561 2022-06-30 18:09:40.000000 mushroom-rl-1.9.1/mushroom_rl/utils/plot.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.042842 mushroom-rl-1.9.1/mushroom_rl/utils/plots/
--rw-rw-r--   0 dave      (1000) dave      (1000)      594 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/utils/plots/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2986 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/plots/common_plots.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2316 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/plots/databuffer.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     9212 2020-08-24 09:07:25.000000 mushroom-rl-1.9.1/mushroom_rl/utils/plots/plot_item_buffer.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7194 2020-05-22 13:14:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/plots/window.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4016 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/utils/preprocessors.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.042842 mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/
--rw-rw-r--   0 dave      (1000) dave      (1000)      156 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3422 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/contacts.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     8573 2022-06-30 18:09:40.000000 mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/index_map.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1689 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/joints_helper.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      529 2021-08-16 13:59:44.000000 mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/observation.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2030 2021-06-09 16:23:11.000000 mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/viewer.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    12423 2022-06-30 18:09:40.000000 mushroom-rl-1.9.1/mushroom_rl/utils/replay_memory.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4797 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/mushroom_rl/utils/running_stats.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3058 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/utils/spaces.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3338 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/utils/table.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3282 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/utils/torch.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3982 2020-01-10 10:20:59.000000 mushroom-rl-1.9.1/mushroom_rl/utils/value_functions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6860 2021-06-09 14:16:14.000000 mushroom-rl-1.9.1/mushroom_rl/utils/variance_parameters.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    10651 2022-11-11 10:39:21.000000 mushroom-rl-1.9.1/mushroom_rl/utils/viewer.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.018842 mushroom-rl-1.9.1/mushroom_rl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1091 2023-02-14 17:19:39.000000 mushroom-rl-1.9.1/mushroom_rl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)    14234 2023-02-14 17:19:39.000000 mushroom-rl-1.9.1/mushroom_rl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-02-14 17:19:39.000000 mushroom-rl-1.9.1/mushroom_rl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2020-08-18 09:21:04.000000 mushroom-rl-1.9.1/mushroom_rl.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      366 2023-02-14 17:19:39.000000 mushroom-rl-1.9.1/mushroom_rl.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-02-14 17:19:39.000000 mushroom-rl-1.9.1/mushroom_rl.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/pyproject.toml
--rw-rw-r--   0 dave      (1000) dave      (1000)       91 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/requirements.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-02-14 17:19:40.042842 mushroom-rl-1.9.1/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     2982 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-02-14 17:19:40.042842 mushroom-rl-1.9.1/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1333 2023-01-31 17:03:54.000000 mushroom-rl-1.9.1/tests/test_imports.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.508830 mushroom-rl-1.9.2/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       42 2023-05-09 13:34:35.000000 mushroom-rl-1.9.2/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1091 2023-06-14 08:53:39.508830 mushroom-rl-1.9.2/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10691 2023-05-09 13:34:35.000000 mushroom-rl-1.9.2/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.400828 mushroom-rl-1.9.2/mushroom_rl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       22 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.400828 mushroom-rl-1.9.2/mushroom_rl/algorithms/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.400828 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      270 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.400828 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/classic_actor_critic/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      148 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/classic_actor_critic/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3780 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/classic_actor_critic/copdac_q.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4610 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/classic_actor_critic/stochastic_ac.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.404828 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      233 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3326 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/a2c.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6467 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/ddpg.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2795 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/deep_actor_critic.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5663 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/ppo.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13654 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/sac.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3958 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/td3.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8518 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/trpo.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.404828 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      222 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.404828 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      254 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1843 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/black_box_optimization.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2270 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/constrained_reps.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5380 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/more.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1902 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/pgpe.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1977 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/reps.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      909 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/rwr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.408828 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      169 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1721 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/enac.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3178 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/gpomdp.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3984 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/policy_gradient.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1910 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/reinforce.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.408828 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      523 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.408828 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      198 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1223 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/batch_td.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1830 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/boosted_fqi.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2023 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/double_fqi.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1724 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/fqi.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2230 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/lspi.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.412828 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      501 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6596 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/abstract_dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2111 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/averaged_dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5595 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/categorical_dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      572 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/double_dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      476 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2215 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/dueling_dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1684 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/maxmin_dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3849 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/noisy_dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4301 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/quantile_dqn.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7049 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/rainbow.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.416828 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      834 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1427 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/double_q_learning.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      796 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/expected_sarsa.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1374 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/maxmin_q_learning.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1471 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/q_lambda.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      712 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/q_learning.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1258 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/r_learning.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2749 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/rq_learning.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      685 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/sarsa.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1483 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/sarsa_lambda.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1804 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/sarsa_lambda_continuous.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1116 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/speedy_q_learning.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1891 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/td.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2477 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/true_online_sarsa_lambda.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3521 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/weighted_q_learning.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.416828 mushroom-rl-1.9.2/mushroom_rl/approximators/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      118 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.416828 mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4147 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/action_regressor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4227 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/ensemble.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2081 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/generic_regressor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2770 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/q_regressor.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.420828 mushroom-rl-1.9.2/mushroom_rl/approximators/parametric/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      175 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/parametric/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2870 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/parametric/cmac.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3641 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/parametric/linear.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    12055 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/parametric/torch_approximator.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8310 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/approximators/regressor.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.420828 mushroom-rl-1.9.2/mushroom_rl/core/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      275 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2962 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/agent.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8927 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/core.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5637 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/environment.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.420828 mushroom-rl-1.9.2/mushroom_rl/core/logger/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      159 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/logger/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4030 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/logger/console_logger.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4085 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/logger/data_logger.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2076 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/logger/logger.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9482 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/core/serialization.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.420828 mushroom-rl-1.9.2/mushroom_rl/distributions/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/distributions/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3958 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/distributions/distribution.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    14862 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/distributions/gaussian.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.424828 mushroom-rl-1.9.2/mushroom_rl/environments/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1574 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5216 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/atari.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3686 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/car_on_hill.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3865 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/cart_pole.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4808 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/dm_control_env.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1777 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/finite_mdp.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.428828 mushroom-rl-1.9.2/mushroom_rl/environments/generators/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      124 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/generators/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4869 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/generators/grid_world.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1990 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/generators/simple_chain.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8411 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/generators/taxi.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4990 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/grid_world.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4481 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/gym_env.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11453 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/habitat_env.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4786 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/igibson_env.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3850 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/inverted_pendulum.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5507 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/lqr.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3592 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/minigrid_env.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    17073 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.428828 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      254 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.428828 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      137 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7569 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/base.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4968 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/defend.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7267 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/double.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4932 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/hit.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5874 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/prepare.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4619 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/repel.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5382 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/single.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5099 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/ball_in_a_cup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.432829 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.432829 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1588 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/double.xml
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3144 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/planar_robot_1.xml
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2888 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/planar_robot_2.xml
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1168 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/single.xml
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1929 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/table.xml
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.432829 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.480829 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/__init__.py
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    16584 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/base_link_convex.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   720584 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/base_link_fine.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split1.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1684 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split10.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1884 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split11.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2084 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split12.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1684 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split13.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split14.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1584 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split15.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1684 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split16.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split17.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1784 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split18.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split2.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1884 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split3.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1584 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split4.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split5.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1184 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split6.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split7.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1884 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split8.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1584 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split9.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    16484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/elbow_link_convex.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   141384 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/elbow_link_fine.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    33484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_convex_decomposition_p1.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   205484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_convex_decomposition_p2.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   154484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_fine.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    23284 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p1.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    60284 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p2.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    56284 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p3.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   362984 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_fine.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    24284 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_pitch_link_convex.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   146084 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_pitch_link_fine.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   104884 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_convex_decomposition_p1.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    13484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_convex_decomposition_p2.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   615684 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_fine.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     7684 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_palm_link_convex.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    44484 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_palm_link_fine.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    35284 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p1.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    34284 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p2.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    33284 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p3.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)   563684 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_fine.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    19284 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_convex_decomposition_p1.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)    63684 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_convex_decomposition_p2.stl
+-rwxrwxr-x   0 dave      (1000) dave      (1000)  1316784 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_fine.stl
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16060 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/model.xml
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4695 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/puddle_world.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11249 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.484829 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       26 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.488829 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      294 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9988 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/base.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8883 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/defend.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7205 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/double.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8599 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/hit.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9611 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/prepare.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8328 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/repel.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6404 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/single.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.488829 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.492829 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9661 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/air_hockey_table.urdf
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.492829 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6474 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/planar_robot_1.urdf
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6474 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/planar_robot_2.urdf
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2799 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/puck.urdf
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4188 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/segway.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4584 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/environments/ship_steering.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.492829 mushroom-rl-1.9.2/mushroom_rl/features/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       99 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.492829 mushroom-rl-1.9.2/mushroom_rl/features/_implementations/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/_implementations/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      643 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/_implementations/basis_features.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      776 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/_implementations/features_implementation.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      485 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/_implementations/functional_features.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1467 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/_implementations/tiles_features.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      704 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/_implementations/torch_features.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.492829 mushroom-rl-1.9.2/mushroom_rl/features/basis/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      174 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/basis/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2353 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/basis/fourier.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2535 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/features/basis/gaussian_rbf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4377 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/features/basis/polynomial.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3996 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/features.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.496830 mushroom-rl-1.9.2/mushroom_rl/features/tensors/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      294 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/features/tensors/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4720 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/features/tensors/basis_tensor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      273 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/tensors/constant_tensor.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2751 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/tensors/random_fourier_tensor.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.496830 mushroom-rl-1.9.2/mushroom_rl/features/tiles/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       96 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/tiles/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4309 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/tiles/tiles.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3102 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/features/tiles/voronoi.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.496830 mushroom-rl-1.9.2/mushroom_rl/policy/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      970 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/policy/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1518 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/policy/deterministic_policy.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3123 2023-05-09 15:20:23.000000 mushroom-rl-1.9.2/mushroom_rl/policy/dmp.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11334 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/policy/gaussian_policy.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4333 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/policy/noise_policy.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3609 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/policy/policy.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3659 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/policy/promps.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6772 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/policy/td_policy.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9643 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/policy/torch_policy.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.496830 mushroom-rl-1.9.2/mushroom_rl/solvers/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/solvers/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2127 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/solvers/car_on_hill.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2572 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/solvers/dynamic_programming.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6979 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/solvers/lqr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.504830 mushroom-rl-1.9.2/mushroom_rl/utils/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3576 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/angles.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.504830 mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      468 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      783 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/callback.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      264 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/collect_dataset.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      712 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/collect_max_q.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      843 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/collect_parameters.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      936 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/collect_q.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6812 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/plot_dataset.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6705 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/dataset.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      991 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/eligibility_trace.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1980 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/utils/features.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1005 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/folder.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1405 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/frames.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1095 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/minibatches.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.504830 mushroom-rl-1.9.2/mushroom_rl/utils/mujoco/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      147 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/mujoco/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      749 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/mujoco/kinematics.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8482 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/mujoco/observation_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5663 2023-06-14 08:39:04.000000 mushroom-rl-1.9.2/mushroom_rl/utils/mujoco/viewer.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2574 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/numerical_gradient.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7074 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/optimizers.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4314 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/parameters.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1561 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/plot.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.508830 mushroom-rl-1.9.2/mushroom_rl/utils/plots/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      594 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/plots/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2986 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/plots/common_plots.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2316 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/plots/databuffer.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     9212 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/plots/plot_item_buffer.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7194 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/plots/window.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4016 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/preprocessors.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.508830 mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      156 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3422 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/contacts.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8573 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/index_map.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1689 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/joints_helper.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      529 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/observation.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2030 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/viewer.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    12423 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/replay_memory.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4797 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/running_stats.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3058 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/spaces.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3338 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/table.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3282 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/torch.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3982 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/value_functions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     6860 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/variance_parameters.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10651 2023-03-06 16:16:57.000000 mushroom-rl-1.9.2/mushroom_rl/utils/viewer.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-14 08:53:39.400828 mushroom-rl-1.9.2/mushroom_rl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1091 2023-06-14 08:53:39.000000 mushroom-rl-1.9.2/mushroom_rl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)    14256 2023-06-14 08:53:39.000000 mushroom-rl-1.9.2/mushroom_rl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-14 08:53:39.000000 mushroom-rl-1.9.2/mushroom_rl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-14 08:53:39.000000 mushroom-rl-1.9.2/mushroom_rl.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      366 2023-06-14 08:53:39.000000 mushroom-rl-1.9.2/mushroom_rl.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       12 2023-06-14 08:53:39.000000 mushroom-rl-1.9.2/mushroom_rl.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-09 13:34:35.000000 mushroom-rl-1.9.2/pyproject.toml
+-rw-rw-r--   0 dave      (1000) dave      (1000)       91 2023-05-09 13:34:35.000000 mushroom-rl-1.9.2/requirements.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-06-14 08:53:39.508830 mushroom-rl-1.9.2/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2982 2023-05-09 13:34:35.000000 mushroom-rl-1.9.2/setup.py
```

### Comparing `mushroom-rl-1.9.1/PKG-INFO` & `mushroom-rl-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mushroom-rl
-Version: 1.9.1
+Version: 1.9.2
 Summary: A Python library for Reinforcement Learning experiments.
 Home-page: https://github.com/MushroomRL/mushroom-rl
 Author: Carlo D'Eramo, Davide Tateo
 Author-email: carlo.deramo@gmail.com
 License: MIT
 Description: MushroomRL is a Python Reinforcement Learning (RL) library whose modularity allows to easily use well-known Python libraries for tensor computation (e.g. PyTorch, Tensorflow) and RL benchmarks (e.g. OpenAI Gym, PyBullet, Deepmind Control Suite). It allows to perform RL experiments in a simple way providing classical RL algorithms (e.g. Q-Learning, SARSA, FQI), and deep RL algorithms (e.g. DQN, DDPG, SAC, TD3, TRPO, PPO). Full documentation available at http://mushroomrl.readthedocs.io/en/latest/.
 Platform: UNKNOWN
```

### Comparing `mushroom-rl-1.9.1/README.rst` & `mushroom-rl-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/classic_actor_critic/copdac_q.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/classic_actor_critic/copdac_q.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/classic_actor_critic/stochastic_ac.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/classic_actor_critic/stochastic_ac.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/a2c.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/a2c.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/ddpg.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/ddpg.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/deep_actor_critic.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/deep_actor_critic.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/ppo.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/ppo.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/sac.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/sac.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/td3.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/td3.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/actor_critic/deep_actor_critic/trpo.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/actor_critic/deep_actor_critic/trpo.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/black_box_optimization.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/black_box_optimization.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/constrained_reps.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/constrained_reps.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/more.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/more.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/pgpe.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/pgpe.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/reps.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/reps.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/black_box_optimization/rwr.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/black_box_optimization/rwr.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/enac.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/enac.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/gpomdp.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/gpomdp.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/policy_gradient.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/policy_gradient.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/policy_search/policy_gradient/reinforce.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/policy_search/policy_gradient/reinforce.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/__init__.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/__init__.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/batch_td.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/batch_td.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/boosted_fqi.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/boosted_fqi.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/double_fqi.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/double_fqi.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/fqi.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/fqi.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/batch_td/lspi.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/batch_td/lspi.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/abstract_dqn.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/abstract_dqn.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/averaged_dqn.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/averaged_dqn.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/categorical_dqn.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/categorical_dqn.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/double_dqn.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/double_dqn.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/dueling_dqn.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/dueling_dqn.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/maxmin_dqn.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/maxmin_dqn.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/noisy_dqn.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/noisy_dqn.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/quantile_dqn.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/quantile_dqn.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/dqn/rainbow.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/dqn/rainbow.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/__init__.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/__init__.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/double_q_learning.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/double_q_learning.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/expected_sarsa.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/expected_sarsa.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/maxmin_q_learning.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/maxmin_q_learning.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/q_lambda.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/q_lambda.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/q_learning.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/q_learning.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/r_learning.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/r_learning.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/rq_learning.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/rq_learning.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/sarsa.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/sarsa.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/sarsa_lambda.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/sarsa_lambda.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/sarsa_lambda_continuous.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/sarsa_lambda_continuous.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/speedy_q_learning.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/speedy_q_learning.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/td.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/td.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/true_online_sarsa_lambda.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/true_online_sarsa_lambda.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/algorithms/value/td/weighted_q_learning.py` & `mushroom-rl-1.9.2/mushroom_rl/algorithms/value/td/weighted_q_learning.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/action_regressor.py` & `mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/action_regressor.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/ensemble.py` & `mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/ensemble.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/generic_regressor.py` & `mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/generic_regressor.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/approximators/_implementations/q_regressor.py` & `mushroom-rl-1.9.2/mushroom_rl/approximators/_implementations/q_regressor.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/approximators/parametric/cmac.py` & `mushroom-rl-1.9.2/mushroom_rl/approximators/parametric/cmac.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/approximators/parametric/linear.py` & `mushroom-rl-1.9.2/mushroom_rl/approximators/parametric/linear.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/approximators/parametric/torch_approximator.py` & `mushroom-rl-1.9.2/mushroom_rl/approximators/parametric/torch_approximator.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/approximators/regressor.py` & `mushroom-rl-1.9.2/mushroom_rl/approximators/regressor.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/core/agent.py` & `mushroom-rl-1.9.2/mushroom_rl/core/agent.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/core/core.py` & `mushroom-rl-1.9.2/mushroom_rl/core/core.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/core/environment.py` & `mushroom-rl-1.9.2/mushroom_rl/core/environment.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/core/logger/console_logger.py` & `mushroom-rl-1.9.2/mushroom_rl/core/logger/console_logger.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/core/logger/data_logger.py` & `mushroom-rl-1.9.2/mushroom_rl/core/logger/data_logger.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/core/logger/logger.py` & `mushroom-rl-1.9.2/mushroom_rl/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/core/serialization.py` & `mushroom-rl-1.9.2/mushroom_rl/core/serialization.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/distributions/distribution.py` & `mushroom-rl-1.9.2/mushroom_rl/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/distributions/gaussian.py` & `mushroom-rl-1.9.2/mushroom_rl/distributions/gaussian.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/__init__.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/atari.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/atari.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/car_on_hill.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/car_on_hill.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/cart_pole.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/cart_pole.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/dm_control_env.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/dm_control_env.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/finite_mdp.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/finite_mdp.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/generators/grid_world.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/generators/grid_world.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/generators/simple_chain.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/generators/simple_chain.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/generators/taxi.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/generators/taxi.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/grid_world.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/grid_world.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/gym_env.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/gym_env.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/habitat_env.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/habitat_env.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/igibson_env.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/igibson_env.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/inverted_pendulum.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/inverted_pendulum.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/lqr.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/lqr.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/minigrid_env.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/minigrid_env.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/base.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/base.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/defend.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/defend.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/double.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/double.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/hit.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/hit.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/prepare.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/prepare.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/repel.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/repel.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/air_hockey/single.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/air_hockey/single.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/ball_in_a_cup.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/ball_in_a_cup.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/double.xml` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/double.xml`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/planar_robot_1.xml` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/planar_robot_1.xml`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/planar_robot_2.xml` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/planar_robot_2.xml`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/single.xml` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/single.xml`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/air_hockey/table.xml` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/air_hockey/table.xml`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/base_link_convex.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/base_link_convex.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/base_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/base_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split1.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split1.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split10.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split10.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split11.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split11.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split12.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split12.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split13.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split13.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split14.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split14.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split15.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split15.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split16.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split16.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split17.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split17.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split18.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split18.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split2.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split2.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split3.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split3.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split4.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split4.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split5.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split5.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split6.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split6.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split7.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split7.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split8.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split8.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split9.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/cup_split9.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/elbow_link_convex.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/elbow_link_convex.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/elbow_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/elbow_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_convex_decomposition_p1.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_convex_decomposition_p1.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_convex_decomposition_p2.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_convex_decomposition_p2.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/forearm_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p1.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p1.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p2.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p2.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p3.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_convex_decomposition_p3.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_pitch_link_convex.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_pitch_link_convex.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_pitch_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/shoulder_pitch_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_convex_decomposition_p1.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_convex_decomposition_p1.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_convex_decomposition_p2.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_convex_decomposition_p2.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/upper_arm_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_palm_link_convex.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_palm_link_convex.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_palm_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_palm_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p1.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p1.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p2.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p2.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p3.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_convex_decomposition_p3.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_pitch_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_convex_decomposition_p1.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_convex_decomposition_p1.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_convex_decomposition_p2.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_convex_decomposition_p2.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_fine.stl` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/meshes/wrist_yaw_link_fine.stl`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/model.xml` & `mushroom-rl-1.9.2/mushroom_rl/environments/mujoco_envs/data/ball_in_a_cup/model.xml`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/puddle_world.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/puddle_world.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/base.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/base.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/defend.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/defend.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/double.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/double.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/hit.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/hit.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/prepare.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/prepare.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/repel.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/repel.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/air_hockey/single.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/air_hockey/single.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/air_hockey_table.urdf` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/air_hockey_table.urdf`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/planar_robot_1.urdf` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/planar_robot_1.urdf`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/planar_robot_2.urdf` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/planar/planar_robot_2.urdf`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/pybullet_envs/data/air_hockey/puck.urdf` & `mushroom-rl-1.9.2/mushroom_rl/environments/pybullet_envs/data/air_hockey/puck.urdf`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/segway.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/segway.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/environments/ship_steering.py` & `mushroom-rl-1.9.2/mushroom_rl/environments/ship_steering.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/_implementations/basis_features.py` & `mushroom-rl-1.9.2/mushroom_rl/features/_implementations/basis_features.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/_implementations/features_implementation.py` & `mushroom-rl-1.9.2/mushroom_rl/features/_implementations/features_implementation.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/_implementations/tiles_features.py` & `mushroom-rl-1.9.2/mushroom_rl/features/_implementations/tiles_features.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/_implementations/torch_features.py` & `mushroom-rl-1.9.2/mushroom_rl/features/_implementations/torch_features.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/basis/fourier.py` & `mushroom-rl-1.9.2/mushroom_rl/features/basis/fourier.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/basis/gaussian_rbf.py` & `mushroom-rl-1.9.2/mushroom_rl/features/basis/gaussian_rbf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import numpy as np
 from mushroom_rl.utils.features import uniform_grid
 
 
 class GaussianRBF:
     r"""
-    Class implementing Gaussian radial basis functions. The value of the feature
-    is computed using the formula:
+    Class implementing Gaussian radial basis functions. The value of the feature is computed using the formula:
     
     .. math::
         \sum \dfrac{(X_i - \mu_i)^2}{\sigma_i}
 
-    where X is the input, \mu is the mean vector and \sigma is the scale
-    parameter vector.
+    where X is the input, \mu is the mean vector and \sigma is the scale parameter vector.
 
     """
     def __init__(self, mean, scale, dimensions=None):
         """
         Constructor.
 
         Args:
             mean (np.ndarray): the mean vector of the feature;
             scale (np.ndarray): the scale vector of the feature;
-            dimensions (list, None): list of the dimensions of the input to be
-                considered by the feature. The number of dimensions must match
-                the dimensionality of ``mean`` and ``scale``.
+            dimensions (list, None): list of the dimensions of the input to be considered by the feature. The number of
+                dimensions must match the dimensionality of ``mean`` and ``scale``.
 
         """
         self._mean = mean
         self._scale = scale
         self._dim = dimensions
 
     def __call__(self, x):
@@ -39,38 +36,38 @@
     def __str__(self):
         name = 'GaussianRBF ' + str(self._mean) + ' ' + str(self._scale)
         if self._dim is not None:
             name += ' ' + str(self._dim)
         return name
 
     @staticmethod
-    def generate(n_centers, low, high, dimensions=None):
+    def generate(n_centers, low, high, dimensions=None, eta=0.25):
         r"""
-        Factory method to build uniformly spaced gaussian radial basis functions
-        with a 25\% overlap.
+        Factory method to build uniformly spaced gaussian radial basis functions with `eta` overlap.
 
         Args:
-            n_centers (list): list of the number of radial basis functions to be
-                used for each dimension.
+            n_centers (list): list of the number of radial basis functions to be used for each dimension.
             low (np.ndarray): lowest value for each dimension;
             high (np.ndarray): highest value for each dimension;
-            dimensions (list, None): list of the dimensions of the input to be
-                considered by the feature. The number of dimensions must match
-                the number of elements in ``n_centers`` and ``low``.
+            dimensions (list, None): list of the dimensions of the input to be considered by the feature. The number of
+                dimensions must match the number of elements in ``n_centers`` and ``low``;
+            eta (float, 0.25): percentage of overlap between the features.
 
         Returns:
             The list of the generated radial basis functions.
 
         """
         n_features = len(low)
         assert len(n_centers) == n_features
         assert len(low) == len(high)
         assert dimensions is None or n_features == len(dimensions)
 
-        grid, b = uniform_grid(n_centers, low, high)
+        grid, w = uniform_grid(n_centers, low, high, eta)
+
+        b = 2*(w/3)**2
 
         basis = list()
         for i in range(len(grid)):
             v = grid[i, :]
             bf = GaussianRBF(v, b, dimensions)
             basis.append(bf)
```

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/basis/polynomial.py` & `mushroom-rl-1.9.2/mushroom_rl/features/basis/polynomial.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,43 +8,59 @@
     
     .. math::
         \prod X_i^{d_i}
 
     where X is the input and d is the vector of the exponents of the polynomial.
 
     """
-    def __init__(self, dimensions=None, degrees=None):
+    def __init__(self, dimensions=None, degrees=None, low=None, high=None):
         """
         Constructor. If both parameters are None, the constant feature is built.
 
         Args:
-            dimensions (list, None): list of the dimensions of the input to be
-                considered by the feature;
-            degrees (list, None): list of the degrees of each dimension to be
-                considered by the feature. It must match the number of elements
-                of ``dimensions``.
+            dimensions (list, None): list of the dimensions of the input to be considered by the feature;
+            degrees (list, None): list of the degrees of each dimension to be considered by the feature.
+                It must match the number of elements of ``dimensions``;
+            low (np.ndarray, None): array specifying the lower bound of the action space, used to normalize the
+                state between -1 and 1;
+            high (np.ndarray, None): array specifying the lower bound of the action space, used to normalize the
+                state between -1 and 1;
 
         """
+        assert (dimensions is None and degrees is None) or (
+                len(dimensions) == len(degrees))
+
+        assert (low is None and high is None) or (low is not None and high is not None)
+
         self._dim = dimensions
         self._deg = degrees
 
-        assert (self._dim is None and self._deg is None) or (
-            len(self._dim) == len(self._deg))
+        if low is not None:
+            self._mean = (low + high) / 2
+            self._delta = (high - low) / 2
+        else:
+            self._mean = None
 
     def __call__(self, x):
 
         if self._dim is None:
             return 1
 
         out = 1
+        x_n = self._normalize(x)
         for i, d in zip(self._dim, self._deg):
-            out *= x[i]**d
+            out *= x_n[i]**d
 
         return out
 
+    def _normalize(self, x):
+        if self._mean is not None:
+            return (x - self._mean) / self._delta
+        return x
+
     def __str__(self):
         if self._deg is None:
             return '1'
 
         name = ''
         for i, d in zip(self._dim, self._deg):
             name += 'x[' + str(i) + ']'
@@ -80,32 +96,36 @@
                         else:
                             pattern[-1] += 1
                         break
                 yield pattern
             pattern[-1] = 0
 
     @staticmethod
-    def generate(max_degree, input_size):
+    def generate(max_degree, input_size, low=None, high=None):
         """
         Factory method to build a polynomial of order ``max_degree`` based on
         the first ``input_size`` dimensions of the input.
 
         Args:
             max_degree (int): maximum degree of the polynomial;
-            input_size (int): size of the input.
+            input_size (int): size of the input;
+            low (np.ndarray, None): array specifying the lower bound of the action space, used to normalize the
+                state between -1 and 1;
+            high (np.ndarray, None): array specifying the lower bound of the action space, used to normalize the
+                state between -1 and 1;
 
         Returns:
             The list of the generated polynomial basis functions.
 
         """
         assert (max_degree >= 0)
         assert (input_size > 0)
 
         basis_list = [PolynomialBasis()]
 
         for e in PolynomialBasis._compute_exponents(max_degree, input_size):
             dims = np.reshape(np.argwhere(e != 0), -1)
             degs = e[e != 0]
 
-            basis_list.append(PolynomialBasis(dims, degs))
+            basis_list.append(PolynomialBasis(dims, degs, low, high))
 
         return basis_list
```

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/features.py` & `mushroom-rl-1.9.2/mushroom_rl/features/features.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/tensors/random_fourier_tensor.py` & `mushroom-rl-1.9.2/mushroom_rl/features/tensors/random_fourier_tensor.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/tiles/tiles.py` & `mushroom-rl-1.9.2/mushroom_rl/features/tiles/tiles.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/features/tiles/voronoi.py` & `mushroom-rl-1.9.2/mushroom_rl/features/tiles/voronoi.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/policy/__init__.py` & `mushroom-rl-1.9.2/mushroom_rl/policy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .policy import Policy, ParametricPolicy
 from .noise_policy import OrnsteinUhlenbeckPolicy, ClippedGaussianPolicy
 from .td_policy import TDPolicy, Boltzmann, EpsGreedy, Mellowmax
 from .gaussian_policy import GaussianPolicy, DiagonalGaussianPolicy, \
      StateStdGaussianPolicy, StateLogStdGaussianPolicy
 from .deterministic_policy import DeterministicPolicy
 from .torch_policy import TorchPolicy, GaussianTorchPolicy, BoltzmannTorchPolicy
+from .promps import ProMP
 
 
 __all_td__ = ['TDPolicy', 'Boltzmann', 'EpsGreedy', 'Mellowmax']
 __all_parametric__ = ['ParametricPolicy', 'GaussianPolicy',
                       'DiagonalGaussianPolicy', 'StateStdGaussianPolicy',
-                      'StateLogStdGaussianPolicy']
+                      'StateLogStdGaussianPolicy', 'ProMP']
 __all_torch__ = ['TorchPolicy', 'GaussianTorchPolicy', 'BoltzmannTorchPolicy']
 
 __all__ = ['Policy',  'DeterministicPolicy', 'OrnsteinUhlenbeckPolicy', 'ClippedGaussianPolicy'] \
           + __all_td__ + __all_parametric__ + __all_torch__
```

### Comparing `mushroom-rl-1.9.1/mushroom_rl/policy/deterministic_policy.py` & `mushroom-rl-1.9.2/mushroom_rl/policy/deterministic_policy.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/policy/gaussian_policy.py` & `mushroom-rl-1.9.2/mushroom_rl/policy/gaussian_policy.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/policy/noise_policy.py` & `mushroom-rl-1.9.2/mushroom_rl/policy/noise_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,14 @@
         self._sigma = sigma
         self._low = low
         self._high = high
 
         self._add_save_attr(
             _approximator='mushroom',
             _predict_params='pickle',
-            _inv_sigma='numpy',
             _sigma='numpy',
             _low='numpy',
             _high='numpy'
         )
 
     def __call__(self, state, action):
         raise NotImplementedError
```

### Comparing `mushroom-rl-1.9.1/mushroom_rl/policy/policy.py` & `mushroom-rl-1.9.2/mushroom_rl/policy/policy.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/policy/td_policy.py` & `mushroom-rl-1.9.2/mushroom_rl/policy/td_policy.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/policy/torch_policy.py` & `mushroom-rl-1.9.2/mushroom_rl/policy/torch_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,21 @@
 
 
 class BoltzmannTorchPolicy(TorchPolicy):
     """
     Torch policy implementing a Boltzmann policy.
 
     """
+    class CategoricalWrapper(torch.distributions.Categorical):
+        def __init__(self, logits):
+            super().__init__(logits=logits)
+
+        def log_prob(self, value):
+            return super().log_prob(value.squeeze())
+
     def __init__(self, network, input_shape, output_shape, beta, use_cuda=False, **params):
         """
         Constructor.
 
         Args:
             network (object): the network class used to implement the mean
                 regressor;
@@ -296,22 +303,22 @@
 
         if len(action.shape) > 1:
             return action
         else:
             return action.unsqueeze(0)
 
     def log_prob_t(self, state, action):
-        return self.distribution_t(state).log_prob(action.squeeze())[:, None]
+        return self.distribution_t(state).log_prob(action)[:, None]
 
     def entropy_t(self, state):
         return torch.mean(self.distribution_t(state).entropy())
 
     def distribution_t(self, state):
         logits = self._logits(state, **self._predict_params, output_tensor=True) * self._beta(state.numpy())
-        return torch.distributions.Categorical(logits=logits)
+        return BoltzmannTorchPolicy.CategoricalWrapper(logits)
 
     def set_weights(self, weights):
         self._logits.set_weights(weights)
 
     def get_weights(self):
         return self._logits.get_weights()
```

### Comparing `mushroom-rl-1.9.1/mushroom_rl/solvers/car_on_hill.py` & `mushroom-rl-1.9.2/mushroom_rl/solvers/car_on_hill.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/solvers/dynamic_programming.py` & `mushroom-rl-1.9.2/mushroom_rl/solvers/dynamic_programming.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/solvers/lqr.py` & `mushroom-rl-1.9.2/mushroom_rl/solvers/lqr.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/angles.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/angles.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/callback.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/collect_max_q.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/collect_max_q.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/collect_parameters.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/collect_parameters.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/collect_q.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/collect_q.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/callbacks/plot_dataset.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/callbacks/plot_dataset.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/dataset.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/eligibility_trace.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/eligibility_trace.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/features.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/features.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 import numpy as np
 
 
-def uniform_grid(n_centers, low, high):
+def uniform_grid(n_centers, low, high, eta=0.25, cyclic=False):
     """
     This function is used to create the parameters of uniformly spaced radial
-    basis functions with 25% of overlap. It creates a uniformly spaced grid of
-    ``n_centers[i]`` points in each ``ranges[i]``. Also returns a vector
-    containing the appropriate scales of the radial basis functions.
+    basis functions with `eta` of overlap. It creates a uniformly spaced grid of
+    ``n_centers[i]`` points in each dimension i. Also returns a vector
+    containing the appropriate width of the radial basis functions.
 
     Args:
          n_centers (list): number of centers of each dimension;
          low (np.ndarray): lowest value for each dimension;
-         high (np.ndarray): highest value for each dimension.
+         high (np.ndarray): highest value for each dimension;
+         eta (float, 0.25): overlap between two radial basis functions;
+         cyclic (bool, False): whether the state space is a ring or not
 
     Returns:
-        The uniformly spaced grid and the scale vector.
+        The uniformly spaced grid and the width vector.
 
     """
+    assert 0 < eta < 1.0
+
     n_features = len(low)
-    b = np.zeros(n_features)
+    w = np.zeros(n_features)
     c = list()
     tot_points = 1
     for i, n in enumerate(n_centers):
         start = low[i]
         end = high[i]
-
-        b[i] = (end - start) ** 2 / n ** 3
-        m = abs(start - end) / n
+        # m = abs(start - end) / n
         if n == 1:
+            w[i] = abs(end - start) / 2
             c_i = (start + end) / 2.
             c.append(np.array([c_i]))
         else:
-            c_i = np.linspace(start - m * .1, end + m * .1, n)
+            if cyclic:
+                end_new = end - abs(end-start) / n
+            else:
+                end_new = end
+            w[i] = (1 + eta) * abs(end_new - start) / n
+            c_i = np.linspace(start, end_new, n)
             c.append(c_i)
         tot_points *= n
 
     n_rows = 1
     n_cols = 0
 
     grid = np.zeros((tot_points, n_features))
@@ -52,8 +60,8 @@
                 grid[idx_r, n_cols] = discrete_values[i1]
 
             i1 += 1
 
         n_cols += 1
         n_rows *= len(discrete_values)
 
-    return grid, b
+    return grid, w
```

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/folder.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/folder.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/frames.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/frames.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/minibatches.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/minibatches.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/mujoco/kinematics.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/mujoco/kinematics.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/mujoco/observation_helper.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/mujoco/observation_helper.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/mujoco/viewer.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/mujoco/viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,26 @@
     """
     Class that creates a Glfw viewer for mujoco environments.
     Controls:
         Space: Pause / Unpause simulation
         c: Turn contact force and constraint visualisation on / off
         t: Make models transparent
     """
-    def __init__(self, model, dt, width=1920, height=1080, start_paused=False):
+    def __init__(self, model, dt, width=1920, height=1080, start_paused=False, custom_render_callback=None):
         self.button_left = False
         self.button_right = False
         self.button_middle = False
         self.last_x = 0
         self.last_y = 0
         self.dt = dt
 
         self.frames = 0
         self.start_time = time.time()
         glfw.init()
+        glfw.window_hint(glfw.COCOA_RETINA_FRAMEBUFFER, 0)
 
         self._loop_count = 0
         self._time_per_render = 1 / 60.
         self._paused = start_paused
 
         self._window = glfw.create_window(width=width, height=height, title="MuJoCo", monitor=None, share=None)
         glfw.make_context_current(self._window)
@@ -49,14 +50,16 @@
         mujoco.mjv_defaultFreeCamera(model, self._camera)
 
         self._viewport = mujoco.MjrRect(0, 0, width, height)
         self._context = mujoco.MjrContext(model, mujoco.mjtFontScale(100))
 
         self.rgb_buffer = np.empty((width, height, 3), dtype=np.uint8)
 
+        self.custom_render_callback = custom_render_callback
+
     def mouse_button(self, window, button, act, mods):
         self.button_left = glfw.get_mouse_button(self._window, glfw.MOUSE_BUTTON_LEFT) == glfw.PRESS
         self.button_right = glfw.get_mouse_button(self._window, glfw.MOUSE_BUTTON_RIGHT) == glfw.PRESS
         self.button_middle = glfw.get_mouse_button(self._window, glfw.MOUSE_BUTTON_MIDDLE) == glfw.PRESS
 
         self.last_x, self.last_y = glfw.get_cursor_pos(self._window)
 
@@ -109,16 +112,20 @@
             render_start = time.time()
 
             mujoco.mjv_updateScene(self._model, data, self._scene_option, None, self._camera,
                                    mujoco.mjtCatBit.mjCAT_ALL,
                                    self._scene)
 
             self._viewport.width, self._viewport.height = glfw.get_window_size(self._window)
+
             mujoco.mjr_render(self._viewport, self._scene, self._context)
 
+            if self.custom_render_callback is not None:
+                self.custom_render_callback(self._viewport, self._context)
+
             glfw.swap_buffers(self._window)
             glfw.poll_events()
 
             self.frames += 1
 
             if glfw.window_should_close(self._window):
                 self.stop()
@@ -139,8 +146,7 @@
         while self._loop_count > 0:
             render_inner_loop(self)
             self._loop_count -= 1
 
     def stop(self):
         glfw.destroy_window(self._window)
 
-
```

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/numerical_gradient.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/numerical_gradient.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/optimizers.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/parameters.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/plot.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/plot.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/plots/__init__.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/plots/common_plots.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/plots/common_plots.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/plots/databuffer.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/plots/databuffer.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/plots/plot_item_buffer.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/plots/plot_item_buffer.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/plots/window.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/plots/window.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/preprocessors.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/preprocessors.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/contacts.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/contacts.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/index_map.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/index_map.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/joints_helper.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/joints_helper.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/observation.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/observation.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/pybullet/viewer.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/pybullet/viewer.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/replay_memory.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/replay_memory.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/running_stats.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/running_stats.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/spaces.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/spaces.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/table.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/table.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/torch.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/torch.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/value_functions.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/value_functions.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/variance_parameters.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/variance_parameters.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl/utils/viewer.py` & `mushroom-rl-1.9.2/mushroom_rl/utils/viewer.py`

 * *Files identical despite different names*

### Comparing `mushroom-rl-1.9.1/mushroom_rl.egg-info/PKG-INFO` & `mushroom-rl-1.9.2/mushroom_rl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mushroom-rl
-Version: 1.9.1
+Version: 1.9.2
 Summary: A Python library for Reinforcement Learning experiments.
 Home-page: https://github.com/MushroomRL/mushroom-rl
 Author: Carlo D'Eramo, Davide Tateo
 Author-email: carlo.deramo@gmail.com
 License: MIT
 Description: MushroomRL is a Python Reinforcement Learning (RL) library whose modularity allows to easily use well-known Python libraries for tensor computation (e.g. PyTorch, Tensorflow) and RL benchmarks (e.g. OpenAI Gym, PyBullet, Deepmind Control Suite). It allows to perform RL experiments in a simple way providing classical RL algorithms (e.g. Q-Learning, SARSA, FQI), and deep RL algorithms (e.g. DQN, DDPG, SAC, TD3, TRPO, PPO). Full documentation available at http://mushroomrl.readthedocs.io/en/latest/.
 Platform: UNKNOWN
```

### Comparing `mushroom-rl-1.9.1/mushroom_rl.egg-info/SOURCES.txt` & `mushroom-rl-1.9.2/mushroom_rl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
 setup.py
 mushroom_rl/__init__.py
 mushroom_rl.egg-info/PKG-INFO
@@ -201,25 +200,27 @@
 mushroom_rl/features/_implementations/tiles_features.py
 mushroom_rl/features/_implementations/torch_features.py
 mushroom_rl/features/basis/__init__.py
 mushroom_rl/features/basis/fourier.py
 mushroom_rl/features/basis/gaussian_rbf.py
 mushroom_rl/features/basis/polynomial.py
 mushroom_rl/features/tensors/__init__.py
+mushroom_rl/features/tensors/basis_tensor.py
 mushroom_rl/features/tensors/constant_tensor.py
-mushroom_rl/features/tensors/gaussian_tensor.py
 mushroom_rl/features/tensors/random_fourier_tensor.py
 mushroom_rl/features/tiles/__init__.py
 mushroom_rl/features/tiles/tiles.py
 mushroom_rl/features/tiles/voronoi.py
 mushroom_rl/policy/__init__.py
 mushroom_rl/policy/deterministic_policy.py
+mushroom_rl/policy/dmp.py
 mushroom_rl/policy/gaussian_policy.py
 mushroom_rl/policy/noise_policy.py
 mushroom_rl/policy/policy.py
+mushroom_rl/policy/promps.py
 mushroom_rl/policy/td_policy.py
 mushroom_rl/policy/torch_policy.py
 mushroom_rl/solvers/__init__.py
 mushroom_rl/solvers/car_on_hill.py
 mushroom_rl/solvers/dynamic_programming.py
 mushroom_rl/solvers/lqr.py
 mushroom_rl/utils/__init__.py
@@ -260,9 +261,8 @@
 mushroom_rl/utils/plots/plot_item_buffer.py
 mushroom_rl/utils/plots/window.py
 mushroom_rl/utils/pybullet/__init__.py
 mushroom_rl/utils/pybullet/contacts.py
 mushroom_rl/utils/pybullet/index_map.py
 mushroom_rl/utils/pybullet/joints_helper.py
 mushroom_rl/utils/pybullet/observation.py
-mushroom_rl/utils/pybullet/viewer.py
-tests/test_imports.py
+mushroom_rl/utils/pybullet/viewer.py
```

### Comparing `mushroom-rl-1.9.1/setup.py` & `mushroom-rl-1.9.2/setup.py`

 * *Files identical despite different names*

