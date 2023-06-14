# Comparing `tmp/pyrfuniverse-0.8.3.tar.gz` & `tmp/pyrfuniverse-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfuniverse-0.8.3.tar", last modified: Thu Apr 13 03:57:00 2023, max compression
+gzip compressed data, was "pyrfuniverse-0.8.4.tar", last modified: Sat May  6 08:25:23 2023, max compression
```

## Comparing `pyrfuniverse-0.8.3.tar` & `pyrfuniverse-0.8.4.tar`

### file list

```diff
@@ -1,167 +1,176 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.412731 pyrfuniverse-0.8.3/
--rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.8.3/LICENSE
--rw-rw-rw-   0        0        0      269 2023-04-13 03:57:00.412731 pyrfuniverse-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     2639 2023-04-10 05:02:29.000000 pyrfuniverse-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 03:56:59.656519 pyrfuniverse-0.8.3/pyrfuniverse/
--rw-rw-rw-   0        0        0      758 2023-04-13 03:24:35.000000 pyrfuniverse-0.8.3/pyrfuniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:56:59.756619 pyrfuniverse-0.8.3/pyrfuniverse/attributes/
--rw-rw-rw-   0        0        0     1312 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/activelightsensor_attr.py
--rw-rw-rw-   0        0        0    13595 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/base_attr.py
--rw-rw-rw-   0        0        0    17611 2023-04-10 10:01:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/camera_attr.py
--rw-rw-rw-   0        0        0      403 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/cloth_attr.py
--rw-rw-rw-   0        0        0     1074 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/collider_attr.py
--rw-rw-rw-   0        0        0    31372 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/controller_attr.py
--rw-rw-rw-   0        0        0     1162 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/custom_attr.py
--rw-rw-rw-   0        0        0     1143 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/digit_attr.py
--rw-rw-rw-   0        0        0     3498 2023-04-06 04:49:14.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/gameobject_attr.py
--rw-rw-rw-   0        0        0     5346 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/graspsim_attr.py
--rw-rw-rw-   0        0        0     8403 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/humanbody_attr.py
--rw-rw-rw-   0        0        0     3157 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/light_attr.py
--rw-rw-rw-   0        0        0     1647 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/pointcloud_attr.py
--rw-rw-rw-   0        0        0     3103 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/rigidbody_attr.py
--rw-rw-rw-   0        0        0      407 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/attributes/softbody_attr.py
--rw-rw-rw-   0        0        0    23240 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/base_env.py
--rw-rw-rw-   0        0        0     1885 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:56:59.944455 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/
--rw-rw-rw-   0        0        0      835 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/__init__.py
--rw-rw-rw-   0        0        0     3785 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_action_pb2.py
--rw-rw-rw-   0        0        0     3885 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py
--rw-rw-rw-   0        0        0     5849 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_info_pb2.py
--rw-rw-rw-   0        0        0     8080 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/brain_parameters_pb2.py
--rw-rw-rw-   0        0        0     5258 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/capabilities_pb2.py
--rw-rw-rw-   0        0        0     2073 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/command_pb2.py
--rw-rw-rw-   0        0        0     2134 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py
--rw-rw-rw-   0        0        0     4261 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py
--rw-rw-rw-   0        0        0     4647 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/engine_configuration_pb2.py
--rw-rw-rw-   0        0        0     2709 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/header_pb2.py
--rw-rw-rw-   0        0        0     9625 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/observation_pb2.py
--rw-rw-rw-   0        0        0     1979 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/space_type_pb2.py
--rw-rw-rw-   0        0        0    12746 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/training_analytics_pb2.py
--rw-rw-rw-   0        0        0     3893 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_input_pb2.py
--rw-rw-rw-   0        0        0     4553 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_message_pb2.py
--rw-rw-rw-   0        0        0     3928 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_output_pb2.py
--rw-rw-rw-   0        0        0     4512 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py
--rw-rw-rw-   0        0        0     5963 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py
--rw-rw-rw-   0        0        0     8094 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py
--rw-rw-rw-   0        0        0     7216 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py
--rw-rw-rw-   0        0        0     2353 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_to_external_pb2.py
--rw-rw-rw-   0        0        0     1775 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py
--rw-rw-rw-   0        0        0     5172 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/env_utils.py
--rw-rw-rw-   0        0        0    22704 2023-04-07 06:51:48.000000 pyrfuniverse-0.8.3/pyrfuniverse/environment.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.026548 pyrfuniverse-0.8.3/pyrfuniverse/envs/
--rw-rw-rw-   0        0        0    14453 2023-04-07 06:50:32.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/__init__.py
--rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/balance_ball_env.py
--rw-rw-rw-   0        0        0    24331 2023-04-12 12:00:38.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/base_env.py
--rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/bouncer_env.py
--rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/franka_grasp_env.py
--rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/franka_push_env.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.068341 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/
--rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/__init__.py
--rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/nail_can_env.py
--rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/nail_card_env.py
--rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
--rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
--rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
--rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
--rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.081873 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/
--rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/cleaner_env.py
--rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/navigation_env.py
--rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent_navigation_env.py
--rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.123240 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/
--rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/__init__.py
--rw-rw-rw-   0        0        0     7357 2022-12-15 06:20:36.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_cloth_env.py
--rw-rw-rw-   0        0        0     7455 2022-12-15 06:20:57.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
--rw-rw-rw-   0        0        0    10181 2022-12-15 08:02:41.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_robotics_env.py
--rw-rw-rw-   0        0        0     8041 2022-12-15 06:20:52.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_softbody_env.py
--rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/pick_and_place_env.py
--rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/push_env.py
--rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/reach_env.py
--rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/roller_env.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.132265 pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotics/
--rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotics/__init__.py
--rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
--rw-rw-rw-   0        0        0     9736 2023-02-15 08:33:33.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
--rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/ur5_box_env.py
--rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.3/pyrfuniverse/envs/ur5_drawer_env.py
--rw-rw-rw-   0        0        0     1621 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/exception.py
--rw-rw-rw-   0        0        0     1866 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/logging_util.py
--rw-rw-rw-   0        0        0     3924 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/mock_communicator.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.161918 pyrfuniverse-0.8.3/pyrfuniverse/registry/
--rw-rw-rw-   0        0        0      114 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/__init__.py
--rw-rw-rw-   0        0        0     1855 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/base_registry_entry.py
--rw-rw-rw-   0        0        0     8085 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/binary_utils.py
--rw-rw-rw-   0        0        0     3256 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/remote_registry_entry.py
--rw-rw-rw-   0        0        0     5017 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/registry/unity_env_registry.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.192601 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/
--rw-rw-rw-   0        0        0      496 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/__init__.py
--rw-rw-rw-   0        0        0    10343 2023-04-07 06:50:42.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/asset_channel.py
--rw-rw-rw-   0        0        0     1248 2023-03-15 04:59:29.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/asset_channel_ext.py
--rw-rw-rw-   0        0        0     1738 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/debug_channel.py
--rw-rw-rw-   0        0        0     2244 2023-04-06 04:49:14.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/instance_channel.py
--rw-rw-rw-   0        0        0     2198 2022-08-25 10:50:54.000000 pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py
--rw-rw-rw-   0        0        0     6426 2022-09-28 07:41:12.000000 pyrfuniverse-0.8.3/pyrfuniverse/rpc_communicator.py
--rw-rw-rw-   0        0        0    16840 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/rpc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.239722 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/
--rw-rw-rw-   0        0        0      230 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/__init__.py
--rw-rw-rw-   0        0        0     4935 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/engine_configuration_channel.py
--rw-rw-rw-   0        0        0     3872 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/environment_parameters_channel.py
--rw-rw-rw-   0        0        0     2226 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/float_properties_channel.py
--rw-rw-rw-   0        0        0     3366 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/incoming_message.py
--rw-rw-rw-   0        0        0     1960 2022-09-06 06:01:55.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/outgoing_message.py
--rw-rw-rw-   0        0        0     1300 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/raw_bytes_channel.py
--rw-rw-rw-   0        0        0     1502 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/side_channel.py
--rw-rw-rw-   0        0        0     3745 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/side_channel_manager.py
--rw-rw-rw-   0        0        0     1875 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/side_channel/stats_side_channel.py
--rw-rw-rw-   0        0        0    11684 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/timers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.297933 pyrfuniverse-0.8.3/pyrfuniverse/utils/
--rw-rw-rw-   0        0        0      181 2022-10-31 06:20:22.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/__init__.py
--rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/active_depth_generate.py
--rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/controller.py
--rw-rw-rw-   0        0        0    10354 2023-02-10 17:44:40.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/depth_processor.py
--rw-rw-rw-   0        0        0     3218 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/interpolate_utils.py
--rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/jaco_controller.py
--rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/kinova_controller.py
--rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/os_utils.py
--rw-rw-rw-   0        0        0     2656 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/rfuniverse_utility.py
--rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/stretch_controller.py
--rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/tobor_controller.py
--rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.3/pyrfuniverse/utils/ur5_controller.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:56:59.670053 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/
--rw-rw-rw-   0        0        0      269 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6086 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-10-31 04:29:22.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      120 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 03:56:59.000000 pyrfuniverse-0.8.3/pyrfuniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 03:57:00.412731 pyrfuniverse-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-04-07 06:52:00.000000 pyrfuniverse-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:57:00.411729 pyrfuniverse-0.8.3/test/
--rw-rw-rw-   0        0        0     5651 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_active_depth.py
--rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_articulation_ik.py
--rw-rw-rw-   0        0        0      766 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_camera_image.py
--rw-rw-rw-   0        0        0     1197 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_custom_message.py
--rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.8.3/test/test_debug.py
--rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.8.3/test/test_digit.py
--rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_grasp_pose.py
--rw-rw-rw-   0        0        0     2758 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_grasp_sim.py
--rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.8.3/test/test_heat_map.py
--rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_humanbody_ik.py
--rw-rw-rw-   0        0        0     1996 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_label.py
--rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_light.py
--rw-rw-rw-   0        0        0      589 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_load_mesh.py
--rw-rw-rw-   0        0        0     1010 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_load_urdf.py
--rw-rw-rw-   0        0        0     1137 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_object_data.py
--rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.8.3/test/test_pick_and_place.py
--rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.8.3/test/test_pick_and_place_flexiv.py
--rw-rw-rw-   0        0        0      570 2022-12-18 09:24:39.000000 pyrfuniverse-0.8.3/test/test_pick_and_place_gym.py
--rw-rw-rw-   0        0        0     1746 2023-03-15 04:45:24.000000 pyrfuniverse-0.8.3/test/test_point_cloud.py
--rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_point_cloud_render.py
--rw-rw-rw-   0        0        0     1891 2023-03-15 04:50:29.000000 pyrfuniverse-0.8.3/test/test_point_cloud_with_intrinsic_matrix.py
--rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.8.3/test/test_save_gripper.py
--rw-rw-rw-   0        0        0      380 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_save_obj.py
--rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.3/test/test_scene.py
--rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.8.3/test/test_tobor_move.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.387881 pyrfuniverse-0.8.4/
+-rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.8.4/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-05-06 08:25:23.387881 pyrfuniverse-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2766 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:22.644911 pyrfuniverse-0.8.4/pyrfuniverse/
+-rw-rw-rw-   0        0        0      758 2023-05-06 07:33:51.000000 pyrfuniverse-0.8.4/pyrfuniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:22.754807 pyrfuniverse-0.8.4/pyrfuniverse/attributes/
+-rw-rw-rw-   0        0        0     1338 2023-05-06 06:06:02.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/activelightsensor_attr.py
+-rw-rw-rw-   0        0        0    15090 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/base_attr.py
+-rw-rw-rw-   0        0        0    18228 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/camera_attr.py
+-rw-rw-rw-   0        0        0      528 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/cloth_attr.py
+-rw-rw-rw-   0        0        0     1229 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/collider_attr.py
+-rw-rw-rw-   0        0        0    34155 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/controller_attr.py
+-rw-rw-rw-   0        0        0     1563 2023-05-05 11:23:54.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/custom_attr.py
+-rw-rw-rw-   0        0        0     1141 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/digit_attr.py
+-rw-rw-rw-   0        0        0     2521 2023-05-06 06:06:02.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/falling_cloth_attr.py
+-rw-rw-rw-   0        0        0     3655 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/gameobject_attr.py
+-rw-rw-rw-   0        0        0     5700 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/graspsim_attr.py
+-rw-rw-rw-   0        0        0     8856 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/humanbody_attr.py
+-rw-rw-rw-   0        0        0     3591 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/light_attr.py
+-rw-rw-rw-   0        0        0     1998 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/pointcloud_attr.py
+-rw-rw-rw-   0        0        0     3460 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/rigidbody_attr.py
+-rw-rw-rw-   0        0        0      529 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/attributes/softbody_attr.py
+-rw-rw-rw-   0        0        0    23240 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/base_env.py
+-rw-rw-rw-   0        0        0     1928 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:22.934702 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/
+-rw-rw-rw-   0        0        0      835 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/__init__.py
+-rw-rw-rw-   0        0        0     3785 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/agent_action_pb2.py
+-rw-rw-rw-   0        0        0     3885 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py
+-rw-rw-rw-   0        0        0     5849 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/agent_info_pb2.py
+-rw-rw-rw-   0        0        0     8080 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/brain_parameters_pb2.py
+-rw-rw-rw-   0        0        0     5258 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/capabilities_pb2.py
+-rw-rw-rw-   0        0        0     2073 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/command_pb2.py
+-rw-rw-rw-   0        0        0     2134 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py
+-rw-rw-rw-   0        0        0     4261 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py
+-rw-rw-rw-   0        0        0     4647 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/engine_configuration_pb2.py
+-rw-rw-rw-   0        0        0     2709 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/header_pb2.py
+-rw-rw-rw-   0        0        0     9625 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/observation_pb2.py
+-rw-rw-rw-   0        0        0     1979 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/space_type_pb2.py
+-rw-rw-rw-   0        0        0    12746 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/training_analytics_pb2.py
+-rw-rw-rw-   0        0        0     3893 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_input_pb2.py
+-rw-rw-rw-   0        0        0     4553 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_message_pb2.py
+-rw-rw-rw-   0        0        0     3928 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_output_pb2.py
+-rw-rw-rw-   0        0        0     4512 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py
+-rw-rw-rw-   0        0        0     5963 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py
+-rw-rw-rw-   0        0        0     8094 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py
+-rw-rw-rw-   0        0        0     7216 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py
+-rw-rw-rw-   0        0        0     2353 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_to_external_pb2.py
+-rw-rw-rw-   0        0        0     1775 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5302 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/env_utils.py
+-rw-rw-rw-   0        0        0    22704 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/environment.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:22.994353 pyrfuniverse-0.8.4/pyrfuniverse/envs/
+-rw-rw-rw-   0        0        0    14453 2023-04-07 06:50:32.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/__init__.py
+-rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/balance_ball_env.py
+-rw-rw-rw-   0        0        0    27320 2023-05-06 06:57:55.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/base_env.py
+-rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/bouncer_env.py
+-rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/franka_grasp_env.py
+-rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/franka_push_env.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.028863 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/
+-rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/__init__.py
+-rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/nail_can_env.py
+-rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/nail_card_env.py
+-rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
+-rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
+-rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
+-rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
+-rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.041395 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_agent/
+-rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_agent/cleaner_env.py
+-rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_agent/navigation_env.py
+-rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_agent_navigation_env.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.056906 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_physics/
+-rw-rw-rw-   0        0        0      871 2023-05-06 03:28:26.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_physics/__init__.py
+-rw-rw-rw-   0        0        0    15160 2023-05-06 06:55:59.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
+-rw-rw-rw-   0        0        0     8907 2023-05-06 06:23:01.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
+-rw-rw-rw-   0        0        0    10805 2023-05-06 05:15:38.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
+-rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.102927 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/
+-rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/__init__.py
+-rw-rw-rw-   0        0        0     7357 2022-12-15 06:20:36.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/franka_cloth_env.py
+-rw-rw-rw-   0        0        0     7455 2022-12-15 06:20:57.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
+-rw-rw-rw-   0        0        0    10096 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/franka_robotics_env.py
+-rw-rw-rw-   0        0        0     8041 2022-12-15 06:20:52.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/franka_softbody_env.py
+-rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/pick_and_place_env.py
+-rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/push_env.py
+-rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/reach_env.py
+-rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/roller_env.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.115434 pyrfuniverse-0.8.4/pyrfuniverse/envs/tobor_robotics/
+-rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/tobor_robotics/__init__.py
+-rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
+-rw-rw-rw-   0        0        0     9736 2023-02-15 08:33:33.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
+-rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/ur5_box_env.py
+-rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.4/pyrfuniverse/envs/ur5_drawer_env.py
+-rw-rw-rw-   0        0        0     1707 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/exception.py
+-rw-rw-rw-   0        0        0     1929 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/logging_util.py
+-rw-rw-rw-   0        0        0     4035 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/mock_communicator.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.137434 pyrfuniverse-0.8.4/pyrfuniverse/registry/
+-rw-rw-rw-   0        0        0      114 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/registry/__init__.py
+-rw-rw-rw-   0        0        0     1855 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/registry/base_registry_entry.py
+-rw-rw-rw-   0        0        0     8085 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/registry/binary_utils.py
+-rw-rw-rw-   0        0        0     3256 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/registry/remote_registry_entry.py
+-rw-rw-rw-   0        0        0     5017 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/registry/unity_env_registry.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.167461 pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/
+-rw-rw-rw-   0        0        0      496 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/__init__.py
+-rw-rw-rw-   0        0        0    10422 2023-05-06 05:20:26.000000 pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/asset_channel.py
+-rw-rw-rw-   0        0        0     1317 2023-05-05 11:23:54.000000 pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/asset_channel_ext.py
+-rw-rw-rw-   0        0        0     1738 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/debug_channel.py
+-rw-rw-rw-   0        0        0     2244 2023-05-05 07:36:54.000000 pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/instance_channel.py
+-rw-rw-rw-   0        0        0     2198 2022-08-25 10:50:54.000000 pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py
+-rw-rw-rw-   0        0        0     6579 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/rpc_communicator.py
+-rw-rw-rw-   0        0        0    16840 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/rpc_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.208126 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/
+-rw-rw-rw-   0        0        0      230 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/__init__.py
+-rw-rw-rw-   0        0        0     4935 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/engine_configuration_channel.py
+-rw-rw-rw-   0        0        0     3872 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/environment_parameters_channel.py
+-rw-rw-rw-   0        0        0     2226 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/float_properties_channel.py
+-rw-rw-rw-   0        0        0     3366 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/incoming_message.py
+-rw-rw-rw-   0        0        0     1960 2022-09-06 06:01:55.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/outgoing_message.py
+-rw-rw-rw-   0        0        0     1300 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/raw_bytes_channel.py
+-rw-rw-rw-   0        0        0     1502 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/side_channel.py
+-rw-rw-rw-   0        0        0     3745 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/side_channel_manager.py
+-rw-rw-rw-   0        0        0     1875 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/side_channel/stats_side_channel.py
+-rw-rw-rw-   0        0        0    12046 2023-05-05 07:34:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/timers.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.259842 pyrfuniverse-0.8.4/pyrfuniverse/utils/
+-rw-rw-rw-   0        0        0      181 2022-10-31 06:20:22.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/active_depth_generate.py
+-rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/controller.py
+-rw-rw-rw-   0        0        0    11646 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/depth_processor.py
+-rw-rw-rw-   0        0        0     3218 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/interpolate_utils.py
+-rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/jaco_controller.py
+-rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/kinova_controller.py
+-rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/os_utils.py
+-rw-rw-rw-   0        0        0     3569 2023-05-05 07:38:30.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/rfuniverse_utility.py
+-rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/stretch_controller.py
+-rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/tobor_controller.py
+-rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.4/pyrfuniverse/utils/ur5_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:22.657927 pyrfuniverse-0.8.4/pyrfuniverse.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-05-06 08:25:22.000000 pyrfuniverse-0.8.4/pyrfuniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6442 2023-05-06 08:25:22.000000 pyrfuniverse-0.8.4/pyrfuniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 08:25:22.000000 pyrfuniverse-0.8.4/pyrfuniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2022-10-31 04:29:22.000000 pyrfuniverse-0.8.4/pyrfuniverse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      120 2023-05-06 08:25:22.000000 pyrfuniverse-0.8.4/pyrfuniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 08:25:22.000000 pyrfuniverse-0.8.4/pyrfuniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 08:25:23.387881 pyrfuniverse-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-04-07 06:52:00.000000 pyrfuniverse-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 08:25:23.386880 pyrfuniverse-0.8.4/test/
+-rw-rw-rw-   0        0        0     5651 2023-05-05 07:36:54.000000 pyrfuniverse-0.8.4/test/test_active_depth.py
+-rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_articulation_ik.py
+-rw-rw-rw-   0        0        0      766 2023-05-05 07:36:54.000000 pyrfuniverse-0.8.4/test/test_camera_image.py
+-rw-rw-rw-   0        0        0      279 2023-05-06 05:55:09.000000 pyrfuniverse-0.8.4/test/test_catching_cloth_gym.py
+-rw-rw-rw-   0        0        0     1143 2023-05-05 11:23:54.000000 pyrfuniverse-0.8.4/test/test_custom_message.py
+-rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.8.4/test/test_debug.py
+-rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.8.4/test/test_digit.py
+-rw-rw-rw-   0        0        0      217 2023-05-06 03:26:42.000000 pyrfuniverse-0.8.4/test/test_flexiv_cutting_gym.py
+-rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_grasp_pose.py
+-rw-rw-rw-   0        0        0     2758 2023-05-05 07:36:54.000000 pyrfuniverse-0.8.4/test/test_grasp_sim.py
+-rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.8.4/test/test_heat_map.py
+-rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_humanbody_ik.py
+-rw-rw-rw-   0        0        0     1996 2023-05-05 07:36:54.000000 pyrfuniverse-0.8.4/test/test_label.py
+-rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_light.py
+-rw-rw-rw-   0        0        0      589 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_load_mesh.py
+-rw-rw-rw-   0        0        0     1010 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_load_urdf.py
+-rw-rw-rw-   0        0        0     1137 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_object_data.py
+-rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.8.4/test/test_pick_and_place.py
+-rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.8.4/test/test_pick_and_place_flexiv.py
+-rw-rw-rw-   0        0        0      570 2022-12-18 09:24:39.000000 pyrfuniverse-0.8.4/test/test_pick_and_place_gym.py
+-rw-rw-rw-   0        0        0     1746 2023-05-05 07:36:54.000000 pyrfuniverse-0.8.4/test/test_point_cloud.py
+-rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_point_cloud_render.py
+-rw-rw-rw-   0        0        0     1938 2023-05-05 07:36:54.000000 pyrfuniverse-0.8.4/test/test_point_cloud_with_intrinsic_matrix.py
+-rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.8.4/test/test_save_gripper.py
+-rw-rw-rw-   0        0        0      380 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_save_obj.py
+-rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.4/test/test_scene.py
+-rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.8.4/test/test_tobor_move.py
+-rw-rw-rw-   0        0        0      266 2023-05-06 04:59:45.000000 pyrfuniverse-0.8.4/test/test_water_shooting_gym.py
```

### Comparing `pyrfuniverse-0.8.3/LICENSE` & `pyrfuniverse-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/README.md` & `pyrfuniverse-0.8.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,87 @@
-# pyrfuniverse
-
-[![Pypi](https://img.shields.io/pypi/v/pyrfuniverse.svg)](https://pypi.org/project/pyrfuniverse/)
-
-`pyrfuniverse` is a python package used to interact with `RFUniverse` simulation environment. It is developed upon
-[ML-Agents](https://github.com/Unity-Technologies/ml-agents) and produce new features.
-
-[Documentation](https://knotty-watch-cad.notion.site/RFUniverse-3afda956497b4c33b5a45f68b49d9816)：It is currently mostly in Chinese, we are working on finishing it and translating to English.
-
-**Note:** current branch is under development.
-
-## Installation
-
-### 1. Create a new conda virtual environment and activate it.
-
-```shell
-conda create -n rfuniverse python=3.8 -y
-conda activate rfuniverse
-```
-
-### 2. Clone this repository and move here in command line.
-
-```shell
-git clone https://github.com/mvig-robotflow/pyrfuniverse.git
-cd pyrfuniverse
-```
-
-### 3. Install the python requirements.
-
-```shell
-pip install -r requirements.txt
-```
-
-For users in China, please remember to change mirror by the following command. This can significantly accelerate
-downloading speed.
-
-```shell
-pip install -i https://mirrors.aliyun.com/pypi/simple -r requirements.txt
-```
-
-### 4. Install `pyrfuniverse`.
-
-If you want to use `pyrfuniverse` without modifying source code, run the following commands to copy source code to your conda directory.
-
-```shell
-python setup.py install
-```
-
-Otherwise, you may want to modify source code, then run the following command to construct the link in your conda directory.
-
-```shell
-pip install -e .
-```
-
-## Headless mode
-
-If you want to run `RFUniverse` on ubuntu server, you will need **headless** mode so that no GUI window will be
-generated. To fix this, we use `virtual display` to render on virtual devices, inspired by
-[furniture](https://github.com/clvrai/furniture/blob/master/docs/installation.md#virtual-display-on-headless-machines).
-You will need the following commands to configure your ubuntu server
-
-```shell
-sudo apt-get install xserver-xorg libglu1-mesa-dev freeglut3-dev mesa-common-dev libxmu-dev libxi-dev
-```
-
-Then, restart your server and connect your server to a screen. The screen won't render anything, but there must be a
-display device connecting to your server.
-
-```shell
-# Configure nvidia-x
-sudo nvidia-xconfig -a --use-display-device=None --virtual=1280x1024
-
-# Configure environment variable
-export DISPLAY=:1
-
-# Launch a virtual display
-sudo /usr/bin/X :1 &
-```
-
-Here's a [demo](./docs/headless_mode_demo.md). I strongly recommend you run this demo first to test your virtual display
-configuration.
-
-After this, you can use `RFUniverse` on ubuntu server freely!
+# pyrfuniverse
+
+[![Pypi](https://img.shields.io/pypi/v/pyrfuniverse.svg)](https://pypi.org/project/pyrfuniverse/)
+
+`pyrfuniverse` is a python package used to interact with `RFUniverse` simulation environment. It is developed upon
+[ML-Agents](https://github.com/Unity-Technologies/ml-agents) and produce new features.
+
+[Documentation](https://mvig-robotflow.github.io/pyrfuniverse/)
+
+[Homepage](https://sites.google.com/view/rfuniverse)
+
+<!-- [Documentation-Chinese](https://knotty-watch-cad.notion.site/RFUniverse-3afda956497b4c33b5a45f68b49d9816) -->
+
+**Note:** current branch is under development.
+
+## Installation
+
+### 1. Create a new conda virtual environment and activate it.
+
+```shell
+conda create -n rfuniverse python=3.8 -y
+conda activate rfuniverse
+```
+
+### 2. Clone this repository and move here in command line.
+
+```shell
+git clone https://github.com/mvig-robotflow/pyrfuniverse.git
+cd pyrfuniverse
+```
+
+### 3. Install the python requirements.
+
+```shell
+pip install -r requirements.txt
+```
+
+For users in China, please remember to change mirror by the following command. This can significantly accelerate
+downloading speed.
+
+```shell
+pip install -i https://mirrors.aliyun.com/pypi/simple -r requirements.txt
+```
+
+### 4. Install `pyrfuniverse`.
+
+If you want to use `pyrfuniverse` without modifying source code, run the following commands to copy source code to your conda directory.
+
+```shell
+python setup.py install
+```
+
+Otherwise, you may want to modify source code, then run the following command to construct the link in your conda directory.
+
+```shell
+pip install -e .
+```
+
+## Headless mode
+
+If you want to run `RFUniverse` on ubuntu server, you will need **headless** mode so that no GUI window will be
+generated. To fix this, we use `virtual display` to render on virtual devices, inspired by
+[furniture](https://github.com/clvrai/furniture/blob/master/docs/installation.md#virtual-display-on-headless-machines).
+You will need the following commands to configure your ubuntu server
+
+```shell
+sudo apt-get install xserver-xorg libglu1-mesa-dev freeglut3-dev mesa-common-dev libxmu-dev libxi-dev
+```
+
+Then, restart your server and connect your server to a screen. The screen won't render anything, but there must be a
+display device connecting to your server.
+
+```shell
+# Configure nvidia-x
+sudo nvidia-xconfig -a --use-display-device=None --virtual=1280x1024
+
+# Configure environment variable
+export DISPLAY=:1
+
+# Launch a virtual display
+sudo /usr/bin/X :1 &
+```
+
+Here's a [demo](./docs/headless_mode_demo.md). I strongly recommend you run this demo first to test your virtual display
+configuration.
+
+After this, you can use `RFUniverse` on ubuntu server freely!
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/__init__.py` & `pyrfuniverse-0.8.4/pyrfuniverse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the library that will be used to upload to pypi
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 import os.path
 import json
 
 def read_config():
     if not os.path.exists(config_path):
         config = {}
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/__init__.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,13 +8,17 @@
 from pyrfuniverse.attributes.rigidbody_attr import RigidbodyAttr
 from pyrfuniverse.attributes.cloth_attr import ClothAttr
 from pyrfuniverse.attributes.softbody_attr import SoftbodyAttr
 from pyrfuniverse.attributes.humanbody_attr import HumanbodyAttr
 from pyrfuniverse.attributes.graspsim_attr import GraspSimAttr
 from pyrfuniverse.attributes.digit_attr import DigitAttr
 from pyrfuniverse.attributes.pointcloud_attr import PointCloudAttr
+from pyrfuniverse.attributes.falling_cloth_attr import FallingClothAttr
 from pyrfuniverse.attributes.custom_attr import CustomAttr
 
-# 新增脚本的命名规则必须是 *_attr,此处名称必须与Unity中保持一致
 __all__ = [
-    'base_attr', 'camera_attr', 'activelightsensor_attr', 'collider_attr', 'controller_attr', 'gameobject_attr', 'rigidbody_attr', 'cloth_attr', 'softbody_attr', 'humanbody_attr', 'graspsim_attr', 'digit_attr', 'pointcloud_attr', 'custom_attr'
+    'base_attr', 'camera_attr', 'activelightsensor_attr',
+    'collider_attr', 'controller_attr', 'gameobject_attr',
+    'rigidbody_attr', 'cloth_attr', 'softbody_attr',
+    'humanbody_attr', 'graspsim_attr', 'digit_attr',
+    'pointcloud_attr', 'falling_cloth_attr', 'custom_attr'
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/activelightsensor_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/activelightsensor_attr.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,27 +7,29 @@
     IncomingMessage,
     OutgoingMessage,
 )
 
 
 class ActiveLightSensorAttr(attr.CameraAttr):
     """
-    红外深度传感器类，能够获取模拟真实深度相机噪声的深度图
+    Class of IR-based depth sensor, which can simulate the noise of 
+    real-world depth camera and produce depth image in similar pattern.
     """
     def __init__(self, env, id: int, data=None):
         super().__init__(env, id, data)
         self.main_intrinsic_matrix = np.eye(4)
         self.ir_intrinsic_matrix = np.eye(4)
 
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-            self.data['active_depth'] 红外深度图，shape = [w,h]
+            Dict: A dict containing useful information of this class.\n
+            self.data['active_depth']: IR-based depth, shape = (w,h)
         """
         super().parse_message(msg)
         if msg.read_bool() is True:
             self.data['ir_left'] = base64.b64decode(msg.read_string())
             self.data['ir_right'] = base64.b64decode(msg.read_string())
 
             image_left = np.frombuffer(self.data['ir_left'], dtype=np.uint8)
@@ -59,22 +61,19 @@
                                                                                         use_noise=False)
             self.data['active_depth'][self.data['active_depth'] > 8.] = 0
             self.data['active_depth'][self.data['active_depth'] < 0.1] = 0
         return self.data
 
     def GetActiveDepth(self, main_intrinsic_matrix_local: list, ir_intrinsic_matrix_local: list):
         """
-        获取红外深度图
+        Get IR-based depth image.
 
         Args:
-            main_intrinsic_matrix_local: List[float]主相机内参
-            ir_intrinsic_matrix_local: List[float]红外相机内参
-
-        Returns:
-            调用此接口并step后，从self.data['active_depth']获取结果
+            main_intrinsic_matrix_local: List[float] The intrinsic matrix of main camera.
+            ir_intrinsic_matrix_local: List[float] The intrinsic matrix of IR-based camera.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('GetActiveDepth')
         self.main_intrinsic_matrix = np.reshape(main_intrinsic_matrix_local, [3, 3]).T
         self.ir_intrinsic_matrix = np.reshape(ir_intrinsic_matrix_local, [3, 3]).T
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/base_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/base_attr.py`

 * *Files 8% similar despite different names*

```diff
@@ -179,47 +179,50 @@
     msg.write_float32(kwargs['point'][1])
     msg.write_float32(kwargs['point'][2])
     return msg
 
 
 class BaseAttr:
     """
-    基础Attr类，包含物体加载删除移动等通用功能
+    Base attribute class, which includes general functions such as 
+    object loading, deleting and transforming.
     """
     def __init__(self, env, id: int, data=None):
         if data is None:
             data = {}
         self.env = env
         self.id = id
         self.data = data
 
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-            self.data['name'] 物体名称
+            Dict: A dict containing useful information of this class.
 
-            self.data['position'] 物体世界坐标
+            self.data['name']: The name of the object.
 
-            self.data['rotation'] 物体世界欧拉角
+            self.data['position']: The position of the object in world coordinate.
 
-            self.data['quaternion'] 物体世界四元数
+            self.data['rotation']: The euler angle of the object in world coordinate.
 
-            self.data['local_position'] 物体局部坐标
+            self.data['quaternion']: The quaternion of the object in world coordinate.
 
-            self.data['local_rotation'] 物体局部欧拉角
+            self.data['local_position']: The position of the object in its parent's local coordinate.
 
-            self.data['local_quaternion'] 物体局部四元数
+            self.data['local_rotation']: The euler angle of the object in its parent's local coordinate.
 
-            self.data['local_to_world_matrix'] 物体局部坐标转世界坐标矩阵
+            self.data['local_quaternion']: The quaternion of the object in its parent's local coordinate.
 
-            self.data['result_local_point'] 物体局部坐标转世界坐标结果
+            self.data['local_to_world_matrix']: The transformation matrix from local to world coordinate.
 
-            self.data['result_world_point'] 物体世界坐标转局部坐标结果
+            self.data['result_local_point']: The result of transforming object from local to world coordinate.
+
+            self.data['result_world_point']: The result of transforming object from world to local coordinate.
         """
         self.data['name'] = msg.read_string()
         self.data['position'] = [msg.read_float32() for _ in range(3)]
         self.data['rotation'] = [msg.read_float32() for _ in range(3)]
         self.data['quaternion'] = [msg.read_float32() for _ in range(4)]
         self.data['local_position'] = [msg.read_float32() for _ in range(3)]
         self.data['local_rotation'] = [msg.read_float32() for _ in range(3)]
@@ -231,33 +234,34 @@
             self.data['result_local_point'] = msg.read_float32_list()
         if msg.read_bool() is True:
             self.data['result_world_point'] = msg.read_float32_list()
         return self.data
 
     def SetType(self, attr_type: type):
         """
-        设置物体Attr类型
+        Set the attribute type of this object
 
         Args:
-            attr_type:类型参数
+            attr_type: Any attribute in pyrfuniverse.attributes.
 
-        Returns:目标类型实例
+        Returns:
+            The target attribute.
         """
         self.env.attrs[self.id] = attr_type(self.env, self.id, self.data)
         return self.env.attrs[self.id]
 
     def SetTransform(self, position: list = None, rotation: list = None, scale: list = None, is_world: bool = True):
         """
-        使用Vector3设置物体pose
+        Set the transform of this object, including position, rotation, scale and coordinate.
 
         Args:
-            position: 位置
-            rotation: 旋转
-            scale: 缩放
-            is_world: 世界空间/局部空间
+            position: A list of length 3, representing the target position value of object.
+            rotation: A list of length 3, representing the target euler angle value of object.
+            scale: A list of length 3, representing the target scale value of object.
+            is_world: Bool, True for world coordinate, False for local coordinate.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetTransform')
         msg.write_bool(position is not None)
         msg.write_bool(rotation is not None)
@@ -279,55 +283,55 @@
                 msg.write_float32(scale[i])
         msg.write_bool(is_world)
 
         self.env.instance_channel.send_message(msg)
 
     def Translate(self, translation: list, is_world: bool = True):
         """
-        物体平移
+        Translate this object.
 
         Args:
-            translation: 平移量
-            is_world: 世界空间/局部空间
+            translation: A list of length 3, representing the translation from current position.
+            is_world: Bool, True for world coordinate, False for local coordinate.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('Translate')
         for i in range(3):
             msg.write_float32(translation[i])
         msg.write_bool(is_world)
 
         self.env.instance_channel.send_message(msg)
 
     def Rotate(self, rotation: list, is_world: bool = True):
         """
-        物体旋转
+        Rotate this object.
 
         Args:
-            rotation: 旋转量
-            is_world: 世界空间/局部空间
+            rotation: A list of length 3, representing the euler-angle-format rotation from current euler angle.
+            is_world: Bool, True for world coordinate, False for local coordinate.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('Rotate')
         for i in range(3):
             msg.write_float32(rotation[i])
         msg.write_bool(is_world)
 
         self.env.instance_channel.send_message(msg)
 
     def SetRotationQuaternion(self, quaternion: list = None, is_world: bool = True):
         """
-        使用四元数设置物体旋转
+        Rotate this object using quaternion.
 
         Args:
-            quaternion: 四元数
-            is_world: 世界空间or局部空间
+            quaternion: A list of length 4, representing the quaternion from current pose.
+            is_world: Bool, True for world coordinate, False for local coordinate.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetRotationQuaternion')
         assert type(quaternion) == list and len(quaternion) == 3, \
             'Argument quaternion must be a 4-d list.'
@@ -335,127 +339,127 @@
             msg.write_float32(quaternion[i])
         msg.write_bool(is_world)
 
         self.env.instance_channel.send_message(msg)
 
     def SetActive(self, active: bool):
         """
-        设置物体激活状态
+        Set the activeness of this obeject.
 
         Args:
-            active: 激活/非激活
+            active: Bool, True for active, False for inactive.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetActive')
         msg.write_bool(active)
 
         self.env.instance_channel.send_message(msg)
 
     def SetParent(self, parent_id: int, parent_name: str = ''):
         """
-        设置父物体
+        Set the parent of this object.
 
         Args:
-            parent_id: 父物体ID
-            parent_name: 父物体内节点名
+            parent_id: Int, the id of parent object.
+            parent_name: Str, the name of parent object.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetParent')
         msg.write_int32(parent_id)
         msg.write_string(parent_name)
 
         self.env.instance_channel.send_message(msg)
 
     def SetLayer(self, layer: int):
         """
-        设置物体层
+        Set the layer in Unity of this object.
 
         Args:
-            layer: 层编号
+            layer: Int, the number of layer.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetLayer')
         msg.write_int32(layer)
 
         self.env.instance_channel.send_message(msg)
 
     def Copy(self, new_id: int):
         """
-        复制物体
+        Duplicate an object.
 
         Args:
-            new_id: 新物体的ID
+            new_id: Int, the id of new object.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('Copy')
         msg.write_int32(new_id)
 
         self.env.instance_channel.send_message(msg)
 
         self.env.attrs[new_id] = type(self)(self.env, new_id, self.data)
         return self.env.attrs[new_id]
 
     def Destroy(self):
         """
-        删除物体
+        Destroy this object in Unity.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('Destroy')
 
         self.env.instance_channel.send_message(msg)
         self.env.attrs.pop(self.id)
 
     def SetRFMoveColliderActive(self, active: bool):
         """
-        设置物体在RFMove中的碰撞开关
+        Set the collider active or inactive in RFMove.
 
         Args:
-            active:
+            active: Bool, True for active and False for inactive.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetRFMoveColliderActive')
         msg.write_bool(active)
 
         self.env.instance_channel.send_message(msg)
 
     def GetLoaclPointFromWorld(self, point: list):
         """
-        转换局部坐标到世界坐标
+        Transform a point from local coordinate to world coordinate.
 
         Args:
-            point:局部坐标
+            point: A list of length 3, representing the position of a point.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('GetLoaclPointFromWorld')
         msg.write_float32(point[0])
         msg.write_float32(point[1])
         msg.write_float32(point[2])
 
         self.env.instance_channel.send_message(msg)
 
     def GetWorldPointFromLocal(self, point: list):
         """
-        转换世界坐标到局部坐标
+        Transform a point from world coordinate to local coordinate.
 
         Args:
-            point:世界坐标
+            point: A list of length 3, representing the position of a point.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('GetWorldPointFromLocal')
         msg.write_float32(point[0])
         msg.write_float32(point[1])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/camera_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/camera_attr.py`

 * *Files 21% similar despite different names*

```diff
@@ -139,44 +139,47 @@
         else:
             msg.write_float32(60)
     return msg
 
 
 class CameraAttr(attr.BaseAttr):
     """
-    相机类，可获取各种相机截图
+    Camera attribute class, which can capture many kinds of screenshot
+    of the scene in RFUniverse.
     """
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-            self.data['width'] 图像宽度
+            Dict: A dict containing useful information of this class.
+        
+            self.data['width']: The width of image.
 
-            self.data['height'] 图像高度
+            self.data['height']: The height of image.
 
-            self.data['fov'] 相机FOV
+            self.data['fov']: The field of view of camera.
 
-            self.data['rgb'] RGB图像bytes
+            self.data['rgb']: The bytes of rgb image.
 
-            self.data['normal'] 法线图像bytes
+            self.data['normal']: The bytes of normal image.
 
-            self.data['id_map'] ID图像bytes
+            self.data['id_map']: The bytes of instance segmentation mask image.
 
-            self.data['depth'] 深度图像bytes
+            self.data['depth']: The bytes of depth image.
 
-            self.data['depth_exr'] EXR深度图像bytes
+            self.data['depth_exr']: The bytes of depth image in exr format.
 
-            self.data['amodal_mask'] amodal_mask图bytes
+            self.data['amodal_mask']: The bytes of amodal mask image.
 
-            self.data['heat_map'] heat_map图bytes
+            self.data['heat_map']: The bytes of heat map image.
 
-            self.data['2d_bounding_box'] 相机屏幕坐标系下2d_bounding_box数据
+            self.data['2d_bounding_box']: The 2d bouding box of objects in camera (image) coordinate.
 
-            self.data['3d_bounding_box'] 世界空间3d_bounding_box数据
+            self.data['3d_bounding_box']: The 3d bounding box of objects in world coordinate.
         """
         super().parse_message(msg)
         self.data['width'] = msg.read_int32()
         self.data['height'] = msg.read_int32()
         self.data['fov'] = msg.read_float32()
         if msg.read_bool() is True:
             self.data['rgb'] = base64.b64decode(msg.read_string())
@@ -209,35 +212,32 @@
                 self.data['3d_bounding_box'][item_id]['position'] = [msg.read_float32() for _ in range(3)]
                 self.data['3d_bounding_box'][item_id]['rotation'] = [msg.read_float32() for _ in range(3)]
                 self.data['3d_bounding_box'][item_id]['size'] = [msg.read_float32() for _ in range(3)]
         return self.data
 
     def AlignView(self):
         """
-        使相机对准当前视口视角
+        Make the camera in RFUniverse align the current view in GUI.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('AlignView')
 
         self.env.instance_channel.send_message(msg)
 
     def GetRGB(self, width: int = 512, height: int = 512, fov: float = 60., intrinsic_matrix=None):
         """
-        获取相机的RGB图像
+        Get the camera RGB image.
 
         Args:
-            width: 图像分辨率宽度
-            height: 图像分辨率高度
-            fov: 相机FOV
-            intrinsic_matrix: List[9]相机内参，当传入时，width、height、fov参数无效
-
-        Returns:
-            调用此接口并step后，从self.data['rgb']获取结果
+            width: Int, the width of image.
+            height: Int, the height of image.
+            fov: Float, the field of view for camera.
+            intrinsic_matrix: A list of length 9, representing the camera intrinsic matrix. When this parameter is passed, `width`, `height` and `fov` will be ignroed.
         """
         if intrinsic_matrix is None:
             intrinsic_matrix = []
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
@@ -251,24 +251,21 @@
             msg.write_int32(height)
             msg.write_float32(fov)
 
         self.env.instance_channel.send_message(msg)
 
     def GetNormal(self, width: int = 512, height: int = 512, fov: float = 60., intrinsic_matrix=None):
         """
-        获取相机的世界空间法线图像
+        Get the normal image in world coordinate.
 
         Args:
-            width: 图像分辨率宽度
-            height: 图像分辨率高度
-            fov: 相机FOV
-            intrinsic_matrix: List[9]相机内参，当传入时，width、height、fov参数无效
-
-        Returns:
-            调用此接口并step后，从self.data['normal']获取结果
+            width: Int, the width of image.
+            height: Int, the height of image.
+            fov: Float, the field of view for camera.
+            intrinsic_matrix: A list of length 9, representing the camera intrinsic matrix. When this parameter is passed, `width`, `height` and `fov` will be ignroed.
         """
         if intrinsic_matrix is None:
             intrinsic_matrix = []
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
@@ -282,24 +279,21 @@
             msg.write_int32(height)
             msg.write_float32(fov)
 
         self.env.instance_channel.send_message(msg)
 
     def GetID(self, width: int = 512, height: int = 512, fov: float = 60., intrinsic_matrix=None):
         """
-        获取相机的ID图像，每个像素的颜色值由物体ID计算而来，见rfuniverse_utility.GetColorFromID
+        Get the instance segmentation mask image. The color for each pixel is computed from object ID, see `pyrfuniverse.utils.rfuniverse_utility.GetColorFromID` for more details.
 
         Args:
-            width: 图像分辨率宽度
-            height: 图像分辨率高度
-            fov: 相机FOV
-            intrinsic_matrix: List[9]相机内参，当传入时，width、height、fov参数无效
-
-        Returns:
-            调用此接口并step后，从self.data['id_map']获取结果
+            width: Int, the width of image.
+            height: Int, the height of image.
+            fov: Float, the field of view for camera.
+            intrinsic_matrix: A list of length 9, representing the camera intrinsic matrix. When this parameter is passed, `width`, `height` and `fov` will be ignroed.
         """
         if intrinsic_matrix is None:
             intrinsic_matrix = []
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
@@ -313,26 +307,23 @@
             msg.write_int32(height)
             msg.write_float32(fov)
 
         self.env.instance_channel.send_message(msg)
 
     def GetDepth(self, zero_dis: float, one_dis: float, width: int = 512, height: int = 512, fov: float = 60., intrinsic_matrix=None):
         """
-        获取相机的深度图像，由于8位深度图精度低，因此需要限制范围以提高精度
+        Get the depth image from camera. Since eacg pixel of depth image returned from this function is 8-bit, user should limit the depth range (`zero_dis` and `one_dis`) for more accurate results.
 
         Args:
-            zero_dis: 黑色像素表示深度
-            one_dis: 白像素表示深度
-            width: 图像分辨率宽度
-            height: 图像分辨率高度
-            fov: 相机FOV
-            intrinsic_matrix: List[9]相机内参，当传入时，width、height、fov参数无效
-
-        Returns:
-            调用此接口并step后，从self.data['depth']获取结果
+            zero_dis: The minimum distance in calculation.
+            one_dis: The maximum distance in calculation.
+            width: Int, the width of image.
+            height: Int, the height of image.
+            fov: Float, the field of view for camera.
+            intrinsic_matrix: A list of length 9, representing the camera intrinsic matrix. When this parameter is passed, `width`, `height` and `fov` will be ignroed.
         """
         if intrinsic_matrix is None:
             intrinsic_matrix = []
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
@@ -348,24 +339,21 @@
             msg.write_int32(height)
             msg.write_float32(fov)
 
         self.env.instance_channel.send_message(msg)
 
     def GetDepthEXR(self, width: int = 512, height: int = 512, fov: float = 60., intrinsic_matrix=None):
         """
-        获取相机的世界空间深度图像，EXR格式图像支持存储32位信息，因此无需限制范围
+        Get the depth image from camera. This function returns EXR format image bytes and each pixel is 32-bit.
 
         Args:
-            width: 图像分辨率宽度
-            height: 图像分辨率高度
-            fov: 相机FOV
-            intrinsic_matrix: List[9]相机内参，当传入时，width、height、fov参数无效
-
-        Returns:
-            调用此接口并step后，从self.data['depth_exr']获取结果
+            width: Int, the width of image.
+            height: Int, the height of image.
+            fov: Float, the field of view for camera.
+            intrinsic_matrix: A list of length 9, representing the camera intrinsic matrix. When this parameter is passed, `width`, `height` and `fov` will be ignroed.
         """
         if intrinsic_matrix is None:
             intrinsic_matrix = []
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
@@ -379,25 +367,22 @@
             msg.write_int32(height)
             msg.write_float32(fov)
 
         self.env.instance_channel.send_message(msg)
 
     def GetAmodalMask(self, target_id: int, width: int = 512, height: int = 512, fov: float = 60., intrinsic_matrix=None):
         """
-        获取目标物体的Amodal Mask图像
+        Get the amodal mask image for target object.
 
         Args:
-            target_id: 目标物体ID
-            width: 图像分辨率宽度
-            height: 图像分辨率高度
-            fov: 相机FOV
-            intrinsic_matrix: List[9]相机内参，当传入时，width、height、fov参数无效
-
-        Returns:
-            调用此接口并step后，从self.data['amodal_mask']获取结果
+            target_id: The target object ID.
+            width: Int, the width of image.
+            height: Int, the height of image.
+            fov: Float, the field of view for camera.
+            intrinsic_matrix: A list of length 9, representing the camera intrinsic matrix. When this parameter is passed, `width`, `height` and `fov` will be ignroed.
         """
         if intrinsic_matrix is None:
             intrinsic_matrix = []
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
@@ -431,25 +416,22 @@
         msg.write_int32(self.id)
         msg.write_string('EndHeatMapRecord')
 
         self.env.instance_channel.send_message(msg)
 
     def GetHeatMap(self, width: int = 512, height: int = 512, radius: int = 50, fov: float = 60., intrinsic_matrix=None):
         """
-        获取目标物体的HeatMap图像
+        Get the heat map image.
 
         Args:
-            width: 图像分辨率宽度
-            height: 图像分辨率高度
-            radius: 热力图半径
-            fov: 相机FOV
-            intrinsic_matrix: List[9]相机内参，当传入时，width、height、fov参数无效
-
-        Returns:
-            调用此接口并step后，从self.data['heat_map']获取结果
+            width: Int, the width of image.
+            height: Int, the height of image.
+            radius: The radius of heat map.
+            fov: Float, the field of view for camera.
+            intrinsic_matrix: A list of length 9, representing the camera intrinsic matrix. When this parameter is passed, `width`, `height` and `fov` will be ignroed.
         """
         if intrinsic_matrix is None:
             intrinsic_matrix = []
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
@@ -464,24 +446,22 @@
             msg.write_int32(height)
             msg.write_float32(fov)
 
         self.env.instance_channel.send_message(msg)
 
     def Get2DBBox(self, width: int = 512, height: int = 512, fov: float = 60., intrinsic_matrix=None):
         """
-        获取相机中物体的2DBBox
+        Get the 2d bounding box of objects in current camera view.
 
         Args:
-            width: 图像分辨率宽度
-            height: 图像分辨率高度
-            fov: 相机FOV
-            intrinsic_matrix: List[9]相机内参，当传入时，width、height、fov参数无效
-
-        Returns:
-            调用此接口并step后，从self.data['2d_bounding_box']获取结果
+            width: Int, the width of image.
+            height: Int, the height of image.
+            radius: The radius of heat map.
+            fov: Float, the field of view for camera.
+            intrinsic_matrix: A list of length 9, representing the camera intrinsic matrix. When this parameter is passed, `width`, `height` and `fov` will be ignroed.
         """
         if intrinsic_matrix is None:
             intrinsic_matrix = []
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
@@ -495,18 +475,15 @@
             msg.write_int32(height)
             msg.write_float32(fov)
 
         self.env.instance_channel.send_message(msg)
 
     def Get3DBBox(self):
         """
-        获取物体的3DBBox
-
-        Returns:
-            调用此接口并step后，从self.data['3d_bounding_box']获取结果
+        Get the 3d bounding box of objects in world coordinate.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('Get3DBBox')
 
         self.env.instance_channel.send_message(msg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/collider_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/collider_attr.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,29 +15,29 @@
     msg.write_int32(kwargs['id'])
     msg.write_string('GenerateVHACDColider')
     return msg
 
 
 class ColliderAttr(attr.GameObjectAttr):
     """
-    具有碰撞体的物体类
+    Collider class for objects who have collider in Unity.
     """
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-
+            Dict: A dict containing useful information of this class.
         """
         super().parse_message(msg)
         return self.data
 
     def GenerateVHACDColider(self):
         """
-        使用VHACD算法生成物体碰撞体
+        Generate convex colliders using VHACD algorithm.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('GenerateVHACDColider')
 
         self.env.instance_channel.send_message(msg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/controller_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/controller_attr.py`

 * *Files 18% similar despite different names*

```diff
@@ -414,54 +414,56 @@
         msg.write_float32(kwargs['rotation'][1])
         msg.write_float32(kwargs['rotation'][2])
     return msg
 
 
 class ControllerAttr(attr.ColliderAttr):
     """
-    机械臂控制器类
+    Robot controller class, which will control robot arms, hands and embodied robots.
     """
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-            self.data['number_of_joints'] 机械臂关节数量
+            Dict: A dict containing useful information of this class.
 
-            self.data['positions'] 机械臂节点位置
+            self.data['number_of_joints']: The number of joints in an articulation.
 
-            self.data['rotations'] 机械臂节点旋转角度
+            self.data['positions']: The position of each part in an articulation.
 
-            self.data['quaternion'] 机械臂节点旋转四元数
+            self.data['rotations']: The rotation of each part in an articulation.
 
-            self.data['local_positions'] 机械臂节点局部位置
+            self.data['quaternion']: The quaternion of each part in an articulation.
 
-            self.data['local_rotations'] 机械臂节点局部旋转角度
+            self.data['local_positions']: The local position of each part in an articulation.
 
-            self.data['local_quaternion'] 机械臂节点局部旋转四元数
+            self.data['local_rotations']: The local rotation of each part in an articulation.
 
-            self.data['velocities'] 机械臂节点速度
+            self.data['local_quaternion']: The local quaternion of each part in an articulation.
 
-            self.data['number_of_moveable_joints'] 机械臂活动关节数量
+            self.data['velocities']: The velocity of each part in an articulation.
 
-            self.data['joint_positions'] 机械臂关节在自由度空间下位置
+            self.data['number_of_moveable_joints']: The number of moveable joints in an articulation.
 
-            self.data['joint_velocities'] 机械臂关节在自由度空间下速度
+            self.data['joint_positions']: The joint position of each moveable joint in an articulation.
 
-            self.data['all_stable'] 机械臂所有关节移动完成
+            self.data['joint_velocities']: The joint velocity of each moveable joint in an articulation.
 
-            self.data['move_done'] 机械臂IK移动完成状态
+            self.data['all_stable']: Whether all joints have finished moving.
 
-            self.data['rotate_done'] 机械臂IK旋转完成状态
+            self.data['move_done']: Whether robot arm IK has finished moving.
 
-            self.data['gravity_forces'] InverseDynamics抵消重力所需的力
+            self.data['rotate_done']: Whether robot arm IK has finished rotating.
 
-            self.data['coriolis_centrifugal_forces'] InverseDynamics抵消离心力所需的力
+            self.data['gravity_forces']: Inverse Dynamics force needed to counteract gravity.
 
-            self.data['drive_forces'] InverseDynamics驱动力
+            self.data['coriolis_centrifugal_forces']: Inverse Dynamics force needed to counteract coriolis centrifugal forces.
+
+            self.data['drive_forces']: Inverse Dynamics drive forces.
         """
         super().parse_message(msg)
         self.data['number_of_joints'] = msg.read_int32()
         # Position
         self.data['positions'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
         # RotationEuler
         self.data['rotations'] = np.array(msg.read_float32_list()).reshape([-1, 3]).tolist()
@@ -489,19 +491,19 @@
             self.data['gravity_forces'] = msg.read_float32_list()
             self.data['coriolis_centrifugal_forces'] = msg.read_float32_list()
             self.data['drive_forces'] = msg.read_float32_list()
         return self.data
 
     def SetJointPosition(self, joint_positions: list, speed_scales = None):
         """
-        设置机械臂所有关节目标位置
+        Set the target joint position for each moveable joint and move with PD control.
 
         Args:
-            joint_positions: 目标位置
-            speed_scales: 速度倍数
+            joint_positions: A list of float, representing the target joint positions.
+            speed_scales: A list of float, representing the speed scale.
         """
         num_joints = len(joint_positions)
         if speed_scales is None:
             speed_scales = [1.0 for i in range(num_joints)]
         assert num_joints == len(speed_scales), \
             'The length of joint_positions and speed_scales are not equal.'
 
@@ -512,70 +514,70 @@
         msg.write_float32_list(joint_positions)
         msg.write_float32_list(speed_scales)
 
         self.env.instance_channel.send_message(msg)
 
     def SetJointPositionDirectly(self, joint_positions: list):
         """
-        立即设置机械臂所有关节位置
+        Set the target joint position for each moveable joint and move directly.
 
         Args:
-            joint_positions: 目标位置
+            joint_positions: A list of float, representing the target joint positions.
         """
         num_joints = len(joint_positions)
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetJointPositionDirectly')
         msg.write_float32_list(joint_positions)
 
         self.env.instance_channel.send_message(msg)
 
     def SetIndexJointPosition(self, index: int, joint_position: float):
         """
-        设置机械臂指定关节目标位置
+        Set the target joint position for a given joint and move with PD control.
 
         Args:
-            index: 关节序号
-            joint_position: 目标位置
+            index: Int, joint index.
+            joint_position: Float, the target joint position.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetIndexJointPosition')
         msg.write_int32(index)
         msg.write_float32(joint_position)
 
         self.env.instance_channel.send_message(msg)
 
     def SetIndexJointPositionDirectly(self, index: int, joint_position: float):
         """
-        立即设置机械臂指定关节位置
+        Set the target joint position for a given joint and move directly.
 
         Args:
-            index: 关节序号
-            joint_position: 目标位置
+            index: Int, joint index.
+            joint_position: Float, the target joint position.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetIndexJointPositionDirectly')
         msg.write_int32(index)
         msg.write_float32(joint_position)
 
         self.env.instance_channel.send_message(msg)
 
     def SetJointPositionContinue(self, interval: int, time_joint_positions: list):
         """
-        持续设置机械臂所有关节目标位置
+        Set the target joint position for each moveable joint and move with PD control continuously.
 
         Args:
-            interval: 设置时间间隔(毫秒)
-            time_joint_positions: 每个time的目标位置
+            interval: Float, the time interval.
+            time_joint_positions: A list of float list, representing the target joint positions at each time step.
 
         Returns:
 
         """
         num_times = len(time_joint_positions)
 
         msg = OutgoingMessage()
@@ -587,52 +589,52 @@
         for i in range(num_times):
             msg.write_float32_list(time_joint_positions[i])
 
         self.env.instance_channel.send_message(msg)
 
     def SetJointVelocity(self, joint_velocitys: list):
         """
-        设置机械臂所有关节目标速度
+        Set the target joint velocity for each moveable joint.
 
         Args:
-            joint_velocitys: 目标速度
+            joint_velocitys: A list of float, representing the target joint velocities.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetJointVelocity')
         msg.write_float32_list(joint_velocitys)
 
         self.env.instance_channel.send_message(msg)
 
     def SetIndexJointVelocity(self, index: int, joint_velocity: float):
         """
-        设置机械臂指定关节目标速度
+        Set the target joint velocity for a given joint.
 
         Args:
-            index: 关节序号
-            joint_velocity: 目标速度
+            index: Int, joint index.
+            joint_velocity: A list of float, representing the target joint velocities.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetIndexJointVelocity')
         msg.write_int32(index)
         msg.write_float32(joint_velocity)
 
         self.env.instance_channel.send_message(msg)
 
     def AddJointForce(self, joint_forces: list):
         """
-        为机械臂所有关节施加力
+        Add force to each moveable joint.
 
         Args:
-            joint_forces: 力
+            joint_forces: A list of forces, representing the added forces.
         """
-        num_joints = len(joint_positions)
+        num_joints = len(joint_forces)
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('AddJointForce')
         msg.write_int32(num_joints)
         for i in range(num_joints):
@@ -640,21 +642,21 @@
             msg.write_float32(joint_forces[i][1])
             msg.write_float32(joint_forces[i][2])
 
         self.env.instance_channel.send_message(msg)
 
     def AddJointForceAtPosition(self, joint_forces: list, force_positions: list):
         """
-        为机械臂所有关节指定位置施加力
+        Add force to each moveable joint at a given position.
 
         Args:
-            joint_forces: 力
-            force_positions: 施力点
+            joint_forces: A list of forces, representing the added forces.
+            force_positions: A list of positions, representing the positions for forces.
         """
-        num_joints = len(joint_positions)
+        num_joints = len(joint_forces)
         assert len(joint_forces) == len(force_positions), \
             'The length of joint_forces and force_positions are not equal.'
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('AddJointForceAtPosition')
@@ -667,20 +669,20 @@
             msg.write_float32(force_positions[i][1])
             msg.write_float32(force_positions[i][2])
 
         self.env.instance_channel.send_message(msg)
 
     def AddJointTorque(self, joint_torques: list):
         """
-        为机械臂所有关节施加力矩
+        Add torque to each moveable joint.
 
         Args:
-            joint_torques: 力矩
+            joint_torques: A list of torques, representing the added torques.
         """
-        num_joints = len(joint_torque)
+        num_joints = len(joint_torques)
 
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('AddJointTorque')
         msg.write_int32(num_joints)
         for i in range(num_joints):
@@ -689,166 +691,152 @@
             msg.write_float32(joint_torques[i][2])
 
         self.env.instance_channel.send_message(msg)
 
     # only work on unity 2022.1+
     def GetJointInverseDynamicsForce(self):
         """
-        获取机械臂所有关节逆动力学数据
-
-        Returns:
-            调用此接口并step后，从
-            self.data['gravity_forces']
-            self.data['coriolis_centrifugal_forces']
-            self.data['drive_forces']
-            获取结果
+        Get the joint inverse dynamic force of each moveable joint. Note that this function only works in Unity version >= 2022.1.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('GetJointInverseDynamicsForce')
 
         self.env.instance_channel.send_message(msg)
 
     def SetImmovable(self, immovable: bool):
         """
-        设置机械臂是否不可移动
+        Set whether the base of articulation is immovable.
 
         Args:
-            immovable: 是否不可移动
+            immovable: Bool, True for immovable, False for movable.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetImmovable')
         msg.write_bool(immovable)
 
         self.env.instance_channel.send_message(msg)
 
     def MoveForward(self, distance: float, speed: float):
         """
-        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动前进
-        最初用于Tobor机器人
+        Move robot forward. Only works if the robot controller has implemented functions inherited from `ICustomMove.cs`. See https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ICustomMove.cs and https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ToborMove.cs for more details.
 
         Args:
-            distance:距离
-            speed:速度
+            distance: Float, distance.
+            speed: Float, velocity.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('MoveForward')
         msg.write_float32(distance)
         msg.write_float32(speed)
 
         self.env.instance_channel.send_message(msg)
 
     def MoveBack(self, distance: float, speed: float):
         """
-        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动后退
-        最初用于Tobor机器人
+        Move robot backword. Only works if the robot controller has implemented functions inherited from `ICustomMove.cs`. See https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ICustomMove.cs and https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ToborMove.cs for more details.
 
         Args:
-            distance:距离
-            speed:速度
+            distance: Float, distance.
+            speed: Float, velocity.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('MoveBack')
         msg.write_float32(distance)
         msg.write_float32(speed)
 
         self.env.instance_channel.send_message(msg)
 
     def TurnLeft(self, angle: float, speed: float):
         """
-        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动左转
-        最初用于Tobor机器人
+        Turn robot left. Only works if the robot controller has implemented functions inherited from `ICustomMove.cs`. See https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ICustomMove.cs and https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ToborMove.cs for more details.
 
         Args:
-            angle:角度
-            speed:速度
+            angle: Float, rotation angle.
+            speed: Float, velocity.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('TurnLeft')
         msg.write_float32(angle)
         msg.write_float32(speed)
 
         self.env.instance_channel.send_message(msg)
 
     def TurnRight(self, angle: float, speed: float):
         """
-        如果机器人在Unity端添加了继承ICustomMove接口的脚本，可通过此接口驱动右转
-        最初用于Tobor机器人
+        Turn robot right. Only works if the robot controller has implemented functions inherited from `ICustomMove.cs`. See https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ICustomMove.cs and https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ToborMove.cs for more details.
 
         Args:
-            angle:角度
-            speed:速度
+            angle: Float, rotation angle.
+            speed: Float, velocity.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('TurnRight')
         msg.write_float32(angle)
         msg.write_float32(speed)
 
         self.env.instance_channel.send_message(msg)
 
     def GripperOpen(self):
         """
-        如果夹爪在Unity端添加了继承ICustomGripper接口的脚本，可通过此接口驱动张开
+        Open the gripper. Only works if the robot controller has implemented functions inherited from `ICustomGripper.cs`. See https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ICustomGripper.cs and https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/GeneralGripper.cs for more details.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('GripperOpen')
 
         self.env.instance_channel.send_message(msg)
 
     def GripperClose(self):
         """
-        如果夹爪在Unity端添加了继承ICustomGripper接口的脚本，可通过此接口驱动闭合
+        Close the gripper. Only works if the robot controller has implemented functions inherited from `ICustomGripper.cs`. See https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/ICustomGripper.cs and https://github.com/mvig-robotflow/rfuniverse/blob/main/Assets/RFUniverse/Scripts/Utils/GeneralGripper.cs for more details.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('GripperClose')
 
         self.env.instance_channel.send_message(msg)
 
     def EnabledNativeIK(self, enabled: bool):
         """
-        启用/禁用机械臂的原生IK
+        Enable or disable the native IK algorithm.
 
         Args:
-            enabled: 启用/禁用
+            enabled: Bool, True for enable and False for disable.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('EnabledNativeIK')
         msg.write_bool(enabled)
 
         self.env.instance_channel.send_message(msg)
 
     def IKTargetDoMove(self, position: list, duration: float, speed_based: bool = True, relative: bool = False):
         """
-        原生IK末端点移动
+        Native IK target movement.
 
         Args:
-            position: 绝对位置或相对位置
-            duration: 移动持续时间或移动速度
-            speed_based: 指定duration表示移动持续时间还是移动速度
-            relative: 指定position表示绝对位置还是相对位置
-
-        Returns:
-            当移动完成时，self.data['move_done']会被置为True
+            position: A list of length 3, representing the position.
+            duration: Float, if `speed_based` is True, it represents movement duration; otherwise, it represents movement speed.
+            speed_based: Bool.
+            relative: Bool, if True, `position` is relative; otherwise, `position` is absolute.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('IKTargetDoMove')
         msg.write_float32(position[0])
         msg.write_float32(position[1])
@@ -857,24 +845,21 @@
         msg.write_bool(speed_based)
         msg.write_bool(relative)
 
         self.env.instance_channel.send_message(msg)
 
     def IKTargetDoRotate(self, rotation: list, duration: float, speed_based: bool = True, relative: bool = False):
         """
-        原生IK末端点Vector3旋转
+        Native IK target rotation.
 
         Args:
-            rotation: 绝对旋转或相对旋转
-            duration: 旋转持续时间或旋转速度
-            speed_based: 指定duration表示旋转持续时间还是旋转速度
-            relative: 指定position表示绝对旋转还是相对旋转
-
-        Returns:
-            当旋转完成时，self.data['rotate_done']会被置为True
+            rotation: A list of length 3, representing the rotation.
+            duration: Float, if `speed_based` is True, it represents movement duration; otherwise, it represents movement speed.
+            speed_based: Bool.
+            relative: Bool, if True, `rotation` is relative; otherwise, `rotation` is absolute.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('IKTargetDoRotate')
         msg.write_float32(rotation[0])
         msg.write_float32(rotation[1])
@@ -883,24 +868,21 @@
         msg.write_bool(speed_based)
         msg.write_bool(relative)
 
         self.env.instance_channel.send_message(msg)
 
     def IKTargetDoRotateQuaternion(self, quaternion: list, duration: float, speed_based: bool = True, relative: bool = False):
         """
-        原生IK末端点四元数旋转
+        Native IK target rotation using quaternion.
 
         Args:
-            quaternion: 绝对旋转或相对旋转
-            duration: 旋转持续时间或旋转速度
-            speed_based: 指定duration表示旋转持续时间还是旋转速度
-            relative: 指定position表示绝对旋转还是相对旋转
-
-        Returns:
-            当旋转完成时，self.data['rotate_done']会被置为True
+            quaternion: A list of length 4, representing the quaternion.
+            duration: Float, if `speed_based` is True, it represents movement duration; otherwise, it represents movement speed.
+            speed_based: Bool.
+            relative: Bool, if True, `quaternion` is relative; otherwise, `quaternion` is absolute.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('IKTargetDoRotateQuaternion')
         msg.write_float32(quaternion[0])
         msg.write_float32(quaternion[1])
@@ -910,42 +892,42 @@
         msg.write_bool(speed_based)
         msg.write_bool(relative)
 
         self.env.instance_channel.send_message(msg)
 
     def IKTargetDoComplete(self):
         """
-        使原生IK末端点移动/旋转立即完成
+        Make native IK target movement / rotation complete directly.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('IKTargetDoComplete')
 
         self.env.instance_channel.send_message(msg)
 
     def IKTargetDoKill(self):
         """
-        使原生IK末端点移动/旋转停止
+        Make native IK target movement / rotation stop.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('IKTargetDoKill')
 
         self.env.instance_channel.send_message(msg)
 
     def SetIKTargetOffset(self, position: list = [0.,0.,0.], rotation: list = [0.,0.,0.], quaternion: list = None):
         """
-        设置原生IK末端点的偏移
+        Set the new IK target by setting offset to the original target of native IK.
 
         Args:
-            position: 偏移位置
-            rotation: 偏移旋转Vector3
-            quaternion: 偏移旋转四元数，此值覆盖rotation
+            position: A list of length 3, representing the position offset to original target.
+            rotation: A list of length 3, representing the rotation offset to original target.
+            quaternion: A list of length 4, representing the quaternion offset to original target. If this parameter is specified, `rotation` will be ignored.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetIKTargetOffset')
         msg.write_float32(position[0])
         msg.write_float32(position[1])
@@ -961,11 +943,11 @@
             msg.write_float32(rotation[1])
             msg.write_float32(rotation[2])
 
         self.env.instance_channel.send_message(msg)
 
     def WaitDo(self):
         """
-        等待原生IK末端点移动/旋转完成
+        Wait for the native IK target movement / rotation complete.
         """
         while not self.data['move_done'] or not self.data['rotate_done']:
             self.env.step()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/gameobject_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/gameobject_attr.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,85 +45,83 @@
         msg.write_float32(kwargs['color'][i])
 
     return msg
 
 
 class GameObjectAttr(attr.BaseAttr):
     """
-    基本视觉物体类
+    Basic game object attribute class.
     """
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-            self.data['3d_bounding_box'] 物体3D包围盒
+            Dict: A dict containing useful information of this class.
+
+            self.data['3d_bounding_box']: The 3d bounding box of objects.
         """
         super().parse_message(msg)
         if msg.read_bool():
             self.data['3d_bounding_box'] = {}
             self.data['3d_bounding_box']['position'] = [msg.read_float32() for _ in range(3)]
             self.data['3d_bounding_box']['rotation'] = [msg.read_float32() for _ in range(3)]
             self.data['3d_bounding_box']['size'] = [msg.read_float32() for _ in range(3)]
         return self.data
 
     def SetColor(self, color: list):
         """
-        设置物体颜色
+        Set object color.
 
         Args:
-            color: 颜色，长度为4，分别为RGBA[0-1]
+            color: A list of length 4, represenging r, g, b and a. Each float is in range (0, 1).
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetColor')
         for i in range(4):
             msg.write_float32(color[i])
 
         self.env.instance_channel.send_message(msg)
 
     def EnabledRender(self, enabled: bool):
         """
-        启用或禁用渲染
+        Enable or disable rendering system.
 
         Args:
-            enabled: 是否启用渲染
+            enabled: Bool, Ture for enable rendering and False for disable rendering.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('EnabledRender')
         msg.write_bool(enabled)
 
         self.env.instance_channel.send_message(msg)
 
     def SetTexture(self, path: str):
         """
-        设置物体纹理
+        Set the texture of object.
 
         Args:
-            path: 纹理贴图绝对路径
+            path: Str, the absolute path for texture file.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetTexture')
         msg.write_string(path)
 
         self.env.instance_channel.send_message(msg)
 
     def Get3DBBox(self):
         """
-        获取该物体3D Bounding Box
-
-        Returns:
-            调用此接口并step后，从
-            self.data['3d_bounding_box']
-            获取结果
+        Get the 3d bounding box of this object.
+        
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('Get3DBBox')
 
         self.env.instance_channel.send_message(msg)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/humanbody_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/humanbody_attr.py`

 * *Files 20% similar despite different names*

```diff
@@ -96,43 +96,42 @@
     msg.write_string('HumanIKTargetDoKill')
     msg.write_int32(kwargs['index'])
     return msg
 
 
 class HumanbodyAttr(attr.BaseAttr):
     """
-    人体IK类
+    Human body Inverse Kinematic class.
     """
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-            self.data['move_done'] 移动完成
+            Dict: A dict containing useful information of this class.
 
-            self.data['rotate_done'] 旋转完成
+            self.data['move_done']: Whether the movement has finished.
+
+            self.data['rotate_done']: Whether the rotation has finished.
         """
         super().parse_message(msg)
         self.data['move_done'] = msg.read_bool()
         self.data['rotate_done'] = msg.read_bool()
         return self.data
 
     def HumanIKTargetDoMove(self, index: int, position: list, duration: float, speed_based: bool = True, relative: bool = False):
         """
-        人体IK目标点移动
+        Human body Inverse Kinematics target movement.
 
         Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
-            position: 绝对位置或相对位置
-            duration: 移动持续时间或移动速度
-            speed_based: 指定duration表示移动持续时间还是移动速度
-            relative: 指定position表示绝对位置还是相对位置
-
-        Returns:
-            当移动完成时，self.data['move_done']会被置为True
+            index: Int, the target for movement. 0 for left hand, 1 for right hand,2 for left foot, 3 for right foot, 4 for head.
+            position: A list of length 3, representing the position.
+            duration: Float, if `speed_based` is True, it represents movement duration; otherwise, it represents movement speed.
+            speed_based: Bool.
+            relative: Bool, if True, `position` is relative; otherwise, `position` is absolute.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('HumanIKTargetDoMove')
         msg.write_int32(index)
         msg.write_float32(position[0])
@@ -142,25 +141,22 @@
         msg.write_bool(speed_based)
         msg.write_bool(relative)
 
         self.env.instance_channel.send_message(msg)
 
     def HumanIKTargetDoRotate(self, index: int, rotation: list, duration: float, speed_based: bool = True, relative: bool = False):
         """
-        人体IK目标点旋转
+        Human body Inverse Kinematics target rotation.
 
         Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
-            rotation: 绝对旋转或相对旋转
-            duration: 旋转持续时间或旋转速度
-            speed_based: 指定duration表示旋转持续时间还是旋转速度
-            relative: 指定position表示绝对旋转还是相对旋转
-
-        Returns:
-            当旋转完成时，self.data['rotate_done']会被置为True
+            index: Int, the target for movement. 0 for left hand, 1 for right hand,2 for left foot, 3 for right foot, 4 for head.
+            rotation: A list of length 3, representing the rotation.
+            duration: Float, if `speed_based` is True, it represents movement duration; otherwise, it represents movement speed.
+            speed_based: Bool.
+            relative: Bool, if True, `rotation` is relative; otherwise, `rotation` is absolute.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('HumanIKTargetDoRotate')
         msg.write_int32(index)
         msg.write_float32(rotation[0])
@@ -170,25 +166,22 @@
         msg.write_bool(speed_based)
         msg.write_bool(relative)
 
         self.env.instance_channel.send_message(msg)
 
     def HumanIKTargetDoRotateQuaternion(self, index: int, quaternion: list, duration: float, speed_based: bool = True, relative: bool = False):
         """
-        人体IK目标点四元数旋转
+        Human body Inverse Kinematics target rotation using quaternion.
 
         Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
-            quaternion: 绝对旋转或相对旋转
-            duration: 旋转持续时间或旋转速度
-            speed_based: 指定duration表示旋转持续时间还是旋转速度
-            relative: 指定position表示绝对旋转还是相对旋转
-
-        Returns:
-            当旋转完成时，self.data['rotate_done']会被置为True
+            index: Int, the target for movement. 0 for left hand, 1 for right hand,2 for left foot, 3 for right foot, 4 for head.
+            quaternion: A list of length 4, representing the quaternion.
+            duration: Float, if `speed_based` is True, it represents movement duration; otherwise, it represents movement speed.
+            speed_based: Bool.
+            relative: Bool, if True, `quaternion` is relative; otherwise, `quaternion` is absolute.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('HumanIKTargetDoRotateQuaternion')
         msg.write_int32(index)
         msg.write_float32(quaternion[0])
@@ -201,42 +194,42 @@
 
         self.env.instance_channel.send_message(msg)
 
         self.env.instance_channel.send_message(msg)
 
     def HumanIKTargetDoComplete(self, index: int):
         """
-        使人体IK目标点移动/旋转立即完成
+        Make the human body IK target movement / rotation complete directly.
 
         Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
+            index: Int, the target for movement. 0 for left hand, 1 for right hand,2 for left foot, 3 for right foot, 4 for head.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('HumanIKTargetDoComplete')
         msg.write_int32(index)
 
         self.env.instance_channel.send_message(msg)
 
     def HumanIKTargetDoKill(self, index: int):
         """
-        使人体IK目标点移动/旋转停止
+        Make the human body IK target movement / rotation stop.
 
         Args:
-            index: 移动的目标：0-左手，1-右手，2-左脚，3-右脚，4-头部
+            index: Int, the target for movement. 0 for left hand, 1 for right hand,2 for left foot, 3 for right foot, 4 for head.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('HumanIKTargetDoKill')
         msg.write_int32(index)
 
         self.env.instance_channel.send_message(msg)
 
     def WaitDo(self):
         """
-        等待人体IK移动/旋转完成
+        Wait for the human body IK target movement / rotation complete.
         """
         while not self.data['move_done'] or not self.data['rotate_done']:
             self.env.step()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/light_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/light_attr.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,128 +5,128 @@
     IncomingMessage,
     OutgoingMessage,
 )
 
 
 class LightType(Enum):
     """
-    光源类型,与Unity中的LightType一致
+    The type of light, keeping same name with LightType (https://docs.unity3d.com/ScriptReference/LightType.html) in Unity.
     """
     Spot = 0
     Directional = 1
     Point = 2
     Area = 3  # 不可用
     Disc = 4  # 不可用
 
 
 class LightShadow(Enum):
     """
-    阴影类型,与Unity中的LightShadows一致
+    The type of shadow, keeping same name with LightShadows (https://docs.unity3d.com/ScriptReference/LightShadows.html) in Unity.
     """
     NoneShadow = 0
     Hard = 1
     Soft = 2
 
 
 class LightAttr(attr.BaseAttr):
     """
-    灯光类
+    Light attribute class.
     """
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-
+            Dict: A dict containing useful information of this class.
         """
         super().parse_message(msg)
         return self.data
 
     def SetColor(self, color: list):
         """
-        设置灯光颜色
+        Set the color of light.
 
         Args:
-            color: 颜色,长度为3,分别为RGB三个通道的值,范围为0-1
+            color: A list of length 3, representing the R, G and B channel, in range [0, 1].
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetColor')
         for i in range(3):
             msg.write_float32(color[i])
 
         self.env.instance_channel.send_message(msg)
 
     def SetType(self, light_type: LightType):
         """
-        设置灯光类型
+        Set the type of light.
 
         Args:
-            light_type: 灯光类型,参考LightType
+            light_type: LightType, the type of light.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetType')
         msg.write_int32(light_type.value)
 
         self.env.instance_channel.send_message(msg)
 
     def SetShadow(self, light_shadow: LightShadow):
         """
-        设置灯光阴影类型
+        Set the type of shadow.
 
         Args:
-            light_shadow: 灯光阴影类型,参考LightShadow
+            light_shadow: LightShadow, the type of the shadow.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetShadow')
         msg.write_float32(light_shadow.value)
 
         self.env.instance_channel.send_message(msg)
 
     def SetIntensity(self, light_intensity: float):
         """
-        设置灯光强度
+        Set the intensity of light.
 
         Args:
-            light_intensity: 灯光强度
+            light_intensity: Float, the intensity of light.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetIntensity')
         msg.write_float32(light_intensity)
 
         self.env.instance_channel.send_message(msg)
 
     def SetRange(self, light_range: float):
         """
-        设置灯光范围(仅灯光类型为Spot和Point时有效)
+        Set the range of light. (Only available when the LightType is `LightType.Spot` or `LightType.Point`)
 
         Args:
-            light_range: 灯光范围
+            light_range: Float, the range of light.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetRange')
         msg.write_float32(light_range)
 
         self.env.instance_channel.send_message(msg)
 
     def SetSpotAngle(self, spot_angle: float):
         """
-        设置灯光角度(仅灯光类型为Spot时有效)
+        Set the angle of light. (Only available when the LightType is `LightType.Spot`)
 
         Args:
-            spot_angle: 灯光角度
+            spot_angle: Float, the angle of light.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetSpotAngle')
         msg.write_float32(spot_angle)
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/pointcloud_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/pointcloud_attr.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,35 +5,36 @@
     IncomingMessage,
     OutgoingMessage,
 )
 
 
 class PointCloudAttr(attr.BaseAttr):
     """
-    点云渲染类
+    Point cloud rendering class.
     """
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-
+            Dict: A dict containing useful information of this class.
         """
         super().parse_message(msg)
         return self.data
 
     def ShowPointCloud(self, positions: list = [], colors: list = [], ply_path: str = None, radius: float = 0.01):
         """
-        显示点云
+        Display point cloud in Unity.
 
         Args:
-            positions: 点位置列表
-            colors: 点颜色列表
-            ply_path: .ply文件列表，如果不为空，则positions和colors参数无效
-            radius: 点半径
+            positions: A list of positions of points in a point cloud.
+            colors: A list of colors of points (range [0, 1]) in a point cloud.
+            ply_path: Str, the absolute path of `.ply` file. If this parameter is specified, `positions`
+                and `colors` will be ignored.
+            radius: Float, the radius of the point cloud.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('ShowPointCloud')
         msg.write_bool(ply_path is not None)
         if ply_path is not None:
@@ -43,18 +44,18 @@
             msg.write_float32_list(np.array(colors).reshape(-1).tolist())
         msg.write_float32(radius)
 
         self.env.instance_channel.send_message(msg)
 
     def SetRadius(self, radius: float):
         """
-        设置点半径
+        Set the radius for points in a point cloud.
 
         Args:
-            radius: 半径
+            radius: Float, the radius.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetRadius')
         msg.write_float32(radius)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/attributes/rigidbody_attr.py` & `pyrfuniverse-0.8.4/pyrfuniverse/attributes/rigidbody_attr.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,68 +46,70 @@
     msg.write_float32(kwargs['velocity'][1])
     msg.write_float32(kwargs['velocity'][2])
 
     return msg
 
 class RigidbodyAttr(attr.ColliderAttr):
     """
-    刚体类
+    Rigid body class.
     """
     def parse_message(self, msg: IncomingMessage) -> dict:
         """
-        解析消息
+        Parse messages. This function is called by internal function.
 
         Returns:
-            self.data['velocity'] 刚体速度 Vecter3
+            Dict: A dict containing useful information of this class.
 
-            self.data['angular_vel'] 刚体角速度 Vecter3
+            self.data['velocity']: The velocity of the object.
+
+            self.data['angular_vel']: The angular velcity of the object.
         """
         super().parse_message(msg)
         self.data['velocity'] = [msg.read_float32() for _ in range(3)]
         self.data['angular_vel'] = [msg.read_float32() for _ in range(3)]
         return self.data
 
     def SetMass(self, mass: float):
         """
-        设置刚体质量
+        Set the mass of this rigid body object
 
         Args:
-            mass: 刚体质量
+            mass: Float, representing the mass of this rigid body.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetMass')
         msg.write_float32(mass)
 
         self.env.instance_channel.send_message(msg)
 
     def AddForce(self, force: list):
         """
-        为刚体施加力
+        Add force to this rigid body object.
 
         Args:
-            force: 力 Vecter3
+            force: A list of length 3, representing the force added to this rigid body.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('AddForce')
         msg.write_float32(force[0])
         msg.write_float32(force[1])
         msg.write_float32(force[2])
 
         self.env.instance_channel.send_message(msg)
 
     def SetVelocity(self, velocity: list):
         """
-        设置刚体速度
+        Set the velocity of this rigid body object.
 
         Args:
-            velocity: 速度 Vecter3
+            velocity: A list of length 3, representing the velocity of this rigid body.
         """
         msg = OutgoingMessage()
 
         msg.write_int32(self.id)
         msg.write_string('SetVelocity')
         msg.write_float32(velocity[0])
         msg.write_float32(velocity[1])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/base_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/base_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import Callable, Optional
-from pyrfuniverse.communicator_objects.unity_output_pb2 import UnityOutputProto
-from pyrfuniverse.communicator_objects.unity_input_pb2 import UnityInputProto
-
-
-# Function to call while waiting for a connection timeout.
-# This should raise an exception if it needs to break from waiting for the timeout.
-PollCallback = Callable[[], None]
-
-
-class Communicator:
-    def __init__(self, worker_id=0, base_port=5005):
-        """
-        Python side of the communication. Must be used in pair with the right Unity Communicator equivalent.
-
-        :int worker_id: Offset from base_port. Used for training multiple environments simultaneously.
-        :int base_port: Baseline port number to connect to Unity environment over. worker_id increments over this.
-        """
-
-    def initialize(
-        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
-    ) -> UnityOutputProto:
-        """
-        Used to exchange initialization parameters between Python and the Environment
-        :param inputs: The initialization input that will be sent to the environment.
-        :param poll_callback: Optional callback to be used while polling the connection.
-        :return: UnityOutput: The initialization output sent by Unity
-        """
-
-    def exchange(
-        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
-    ) -> Optional[UnityOutputProto]:
-        """
-        Used to send an input and receive an output from the Environment
-        :param inputs: The UnityInput that needs to be sent the Environment
-        :param poll_callback: Optional callback to be used while polling the connection.
-        :return: The UnityOutputs generated by the Environment
-        """
-
-    def close(self):
-        """
-        Sends a shutdown signal to the unity environment, and closes the connection.
-        """
+from typing import Callable, Optional
+from pyrfuniverse.communicator_objects.unity_output_pb2 import UnityOutputProto
+from pyrfuniverse.communicator_objects.unity_input_pb2 import UnityInputProto
+
+
+# Function to call while waiting for a connection timeout.
+# This should raise an exception if it needs to break from waiting for the timeout.
+PollCallback = Callable[[], None]
+
+
+class Communicator:
+    def __init__(self, worker_id=0, base_port=5005):
+        """
+        Python side of the communication. Must be used in pair with the right Unity Communicator equivalent.
+
+        :int worker_id: Offset from base_port. Used for training multiple environments simultaneously.
+        :int base_port: Baseline port number to connect to Unity environment over. worker_id increments over this.
+        """
+
+    def initialize(
+        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
+    ) -> UnityOutputProto:
+        """
+        Used to exchange initialization parameters between Python and the Environment
+        :param inputs: The initialization input that will be sent to the environment.
+        :param poll_callback: Optional callback to be used while polling the connection.
+        :return: UnityOutput: The initialization output sent by Unity
+        """
+
+    def exchange(
+        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
+    ) -> Optional[UnityOutputProto]:
+        """
+        Used to send an input and receive an output from the Environment
+        :param inputs: The UnityInput that needs to be sent the Environment
+        :param poll_callback: Optional callback to be used while polling the connection.
+        :return: The UnityOutputs generated by the Environment
+        """
+
+    def close(self):
+        """
+        Sends a shutdown signal to the unity environment, and closes the connection.
+        """
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/__init__.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_action_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/agent_action_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/agent_info_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/agent_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/brain_parameters_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/brain_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/capabilities_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/capabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/command_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/command_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/engine_configuration_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/engine_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/header_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/header_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/observation_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/observation_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/space_type_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/space_type_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/training_analytics_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/training_analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_input_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_input_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_message_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_message_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_output_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_output_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_to_external_pb2.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_to_external_pb2.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py` & `pyrfuniverse-0.8.4/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/env_utils.py` & `pyrfuniverse-0.8.4/pyrfuniverse/env_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-import glob
-import os
-import subprocess
-from sys import platform
-from typing import Optional, List
-from pyrfuniverse.logging_util import get_logger, DEBUG
-from pyrfuniverse.exception import UnityEnvironmentException
-
-
-logger = get_logger(__name__)
-
-
-def get_platform():
-    """
-    returns the platform of the operating system : linux, darwin or win32
-    """
-    return platform
-
-
-def validate_environment_path(env_path: str) -> Optional[str]:
-    """
-    Strip out executable extensions of the env_path
-    :param env_path: The path to the executable
-    """
-    env_path = (
-        env_path.strip()
-        .replace(".app", "")
-        .replace(".exe", "")
-        .replace(".x86_64", "")
-        .replace(".x86", "")
-    )
-    true_filename = os.path.basename(os.path.normpath(env_path))
-    logger.debug(f"The true file name is {true_filename}")
-
-    if not (glob.glob(env_path) or glob.glob(env_path + ".*")):
-        return None
-
-    cwd = os.getcwd()
-    launch_string = None
-    true_filename = os.path.basename(os.path.normpath(env_path))
-    if get_platform() == "linux" or get_platform() == "linux2":
-        candidates = glob.glob(os.path.join(cwd, env_path) + ".x86_64")
-        if len(candidates) == 0:
-            candidates = glob.glob(os.path.join(cwd, env_path) + ".x86")
-        if len(candidates) == 0:
-            candidates = glob.glob(env_path + ".x86_64")
-        if len(candidates) == 0:
-            candidates = glob.glob(env_path + ".x86")
-        if len(candidates) == 0:
-            if os.path.isfile(env_path):
-                candidates = [env_path]
-        if len(candidates) > 0:
-            launch_string = candidates[0]
-
-    elif get_platform() == "darwin":
-        candidates = glob.glob(
-            os.path.join(cwd, env_path + ".app", "Contents", "MacOS", true_filename)
-        )
-        if len(candidates) == 0:
-            candidates = glob.glob(
-                os.path.join(env_path + ".app", "Contents", "MacOS", true_filename)
-            )
-        if len(candidates) == 0:
-            candidates = glob.glob(
-                os.path.join(cwd, env_path + ".app", "Contents", "MacOS", "*")
-            )
-        if len(candidates) == 0:
-            candidates = glob.glob(
-                os.path.join(env_path + ".app", "Contents", "MacOS", "*")
-            )
-        if len(candidates) > 0:
-            launch_string = candidates[0]
-    elif get_platform() == "win32":
-        candidates = glob.glob(os.path.join(cwd, env_path + ".exe"))
-        if len(candidates) == 0:
-            candidates = glob.glob(env_path + ".exe")
-        if len(candidates) == 0:
-            # Look for e.g. 3DBall\UnityEnvironment.exe
-            crash_handlers = set(
-                glob.glob(os.path.join(cwd, env_path, "UnityCrashHandler*.exe"))
-            )
-            candidates = [
-                c
-                for c in glob.glob(os.path.join(cwd, env_path, "*.exe"))
-                if c not in crash_handlers
-            ]
-        if len(candidates) > 0:
-            launch_string = candidates[0]
-    return launch_string
-
-
-def launch_executable(file_name: str, args: List[str]) -> subprocess.Popen:
-    """
-    Launches a Unity executable and returns the process handle for it.
-    :param file_name: the name of the executable
-    :param args: List of string that will be passed as command line arguments
-    when launching the executable.
-    """
-    launch_string = validate_environment_path(file_name)
-    if launch_string is None:
-        raise UnityEnvironmentException(
-            f"Couldn't launch the {file_name} environment. Provided filename does not match any environments."
-        )
-    else:
-        logger.debug(f"The launch string is {launch_string}")
-        logger.debug(f"Running with args {args}")
-        # Launch Unity environment
-        subprocess_args = [launch_string] + args
-        # std_out_option = DEVNULL means the outputs will not be displayed on terminal.
-        # std_out_option = None is default behavior: the outputs are displayed on terminal.
-        std_out_option = subprocess.DEVNULL if logger.level > DEBUG else None
-        try:
-            return subprocess.Popen(
-                subprocess_args,
-                # start_new_session=True means that signals to the parent python process
-                # (e.g. SIGINT from keyboard interrupt) will not be sent to the new process on POSIX platforms.
-                # This is generally good since we want the environment to have a chance to shutdown,
-                # but may be undesirable in come cases; if so, we'll add a command-line toggle.
-                # Note that on Windows, the CTRL_C signal will still be sent.
-                start_new_session=True,
-                stdout=std_out_option,
-                stderr=std_out_option,
-            )
-        except PermissionError as perm:
-            # This is likely due to missing read or execute permissions on file.
-            raise UnityEnvironmentException(
-                f"Error when trying to launch environment - make sure "
-                f"permissions are set correctly. For example "
-                f'"chmod -R 755 {launch_string}"'
-            ) from perm
+import glob
+import os
+import subprocess
+from sys import platform
+from typing import Optional, List
+from pyrfuniverse.logging_util import get_logger, DEBUG
+from pyrfuniverse.exception import UnityEnvironmentException
+
+
+logger = get_logger(__name__)
+
+
+def get_platform():
+    """
+    returns the platform of the operating system : linux, darwin or win32
+    """
+    return platform
+
+
+def validate_environment_path(env_path: str) -> Optional[str]:
+    """
+    Strip out executable extensions of the env_path
+    :param env_path: The path to the executable
+    """
+    env_path = (
+        env_path.strip()
+        .replace(".app", "")
+        .replace(".exe", "")
+        .replace(".x86_64", "")
+        .replace(".x86", "")
+    )
+    true_filename = os.path.basename(os.path.normpath(env_path))
+    logger.debug(f"The true file name is {true_filename}")
+
+    if not (glob.glob(env_path) or glob.glob(env_path + ".*")):
+        return None
+
+    cwd = os.getcwd()
+    launch_string = None
+    true_filename = os.path.basename(os.path.normpath(env_path))
+    if get_platform() == "linux" or get_platform() == "linux2":
+        candidates = glob.glob(os.path.join(cwd, env_path) + ".x86_64")
+        if len(candidates) == 0:
+            candidates = glob.glob(os.path.join(cwd, env_path) + ".x86")
+        if len(candidates) == 0:
+            candidates = glob.glob(env_path + ".x86_64")
+        if len(candidates) == 0:
+            candidates = glob.glob(env_path + ".x86")
+        if len(candidates) == 0:
+            if os.path.isfile(env_path):
+                candidates = [env_path]
+        if len(candidates) > 0:
+            launch_string = candidates[0]
+
+    elif get_platform() == "darwin":
+        candidates = glob.glob(
+            os.path.join(cwd, env_path + ".app", "Contents", "MacOS", true_filename)
+        )
+        if len(candidates) == 0:
+            candidates = glob.glob(
+                os.path.join(env_path + ".app", "Contents", "MacOS", true_filename)
+            )
+        if len(candidates) == 0:
+            candidates = glob.glob(
+                os.path.join(cwd, env_path + ".app", "Contents", "MacOS", "*")
+            )
+        if len(candidates) == 0:
+            candidates = glob.glob(
+                os.path.join(env_path + ".app", "Contents", "MacOS", "*")
+            )
+        if len(candidates) > 0:
+            launch_string = candidates[0]
+    elif get_platform() == "win32":
+        candidates = glob.glob(os.path.join(cwd, env_path + ".exe"))
+        if len(candidates) == 0:
+            candidates = glob.glob(env_path + ".exe")
+        if len(candidates) == 0:
+            # Look for e.g. 3DBall\UnityEnvironment.exe
+            crash_handlers = set(
+                glob.glob(os.path.join(cwd, env_path, "UnityCrashHandler*.exe"))
+            )
+            candidates = [
+                c
+                for c in glob.glob(os.path.join(cwd, env_path, "*.exe"))
+                if c not in crash_handlers
+            ]
+        if len(candidates) > 0:
+            launch_string = candidates[0]
+    return launch_string
+
+
+def launch_executable(file_name: str, args: List[str]) -> subprocess.Popen:
+    """
+    Launches a Unity executable and returns the process handle for it.
+    :param file_name: the name of the executable
+    :param args: List of string that will be passed as command line arguments
+    when launching the executable.
+    """
+    launch_string = validate_environment_path(file_name)
+    if launch_string is None:
+        raise UnityEnvironmentException(
+            f"Couldn't launch the {file_name} environment. Provided filename does not match any environments."
+        )
+    else:
+        logger.debug(f"The launch string is {launch_string}")
+        logger.debug(f"Running with args {args}")
+        # Launch Unity environment
+        subprocess_args = [launch_string] + args
+        # std_out_option = DEVNULL means the outputs will not be displayed on terminal.
+        # std_out_option = None is default behavior: the outputs are displayed on terminal.
+        std_out_option = subprocess.DEVNULL if logger.level > DEBUG else None
+        try:
+            return subprocess.Popen(
+                subprocess_args,
+                # start_new_session=True means that signals to the parent python process
+                # (e.g. SIGINT from keyboard interrupt) will not be sent to the new process on POSIX platforms.
+                # This is generally good since we want the environment to have a chance to shutdown,
+                # but may be undesirable in come cases; if so, we'll add a command-line toggle.
+                # Note that on Windows, the CTRL_C signal will still be sent.
+                start_new_session=True,
+                stdout=std_out_option,
+                stderr=std_out_option,
+            )
+        except PermissionError as perm:
+            # This is likely due to missing read or execute permissions on file.
+            raise UnityEnvironmentException(
+                f"Error when trying to launch environment - make sure "
+                f"permissions are set correctly. For example "
+                f'"chmod -R 755 {launch_string}"'
+            ) from perm
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/environment.py` & `pyrfuniverse-0.8.4/pyrfuniverse/environment.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/__init__.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/balance_ball_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/balance_ball_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/base_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/base_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,27 +53,37 @@
     with open(log_file, 'w') as f:
         for id in worker_id_in_use:
             f.write(str(id) + '\n')
 
 
 class RFUniverseBaseEnv(ABC):
     """
-    RFUnivers基础环境类
+    RFUniverse base environment class.
+
+    Args:
+        executable_file: Str, the absolute path of Unity executable file. None for last used executable file; "@editor" for using Unity Editor.
+        scene_file: Str, the absolute path of Unity scene JSON file. All JSON files locate at `StraemingAssets/SceneData` by default.
+        assets: List, the list of pre-load assets. All assets in the list will be pre-loaded in Unity when the environment is initialized, which will save time during instanciating.
+        graphics: Bool, True for showing GUI and False for headless mode.
     """
     metadata = {'render.modes': ['human', 'rgb_array']}
 
     def __init__(
         self,
         executable_file: str = None,
         scene_file: str = None,
-        custom_channels: list = [],
-        assets: list = [],
+        custom_channels=None,
+        assets=None,
         graphics: bool = True,
         **kwargs
     ):
+        if custom_channels is None:
+            custom_channels = []
+        if assets is None:
+            assets = []
         # time step
         self.t = 0
         self.worker_id = select_available_worker_id()
         # initialize rfuniverse channels
         self.channels = custom_channels.copy()
         self._init_channels(kwargs)
         self.assets = assets
@@ -110,18 +120,18 @@
         else:
             self.env = UnityEnvironment(
                 worker_id=0,
                 side_channels=self.channels,
                 no_graphics=not self.graphics,
             )
         self._SendVersion()
-        if self.scene_file is not None:
-            self.LoadSceneAsync(self.scene_file, True)
         if len(self.assets) > 0:
             self._PreLoadAssetsAsync(self.assets, True)
+        if self.scene_file is not None:
+            self.LoadSceneAsync(self.scene_file, True)
         self.env.reset()
 
     def _init_channels(self, kwargs: dict):
         # Compulsory channels
         # Environment parameters channel
         self.env_param_channel = EnvironmentParametersChannel()
         self.channels.append(self.env_param_channel)
@@ -134,37 +144,40 @@
         self.channels.append(self.debug_channel)
 
     def _step(self):
         self.env.step()
 
     def step(self, count: int = 1):
         """
-        将已经调用的接口消息发送给Unity，执行一步仿真，然后接收Unity返回的数据
+        Send the messages of called functions to Unity and simulate for a step, then accept the data from Unity.
 
         Args:
-            count: 执行的步数
+            count: the number of steps for executing Unity simulation.
         """
         if count < 1:
             count = 1
         for _ in range(count):
             self.env.step()
 
     def close(self):
         """
-        关闭环境
+        Close the environment
         """
         delete_worker_id(self.worker_id)
         self.env.close()
 
     def GetAttr(self, id: int):
         """
-        根据ID获取物体
+        Get the attribute instance by object id.
 
         Args:
-            id: 物体ID
+            id: Int, object id.
+
+        Returns:
+            pyrfuniverse.attributes.BaseAttr: An instance of attribute.
         """
         if id not in self.attrs:
             self.attrs[id] = attr.BaseAttr(self, id)
         return self.attrs[id]
 
     #Env API
     def _PreLoadAssetsAsync(self, names: list, auto_wait: bool = False) -> None:
@@ -180,59 +193,77 @@
 
         if auto_wait:
             self.WaitLoadDone()
 
 
     def LoadSceneAsync(self, file: str, auto_wait: bool = False) -> None:
         """
-        异步加载场景
+        Load the scene asynchronisely.
 
         Args:
-            file: 场景Json文件，当该值为路径时，从路径加载场景，否则从StreamingAssets加载场景
-            auto_wait: 是否等待加载完成，如果为True，则在加载完成后才返回
+            file: Str, the scene JSON file. If it's a relative path, it will load from `StraemingAssets`.
+            auto_wait: Bool, if True, this function will not return until the loading is done.
         """
         msg = OutgoingMessage()
 
         msg.write_string('LoadSceneAsync')
         msg.write_string(file)
 
         self.asset_channel.send_message(msg)
 
         if auto_wait:
             self.WaitLoadDone()
 
+    def SwitchSceneAsync(self, name: str, auto_wait: bool = False) -> None:
+        """
+        Switch the scene asynchronisely.
+
+        Args:
+            name: Str, the scene name.
+            auto_wait: Bool, if True, this function will not return until the loading is done.
+        """
+        msg = OutgoingMessage()
+
+        msg.write_string('SwitchSceneAsync')
+        msg.write_string(name)
+
+        self.asset_channel.send_message(msg)
+
+        if auto_wait:
+            self.WaitLoadDone()
+
     def WaitLoadDone(self) -> None:
         """
-        等待加载完成，使用LoadSceneAsync接口后，调用该接口可以等待加载完成
+        Wait for the loading is done.
         """
         self.asset_channel.data['load_done'] = False
         while not self.asset_channel.data['load_done']:
             self.env.step()
 
     def Pend(self) -> None:
         """
-        挂起，直到UnityPlayer中点击EndPend按钮
+        Pend the program until the `EndPend` button in `UnityPlayer` is clicked.
         """
         msg = OutgoingMessage()
 
         msg.write_string('Pend')
 
         self.asset_channel.send_message(msg)
 
         self.asset_channel.data['pend_done'] = False
         while not self.asset_channel.data['pend_done']:
             self.env.step()
 
     def SendMessage(self, message: str, *args) -> None:
         """
-        发送动态消息给Unity
+        Send message to Unity.
 
         Args:
-            message: 消息头
-            *args: 参数列表，支持的参数类型有：str, bool, int, float, list[float]
+            message: Str, the message head.
+            args: List, the list of parameters. We support str, bool, int, float and List[float] types.
         """
         msg = OutgoingMessage()
 
         msg.write_string('SendMessage')
         msg.write_string(message)
         for i in args:
             if type(i) == str:
@@ -248,114 +279,116 @@
             else:
                 print(f'dont support this data type:{type(i)}')
 
         self.asset_channel.send_message(msg)
 
     def AddListener(self, message: str, fun):
         """
-        添加动态消息监听
+        Add listener.
 
         Args:
-            message: 消息头
-            fun: 回调函数
+            message: Str, the message head.
+            fun: Callable, the callback function.
         """
         if message in self.asset_channel.messages:
             if fun in self.asset_channel.messages[message]:
                 self.asset_channel.messages[message].append(fun)
         else:
             self.asset_channel.messages[message] = [fun]
 
     def RemoveListener(self, message: str, fun):
         """
-        移除动态消息监听
+        Remove listener.
 
         Args:
-            message: 消息头
-            fun: 回调函数
+            message: Str, the message head.
+            fun: Callable, the callback function.
         """
         if message in self.asset_channel.messages:
             if fun in self.asset_channel.messages[message]:
                 self.asset_channel.messages[message].remove(fun)
             if len(self.asset_channel.messages[message]) == 0:
                 self.asset_channel.messages[message].pop(message)
 
     def InstanceObject(self, name: str, id: int = None, attr_type: type = attr.BaseAttr):
         """
-        实例化物体
+        Instanciate an object.
 
-        Args:
-            name: 物体名
-                RfUniverseRelease中已有的资源类型及名称:
-                    GameObjcetAttr 静态物体:
-                        GameObject_Box,
-                        GameObject_Capsule,
-                        GameObject_Cylinder,
-                        GameObject_Sphere,
-                        GameObject_Quad,
-
-                        IGbison 环境:
-                            Hainesburg_mesh_texture,
-                            Halfway_mesh_texture,
-                            Hallettsville_mesh_texture,
-                            Hambleton_mesh_texture,
-                            Hammon_mesh_texture,
-                            Hatfield_mesh_texture,
-                            Haxtun_mesh_texture,
-                            Haymarket_mesh_texture,
-                            Hendrix_mesh_texture,
-                            Hercules_mesh_texture,
-                            Highspire_mesh_texture,
-                            Hitchland_mesh_texture,
-
-                    ColliderAttr 带有碰撞体的静态物体:
-                        Collider_Box,
-                        Collider_ObiBox,
-                        Collider_Capsule,
-                        Collider_Cylinder,
-                        Collider_Sphere,
-                        Collider_Quad,
-
-                    RigidbodyAttr 刚体:
-                        Rigidbody_Box,
-                        GameObject_Capsule,
-                        Rigidbody_Cylinder,
-                        Rigidbody_Sphere,
-
-                        77个YCB数据集模型: 详见The YCB Object and Model Set: https://rse-lab.cs.washington.edu/projects/posecnn/
-
-                    ControllerAttr 机械臂及关节体:
-                        gripper:
-                            allegro_hand_right,
-                            bhand,
-                            svh,
-                            robotiq_arg2f_85_model,
-                            dh_robotics_ag95_gripper,
-                        robot:
-                            kinova_gen3,
-                            kinova_gen3_robotiq85,
-                            ur5,
-                            ur5_robotiq85,
-                            franka_panda,
-                            franka_hand,
-                            tobor_robotiq85_robotiq85,
-                            flexivArm,
-                            flexivArm_ag95,
-                            yumi,
-
-                    CameraAttr 相机:
-                        Camera,
-
-                    LightAttr 灯光:
-                        Light,
-
-            id: 物体ID
-            attr_type: 物体类型
+        Built-in assets:
+    
+        GameObjectAttr:
+            Basic Objects:
+                "GameObject_Box",
+                "GameObject_Capsule",
+                "GameObject_Cylinder",
+                "GameObject_Sphere",
+                "GameObject_Quad",
+            IGbison Meshes:
+                "Hainesburg_mesh_texture",
+                "Halfway_mesh_texture",
+                "Hallettsville_mesh_texture",
+                "Hambleton_mesh_texture",
+                "Hammon_mesh_texture",
+                "Hatfield_mesh_texture",
+                "Haxtun_mesh_texture",
+                "Haymarket_mesh_texture",
+                "Hendrix_mesh_texture",
+                "Hercules_mesh_texture",
+                "Highspire_mesh_texture",
+                "Hitchland_mesh_texture",
+
+        ColliderAttr:
+            "Collider_Box",
+            "Collider_ObiBox",
+            "Collider_Capsule",
+            "Collider_Cylinder",
+            "Collider_Sphere",
+            "Collider_Quad",
+
+        RigidbodyAttr:
+            Basic Objects:
+                "Rigidbody_Box",
+                "GameObject_Capsule",
+                "Rigidbody_Cylinder",
+                "Rigidbody_Sphere",
+            YCB dataset: 
+                77 models in YCB dataset. See YCB Object and Model Set for detail: https://rse-lab.cs.washington.edu/projects/posecnn/
+
+        ControllerAttr:
+            gripper:
+                "allegro_hand_right",
+                "bhand",
+                "svh",
+                "robotiq_arg2f_85_model",
+                "dh_robotics_ag95_gripper",
+            robot:
+                "kinova_gen3",
+                "kinova_gen3_robotiq85",
+                "ur5",
+                "ur5_robotiq85",
+                "franka_panda",
+                "franka_hand",
+                "tobor_robotiq85_robotiq85",
+                "flexivArm",
+                "flexivArm_ag95",
+                "yumi",
+
+        CameraAttr:
+            "Camera",
+
+        LightAttr:
+            "Light",
+
+        Args:
+            name: Str, object name. Please check the above `built-in assets` list for names.
+            id: Int, object id.
+            attr_type: type(pyrfuniverse.attributes.BaseAttr), the attribute type.
 
         Returns:
-            物体实例
+            type(`attr_type`): The object attribute instance.
         """
         assert id not in self.attrs, \
             'this ID exists'
 
         while id is None or id in self.attrs:
             id = random.randint(100000, 999999)
 
@@ -368,23 +401,23 @@
         self.asset_channel.send_message(msg)
 
         self.attrs[id] = attr_type(self, id)
         return self.attrs[id]
 
     def LoadURDF(self, path: str, id: int = None, native_ik: bool = True) -> attr.ControllerAttr:
         """
-        加载URDF模型
+        Load a model from URDF file.
 
         Args:
-            path: URDF路径
-            id: 物体ID
-            native_ik: 是否启用内置IK
+            path: Str, the URDF file path.
+            id: Int, object id.
+            native_ik: Bool, True for enabling native IK; False for using custom IK.
 
         Returns:
-            ControllerAttr机械臂实例
+            pyrfuniverse.attributes.ControllerAttr: The object attribute intance.
         """
         assert id not in self.attrs, \
             'this ID exists'
 
         while id is None or id in self.attrs:
             id = random.randint(100000, 999999)
 
@@ -398,22 +431,22 @@
         self.asset_channel.send_message(msg)
 
         self.attrs[id] = attr.ControllerAttr(self, id)
         return self.attrs[id]
 
     def LoadMesh(self, path: str, id: int = None) -> attr.RigidbodyAttr:
         """
-        加载Mesh模型
+        Load a model from Mesh file.
 
         Args:
-            path: Mesh路径
-            id: 物体ID
+            path: Str, the Mesh file path.
+            id: Int, object id.
 
         Returns:
-            RigidbodyAttr刚体实例
+            pyrfuniverse.attributes.RigidbodyAttr: The object attribute intance.
         """
         assert id not in self.attrs, \
             'this ID exists'
 
         while id is None or id in self.attrs:
             id = random.randint(100000, 999999)
 
@@ -426,217 +459,217 @@
         self.asset_channel.send_message(msg)
 
         self.attrs[id] = attr.RigidbodyAttr(self, id)
         return self.attrs[id]
 
     def IgnoreLayerCollision(self, layer1: int, layer2: int, ignore: bool) -> None:
         """
-        忽略或启用指定两个层的碰撞
+        Ignore or enable the collision between two layers.
 
         Args:
-            layer1: 层1
-            layer2: 层1
-            ignore: 是否忽略
+            layer1: Int, the layer number of the first layer.
+            layer2: Int, the layer number of the second layer.
+            ignore: Bool, True for ignoring collision between two layers; False for enabling collision between two layers.
         """
         msg = OutgoingMessage()
 
         msg.write_string('IgnoreLayerCollision')
         msg.write_int32(layer1)
         msg.write_int32(layer2)
         msg.write_bool(ignore)
 
         self.asset_channel.send_message(msg)
 
     def GetCurrentCollisionPairs(self) -> None:
         """
-        获取当前碰撞对
+        Get the collision pairs of current collision.
 
         Returns:
-            调用此接口并step后，从env.data['CurrentCollisionPairs']中获取碰撞对
+            Call this function and `step()`, the collision pairs can be got from env.data['CurrentCollisionPairs'].
         """
         msg = OutgoingMessage()
 
         msg.write_string('GetCurrentCollisionPairs')
 
         self.asset_channel.send_message(msg)
 
     def GetRFMoveColliders(self) -> None:
         """
-        获取RFMove碰撞体
+        Get the RFMove colliders.
 
         Returns:
-            调用此接口并step后，从env.data['RFMoveColliders']中获取碰撞体
+            Call this function and `step()`, the collision pairs can be got from env.data['RFMoveColliders'].
         """
         msg = OutgoingMessage()
 
         msg.write_string('GetRFMoveColliders')
 
         self.asset_channel.send_message(msg)
 
     def SetGravity(self, x: float, y: float, z: float) -> None:
         """
-        设置环境重力
+        Set the gravity of environment.
 
         Args:
-            x: 右方向
-            y: 上方向
-            z: 前方向
+            x: Float, gravity on global x-axis (right).
+            y: Float, gravity on global y-axis (up).
+            z: Float, gravity on global z-axis (forward).
         """
         msg = OutgoingMessage()
 
         msg.write_string('SetGravity')
         msg.write_float32(x)
         msg.write_float32(y)
         msg.write_float32(z)
 
         self.asset_channel.send_message(msg)
 
     def SetGroundPhysicMaterial(self, bounciness: float, dynamic_friction: float, static_friction: float, friction_combine: int, bounce_combine: int) -> None:
         """
-        设置环境地面物理材质
+        Set the physics material of ground in environment.
 
         Args:
-            bounciness: 弹力
-            dynamic_friction: 动摩擦力
-            static_friction: 静摩擦力
-            friction_combine: 摩擦力组合方式
-            bounce_combine: 弹力组合方式
+            bounciness: Float, the bounciness.
+            dynamic_friction: Float, the dynamic friction coefficient (0-1).
+            static_friction: Float, the static friction coefficient (0-1).
+            friction_combine: Int, how friction of two colliding objects is combined. 0 for Average, 1 for Minimum, 2 for Maximum and 3 for Multiply. See https://docs.unity3d.com/Manual/class-PhysicMaterial.html for more details.
+            bounce_combine: Int, how bounciness of two colliding objects is combined. The value representation is the same with `friction_combine`.
         """
         msg = OutgoingMessage()
 
         msg.write_string('SetGroundPhysicMaterial')
         msg.write_float32(bounciness)
         msg.write_float32(dynamic_friction)
         msg.write_float32(static_friction)
         msg.write_int32(friction_combine)
         msg.write_int32(bounce_combine)
 
         self.asset_channel.send_message(msg)
 
     def SetTimeStep(self, delta_time: float) -> None:
         """
-        设置环境step时间步长
+        Set the time for a step in Unity.
 
         Args:
-            delta_time: 时间步长(s)
+            delta_time: Float, the time for a step in Unity.
         """
         msg = OutgoingMessage()
 
         msg.write_string('SetTimeStep')
         msg.write_float32(delta_time)
 
         self.asset_channel.send_message(msg)
 
     def SetTimeScale(self, time_scale: float) -> None:
         """
-        设置环境时间缩放比例
+        Set the time scale in Unity.
 
         Args:
-            time_scale: 时间缩放比例
+            time_scale: Float, the time scale in Unity.
         """
         msg = OutgoingMessage()
 
         msg.write_string('SetTimeScale')
         msg.write_float32(time_scale)
 
         self.asset_channel.send_message(msg)
 
     def SetResolution(self, resolution_x: int, resolution_y: int) -> None:
         """
-        设置窗口分辨率
+        Set the resolution of windowed GUI.
 
         Args:
-            resolution_x: 宽度width分辨率
-            resolution_y: 高度height分辨率
+            resolution_x: Int, window width.
+            resolution_y: Int, window height.
         """
         msg = OutgoingMessage()
 
         msg.write_string('SetResolution')
         msg.write_int32(resolution_x)
         msg.write_int32(resolution_y)
 
         self.asset_channel.send_message(msg)
 
     def ExportOBJ(self, items_id: list, save_path: str) -> None:
         """
-        导出指定物体列表为OBJ文件，对于原生Bundle模型，需要在UnityEditor中勾选Read/Write才能正确导出
+        Export the specified object list to OBJ file. For native bundle models, the `Read/Write` must be checked in Unity Editor.
 
         Args:
-            items_id: 物体ID列表
-            save_path: 保存绝对路径
+            items_id: List, the object ids.
+            save_path: Str, the path to save the OBJ files.
         """
         msg = OutgoingMessage()
 
         msg.write_string('ExportOBJ')
         msg.write_int32(len(items_id))
         for i in items_id:
             msg.write_int32(i)
         msg.write_string(save_path)
 
         self.asset_channel.send_message(msg)
 
     def SetShadowDistance(self, distance: float) -> None:
         """
-        设置环境阴影渲染距离
+        Set the shadow distance for rendering in environment.
 
         Args:
-            distance: 距离(m)
+            distance: Float, the shadow distance measured in meter.
         """
         msg = OutgoingMessage()
 
         msg.write_string('SetShadowDistance')
         msg.write_float32(distance)
 
         self.asset_channel.send_message(msg)
 
     def SaveScene(self, file: str) -> None:
         """
-        保存当前场景
+        Save current scene.
 
         Args:
-            file: 存储场景Json路径，当该值为路径时，保存到该路径，否则保存到StreamingAssets
+            file: Str, the file path to save current scene. Default saving to `StreamingAssets` folder.
         """
         msg = OutgoingMessage()
 
         msg.write_string('SaveScene')
         msg.write_string(file)
 
         self.asset_channel.send_message(msg)
 
     def ClearScene(self) -> None:
         """
-        清理当前场景
+        Clear current scene.
         """
         msg = OutgoingMessage()
 
         msg.write_string('ClearScene')
 
         self.asset_channel.send_message(msg)
 
     def AlignCamera(self, camera_id: int) -> None:
         """
-        对齐视口到相机
+        Align current GUI view to a given camera.
 
         Args:
-            camera_id: 相机ID
+            camera_id: Int, camera id.
         """
         msg = OutgoingMessage()
 
         msg.write_string('AlignCamera')
         msg.write_int32(camera_id)
 
         self.asset_channel.send_message(msg)
 
     def SetViewTransform(self, position: list = None, rotation: list = None) -> None:
         """
-        设置视口位置和旋转
+        Set the GUI view.
 
         Args:
-            position: 位置
-            rotation: 旋转
+            position: A list of length 3, representing the position of GUI view.
+            rotation: A list of length 3, representing the rotation of GUI view.
         """
         msg = OutgoingMessage()
 
         msg.write_string('SetViewTransform')
         msg.write_bool(position is not None)
         msg.write_bool(rotation is not None)
         if position is not None:
@@ -652,89 +685,114 @@
 
         self.asset_channel.send_message(msg)
 
 
     #Dubug API
     def DebugGraspPoint(self, enabled: bool = True) -> None:
         """
-        Debug显示机械臂末端点
+        Show or hide end effector of robot arm for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
         """
         msg = OutgoingMessage()
         msg.write_string('DebugGraspPoint')
         msg.write_bool(enabled)
         self.debug_channel.send_message(msg)
 
     def DebugObjectPose(self, enabled: bool = True) -> None:
         """
-        Debug显示物体base点
+        Show or hide object base point for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
         """
         msg = OutgoingMessage()
         msg.write_string('DebugObjectPose')
         msg.write_bool(enabled)
         self.debug_channel.send_message(msg)
 
     def DebugCollisionPair(self, enabled: bool = True) -> None:
         """
-        Debug显示物理碰撞对
+        Show or hide collision pairs for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
         """
         msg = OutgoingMessage()
         msg.write_string('DebugCollisionPair')
         msg.write_bool(enabled)
         self.debug_channel.send_message(msg)
+    
     def DebugColliderBound(self, enabled: bool = True) -> None:
         """
-        Debug显示碰撞包围盒
+        Show or hide collider bounding box for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
         """
         msg = OutgoingMessage()
         msg.write_string('DebugColliderBound')
         msg.write_bool(enabled)
         self.debug_channel.send_message(msg)
 
     def DebugObjectID(self, enabled: bool = True) -> None:
         """
-        Debug显示碰物体ID
+        Show or hide object id for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
         """
         msg = OutgoingMessage()
         msg.write_string('DebugObjectID')
         msg.write_bool(enabled)
         self.debug_channel.send_message(msg)
 
     def Debug3DBBox(self, enabled: bool = True) -> None:
         """
-        Debug显示物体3DBoundingBox
+        Show or hide 3d bounding box of objects for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
         """
         msg = OutgoingMessage()
         msg.write_string('Debug3DBBox')
         msg.write_bool(enabled)
         self.debug_channel.send_message(msg)
 
     def Debug2DBBox(self, enabled: bool = True) -> None:
         """
-        Debug显示物体2DBoundingBox
+        Show or hide 2d bounding box of objects for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
         """
         msg = OutgoingMessage()
         msg.write_string('Debug2DBBox')
         msg.write_bool(enabled)
         self.debug_channel.send_message(msg)
 
     def DebugJointLink(self, enabled: bool = True) -> None:
         """
-        Debug显示关节体Joint信息
+        Show or hide joint information of articulation for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
         """
         msg = OutgoingMessage()
         msg.write_string('DebugJointLink')
         msg.write_bool(enabled)
         self.debug_channel.send_message(msg)
 
     def SendLog(self, log: str) -> None:
         """
-        发送Log消息并显示在Unity窗口
+        Send log messange and show it on Unity GUI window.
 
         Args:
-            log: Log内容
+            log: Str, log message.
         """
         msg = OutgoingMessage()
         msg.write_string('SendLog')
         msg.write_string(log)
         self.debug_channel.send_message(msg)
 
     def _SendVersion(self) -> None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/bouncer_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/bouncer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/franka_grasp_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/franka_grasp_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/franka_push_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/franka_push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/__init__.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/nail_can_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/nail_card_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/cleaner_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_agent/cleaner_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent/navigation_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_agent/navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/multi_agent_navigation_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/multi_agent_navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/rfuniverse_robot_hub_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/rfuniverse_robot_hub_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/__init__.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_cloth_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/franka_cloth_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_robotics_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/franka_robotics_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         self.goal_range_high = np.array([target_xz_range, target_y_range, target_xz_range])
         self.object_range_low = np.array([-object_xz_range, self.height_offset, -object_xz_range])
         self.object_range_high = np.array([object_xz_range, self.height_offset, object_xz_range])
         self.asset_bundle_file = asset_bundle_file
 
         self.seed(seed)
         self._env_setup()
+        self.init_pos = np.array(self.instance_channel.data[9658740]['positions'][3])
         self.t = 0
         self.goal = self._sample_goal()
         self.action_space = spaces.Box(
             low=-1, high=1, shape=(4,), dtype=np.float32
         )
 
         obs = self._get_obs()
@@ -120,20 +121,18 @@
         #     position=list(self.goal)
         # )
         # self._step()
 
         # self.ik_controller.reset()
 
         if self.load_object and self.target_in_air:
-            # Move the robot arm to the object's position, which can accelerate training process
-            # joint_positions = self.ik_controller.calculate_ik(object_pos)
             self.instance_channel.set_action(
                 "IKTargetDoMove",
                 id=965874,
-                position=[object_pos[0], object_pos[1] + 0.1, object_pos[2]],
+                position=[self.init_pos[0], self.init_pos[1], self.init_pos[2]],
                 duration=0,
                 speed_based=False,
             )
             self._step()
             self.instance_channel.set_action(
                 'SetJointPositionDirectly',
                 id=9658740,
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/franka_softbody_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/franka_softbody_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/pick_and_place_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/pick_and_place_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/push_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/robotics/reach_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/robotics/reach_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/roller_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/roller_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/ur5_box_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/ur5_box_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/envs/ur5_drawer_env.py` & `pyrfuniverse-0.8.4/pyrfuniverse/envs/ur5_drawer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/exception.py` & `pyrfuniverse-0.8.4/pyrfuniverse/exception.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-class UnityException(Exception):
-    """
-    Any error related to ml-agents environment.
-    """
-
-    pass
-
-
-class UnityEnvironmentException(UnityException):
-    """
-    Related to errors starting and closing environment.
-    """
-
-    pass
-
-
-class UnityCommunicationException(UnityException):
-    """
-    Related to errors with the communicator.
-    """
-
-    pass
-
-
-class UnityCommunicatorStoppedException(UnityException):
-    """
-    Raised when communicator has stopped gracefully.
-    """
-
-    pass
-
-
-class UnityObservationException(UnityException):
-    """
-    Related to errors with receiving observations.
-    """
-
-    pass
-
-
-class UnityActionException(UnityException):
-    """
-    Related to errors with sending actions.
-    """
-
-    pass
-
-
-class UnityTimeOutException(UnityException):
-    """
-    Related to errors with communication timeouts.
-    """
-
-    pass
-
-
-class UnitySideChannelException(UnityException):
-    """
-    Related to errors with side channels.
-    """
-
-    pass
-
-
-class UnityWorkerInUseException(UnityException):
-    """
-    This error occurs when the port for a certain worker ID is already reserved.
-    """
-
-    MESSAGE_TEMPLATE = (
-        "Couldn't start socket communication because worker number {} is still in use. "
-        "You may need to manually close a previously opened environment "
-        "or use a different worker number."
-    )
-
-    def __init__(self, worker_id):
-        message = self.MESSAGE_TEMPLATE.format(str(worker_id))
-        super().__init__(message)
-
-
-class UnityPolicyException(UnityException):
-    """
-    Related to errors with the Trainer.
-    """
-
-    pass
+class UnityException(Exception):
+    """
+    Any error related to ml-agents environment.
+    """
+
+    pass
+
+
+class UnityEnvironmentException(UnityException):
+    """
+    Related to errors starting and closing environment.
+    """
+
+    pass
+
+
+class UnityCommunicationException(UnityException):
+    """
+    Related to errors with the communicator.
+    """
+
+    pass
+
+
+class UnityCommunicatorStoppedException(UnityException):
+    """
+    Raised when communicator has stopped gracefully.
+    """
+
+    pass
+
+
+class UnityObservationException(UnityException):
+    """
+    Related to errors with receiving observations.
+    """
+
+    pass
+
+
+class UnityActionException(UnityException):
+    """
+    Related to errors with sending actions.
+    """
+
+    pass
+
+
+class UnityTimeOutException(UnityException):
+    """
+    Related to errors with communication timeouts.
+    """
+
+    pass
+
+
+class UnitySideChannelException(UnityException):
+    """
+    Related to errors with side channels.
+    """
+
+    pass
+
+
+class UnityWorkerInUseException(UnityException):
+    """
+    This error occurs when the port for a certain worker ID is already reserved.
+    """
+
+    MESSAGE_TEMPLATE = (
+        "Couldn't start socket communication because worker number {} is still in use. "
+        "You may need to manually close a previously opened environment "
+        "or use a different worker number."
+    )
+
+    def __init__(self, worker_id):
+        message = self.MESSAGE_TEMPLATE.format(str(worker_id))
+        super().__init__(message)
+
+
+class UnityPolicyException(UnityException):
+    """
+    Related to errors with the Trainer.
+    """
+
+    pass
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/mock_communicator.py` & `pyrfuniverse-0.8.4/pyrfuniverse/mock_communicator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-from typing import Optional
-
-from .communicator import Communicator, PollCallback
-from .environment import UnityEnvironment
-from pyrfuniverse.communicator_objects.unity_rl_output_pb2 import UnityRLOutputProto
-from pyrfuniverse.communicator_objects.brain_parameters_pb2 import (
-    BrainParametersProto,
-    ActionSpecProto,
-)
-from pyrfuniverse.communicator_objects.unity_rl_initialization_output_pb2 import (
-    UnityRLInitializationOutputProto,
-)
-from pyrfuniverse.communicator_objects.unity_input_pb2 import UnityInputProto
-from pyrfuniverse.communicator_objects.unity_output_pb2 import UnityOutputProto
-from pyrfuniverse.communicator_objects.agent_info_pb2 import AgentInfoProto
-from pyrfuniverse.communicator_objects.observation_pb2 import (
-    ObservationProto,
-    NONE as COMPRESSION_TYPE_NONE,
-    PNG as COMPRESSION_TYPE_PNG,
-)
-
-
-class MockCommunicator(Communicator):
-    def __init__(
-        self,
-        discrete_action=False,
-        visual_inputs=0,
-        num_agents=3,
-        brain_name="RealFakeBrain",
-        vec_obs_size=3,
-    ):
-        """
-        Python side of the grpc communication. Python is the client and Unity the server
-        """
-        super().__init__()
-        self.is_discrete = discrete_action
-        self.steps = 0
-        self.visual_inputs = visual_inputs
-        self.has_been_closed = False
-        self.num_agents = num_agents
-        self.brain_name = brain_name
-        self.vec_obs_size = vec_obs_size
-
-    def initialize(
-        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
-    ) -> UnityOutputProto:
-        if self.is_discrete:
-            action_spec = ActionSpecProto(
-                num_discrete_actions=2, discrete_branch_sizes=[3, 2]
-            )
-        else:
-            action_spec = ActionSpecProto(num_continuous_actions=2)
-        bp = BrainParametersProto(
-            brain_name=self.brain_name, is_training=True, action_spec=action_spec
-        )
-        rl_init = UnityRLInitializationOutputProto(
-            name="RealFakeAcademy",
-            communication_version=UnityEnvironment.API_VERSION,
-            package_version="mock_package_version",
-            log_path="",
-            brain_parameters=[bp],
-        )
-        output = UnityRLOutputProto(agentInfos=self._get_agent_infos())
-        return UnityOutputProto(rl_initialization_output=rl_init, rl_output=output)
-
-    def _get_agent_infos(self):
-        dict_agent_info = {}
-        list_agent_info = []
-        vector_obs = [1, 2, 3]
-
-        observations = [
-            ObservationProto(
-                compressed_data=None,
-                shape=[30, 40, 3],
-                compression_type=COMPRESSION_TYPE_PNG,
-            )
-            for _ in range(self.visual_inputs)
-        ]
-        vector_obs_proto = ObservationProto(
-            float_data=ObservationProto.FloatData(data=vector_obs),
-            shape=[len(vector_obs)],
-            compression_type=COMPRESSION_TYPE_NONE,
-        )
-        observations.append(vector_obs_proto)
-
-        for i in range(self.num_agents):
-            list_agent_info.append(
-                AgentInfoProto(
-                    reward=1,
-                    done=(i == 2),
-                    max_step_reached=False,
-                    id=i,
-                    observations=observations,
-                )
-            )
-        dict_agent_info["RealFakeBrain"] = UnityRLOutputProto.ListAgentInfoProto(
-            value=list_agent_info
-        )
-        return dict_agent_info
-
-    def exchange(
-        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
-    ) -> UnityOutputProto:
-        result = UnityRLOutputProto(agentInfos=self._get_agent_infos())
-        return UnityOutputProto(rl_output=result)
-
-    def close(self):
-        """
-        Sends a shutdown signal to the unity environment, and closes the grpc connection.
-        """
-        self.has_been_closed = True
+from typing import Optional
+
+from .communicator import Communicator, PollCallback
+from .environment import UnityEnvironment
+from pyrfuniverse.communicator_objects.unity_rl_output_pb2 import UnityRLOutputProto
+from pyrfuniverse.communicator_objects.brain_parameters_pb2 import (
+    BrainParametersProto,
+    ActionSpecProto,
+)
+from pyrfuniverse.communicator_objects.unity_rl_initialization_output_pb2 import (
+    UnityRLInitializationOutputProto,
+)
+from pyrfuniverse.communicator_objects.unity_input_pb2 import UnityInputProto
+from pyrfuniverse.communicator_objects.unity_output_pb2 import UnityOutputProto
+from pyrfuniverse.communicator_objects.agent_info_pb2 import AgentInfoProto
+from pyrfuniverse.communicator_objects.observation_pb2 import (
+    ObservationProto,
+    NONE as COMPRESSION_TYPE_NONE,
+    PNG as COMPRESSION_TYPE_PNG,
+)
+
+
+class MockCommunicator(Communicator):
+    def __init__(
+        self,
+        discrete_action=False,
+        visual_inputs=0,
+        num_agents=3,
+        brain_name="RealFakeBrain",
+        vec_obs_size=3,
+    ):
+        """
+        Python side of the grpc communication. Python is the client and Unity the server
+        """
+        super().__init__()
+        self.is_discrete = discrete_action
+        self.steps = 0
+        self.visual_inputs = visual_inputs
+        self.has_been_closed = False
+        self.num_agents = num_agents
+        self.brain_name = brain_name
+        self.vec_obs_size = vec_obs_size
+
+    def initialize(
+        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
+    ) -> UnityOutputProto:
+        if self.is_discrete:
+            action_spec = ActionSpecProto(
+                num_discrete_actions=2, discrete_branch_sizes=[3, 2]
+            )
+        else:
+            action_spec = ActionSpecProto(num_continuous_actions=2)
+        bp = BrainParametersProto(
+            brain_name=self.brain_name, is_training=True, action_spec=action_spec
+        )
+        rl_init = UnityRLInitializationOutputProto(
+            name="RealFakeAcademy",
+            communication_version=UnityEnvironment.API_VERSION,
+            package_version="mock_package_version",
+            log_path="",
+            brain_parameters=[bp],
+        )
+        output = UnityRLOutputProto(agentInfos=self._get_agent_infos())
+        return UnityOutputProto(rl_initialization_output=rl_init, rl_output=output)
+
+    def _get_agent_infos(self):
+        dict_agent_info = {}
+        list_agent_info = []
+        vector_obs = [1, 2, 3]
+
+        observations = [
+            ObservationProto(
+                compressed_data=None,
+                shape=[30, 40, 3],
+                compression_type=COMPRESSION_TYPE_PNG,
+            )
+            for _ in range(self.visual_inputs)
+        ]
+        vector_obs_proto = ObservationProto(
+            float_data=ObservationProto.FloatData(data=vector_obs),
+            shape=[len(vector_obs)],
+            compression_type=COMPRESSION_TYPE_NONE,
+        )
+        observations.append(vector_obs_proto)
+
+        for i in range(self.num_agents):
+            list_agent_info.append(
+                AgentInfoProto(
+                    reward=1,
+                    done=(i == 2),
+                    max_step_reached=False,
+                    id=i,
+                    observations=observations,
+                )
+            )
+        dict_agent_info["RealFakeBrain"] = UnityRLOutputProto.ListAgentInfoProto(
+            value=list_agent_info
+        )
+        return dict_agent_info
+
+    def exchange(
+        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
+    ) -> UnityOutputProto:
+        result = UnityRLOutputProto(agentInfos=self._get_agent_infos())
+        return UnityOutputProto(rl_output=result)
+
+    def close(self):
+        """
+        Sends a shutdown signal to the unity environment, and closes the grpc connection.
+        """
+        self.has_been_closed = True
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/registry/base_registry_entry.py` & `pyrfuniverse-0.8.4/pyrfuniverse/registry/base_registry_entry.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/registry/binary_utils.py` & `pyrfuniverse-0.8.4/pyrfuniverse/registry/binary_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/registry/remote_registry_entry.py` & `pyrfuniverse-0.8.4/pyrfuniverse/registry/remote_registry_entry.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/registry/unity_env_registry.py` & `pyrfuniverse-0.8.4/pyrfuniverse/registry/unity_env_registry.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/asset_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/asset_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import warnings
 
+import numpy as np
+
 from pyrfuniverse.side_channel.side_channel import (
     IncomingMessage,
     OutgoingMessage,
 )
 from pyrfuniverse.rfuniverse_channel import RFUniverseChannel
 import pyrfuniverse.utils.rfuniverse_utility as utility
 
@@ -120,16 +122,16 @@
         for i in args:
             if type(i) == str:
                 msg.write_string(i)
             elif type(i) == bool:
                 msg.write_bool(i)
             elif type(i) == int:
                 msg.write_int32(i)
-            elif type(i) == float:
-                msg.write_float32(i)
+            elif type(i) == float or type(i) == np.float32 or type(i) == np.float64:
+                msg.write_float32(float(i))
             elif type(i) == list and type(i[0]) == float:
                 msg.write_float32_list(i)
             else:
                 print(f'dont support this data type:{type(i)}')
 
         self.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/debug_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/debug_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/instance_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/instance_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/rpc_communicator.py` & `pyrfuniverse-0.8.4/pyrfuniverse/rpc_communicator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import grpc
-from typing import Optional
-
-from multiprocessing import Pipe
-from sys import platform
-import socket
-import time
-from concurrent.futures import ThreadPoolExecutor
-
-from .communicator import Communicator, PollCallback
-from pyrfuniverse.communicator_objects.unity_to_external_pb2_grpc import (
-    UnityToExternalProtoServicer,
-    add_UnityToExternalProtoServicer_to_server,
-)
-from pyrfuniverse.communicator_objects.unity_message_pb2 import UnityMessageProto
-from pyrfuniverse.communicator_objects.unity_input_pb2 import UnityInputProto
-from pyrfuniverse.communicator_objects.unity_output_pb2 import UnityOutputProto
-from .exception import UnityTimeOutException, UnityWorkerInUseException
-
-
-class UnityToExternalServicerImplementation(UnityToExternalProtoServicer):
-    def __init__(self):
-        self.parent_conn, self.child_conn = Pipe()
-
-    def Initialize(self, request, context):
-        self.child_conn.send(request)
-        return self.child_conn.recv()
-
-    def Exchange(self, request, context):
-        self.child_conn.send(request)
-        return self.child_conn.recv()
-
-
-class RpcCommunicator(Communicator):
-    def __init__(self, worker_id=0, base_port=5005, timeout_wait=30):
-        """
-        Python side of the grpc communication. Python is the server and Unity the client
-
-
-        :int base_port: Baseline port number to connect to Unity environment over. worker_id increments over this.
-        :int worker_id: Offset from base_port. Used for training multiple environments simultaneously.
-        :int timeout_wait: Timeout (in seconds) to wait for a response before exiting.
-        """
-        super().__init__(worker_id, base_port)
-        self.port = base_port + worker_id
-        self.worker_id = worker_id
-        self.timeout_wait = timeout_wait
-        self.server = None
-        self.unity_to_external = None
-        self.is_open = False
-        self.create_server()
-
-    def create_server(self):
-        """
-        Creates the GRPC server.
-        """
-        self.check_port(self.port)
-
-        try:
-            # Establish communication grpc
-            self.server = grpc.server(ThreadPoolExecutor(max_workers=10))
-            self.unity_to_external = UnityToExternalServicerImplementation()
-            add_UnityToExternalProtoServicer_to_server(
-                self.unity_to_external, self.server
-            )
-            # Using unspecified address, which means that grpc is communicating on all IPs
-            # This is so that the docker container can connect.
-            self.server.add_insecure_port("[::]:" + str(self.port))
-            self.server.start()
-            self.is_open = True
-        except Exception:
-            raise UnityWorkerInUseException(self.worker_id)
-
-    def check_port(self, port):
-        """
-        Attempts to bind to the requested communicator port, checking if it is already in use.
-        """
-        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        if platform == "linux" or platform == "linux2":
-            # On linux, the port remains unusable for TIME_WAIT=60 seconds after closing
-            # SO_REUSEADDR frees the port right after closing the environment
-            s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        try:
-            s.bind(("localhost", port))
-        except OSError:
-            raise UnityWorkerInUseException(self.worker_id)
-        finally:
-            s.close()
-
-    def poll_for_timeout(self, poll_callback: Optional[PollCallback] = None) -> None:
-        """
-        Polls the GRPC parent connection for data, to be used before calling recv.  This prevents
-        us from hanging indefinitely in the case where the environment process has died or was not
-        launched.
-
-        Additionally, a callback can be passed to periodically check the state of the environment.
-        This is used to detect the case when the environment dies without cleaning up the connection,
-        so that we can stop sooner and raise a more appropriate error.
-        """
-        deadline = time.monotonic() + self.timeout_wait
-        callback_timeout_wait = self.timeout_wait // 10
-        while time.monotonic() < deadline:
-            if self.unity_to_external.parent_conn.poll(callback_timeout_wait):
-                # Got an acknowledgment from the connection
-                return
-            if poll_callback:
-                # Fire the callback - if it detects something wrong, it should raise an exception.
-                poll_callback()
-
-        # Got this far without reading any data from the connection, so it must be dead.
-        raise UnityTimeOutException(
-            "The Unity environment took too long to respond. Make sure that :\n"
-            "\t The environment does not need user interaction to launch\n"
-            '\t The Agents\' Behavior Parameters > Behavior Type is set to "Default"\n'
-            "\t The environment and the Python interface have compatible versions."
-        )
-
-    def initialize(
-        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
-    ) -> UnityOutputProto:
-        self.poll_for_timeout(poll_callback)
-        aca_param = self.unity_to_external.parent_conn.recv().unity_output
-        message = UnityMessageProto()
-        message.header.status = 200
-        message.unity_input.CopyFrom(inputs)
-        self.unity_to_external.parent_conn.send(message)
-        self.unity_to_external.parent_conn.recv()
-        return aca_param
-
-    def exchange(
-        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
-    ) -> Optional[UnityOutputProto]:
-        message = UnityMessageProto()
-        message.header.status = 200
-        message.unity_input.CopyFrom(inputs)
-        self.unity_to_external.parent_conn.send(message)
-        self.poll_for_timeout(poll_callback)
-        output = self.unity_to_external.parent_conn.recv()
-        if output.header.status != 200:
-            return None
-        return output.unity_output
-
-    def close(self):
-        """
-        Sends a shutdown signal to the unity environment, and closes the grpc connection.
-        """
-        if self.is_open:
-            message_input = UnityMessageProto()
-            message_input.header.status = 400
-            self.unity_to_external.parent_conn.send(message_input)
-            self.unity_to_external.parent_conn.close()
-            self.server.stop(False)
-            self.is_open = False
+import grpc
+from typing import Optional
+
+from multiprocessing import Pipe
+from sys import platform
+import socket
+import time
+from concurrent.futures import ThreadPoolExecutor
+
+from .communicator import Communicator, PollCallback
+from pyrfuniverse.communicator_objects.unity_to_external_pb2_grpc import (
+    UnityToExternalProtoServicer,
+    add_UnityToExternalProtoServicer_to_server,
+)
+from pyrfuniverse.communicator_objects.unity_message_pb2 import UnityMessageProto
+from pyrfuniverse.communicator_objects.unity_input_pb2 import UnityInputProto
+from pyrfuniverse.communicator_objects.unity_output_pb2 import UnityOutputProto
+from .exception import UnityTimeOutException, UnityWorkerInUseException
+
+
+class UnityToExternalServicerImplementation(UnityToExternalProtoServicer):
+    def __init__(self):
+        self.parent_conn, self.child_conn = Pipe()
+
+    def Initialize(self, request, context):
+        self.child_conn.send(request)
+        return self.child_conn.recv()
+
+    def Exchange(self, request, context):
+        self.child_conn.send(request)
+        return self.child_conn.recv()
+
+
+class RpcCommunicator(Communicator):
+    def __init__(self, worker_id=0, base_port=5005, timeout_wait=30):
+        """
+        Python side of the grpc communication. Python is the server and Unity the client
+
+
+        :int base_port: Baseline port number to connect to Unity environment over. worker_id increments over this.
+        :int worker_id: Offset from base_port. Used for training multiple environments simultaneously.
+        :int timeout_wait: Timeout (in seconds) to wait for a response before exiting.
+        """
+        super().__init__(worker_id, base_port)
+        self.port = base_port + worker_id
+        self.worker_id = worker_id
+        self.timeout_wait = timeout_wait
+        self.server = None
+        self.unity_to_external = None
+        self.is_open = False
+        self.create_server()
+
+    def create_server(self):
+        """
+        Creates the GRPC server.
+        """
+        self.check_port(self.port)
+
+        try:
+            # Establish communication grpc
+            self.server = grpc.server(ThreadPoolExecutor(max_workers=10))
+            self.unity_to_external = UnityToExternalServicerImplementation()
+            add_UnityToExternalProtoServicer_to_server(
+                self.unity_to_external, self.server
+            )
+            # Using unspecified address, which means that grpc is communicating on all IPs
+            # This is so that the docker container can connect.
+            self.server.add_insecure_port("[::]:" + str(self.port))
+            self.server.start()
+            self.is_open = True
+        except Exception:
+            raise UnityWorkerInUseException(self.worker_id)
+
+    def check_port(self, port):
+        """
+        Attempts to bind to the requested communicator port, checking if it is already in use.
+        """
+        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        if platform == "linux" or platform == "linux2":
+            # On linux, the port remains unusable for TIME_WAIT=60 seconds after closing
+            # SO_REUSEADDR frees the port right after closing the environment
+            s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        try:
+            s.bind(("localhost", port))
+        except OSError:
+            raise UnityWorkerInUseException(self.worker_id)
+        finally:
+            s.close()
+
+    def poll_for_timeout(self, poll_callback: Optional[PollCallback] = None) -> None:
+        """
+        Polls the GRPC parent connection for data, to be used before calling recv.  This prevents
+        us from hanging indefinitely in the case where the environment process has died or was not
+        launched.
+
+        Additionally, a callback can be passed to periodically check the state of the environment.
+        This is used to detect the case when the environment dies without cleaning up the connection,
+        so that we can stop sooner and raise a more appropriate error.
+        """
+        deadline = time.monotonic() + self.timeout_wait
+        callback_timeout_wait = self.timeout_wait // 10
+        while time.monotonic() < deadline:
+            if self.unity_to_external.parent_conn.poll(callback_timeout_wait):
+                # Got an acknowledgment from the connection
+                return
+            if poll_callback:
+                # Fire the callback - if it detects something wrong, it should raise an exception.
+                poll_callback()
+
+        # Got this far without reading any data from the connection, so it must be dead.
+        raise UnityTimeOutException(
+            "The Unity environment took too long to respond. Make sure that :\n"
+            "\t The environment does not need user interaction to launch\n"
+            '\t The Agents\' Behavior Parameters > Behavior Type is set to "Default"\n'
+            "\t The environment and the Python interface have compatible versions."
+        )
+
+    def initialize(
+        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
+    ) -> UnityOutputProto:
+        self.poll_for_timeout(poll_callback)
+        aca_param = self.unity_to_external.parent_conn.recv().unity_output
+        message = UnityMessageProto()
+        message.header.status = 200
+        message.unity_input.CopyFrom(inputs)
+        self.unity_to_external.parent_conn.send(message)
+        self.unity_to_external.parent_conn.recv()
+        return aca_param
+
+    def exchange(
+        self, inputs: UnityInputProto, poll_callback: Optional[PollCallback] = None
+    ) -> Optional[UnityOutputProto]:
+        message = UnityMessageProto()
+        message.header.status = 200
+        message.unity_input.CopyFrom(inputs)
+        self.unity_to_external.parent_conn.send(message)
+        self.poll_for_timeout(poll_callback)
+        output = self.unity_to_external.parent_conn.recv()
+        if output.header.status != 200:
+            return None
+        return output.unity_output
+
+    def close(self):
+        """
+        Sends a shutdown signal to the unity environment, and closes the grpc connection.
+        """
+        if self.is_open:
+            message_input = UnityMessageProto()
+            message_input.header.status = 400
+            self.unity_to_external.parent_conn.send(message_input)
+            self.unity_to_external.parent_conn.close()
+            self.server.stop(False)
+            self.is_open = False
```

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/rpc_utils.py` & `pyrfuniverse-0.8.4/pyrfuniverse/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/engine_configuration_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/engine_configuration_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/environment_parameters_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/environment_parameters_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/float_properties_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/float_properties_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/incoming_message.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/incoming_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/outgoing_message.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/raw_bytes_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/raw_bytes_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/side_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/side_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/side_channel_manager.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/side_channel_manager.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/side_channel/stats_side_channel.py` & `pyrfuniverse-0.8.4/pyrfuniverse/side_channel/stats_side_channel.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/active_depth_generate.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/active_depth_generate.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/controller.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/interpolate_utils.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/interpolate_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/jaco_controller.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/jaco_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/kinova_controller.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/kinova_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/os_utils.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/stretch_controller.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/stretch_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/tobor_controller.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/tobor_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse/utils/ur5_controller.py` & `pyrfuniverse-0.8.4/pyrfuniverse/utils/ur5_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/pyrfuniverse.egg-info/SOURCES.txt` & `pyrfuniverse-0.8.4/pyrfuniverse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 pyrfuniverse/attributes/base_attr.py
 pyrfuniverse/attributes/camera_attr.py
 pyrfuniverse/attributes/cloth_attr.py
 pyrfuniverse/attributes/collider_attr.py
 pyrfuniverse/attributes/controller_attr.py
 pyrfuniverse/attributes/custom_attr.py
 pyrfuniverse/attributes/digit_attr.py
+pyrfuniverse/attributes/falling_cloth_attr.py
 pyrfuniverse/attributes/gameobject_attr.py
 pyrfuniverse/attributes/graspsim_attr.py
 pyrfuniverse/attributes/humanbody_attr.py
 pyrfuniverse/attributes/light_attr.py
 pyrfuniverse/attributes/pointcloud_attr.py
 pyrfuniverse/attributes/rigidbody_attr.py
 pyrfuniverse/attributes/softbody_attr.py
@@ -76,14 +77,18 @@
 pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
 pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
 pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
 pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
 pyrfuniverse/envs/multi_agent/__init__.py
 pyrfuniverse/envs/multi_agent/cleaner_env.py
 pyrfuniverse/envs/multi_agent/navigation_env.py
+pyrfuniverse/envs/multi_physics/__init__.py
+pyrfuniverse/envs/multi_physics/flexiv_cutting.py
+pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
+pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
 pyrfuniverse/envs/robotics/__init__.py
 pyrfuniverse/envs/robotics/franka_cloth_env.py
 pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
 pyrfuniverse/envs/robotics/franka_robotics_env.py
 pyrfuniverse/envs/robotics/franka_softbody_env.py
 pyrfuniverse/envs/robotics/pick_and_place_env.py
 pyrfuniverse/envs/robotics/push_env.py
@@ -122,17 +127,19 @@
 pyrfuniverse/utils/rfuniverse_utility.py
 pyrfuniverse/utils/stretch_controller.py
 pyrfuniverse/utils/tobor_controller.py
 pyrfuniverse/utils/ur5_controller.py
 test/test_active_depth.py
 test/test_articulation_ik.py
 test/test_camera_image.py
+test/test_catching_cloth_gym.py
 test/test_custom_message.py
 test/test_debug.py
 test/test_digit.py
+test/test_flexiv_cutting_gym.py
 test/test_grasp_pose.py
 test/test_grasp_sim.py
 test/test_heat_map.py
 test/test_humanbody_ik.py
 test/test_label.py
 test/test_light.py
 test/test_load_mesh.py
@@ -143,8 +150,9 @@
 test/test_pick_and_place_gym.py
 test/test_point_cloud.py
 test/test_point_cloud_render.py
 test/test_point_cloud_with_intrinsic_matrix.py
 test/test_save_gripper.py
 test/test_save_obj.py
 test/test_scene.py
-test/test_tobor_move.py
+test/test_tobor_move.py
+test/test_water_shooting_gym.py
```

### Comparing `pyrfuniverse-0.8.3/setup.py` & `pyrfuniverse-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_active_depth.py` & `pyrfuniverse-0.8.4/test/test_active_depth.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_articulation_ik.py` & `pyrfuniverse-0.8.4/test/test_articulation_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_camera_image.py` & `pyrfuniverse-0.8.4/test/test_camera_image.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_custom_message.py` & `pyrfuniverse-0.8.4/test/test_custom_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 )
 
 env = RFUniverseBaseEnv(
     assets=['CustomAttr']
 )
 
 # asset_channel custom message
-env.ext.CustomMessage(message='this is a asset channel python to unity custom message')
+env.ext.CustomMessage(message='this is asset channel custom message')
 env.step()
 print(env.data['custom_message'])
 
 # instance_channel custom message
 custom = env.InstanceObject(name='CustomAttr', id=123456, attr_type=attr.CustomAttr)
-custom.CustomMessage(message='this is a instance channel python to unity custom message')
+custom.CustomMessage(message='this is instance channel custom message')
 env.step()
 print(custom.data['custom_message'])
 
 # dynamic message
 def dynamic_function(msg: IncomingMessage):
     print(msg.read_string())
     print(msg.read_int32())
@@ -29,15 +29,15 @@
     print(msg.read_float32_list())
 
 
 env.AddListener('DynamicMessage', dynamic_function)
 env.SendMessage(
     'DynamicMessage',
     123456,
-    'this is a python to unity dynamic message',
+    'this is dynamic message',
     True,
     4849.6564,
     [616445.085, 9489984.0, 65419596.0, 9849849.0]
 )
 env.step()
 
 env.Pend()
```

### Comparing `pyrfuniverse-0.8.3/test/test_debug.py` & `pyrfuniverse-0.8.4/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_grasp_pose.py` & `pyrfuniverse-0.8.4/test/test_grasp_pose.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_grasp_sim.py` & `pyrfuniverse-0.8.4/test/test_grasp_sim.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_heat_map.py` & `pyrfuniverse-0.8.4/test/test_heat_map.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_humanbody_ik.py` & `pyrfuniverse-0.8.4/test/test_humanbody_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_label.py` & `pyrfuniverse-0.8.4/test/test_label.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_light.py` & `pyrfuniverse-0.8.4/test/test_light.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_load_mesh.py` & `pyrfuniverse-0.8.4/test/test_load_mesh.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_load_urdf.py` & `pyrfuniverse-0.8.4/test/test_load_urdf.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_object_data.py` & `pyrfuniverse-0.8.4/test/test_object_data.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_pick_and_place.py` & `pyrfuniverse-0.8.4/test/test_pick_and_place.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_pick_and_place_flexiv.py` & `pyrfuniverse-0.8.4/test/test_pick_and_place_flexiv.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_pick_and_place_gym.py` & `pyrfuniverse-0.8.4/test/test_pick_and_place_gym.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_point_cloud.py` & `pyrfuniverse-0.8.4/test/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_point_cloud_with_intrinsic_matrix.py` & `pyrfuniverse-0.8.4/test/test_point_cloud_with_intrinsic_matrix.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import os
-os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-import pyrfuniverse.utils.depth_processor as dp
-import numpy as np
-try:
-    import open3d as o3d
-except ImportError:
-    print('This feature requires open3d, please install with `pip install open3d`')
-    raise
-
-env = RFUniverseBaseEnv(scene_file='PointCloud.json')
-
-intrinsic_matrix = [960, 0, 0, 0, 960, 0, 960, 540, 1]
-nd_intrinsic_matrix = np.reshape(intrinsic_matrix, [3, 3]).T
-
-camera1 = env.GetAttr(698548)
-camera1.GetDepthEXR(intrinsic_matrix=intrinsic_matrix)
-camera1.GetRGB(intrinsic_matrix=intrinsic_matrix)
-camera1.GetID(intrinsic_matrix=intrinsic_matrix)
-env.step()
-
-image_rgb = camera1.data['rgb']
-image_depth_exr = camera1.data['depth_exr']
-local_to_world_matrix = camera1.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
-point1 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_rgb, image_depth_exr, nd_intrinsic_matrix, local_to_world_matrix)
-
-camera2 = env.GetAttr(698550)
-camera2.GetDepthEXR(intrinsic_matrix=intrinsic_matrix)
-camera2.GetRGB(intrinsic_matrix=intrinsic_matrix)
-camera2.GetID(intrinsic_matrix=intrinsic_matrix)
-env.step()
-
-image_rgb = camera2.data['rgb']
-image_depth_exr = camera2.data['depth_exr']
-local_to_world_matrix = camera2.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
-point2 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_rgb, image_depth_exr, nd_intrinsic_matrix, local_to_world_matrix)
-env.close()
-
-# unity space to open3d space and show
-point1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-point2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
-coorninate = o3d.geometry.TriangleMesh.create_coordinate_frame()
-o3d.visualization.draw_geometries([point1, point2, coorninate])
-
+import os
+os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+import pyrfuniverse.utils.depth_processor as dp
+import numpy as np
+try:
+    import open3d as o3d
+except ImportError:
+    print('This feature requires open3d, please install with `pip install open3d`')
+    raise
+
+env = RFUniverseBaseEnv(scene_file='PointCloud.json')
+
+intrinsic_matrix = [960, 0, 0, 0, 960, 0, 960, 540, 1]
+nd_intrinsic_matrix = np.reshape(intrinsic_matrix, [3, 3]).T
+
+camera1 = env.GetAttr(698548)
+camera1.GetDepthEXR(intrinsic_matrix=intrinsic_matrix)
+camera1.GetRGB(intrinsic_matrix=intrinsic_matrix)
+camera1.GetID(intrinsic_matrix=intrinsic_matrix)
+env.step()
+
+image_rgb = camera1.data['rgb']
+image_depth_exr = camera1.data['depth_exr']
+local_to_world_matrix = camera1.data['local_to_world_matrix']
+local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
+point1 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_rgb, image_depth_exr, nd_intrinsic_matrix, local_to_world_matrix)
+
+camera2 = env.GetAttr(698550)
+camera2.GetDepthEXR(intrinsic_matrix=intrinsic_matrix)
+camera2.GetRGB(intrinsic_matrix=intrinsic_matrix)
+camera2.GetID(intrinsic_matrix=intrinsic_matrix)
+env.step()
+
+image_rgb = camera2.data['rgb']
+image_depth_exr = camera2.data['depth_exr']
+local_to_world_matrix = camera2.data['local_to_world_matrix']
+local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
+point2 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_rgb, image_depth_exr, nd_intrinsic_matrix, local_to_world_matrix)
+env.close()
+
+# unity space to open3d space and show
+point1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+point2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
+coorninate = o3d.geometry.TriangleMesh.create_coordinate_frame()
+o3d.visualization.draw_geometries([point1, point2, coorninate])
+
```

### Comparing `pyrfuniverse-0.8.3/test/test_save_gripper.py` & `pyrfuniverse-0.8.4/test/test_save_gripper.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_scene.py` & `pyrfuniverse-0.8.4/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.3/test/test_tobor_move.py` & `pyrfuniverse-0.8.4/test/test_tobor_move.py`

 * *Files identical despite different names*

