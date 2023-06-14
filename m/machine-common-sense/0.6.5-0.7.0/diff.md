# Comparing `tmp/machine_common_sense-0.6.5.tar.gz` & `tmp/machine_common_sense-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/machine_common_sense-0.6.5.tar", last modified: Tue Feb 21 02:14:04 2023, max compression
+gzip compressed data, was "dist/machine_common_sense-0.7.0.tar", last modified: Wed Jun 14 20:55:56 2023, max compression
```

## Comparing `machine_common_sense-0.6.5.tar` & `machine_common_sense-0.7.0.tar`

### file list

```diff
@@ -1,91 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense/
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    24216 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/controller_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/controller_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/controller_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/controller_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/goal_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/history_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/object_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28715 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/return_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scene_history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/cache_addressables.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/config_level1.ini
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/config_level1_debug.ini
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/config_level2.ini
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/config_level2_debug.ini
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/config_no_debug.ini
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/config_oracle.ini
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/config_oracle_debug.ini
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/config_with_debug.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/extract_ground_truth_from_debug_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/getch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_action_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_follow_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_human_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_init_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_interactive_scenes_follow_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_interactive_scenes_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_interactive_scenes_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_just_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_just_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_last_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_passive_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_reorientation_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_scene_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_scene_with_command_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/run_scripts_config_with_history.ini
--rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/scripts/runner_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/step_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/stringifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/machine_common_sense/unity_executable_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/machine_common_sense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 02:14:04.000000 machine_common_sense-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/mock_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    33347 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    37000 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_controller_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    54221 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_controller_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_goal_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_history_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_history_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_object_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    34892 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    48816 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_step_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_stringifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-02-21 02:13:28.000000 machine_common_sense-0.6.5/tests/test_unity_executable_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense/
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25204 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23438 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/controller_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/controller_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/controller_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/controller_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/goal_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/history_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/object_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29076 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/return_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scene_history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/cache_addressables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/change_file_names_to_cell_ids_make_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/config_level1.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/config_level1_debug.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/config_level2.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/config_level2_debug.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/config_no_debug.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/config_oracle.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/config_oracle_debug.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/config_with_debug.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/extract_ground_truth_from_debug_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/getch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_action_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_follow_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_human_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_init_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_interactive_scenes_follow_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_interactive_scenes_last_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_interactive_scenes_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_interactive_scenes_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_just_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_just_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_last_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_passive_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_reorientation_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_scene_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_scene_with_command_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/run_scripts_config_with_history.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/scripts/runner_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/step_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/stringifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/machine_common_sense/unity_executable_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/machine_common_sense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:55:56.000000 machine_common_sense-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/mock_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36197 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37199 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_controller_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54514 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_controller_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_goal_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_history_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_history_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_object_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34888 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48816 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17140 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_step_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_stringifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-14 20:55:15.000000 machine_common_sense-0.7.0/tests/test_unity_executable_provider.py
```

### Comparing `machine_common_sense-0.6.5/LICENSE` & `machine_common_sense-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/PKG-INFO` & `machine_common_sense-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: machine_common_sense
-Version: 0.6.5
+Version: 0.7.0
 Summary: Machine Common Sense Python API to Unity 3D Simulation Environment
 Home-page: https://github.com/NextCenturyCorporation/MCS/
 Maintainer: Next Century, a wholly owned subsidiary of CACI
 Maintainer-email: mcs-ta2@machinecommonsense.com
 License: Apache-2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Typing :: Typed
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version fury.io](https://badge.fury.io/py/machine-common-sense.svg)](https://pypi.python.org/pypi/machine-common-sense/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/machine-common-sense.svg)](https://pypi.python.org/pypi/machine-common-sense/)
 [![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
@@ -42,15 +43,15 @@
 
 Publish Documentation: [![Publish Docs](https://github.com/NextCenturyCorporation/MCS/actions/workflows/docs-publish.yaml/badge.svg)](https://github.com/NextCenturyCorporation/MCS/actions/workflows/docs-publish.yaml)
 
 Publish to PyPI: [![Publish PyPI](https://github.com/NextCenturyCorporation/MCS/actions/workflows/pypi-publish.yaml/badge.svg)](https://github.com/NextCenturyCorporation/MCS/actions/workflows/pypi-publish.yaml)
 
 # MCS Python Package
 
-Python interface for interacting with MCS AI2Thor environment and running scenes. The latest release of the MCS Python library is `0.6.5`. You can find the latest documentation [here](https://nextcenturycorporation.github.io/MCS).
+Python interface for interacting with MCS AI2Thor environment and running scenes. The latest release of the MCS Python library is `0.7.0`. You can find the latest documentation [here](https://nextcenturycorporation.github.io/MCS).
 
 - [Quickstart Installation](#quickstart-installation)
 - [Usage](#usage)
 - [Documentation](#documentation)
 - [Other MCS GitHub Repositories](#other-mcs-github-repositories)
 - [Troubleshooting/Email](#troubleshooting)
 - [License](#apache-2-open-source-license)
```

### Comparing `machine_common_sense-0.6.5/README.md` & `machine_common_sense-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Publish Documentation: [![Publish Docs](https://github.com/NextCenturyCorporation/MCS/actions/workflows/docs-publish.yaml/badge.svg)](https://github.com/NextCenturyCorporation/MCS/actions/workflows/docs-publish.yaml)
 
 Publish to PyPI: [![Publish PyPI](https://github.com/NextCenturyCorporation/MCS/actions/workflows/pypi-publish.yaml/badge.svg)](https://github.com/NextCenturyCorporation/MCS/actions/workflows/pypi-publish.yaml)
 
 # MCS Python Package
 
-Python interface for interacting with MCS AI2Thor environment and running scenes. The latest release of the MCS Python library is `0.6.5`. You can find the latest documentation [here](https://nextcenturycorporation.github.io/MCS).
+Python interface for interacting with MCS AI2Thor environment and running scenes. The latest release of the MCS Python library is `0.7.0`. You can find the latest documentation [here](https://nextcenturycorporation.github.io/MCS).
 
 - [Quickstart Installation](#quickstart-installation)
 - [Usage](#usage)
 - [Documentation](#documentation)
 - [Other MCS GitHub Repositories](#other-mcs-github-repositories)
 - [Troubleshooting/Email](#troubleshooting)
 - [License](#apache-2-open-source-license)
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/__init__.py` & `machine_common_sense-0.7.0/machine_common_sense/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,33 +26,29 @@
 from .subscriber import add_subscribers
 from .unity_executable_provider import UnityExecutableProvider
 
 logger = logging.getLogger(__name__)
 # Set default logging handler to avoid "No handler found" warnings
 logger.addHandler(logging.NullHandler())
 
-# Timeout at 3 minutes (180 seconds).  It was 60 seconds but
-# this can cause timeouts on EC2 instances
-TIME_LIMIT_SECONDS = 180
-
 
 def get_controller(unity_exec: str, config: ConfigManager):
     """Function to get the controller, pulled into its own
      function so we can time it.  """
     controller = Controller(unity_exec, config)
     return controller
 
 
 def get_controller_with_timeout(unity_exec: str, config: ConfigManager):
     """Wrapper function that sets a timeout for the controller creation.
     If getting the controller times out, None is returned. """
     with concurrent.futures.ThreadPoolExecutor(max_workers=2) as executor:
         future = executor.submit(get_controller, unity_exec, config)
         try:
-            controller = future.result(timeout=TIME_LIMIT_SECONDS)
+            controller = future.result(timeout=config.get_controller_timeout())
             return controller
         except concurrent.futures.TimeoutError as Msg:
             logger.error("Timeout error in creating controller", exc_info=Msg)
 
             # TODO:  Add checks to continue waiting for the controller creation.
             return None
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/action.py` & `machine_common_sense-0.7.0/machine_common_sense/action.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/config_manager.py` & `machine_common_sense-0.7.0/machine_common_sense/config_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -303,52 +303,65 @@
     can_contain_target: Optional[bool]
     obstacle: Optional[bool]
     occluder: Optional[bool]
     position_y: Optional[float]
     stack_target: Optional[bool]
 
 
+class TerminalOutputMode(Enum):
+    ACTIONS = 'actions'
+    MINIMAL = 'minimal'
+    OBJECTS = 'objects'
+    PERFORMER = 'performer'
+    SCENE = 'scene'
+
+
 class ConfigManager:
 
     DEFAULT_ROOM_DIMENSIONS = Vector3d(x=10, y=3, z=10)
     CONFIG_FILE_ENV_VAR = 'MCS_CONFIG_FILE_PATH'
     CONFIG_DEFAULT_SECTION = 'MCS'
     CONFIG_DISABLE_DEPTH_MAPS = 'disable_depth_maps'
     CONFIG_DISABLE_OBJECT_MASKS = 'disable_object_masks'
-    CONFIG_ONLY_RETURN_GOAL_OBJECT = 'only_return_goal_object'
     CONFIG_DISABLE_POSITION = 'disable_position'
     CONFIG_EVALUATION_NAME = 'evaluation_name'
+    CONFIG_GOAL_REWARD = 'goal_reward'
     CONFIG_HISTORY_ENABLED = 'history_enabled'
+    CONFIG_LAVA_PENALTY = 'lava_penalty'
     CONFIG_METADATA_TIER = 'metadata'
     CONFIG_NOISE_ENABLED = 'noise_enabled'
+    CONFIG_ONLY_RETURN_GOAL_OBJECT = 'only_return_goal_object'
     CONFIG_SAVE_DEBUG_IMAGES = 'save_debug_images'
     CONFIG_SAVE_DEBUG_JSON = 'save_debug_json'
     CONFIG_SIZE = 'size'
-    CONFIG_TEAM = 'team'
-    CONFIG_VIDEO_ENABLED = 'video_enabled'
-    CONFIG_LAVA_PENALTY = 'lava_penalty'
-    CONFIG_STEPS_ALLOWED_IN_LAVA = 'steps_allowed_in_lava'
     CONFIG_STEP_PENALTY = 'step_penalty'
-    CONFIG_GOAL_REWARD = 'goal_reward'
+    CONFIG_STEPS_ALLOWED_IN_LAVA = 'steps_allowed_in_lava'
+    CONFIG_TEAM = 'team'
+    CONFIG_TERMINAL_OUTPUT = 'terminal_output'
+    CONFIG_TIMEOUT = 'timeout'
     CONFIG_TOP_DOWN_PLOTTER = 'top_down_plotter'
     CONFIG_TOP_DOWN_CAMERA = 'top_down_camera'
-    CONFIG_TIMEOUT = 'timeout'
+    CONFIG_CONTROLLER_TIMEOUT = 'controller_timeout'
+    CONFIG_VIDEO_ENABLED = 'video_enabled'
 
     # Please keep the aspect ratio as 3:2 because the IntPhys scenes are built
     # on this assumption.
     SCREEN_WIDTH_DEFAULT = 600
     SCREEN_WIDTH_MIN = 450
 
     # Default steps allowed in lava before calling end scene
     STEPS_ALLOWED_IN_LAVA_DEFAULT = 0
 
     # Default time to allow on a single step before timing out
     # is 1 hour (represented in seconds)
     TIMEOUT_DEFAULT = 3600
 
+    # Default time for initalizing a controller.
+    CONTROLLER_TIMEOUT_DEFAULT = 180
+
     def __init__(self, config_file_or_dict=None):
         '''
         Configuration preferences passed in by the user.
         '''
         self._config = configparser.ConfigParser()
 
         # For config, look for environment variable first,
@@ -429,14 +442,42 @@
     def get_team(self):
         return self._config.get(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_TEAM,
             fallback=''
         )
 
+    def get_terminal_output_mode(self) -> List[TerminalOutputMode]:
+        try:
+            # If mode is boolean, return all or nothing.
+            terminal_output_mode = self._config.getboolean(
+                self.CONFIG_DEFAULT_SECTION,
+                self.CONFIG_TERMINAL_OUTPUT,
+                fallback=True
+            )
+            if terminal_output_mode:
+                return [mode for mode in TerminalOutputMode]
+            return []
+        except ValueError:
+            # If mode is string, assume comma separated list.
+            terminal_output_mode = self._config.get(
+                self.CONFIG_DEFAULT_SECTION,
+                self.CONFIG_TERMINAL_OUTPUT,
+                fallback=True
+            )
+            if not terminal_output_mode:
+                return []
+            inputs = terminal_output_mode.split(',')
+            if 'all' in inputs or 'ALL' in inputs:
+                return [mode for mode in TerminalOutputMode]
+            return [
+                mode for mode in TerminalOutputMode
+                if mode.value in inputs or mode.value.upper() in inputs
+            ]
+
     def is_history_enabled(self):
         return self._config.getboolean(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_HISTORY_ENABLED,
             fallback=True
         )
 
@@ -465,79 +506,40 @@
         return self._config.getboolean(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_VIDEO_ENABLED,
             fallback=False
         )
 
     def is_depth_maps_enabled(self) -> bool:
-        metadata_tier = self.get_metadata_tier()
-
-        allowed_by_config = not self._config.getboolean(
+        return not self._config.getboolean(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_DISABLE_DEPTH_MAPS,
             fallback=False
         )
-        allowed_by_metadata_tier = metadata_tier in [
-            MetadataTier.LEVEL_1,
-            MetadataTier.LEVEL_2,
-            MetadataTier.ORACLE,
-        ]
-        if allowed_by_metadata_tier and allowed_by_config:
-            return True
-        else:
-            return False
 
     def is_only_return_object_goal(self) -> bool:
-        metadata_tier = self.get_metadata_tier()
-        allowed_by_config = self._config.getboolean(
+        return self._config.getboolean(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_ONLY_RETURN_GOAL_OBJECT,
             fallback=False
         )
-        allowed_by_metadata_tier = metadata_tier in [
-            MetadataTier.ORACLE
-        ]
-        if allowed_by_metadata_tier and allowed_by_config:
-            return True
-        else:
-            return False
 
     def is_position_disabled(self) -> bool:
-        metadata_tier = self.get_metadata_tier()
-        allowed_by_config = not self._config.getboolean(
+        return self._config.getboolean(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_DISABLE_POSITION,
             fallback=False
         )
-        allowed_by_metadata_tier = metadata_tier in [
-            MetadataTier.ORACLE
-        ]
-
-        if allowed_by_metadata_tier and allowed_by_config:
-            return False
-        else:
-            return True
 
     def is_object_masks_enabled(self) -> bool:
-        metadata_tier = self.get_metadata_tier()
-        allowed_by_config = not self._config.getboolean(
+        return not self._config.getboolean(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_DISABLE_OBJECT_MASKS,
             fallback=False
         )
-        allowed_by_metadata_tier = (metadata_tier != MetadataTier.LEVEL_1 and
-                                    metadata_tier in
-                                    [
-                                        MetadataTier.LEVEL_2,
-                                        MetadataTier.ORACLE,
-                                    ])
-        if allowed_by_metadata_tier and allowed_by_config:
-            return True
-        else:
-            return False
 
     def get_screen_size(self) -> Tuple[int, int]:
         return (self.get_screen_width(), self.get_screen_height())
 
     def get_screen_width(self) -> int:
         return self.get_size()
 
@@ -569,23 +571,50 @@
     def get_steps_allowed_in_lava(self):
         return self._config.getint(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_STEPS_ALLOWED_IN_LAVA,
             fallback=self.STEPS_ALLOWED_IN_LAVA_DEFAULT
         )
 
+    def get_controller_timeout(self):
+        """ Time (in seconds) to allow a run to be idle
+        before attempting to end scene"""
+        return self._config.getint(
+            self.CONFIG_DEFAULT_SECTION,
+            self.CONFIG_CONTROLLER_TIMEOUT,
+            fallback=self.CONTROLLER_TIMEOUT_DEFAULT
+        )
+
+    def set_controller_timeout(self, seconds):
+        """ Time (in seconds) to allow a controller to initialization
+        before attempting to end scene"""
+        return self._config.set(
+            self.CONFIG_DEFAULT_SECTION,
+            self.CONFIG_CONTROLLER_TIMEOUT,
+            seconds
+        )
+
     def get_timeout(self):
         """ Time (in seconds) to allow a run to be idle
         before attempting to end scene"""
         return self._config.getint(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_TIMEOUT,
             fallback=self.TIMEOUT_DEFAULT
         )
 
+    def set_timeout(self, seconds):
+        """ Setting the time (in seconds) to allow a run to be idle
+        before attempting to end scene"""
+        return self._config.set(
+            self.CONFIG_DEFAULT_SECTION,
+            self.CONFIG_TIMEOUT,
+            seconds
+        )
+
     def is_top_down_plotter(self) -> bool:
         """Toggles whether old plotter should be used to create top down
         videos if videos are enabled."""
         return self._config.getboolean(
             self.CONFIG_DEFAULT_SECTION,
             self.CONFIG_TOP_DOWN_PLOTTER,
             fallback=False
@@ -692,14 +721,15 @@
     def retrieve_goal(self, steps_allowed_in_lava=0):
         if not self.goal:
             return self.update_goal_target_image(GoalMetadata(
                 steps_allowed_in_lava=steps_allowed_in_lava
             ))
 
         goal = self.goal
+        goal.metadata = goal.metadata or {}
 
         # Transform action list data from strings to tuples.
         action_list = goal.action_list or []
         for index, action_list_at_step in enumerate(action_list):
             action_list[index] = [
                 Action.input_to_action_and_params(action)
                 if isinstance(action, str) else action
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/controller.py` & `machine_common_sense-0.7.0/machine_common_sense/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,31 +147,32 @@
         '''Meant for use during eval, if a scene is hung on the same step
         for a period of time, end the scene.'''
 
         start_time = time.time()
         self._timer_in_progress = False
         timeout_seconds = self._config.get_timeout()
 
-        if(self._last_step_check < self.__step_number):
+        if (self._last_step_check < self.__step_number):
             # skip step check for Initialize step
-            if(self.__step_number != 0):
+            if (self.__step_number != 0):
                 self._last_step_check = self.__step_number
 
             timer_seconds = timeout_seconds - \
                 ((time.time() - start_time) % timeout_seconds)
             self._timer = threading.Timer(timer_seconds,
                                           self._check_step_for_timeout)
             self._timer.daemon = True
             self._timer.start()
             self._timer_in_progress = True
         else:
             time_str = str(datetime.timedelta(seconds=timeout_seconds))
-            logger.debug(
+            logger.warning(
                 f"Attempting to end scene due to inactivity (user not taking"
-                f" any steps) for {time_str} (hh:mm:ss)")
+                f" any steps). Currently this polls for step progress "
+                f"every {time_str} (hh:mm:ss)")
             self.end_scene(rating=None, score=-1)
 
             _thread.interrupt_main()
 
     @typeguard.typechecked
     def start_scene(
         self, config_data: Union[SceneConfiguration, Dict]) \
@@ -269,19 +270,17 @@
 
                 logger.debug('ENDING PREVIEW PHASE')
 
                 output.image_list = image_list
                 output.depth_map_list = depth_map_list
                 output.object_mask_list = object_mask_list
 
-            logger.debug('NO PREVIEW PHASE')
-
             # TODO Should this be in the if block?  Now that we are using
             # subscribers, we may want to always register
-            if(self._failure_handler_registered is False and
+            if (self._failure_handler_registered is False and
                     self._config.is_history_enabled()):
                 # make sure history file is written when program exits
                 atexit.register(self.end_scene, rating=None, score=-1)
                 self._failure_handler_registered = True
 
         payload = self._create_post_step_event_payload_kwargs(
             ai2thor_step, step_output, pre_restrict_output, output)
@@ -294,16 +293,15 @@
         return output
 
     def _convert_scene_config(self, config_data) -> SceneConfiguration:
         if isinstance(config_data, SceneConfiguration):
             return config_data
         return SceneConfiguration(**config_data)
 
-    @typeguard.typechecked
-    def step(self, action: str, **kwargs) -> Optional[StepMetadata]:
+    def step(self, action: str, **kwargs: str) -> Optional[StepMetadata]:
         """
         Runs the given action within the current scene.
 
         Parameters
         ----------
         action : string
             A selected action string from the list of available actions.
@@ -500,15 +498,15 @@
                         "internal_state": {"test": "some state"}
 
                     }
 
             }
 
         """
-        if(not self._end_scene_called):
+        if (not self._end_scene_called):
             payload = self._create_event_payload_kwargs()
             payload['rating'] = rating
             payload['score'] = score
             payload['report'] = report
 
             self._publish_event(
                 EventType.ON_END_SCENE,
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/controller_events.py` & `machine_common_sense-0.7.0/machine_common_sense/controller_events.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/controller_media.py` & `machine_common_sense-0.7.0/machine_common_sense/controller_media.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/controller_output_handler.py` & `machine_common_sense-0.7.0/machine_common_sense/controller_output_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,16 +319,17 @@
                 None if restrict_non_oracle else
                 self._scene_config.retrieve_lava()
             ),
             object_list=(
                 [] if restrict_non_oracle else self._scene_event.object_list),
             object_mask_list=([] if restrict_object_mask_list else
                               self._scene_event.object_mask_list),
-            position=(
-                None if restrict_non_oracle else self._scene_event.position),
+            position=(None if (
+                restrict_non_oracle or self._config.is_position_disabled()
+            ) else self._scene_event.position),
             performer_radius=self._scene_event.performer_radius,
             performer_reach=self._scene_event.performer_reach,
             return_status=self._scene_event.return_status,
             reward=Reward.calculate_reward(
                 goal, self._scene_event.objects, self._scene_event.agent,
                 self._step_number, self._scene_event.performer_reach,
                 self._scene_event.steps_on_lava,
@@ -358,14 +359,16 @@
                 self._scene_event.physics_frames_per_second),
             structural_object_list=([] if restrict_non_oracle else
                                     self._scene_event.structural_object_list)
         )
 
         if (restrict_non_oracle):
             self.filter_step_output(step_output)
+        elif self._config.is_position_disabled():
+            step_output.position = None
 
         return step_output
 
     def get_restrictions(self, restricted, metadata_tier) -> Tuple:
         restrict_depth_map = (
             restricted and
             metadata_tier == MetadataTier.NONE
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/goal_metadata.py` & `machine_common_sense-0.7.0/machine_common_sense/goal_metadata.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/history_writer.py` & `machine_common_sense-0.7.0/machine_common_sense/history_writer.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/logging_config.py` & `machine_common_sense-0.7.0/machine_common_sense/logging_config.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/material.py` & `machine_common_sense-0.7.0/machine_common_sense/material.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/object_metadata.py` & `machine_common_sense-0.7.0/machine_common_sense/object_metadata.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/parameter.py` & `machine_common_sense-0.7.0/machine_common_sense/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,17 +374,17 @@
             self.OBJECT_IMAGE_COORDS_Y_KEY,
             self.DEFAULT_IMG_COORD,
             "objectId",
             **kwargs
         )
 
     def _validate_and_convert_params(self, **kwargs) -> Tuple[Action, Dict]:
-        """Need a validation/conversion step for what ai2thor will accept as input
-        to keep parameters more simple for the user (in this case, wrapping
-        rotation degrees into an object)
+        """Need a validation/conversion step for what ai2thor will accept as
+        input to keep parameters more simple for the user (in this case,
+        wrapping rotation degrees into an object)
         """
         action = Action(kwargs.get('action'))
         kwargs.pop('action')
         amount = self._get_amount(action, **kwargs)
         force = self._get_force(action, **kwargs)
 
         # TODO Consider the current "head tilt" value while validating the
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/plotter.py` & `machine_common_sense-0.7.0/machine_common_sense/plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -300,15 +300,17 @@
         '''Draw a vertical grid line corresponding to the x-coordinate'''
         img_x = int(self.image_center.x + x_coord * self.scale.x)
         rr, cc = skimage.draw.line(
             c0=img_x,
             r0=int(buffer_y),
             c1=img_x,
             r1=img.shape[0] - 1 - int(buffer_y))
-        img[rr, cc] = self.CENTER_COLOR if x_coord == 0 else self.GRID_COLOR
+        img[rr, cc] = np.array(
+            self.CENTER_COLOR if x_coord == 0 else self.GRID_COLOR
+        ).astype(np.int8)
         return img
 
     def _draw_horizontal_grid_lines(
             self, img: np.ndarray, buffer_x: int) -> np.ndarray:
         '''Draw horizontal lines at each y-coordinate'''
         z_units = math.floor(self._room_size.z / 2)
         # draw horizontal grid lines starting at the center and working out
@@ -322,27 +324,29 @@
         '''Draw a horizontal grid line corresponding to the y-coordinate'''
         img_y = int(self.image_center.y + y_coord * self.scale.y)
         rr, cc = skimage.draw.line(
             c0=int(buffer_x),
             r0=img_y,
             c1=img.shape[1] - 1 - int(buffer_x),
             r1=img_y)
-        img[rr, cc] = self.CENTER_COLOR if y_coord == 0 else self.GRID_COLOR
+        img[rr, cc] = np.array(
+            self.CENTER_COLOR if y_coord == 0 else self.GRID_COLOR
+        ).astype(np.int8)
         return img
 
     def _draw_room_border(self, img: np.ndarray,
                           buffer: ImageCoord) -> np.ndarray:
         '''Outline the room border'''
         x_dim, z_dim, _ = img.shape
         rr, cc = skimage.draw.rectangle_perimeter(
             start=(buffer.y, buffer.x),
             end=(z_dim - buffer.y - 1, x_dim - buffer.x - 1),
             shape=img.shape[:2],
             clip=True)
-        img[rr, cc] = self.BORDER_COLOR
+        img[rr, cc] = np.array(self.BORDER_COLOR).astype(np.int8)
         return img
 
     def _out_of_bounds(
             self, pos: SceneCoord, room_dim: Vector3d) -> bool:
         x_odd_reducer = 0 if room_dim.x % 2 == 0 else 1
         z_odd_reducer = 0 if room_dim.z % 2 == 0 else 1
         return (abs(pos.x) > (room_dim.x - x_odd_reducer) /
@@ -458,15 +462,15 @@
         lower_right: ImageCoord,
         texture_color: colour.C_RGB
     ) -> np.ndarray:
         rr, cc = skimage.draw.rectangle(
             start=(upper_left.y, upper_left.x),
             end=(lower_right.y, lower_right.x),
             shape=img.shape[:2])
-        img[rr, cc] = texture_color
+        img[rr, cc] = np.array(texture_color).astype(np.int8)
         return img
 
     def _draw_holes(self, img: np.ndarray, holes: List,
                     room_dim: Vector3d = Vector3d(x=10, y=0, z=10
                                                   )) -> np.ndarray:
         '''Draw a box with an X to illustrate a floor hole'''
         if holes is None:
@@ -514,36 +518,36 @@
             color: Tuple) -> np.ndarray:
         '''Outline the floor hole'''
         rr, cc = skimage.draw.rectangle_perimeter(
             start=(upper_left.y - 1, upper_left.x + 1),
             end=(lower_right.y + 1, lower_right.x - 1),
             shape=img.shape[:2],
             clip=True)
-        img[rr, cc] = color
+        img[rr, cc] = np.array(color).astype(np.int8)
         return img
 
     def _draw_x(
             self,
             img: np.ndarray,
             upper_left: ImageCoord,
             lower_right: ImageCoord,
             color: Tuple) -> np.ndarray:
         rr, cc = skimage.draw.line(
             r0=upper_left.y,
             c0=upper_left.x,
             r1=lower_right.y,
             c1=lower_right.x)
-        img[rr, cc] = color
+        img[rr, cc] = np.array(color).astype(np.int8)
 
         rr, cc = skimage.draw.line(
             r0=lower_right.y,
             c0=upper_left.x,
             r1=upper_left.y,
             c1=lower_right.x)
-        img[rr, cc] = color
+        img[rr, cc] = np.array(color).astype(np.int8)
         return img
 
     def _export_plot(self, img: np.ndarray) -> PIL.Image.Image:
         '''Export the plot to a PIL Image'''
         return PIL.Image.fromarray(img, "RGB")
 
     def _draw_robot(self, img: np.ndarray, robot_metadata: Dict) -> np.ndarray:
@@ -599,15 +603,15 @@
         for polygon, color in [
             (outer, opposite_color),
             (inner, self.ROBOT_COLOR)
         ]:
             points = list(polygon.exterior.coords)
             cs, rs = self._convert_points(points)
             rr, cc = skimage.draw.polygon(rs, cs, shape=img.shape[:2])
-            img[rr, cc] = color
+            img[rr, cc] = np.array(color).astype(np.int8)
         return img
 
     def _find_plottable_objects(
             self, scene_event: ai2thor.server.Event) -> List:
         '''Find plottable objects from the scene data.
 
         Plottable objects include normal scene objects as well as
@@ -711,19 +715,19 @@
             if not obj.visible:
                 clr = self.BACKGROUND_COLOR
         else:
             rr, cc = skimage.draw.polygon_perimeter(
                 rs,
                 cs,
                 shape=img.shape[:2])
-        img[rr, cc] = clr
+        img[rr, cc] = np.array(clr).astype(np.int8)
 
         # using ramp string prefix assumpation to make ramp determination
         # might be better to have an attribute to leverage
-        if(obj.uuid.startswith('ramp')):
+        if (obj.uuid.startswith('ramp')):
             self._draw_ramp_arrow(img, obj, clr)
 
         return img
 
     def _draw_ramp_arrow(self, img: np.ndarray, obj: SceneAsset,
                          ramp_color: Tuple) -> np.ndarray:
         # convert scene object to a ramp
@@ -744,15 +748,17 @@
                 c0=peak_pt.x,
                 r1=img_pt.y,
                 c1=img_pt.x)
             arrow_color = (
                 self.BACKGROUND_COLOR if ramp_color != self.BACKGROUND_COLOR
                 else self.DEFAULT_COLOR
             )
-            img[rr, cc] = arrow_color if ramp.visible else ramp_color
+            img[rr, cc] = np.array(
+                arrow_color if ramp.visible else ramp_color
+            ).astype(np.int8)
         return img
 
     def _draw_goal(self, img: np.ndarray,
                    obj: SceneAsset) -> np.ndarray:
         '''Draw the goal object of the scene'''
         obj_pts = [(pt.x, pt.z) for pt in obj.bounds.points]
         polygon = geometry.MultiPoint(
@@ -769,15 +775,15 @@
             opposite_color = self.DEFAULT_GOAL_COLOR
 
         cs, rs = self._convert_points(pts)
 
         # Draw a correctly-sized polygon with the opposite of the goal's color.
         # This will create a thick border around the 2nd polygon (see below).
         rr, cc = skimage.draw.polygon(rs, cs, shape=img.shape[:2])
-        img[rr, cc] = opposite_color
+        img[rr, cc] = np.array(opposite_color).astype(np.int8)
 
         # Then draw a smaller polygon on top of the 1st polygon in its middle.
         return self._draw_object(img, obj, is_goal=True)
 
     def _find_opposite_color(self, color: tuple) -> tuple:
         '''Return the exact opposite of the given color.'''
         return (255 - color[0], 255 - color[1], 255 - color[2])
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/recorder.py` & `machine_common_sense-0.7.0/machine_common_sense/recorder.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/return_status.py` & `machine_common_sense-0.7.0/machine_common_sense/return_status.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/reward.py` & `machine_common_sense-0.7.0/machine_common_sense/reward.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,30 +72,38 @@
         '''
         reward = GOAL_NOT_ACHIEVED
         goal_objects = []
 
         metadata = goal.metadata or {}
         # Different goal categories may use different property names
         target_names = ['target', 'targets']
+        # Get the total number of targets.
+        pickup_number = metadata.get('pickup_number') or 0
         for target_name in target_names:
             # Some properties may be dicts, and some may be lists of dicts
             targets = metadata.get(target_name) or []
             targets = targets if isinstance(targets, list) else [targets]
+            # If pickup_number was not defined, use the list's length.
+            if not pickup_number:
+                pickup_number = len(targets)
             for target in targets:
                 goal_id = target.get('id')
                 goal_object = Reward.__get_object_from_list(objects, goal_id)
                 if goal_object:
                     goal_objects.append(goal_object)
 
-        # Only attain the reward if all targets are picked up
-        if goal_objects and all(
-                [obj.get('isPickedUp', False) for obj in goal_objects]):
+        picked_up = len([
+            object_metadata for object_metadata in goal_objects
+            if object_metadata.get('wasPickedUp')
+        ])
+        # Attain the reward if the required number of targets were picked-up.
+        if goal_objects and pickup_number and picked_up >= pickup_number:
             reward = goal_reward
 
-        return reward
+        return round(reward, 4)
 
     @staticmethod
     def _adjust_score_penalty(
             current_score: int,
             number_steps: int,
             steps_on_lava: int,
             lava_penalty: float = LAVA_PENALTY,
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scene_history.py` & `machine_common_sense-0.7.0/machine_common_sense/scene_history.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,14 @@
         yield 'action', self.action
         yield 'args', self.args
         yield 'params', self.params
         yield 'classification', self.classification
         yield 'confidence', self.confidence
         yield 'violations_xy_list', self.violations_xy_list
         yield 'internal_state', self.internal_state
-        yield 'output', dict(self.output) if(
+        yield 'output', dict(self.output) if (
             self.output) is not None else self.output
         yield 'delta_time_millis', self.delta_time_millis
         yield 'target_visible', self.target_visible
         if self.target_is_visible_at_start is not None:
             yield 'target_is_visible_at_start', (
                 self.target_is_visible_at_start)
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/cache_addressables.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/cache_addressables.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/extract_ground_truth_from_debug_files.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/extract_ground_truth_from_debug_files.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/getch_helper.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/getch_helper.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_action_file.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_action_file.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_follow_path.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_follow_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 from machine_common_sense.logging_config import LoggingConfig
 from machine_common_sense.scripts.run_interactive_scenes_follow_path import \
     PathFollower
 
 commands = []
 
 
+"""
+Must be run at oracle metadata level on debug scene(s) with a "path" section.
+"""
+
+
 def parse_args():
     parser = argparse.ArgumentParser(description='Run MCS')
     parser.add_argument(
         'mcs_scene_json_file',
         help='MCS JSON scene configuration file to load')
     parser.add_argument(
         '--mcs_unity_build_file',
@@ -34,15 +39,15 @@
         'save history files properties.')
     return parser.parse_args()
 
 
 path_follower = PathFollower()
 
 
-def run_scene(controller: Controller, scene_data, path):
+def run_scene(controller: Controller, scene_data):
 
     print("Resetting the current scene...")
     output = controller.start_scene(scene_data)
 
     action = 'start'
     while True:
         action, params = path_follower.action_callback(
@@ -55,31 +60,26 @@
 
 
 def main():
     mcs.init_logging(LoggingConfig.get_dev_logging_config())
     args = parse_args()
     scene_data = mcs.load_scene_json_file(args.mcs_scene_json_file)
 
-    path = scene_data.get('debug', {}).get('path')
-    if not path:
-        print("Scene did not have 'debug.path' section")
-        return
-
     controller = mcs.create_controller(
         unity_app_file_path=args.mcs_unity_build_file,
         config_file_or_dict=args.config_file_path,
         unity_cache_version=args.mcs_unity_version)
 
     path_follower.init_callback(controller)
 
     scene_file_path = args.mcs_scene_json_file
     scene_file_name = scene_file_path[scene_file_path.rfind('/') + 1:]
 
     if 'name' not in scene_data.keys():
         scene_data['name'] = scene_file_name[0:scene_file_name.find('.')]
 
     if controller is not None:
-        run_scene(controller, scene_data, path)
+        run_scene(controller, scene_data)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_human_input.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_human_input.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_init_scenes.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_init_scenes.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_just_rotate.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_just_rotate.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_last_action.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_passive_scenes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from runner_script import SingleFileRunnerScript
+from runner_script import MultipleFileRunnerScript
 
 
 def action_callback(scene_data, step_metadata, runner_script):
     last_step = 60
     if (
         'goal' in scene_data.keys(
         ) and 'last_step' in scene_data['goal'].keys()
@@ -14,12 +14,12 @@
             if len(step_metadata.action_list) else (None, None)
         )
         return action, params
     return None, None
 
 
 def main():
-    SingleFileRunnerScript('Last Action', action_callback)
+    MultipleFileRunnerScript('Passive Scenes', action_callback)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_reorientation_scenes.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_reorientation_scenes.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_scene_timer.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_scene_timer.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/run_scene_with_command_file.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/run_scene_with_command_file.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/scripts/runner_script.py` & `machine_common_sense-0.7.0/machine_common_sense/scripts/runner_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from machine_common_sense.controller import Controller
 
 logger = logging.getLogger('machine_common_sense')
 mcs.LoggingConfig.init_logging(mcs.LoggingConfig.get_dev_logging_config())
 
 
 SCRIPT_FOLDER = os.path.dirname(os.path.abspath(__file__))
-BLACK_IMAGE_PATH = SCRIPT_FOLDER + '/black_image.png'
 
 
 class AbstractRunnerScript():
     def __init__(
         self,
         name: str,
         action_callback: Callable[
@@ -26,15 +25,15 @@
             Tuple[str, Dict]
         ],
         init_callback: Callable[[Controller], None] = None
     ):
         self._name = name
         args, filenames = self._read_args()
         if not len(filenames):
-            print('No matching files found... Exiting')
+            logger.debug('No matching files found... Exiting')
             exit()
         self.args = args
 
         debug = (args.save_videos or args.save_gifs or args.debug)
         config_suffix = 'with_debug' if debug else 'no_debug'
         if args.level1:
             config_suffix = 'level1_debug' if debug else 'level1'
@@ -44,46 +43,33 @@
             config_suffix = 'oracle_debug' if debug else 'oracle'
 
         config_file_path = (
             args.config_file or
             SCRIPT_FOLDER + '/config_' + config_suffix + '.ini'
         )
 
-        print('========================================')
+        logger.debug('+' * 79)
         controller = mcs.create_controller(
             unity_app_file_path=args.mcs_unity_build_file,
             unity_cache_version=args.mcs_unity_version,
             config_file_or_dict=config_file_path
         )
 
         if init_callback is not None:
             init_callback(controller)
 
         for filename in filenames:
-            print('Starting next scene timer')
-            begin_time = time.perf_counter()
             scene_name = self.run_scene(
                 controller,
                 filename,
                 action_callback,
                 args.last_step,
                 args.prefix,
                 args.rename
             )
-            end_time = time.perf_counter()
-            time_diff = end_time - begin_time
-            print(f'{scene_name} scene timer: {time_diff:0.4f} seconds')
-            if args.save_videos or args.save_gifs:
-                # Copy the black image into the debug folder as the last frame.
-                frame_image_list = glob.glob(scene_name + '/frame_image_*')
-                frame_count = len(frame_image_list)
-                black_frame = (
-                    scene_name + '/frame_image_' + str(frame_count) + '.png'
-                )
-                subprocess.call(['cp', BLACK_IMAGE_PATH, black_frame])
             if args.save_videos:
                 subprocess.call([
                     'ffmpeg', '-y', '-r', '20', '-i',
                     scene_name + '/frame_image_%d.png',
                     '-vcodec', 'h264', '-vf', 'format=yuv420p',
                     scene_name + '.mp4'
                 ])
@@ -224,20 +210,30 @@
 
         # Override the scene name.
         scene_data['name'] = scene_name
 
         step_metadata = controller.start_scene(scene_data)
         action, params = action_callback(scene_data, step_metadata, self)
 
+        logger.debug(f'[SCENE TIMER] {scene_data["name"]} STARTING')
+        begin_time = time.perf_counter()
+
         while action is not None:
             step_metadata = controller.step(action, **params)
             if step_metadata is None:
                 break
             action, params = action_callback(scene_data, step_metadata, self)
 
+        end_time = time.perf_counter()
+        time_diff = end_time - begin_time
+        logger.debug(
+            f'[SCENE TIMER] {scene_data["name"]} ENDING: '
+            f'{time_diff:0.4f} seconds'
+        )
+
         controller.end_scene()
 
         return scene_data['name']
 
 
 class SingleFileRunnerScript(AbstractRunnerScript):
     def _append_subclass_args_to_parser(
@@ -300,19 +296,19 @@
 
     def _read_subclass_args(
         self,
         parser: argparse.ArgumentParser
     ) -> Tuple[argparse.Namespace, List[str]]:
         args = parser.parse_args()
         filenames = glob.glob(args.mcs_scene_prefix + '*_debug.json')
-        print(
+        logger.debug(
             f'Found {len(filenames)} files matching '
             f'{args.mcs_scene_prefix + "*_debug.json"}'
         )
         if not len(filenames):
-            print('No matching files found... trying non-debug files')
+            logger.debug('No matching files found... trying non-debug files')
             filenames = glob.glob(args.mcs_scene_prefix + '*.json')
-            print(
+            logger.debug(
                 f'Found {len(filenames)} files matching '
                 f'{args.mcs_scene_prefix + "*.json"}'
             )
         return args, sorted(filenames)
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/serializer.py` & `machine_common_sense-0.7.0/machine_common_sense/serializer.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/step_metadata.py` & `machine_common_sense-0.7.0/machine_common_sense/step_metadata.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/machine_common_sense/stringifier.py` & `machine_common_sense-0.7.0/machine_common_sense/stringifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,18 @@
                 else metadata.texture_color_list,
                 metadata.held,
                 metadata.visible,
                 ", ".join(metadata.state_list)
                 if (metadata.state_list is not None)
                 else metadata.state_list,
                 Stringifier.vector_to_string(metadata.position),
-                metadata.distance_in_world,
+                str(round(
+                    metadata.distance_in_world,
+                    Stringifier.NUMBER_OF_DECIMALS
+                )),
                 Stringifier.vector_to_string(metadata.direction),
                 (
                     (
                         "[" +
                         ", ".join(
                             Stringifier.vector_to_string(corner)
                             for corner in metadata.dimensions
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/subscriber.py` & `machine_common_sense-0.7.0/machine_common_sense/subscriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,11 +33,13 @@
             # shouldn't enable both at the same time
         elif config.is_top_down_plotter():
             controller.subscribe(TopdownVideoEventHandler())
         if (config.is_depth_maps_enabled()):
             controller.subscribe(DepthVideoEventHandler())
         if (config.is_object_masks_enabled()):
             controller.subscribe(SegmentationVideoEventHandler())
-    controller.subscribe(ControllerLogger())
+    # Add the logger unless no modes are configured.
+    if config.get_terminal_output_mode():
+        controller.subscribe(ControllerLogger())
     # TODO once we remove evaulation code, we can better handle when,
     # this handler subscribes
     controller.subscribe(HistoryEventHandler())
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense/unity_executable_provider.py` & `machine_common_sense-0.7.0/machine_common_sense/unity_executable_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 LINUX_URL = "https://github.com/NextCenturyCorporation/MCS/releases/download/{ver}/MCS-AI2-THOR-Unity-App-v{ver}-linux.zip"  # noqa
 MAC_URL = "https://github.com/NextCenturyCorporation/MCS/releases/download/{ver}/MCS-AI2-THOR-Unity-App-v{ver}-mac.zip"  # noqa
 LINUX_DEV_URL = "https://ai2thor-unity-releases.s3.amazonaws.com/MCS-AI2-THOR-Unity-App-vdevelop-linux.zip"  # noqa
 MAC_DEV_URL = "https://ai2thor-unity-releases.s3.amazonaws.com/MCS-AI2-THOR-Unity-App-vdevelop-mac.zip"  # noqa
 
 
 class UnityExecutableProvider():
-    '''Automatically provides MCS AI2-THOR Unity executable for the MCS package.
-    Will check a cache and download if necessary'''
+    '''Automatically provides MCS AI2-THOR Unity executable for the MCS
+    package. Will check a cache and download if necessary'''
 
     DOWNLOAD_FILE = "MCS-AI2-THOR-Unity-App-v{}.zip"
     PLATFORM_MAC = "Darwin"
     PLATFORM_LINUX = "Linux"
     PLATFORM_OTHER = "other"
 
     def __init__(self):
@@ -221,16 +221,16 @@
         return self.GZ_FILES
 
     def _get_required_files(self):
         return self.REQUIRED_FILES
 
 
 class LinuxExecutionCache(AbstractExecutionCache):
-    '''Handles Linux specific code for running a cache for MCS Unity executables.
-    '''
+    '''Handles Linux specific code for running a cache for MCS Unity
+    executables.'''
     REQUIRED_FILES = [
         "LinuxPlayer_s.debug",
         "UnityPlayer.so",
         "UnityPlayer_s.debug",
         "MCS-AI2-THOR-Unity-App-v{version}_Data",
         "MCS-AI2-THOR-Unity-App-v{version}.x86_64"]
     EXECUTABLE_FILE = "MCS-AI2-THOR-Unity-App-v{version}.x86_64"
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense.egg-info/PKG-INFO` & `machine_common_sense-0.7.0/machine_common_sense.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: machine-common-sense
-Version: 0.6.5
+Version: 0.7.0
 Summary: Machine Common Sense Python API to Unity 3D Simulation Environment
 Home-page: https://github.com/NextCenturyCorporation/MCS/
 Maintainer: Next Century, a wholly owned subsidiary of CACI
 Maintainer-email: mcs-ta2@machinecommonsense.com
 License: Apache-2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Typing :: Typed
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version fury.io](https://badge.fury.io/py/machine-common-sense.svg)](https://pypi.python.org/pypi/machine-common-sense/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/machine-common-sense.svg)](https://pypi.python.org/pypi/machine-common-sense/)
 [![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
@@ -42,15 +43,15 @@
 
 Publish Documentation: [![Publish Docs](https://github.com/NextCenturyCorporation/MCS/actions/workflows/docs-publish.yaml/badge.svg)](https://github.com/NextCenturyCorporation/MCS/actions/workflows/docs-publish.yaml)
 
 Publish to PyPI: [![Publish PyPI](https://github.com/NextCenturyCorporation/MCS/actions/workflows/pypi-publish.yaml/badge.svg)](https://github.com/NextCenturyCorporation/MCS/actions/workflows/pypi-publish.yaml)
 
 # MCS Python Package
 
-Python interface for interacting with MCS AI2Thor environment and running scenes. The latest release of the MCS Python library is `0.6.5`. You can find the latest documentation [here](https://nextcenturycorporation.github.io/MCS).
+Python interface for interacting with MCS AI2Thor environment and running scenes. The latest release of the MCS Python library is `0.7.0`. You can find the latest documentation [here](https://nextcenturycorporation.github.io/MCS).
 
 - [Quickstart Installation](#quickstart-installation)
 - [Usage](#usage)
 - [Documentation](#documentation)
 - [Other MCS GitHub Repositories](#other-mcs-github-repositories)
 - [Troubleshooting/Email](#troubleshooting)
 - [License](#apache-2-open-source-license)
```

### Comparing `machine_common_sense-0.6.5/machine_common_sense.egg-info/SOURCES.txt` & `machine_common_sense-0.7.0/machine_common_sense.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 machine_common_sense.egg-info/SOURCES.txt
 machine_common_sense.egg-info/dependency_links.txt
 machine_common_sense.egg-info/entry_points.txt
 machine_common_sense.egg-info/requires.txt
 machine_common_sense.egg-info/top_level.txt
 machine_common_sense/scripts/__init__.py
 machine_common_sense/scripts/cache_addressables.py
+machine_common_sense/scripts/change_file_names_to_cell_ids_make_videos.py
 machine_common_sense/scripts/config_level1.ini
 machine_common_sense/scripts/config_level1_debug.ini
 machine_common_sense/scripts/config_level2.ini
 machine_common_sense/scripts/config_level2_debug.ini
 machine_common_sense/scripts/config_no_debug.ini
 machine_common_sense/scripts/config_oracle.ini
 machine_common_sense/scripts/config_oracle_debug.ini
@@ -45,14 +46,15 @@
 machine_common_sense/scripts/extract_ground_truth_from_debug_files.py
 machine_common_sense/scripts/getch_helper.py
 machine_common_sense/scripts/run_action_file.py
 machine_common_sense/scripts/run_follow_path.py
 machine_common_sense/scripts/run_human_input.py
 machine_common_sense/scripts/run_init_scenes.py
 machine_common_sense/scripts/run_interactive_scenes_follow_path.py
+machine_common_sense/scripts/run_interactive_scenes_last_action.py
 machine_common_sense/scripts/run_interactive_scenes_pass.py
 machine_common_sense/scripts/run_interactive_scenes_rotate.py
 machine_common_sense/scripts/run_just_pass.py
 machine_common_sense/scripts/run_just_rotate.py
 machine_common_sense/scripts/run_last_action.py
 machine_common_sense/scripts/run_passive_scenes.py
 machine_common_sense/scripts/run_reorientation_scenes.py
```

### Comparing `machine_common_sense-0.6.5/setup.py` & `machine_common_sense-0.7.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,42 +27,49 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Games/Entertainment :: Simulation',
         'Topic :: Multimedia :: Graphics',
         'Topic :: Multimedia :: Graphics :: 3D Rendering',
         'Typing :: Typed'
     ],
     license='Apache-2',
-    python_requires=">=3.7,<3.10",
+    python_requires=">=3.7,<3.11",
     packages=setuptools.find_packages(),
     package_data={'': ['*.ini'], },
     install_requires=[
-        'shapely>=1.7.0',
-        'colour>=0.1.5',
-        'opencv-python>=4.0',
-        'matplotlib>=3.3',
-        'msgpack>=1.0.0',
-        'numpyencoder>=0.3.0',
         'ai2thor==2.5.0',
-        'scikit-image>=0.17.1',
-        'typeguard>=2.11.1',
-        'pydantic>=1.9.0'
+        'colour==0.1.5',
+        'importlib-metadata==4.2.0; python_version<"3.8"',
+        'importlib-metadata==6.3.0; python_version>="3.8"',
+        'matplotlib==3.5.3; python_version<"3.8"',
+        'matplotlib==3.7.1; python_version>="3.8"',
+        'msgpack==1.0.5',
+        'numpyencoder==0.3.0',
+        'opencv-python==4.4.0.46; python_version<="3.9"',
+        'opencv-python==4.5.4.60; python_version>="3.10"',
+        'pydantic==1.10.7',
+        'requests==2.31.0',
+        'scikit-image==0.19.3',
+        'Shapely==1.7.1; python_version<"3.10"',
+        'Shapely==1.8.5; python_version>="3.10"',
+        'typeguard==3.0.2'
     ],
     entry_points={
         'console_scripts': [
             ('run_in_human_input_mode='
              'machine_common_sense.scripts.run_human_input:main'),
             ('run_scene_timer='
              'machine_common_sense.scripts.run_scene_timer:main'),
```

### Comparing `machine_common_sense-0.6.5/tests/mock_controller.py` & `machine_common_sense-0.7.0/tests/mock_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         # Do NOT call superclass __init__ function
 
         # Need to clear any previously set environment variables
         # so that they don't affect test cases
         check_config_path = os.getenv(
             ConfigManager.CONFIG_FILE_ENV_VAR, None)
 
-        if(check_config_path is not None):
+        if (check_config_path is not None):
             os.environ.pop(ConfigManager.CONFIG_FILE_ENV_VAR)
 
         self._subscribers = []
 
         self._failure_handler_registered = True  # atexit not needed for tests
         self._end_scene_called = False
         self._controller = MockController()
```

### Comparing `machine_common_sense-0.6.5/tests/test_action.py` & `machine_common_sense-0.7.0/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_config_manager.py` & `machine_common_sense-0.7.0/tests/test_config_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
                                                  PhysicsConfig,
                                                  SceneConfiguration,
                                                  SceneObject, SequenceConfig,
                                                  ShowConfig, SingleStepConfig,
                                                  SizeConfig,
                                                  StepBeginEndConfig,
                                                  TeleportConfig,
+                                                 TerminalOutputMode,
                                                  TransformConfig, Vector3d)
 
 
 class TestConfigManager(unittest.TestCase):
 
     def mock_env(**env_vars):
         return patch.dict(os.environ, env_vars, clear=True)
@@ -185,14 +186,19 @@
         self.assertEqual(
             self.config_mngr.get_metadata_tier(),
             MetadataTier.ORACLE)
         self.assertEqual(
             self.config_mngr.get_metadata_tier().value,
             'oracle')
 
+    def test_controller_timeout(self):
+        self.assertEquals(self.config_mngr.get_controller_timeout(), 180)
+        self.config_mngr.set_controller_timeout(str(90))
+        self.assertEquals(self.config_mngr.get_controller_timeout(), 90)
+
     def test_get_size(self):
         self.assertEqual(self.config_mngr.get_size(), 600)
 
         self.config_mngr._config[
             self.config_mngr.CONFIG_DEFAULT_SECTION
         ][
             self.config_mngr.CONFIG_SIZE
@@ -209,14 +215,88 @@
             self.config_mngr.CONFIG_TEAM
         ] = 'team-name'
 
         self.assertEqual(
             self.config_mngr.get_team(),
             'team-name')
 
+    def test_terminal_output_mode(self):
+        all_modes = [
+            TerminalOutputMode.ACTIONS, TerminalOutputMode.MINIMAL,
+            TerminalOutputMode.OBJECTS, TerminalOutputMode.PERFORMER,
+            TerminalOutputMode.SCENE
+        ]
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            all_modes
+        )
+        default_section = self.config_mngr._config[
+            self.config_mngr.CONFIG_DEFAULT_SECTION
+        ]
+
+        default_section['terminal_output'] = 'true'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            all_modes
+        )
+
+        default_section['terminal_output'] = 'all'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            all_modes
+        )
+
+        default_section['terminal_output'] = 'false'
+        self.assertEqual(self.config_mngr.get_terminal_output_mode(), [])
+
+        default_section['terminal_output'] = 'none'
+        self.assertEqual(self.config_mngr.get_terminal_output_mode(), [])
+
+        default_section['terminal_output'] = 'MINIMAL'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            [TerminalOutputMode.MINIMAL]
+        )
+
+        default_section['terminal_output'] = 'minimal'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            [TerminalOutputMode.MINIMAL]
+        )
+
+        default_section['terminal_output'] = 'actions'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            [TerminalOutputMode.ACTIONS]
+        )
+
+        default_section['terminal_output'] = 'objects'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            [TerminalOutputMode.OBJECTS]
+        )
+
+        default_section['terminal_output'] = 'performer'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            [TerminalOutputMode.PERFORMER]
+        )
+
+        default_section['terminal_output'] = 'scene'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            [TerminalOutputMode.SCENE]
+        )
+
+        default_section['terminal_output'] = 'objects,scene'
+        self.assertEqual(
+            self.config_mngr.get_terminal_output_mode(),
+            [TerminalOutputMode.OBJECTS, TerminalOutputMode.SCENE]
+        )
+
     def test_is_history_enabled(self):
         self.assertTrue(self.config_mngr.is_history_enabled())
 
         self.config_mngr._config[
             self.config_mngr.CONFIG_DEFAULT_SECTION
         ][
             self.config_mngr.CONFIG_HISTORY_ENABLED
@@ -275,14 +355,16 @@
         self.config_mngr._config[
             self.config_mngr.CONFIG_DEFAULT_SECTION
         ][
             self.config_mngr.CONFIG_TIMEOUT
         ] = '50'
 
         self.assertEqual(self.config_mngr.get_timeout(), 50)
+        self.config_mngr.set_timeout(str(51))
+        self.assertEqual(self.config_mngr.get_timeout(), 51)
 
 
 class TestSceneConfig(unittest.TestCase):
     def test_objects(self):
         object_config_list = [{
             'id': 'id_1',
             'type': 'type_1'
```

### Comparing `machine_common_sense-0.6.5/tests/test_controller.py` & `machine_common_sense-0.7.0/tests/test_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import shutil
 import unittest
 from types import SimpleNamespace
 from unittest.mock import ANY, MagicMock
 
 import numpy as np
+import typeguard
 
 import machine_common_sense as mcs
 from machine_common_sense.config_manager import (ConfigManager, MetadataTier,
                                                  SceneConfiguration, Vector3d)
 from machine_common_sense.controller_events import EndScenePayload, EventType
 from machine_common_sense.goal_metadata import GoalMetadata
 from machine_common_sense.parameter import Parameter
@@ -45,15 +46,15 @@
         return SimpleNamespace(**mock_scene_event_data)
 
     def create_step_data(self, **kwargs):
         data = dict(
             clockwise=True,
             consistentColors=False,
             continuous=True,
-            disablePosition=True,
+            disablePosition=False,
             goalObjectIds=[],
             gridSize=Parameter.GRID_SIZE,
             horizon=0.0,
             lateral=0,
             logs=True,
             moveMagnitude=mcs.controller.DEFAULT_MOVE,
             objectId=None,
@@ -64,16 +65,16 @@
             onlyReturnObjectGoal=False,
             receptacleObjectId=None,
             receptacleObjectImageCoords={
                 'x': 0,
                 'y': 0
             },
             recordTopDown=False,
-            renderDepthImage=False,
-            renderObjectImage=False,
+            renderDepthImage=True,
+            renderObjectImage=True,
             rotation={'y': 0.0},
             snapToGrid=False,
             straight=1,
             teleportPosition=None,
             teleportRotation=None,
             topDownImagePath=None
         )
@@ -126,14 +127,15 @@
                         "x": 90,
                         "y": -30,
                         "z": 0
                     },
                     "distance": 1.5,
                     "distanceXZ": 1.1,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 12.34,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "p1",
                             "p2",
                             "p3",
                             "p4",
@@ -165,14 +167,15 @@
                         "x": -90,
                         "y": 180,
                         "z": 270
                     },
                     "distance": 2.5,
                     "distanceXZ": 2.0,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 34.56,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "pA",
                             "pB",
                             "pC",
                             "pD",
@@ -205,14 +208,15 @@
                         "x": 180,
                         "y": -60,
                         "z": 0
                     },
                     "distance": 2.5,
                     "distanceXZ": 2.2,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 56.78,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "p11",
                             "p12",
                             "p13",
                             "p14",
@@ -244,14 +248,15 @@
                         "x": -180,
                         "y": 60,
                         "z": 90
                     },
                     "distance": 3.5,
                     "distanceXZ": 3.3,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 78.90,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "pAA",
                             "pBB",
                             "pCC",
                             "pDD",
@@ -362,15 +367,15 @@
                     {
                         "x": 1,
                         "y": 1
                     }
                 ]}
         }
 
-        with self.assertRaises(TypeError):
+        with self.assertRaises(typeguard.TypeCheckError):
             self.controller.end_scene("1.0", np.float64(0.5), {
                 1: {
                     "rating": 1.0,
                     "score": np.float64(.75),
                     "violations_xy_list": [
                         {
                             "x": np.int32(1),
```

### Comparing `machine_common_sense-0.6.5/tests/test_controller_media.py` & `machine_common_sense-0.7.0/tests/test_controller_media.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_controller_output_handler.py` & `machine_common_sense-0.7.0/tests/test_controller_output_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
                         "x": 90,
                         "y": -30,
                         "z": 0
                     },
                     "distance": 1.5,
                     "distanceXZ": 1.1,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 12.34,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "p1",
                             "p2",
                             "p3",
                             "p4",
@@ -132,14 +133,15 @@
                         "x": -90,
                         "y": 180,
                         "z": 270
                     },
                     "distance": 2.5,
                     "distanceXZ": 2.0,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 34.56,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "pA",
                             "pB",
                             "pC",
                             "pD",
@@ -176,14 +178,15 @@
                         "x": 180,
                         "y": -60,
                         "z": 0
                     },
                     "distance": 2.5,
                     "distanceXZ": 2.2,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 56.78,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "p11",
                             "p12",
                             "p13",
                             "p14",
@@ -219,14 +222,15 @@
                         "x": -180,
                         "y": 60,
                         "z": 90
                     },
                     "distance": 3.5,
                     "distanceXZ": 3.3,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 78.90,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "pAA",
                             "pBB",
                             "pCC",
                             "pDD",
@@ -276,14 +280,15 @@
                         "x": 0,
                         "y": 0,
                         "z": 0
                     },
                     "distance": 0,
                     "distanceXZ": 0,
                     "isPickedUp": True,
+                    "wasPickedUp": True,
                     "mass": 1,
                     "objectId": "testId1",
                     "position": {
                         "x": 1,
                         "y": 1,
                         "z": 2
                     },
@@ -307,14 +312,15 @@
                         "x": 90,
                         "y": -30,
                         "z": 0
                     },
                     "distance": 1.5,
                     "distanceXZ": 1.1,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 12.34,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "p1",
                             "p2",
                             "p3",
                             "p4",
@@ -350,14 +356,15 @@
                         "x": -90,
                         "y": 180,
                         "z": 270
                     },
                     "distance": 2.5,
                     "distanceXZ": 2,
                     "isPickedUp": False,
+                    "wasPickedUp": False,
                     "mass": 34.56,
                     "objectBounds": {
                         "objectBoundsCorners": [
                             "pA",
                             "pB",
                             "pC",
                             "pD",
@@ -609,17 +616,17 @@
             actual.object_list[0].simulation_agent_held_object, "")
         self.assertEqual(
             actual.object_list[0].simulation_agent_is_holding_held_object,
             False)
 
         # IF we are at default level, shouldn't depth maps, object masks be
         # restricted?
-        self.assertEqual(len(actual.depth_map_list), 0)
+        self.assertEqual(len(actual.depth_map_list), 1)
         self.assertEqual(len(actual.image_list), 1)
-        self.assertEqual(len(actual.object_mask_list), 0)
+        self.assertEqual(len(actual.object_mask_list), 1)
         '''numpy.testing.assert_almost_equal(
             numpy.array(actual.depth_map_list[0]),
             numpy.array([[30, 60], [90, 120]], dtype=numpy.float32),
             3
         )'''
         self.assertEqual(numpy.array(actual.image_list[0]), image_data)
         '''self.assertEqual(
```

### Comparing `machine_common_sense-0.6.5/tests/test_goal_metadata.py` & `machine_common_sense-0.7.0/tests/test_goal_metadata.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_history_event_handler.py` & `machine_common_sense-0.7.0/tests/test_history_event_handler.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_history_writer.py` & `machine_common_sense-0.7.0/tests/test_history_writer.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_logging_config.py` & `machine_common_sense-0.7.0/tests/test_logging_config.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_material.py` & `machine_common_sense-0.7.0/tests/test_material.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_mcs.py` & `machine_common_sense-0.7.0/tests/test_mcs.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_object_metadata.py` & `machine_common_sense-0.7.0/tests/test_object_metadata.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_parameter.py` & `machine_common_sense-0.7.0/tests/test_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,22 +96,22 @@
             action="TestAction",
             numberProperty=1234,
             goal_object_ids=[],
             stringProperty="test_property")
         expected = {
             "action": "TestAction",
             "continuous": True,
-            "disablePosition": True,
+            "disablePosition": False,
             "goalObjectIds": [],
             "gridSize": 0.1,
             "logs": True,
             "numberProperty": 1234,
             "onlyReturnObjectGoal": False,
-            "renderDepthImage": False,
-            "renderObjectImage": False,
+            "renderDepthImage": True,
+            "renderObjectImage": True,
             "snapToGrid": False,
             "stringProperty": "test_property",
             "consistentColors": False,
             "recordTopDown": False,
             "topDownImagePath": "path"
 
         }
@@ -229,15 +229,15 @@
             action="TestAction",
             numberProperty=1234,
             goal_object_ids=[],
             stringProperty="test_property")
         expected = {
             "action": "TestAction",
             "continuous": True,
-            "disablePosition": True,
+            "disablePosition": False,
             "goalObjectIds": [],
             "gridSize": 0.1,
             "logs": True,
             "numberProperty": 1234,
             "onlyReturnObjectGoal": False,
             "renderDepthImage": True,
             "renderObjectImage": True,
@@ -268,15 +268,15 @@
             "action": "TestAction",
             "continuous": True,
             "disablePosition": True,
             "goalObjectIds": [],
             "gridSize": 0.1,
             "logs": True,
             "numberProperty": 1234,
-            "onlyReturnObjectGoal": False,
+            "onlyReturnObjectGoal": True,
             "renderDepthImage": False,
             "renderObjectImage": False,
             "snapToGrid": False,
             "stringProperty": "test_property",
             "consistentColors": False,
             "recordTopDown": False,
             "topDownImagePath": "path"
@@ -297,22 +297,22 @@
             action="TestAction",
             numberProperty=1234,
             goal_object_ids=[],
             stringProperty="test_property")
         expected = {
             "action": "TestAction",
             "continuous": True,
-            "disablePosition": True,
+            "disablePosition": False,
             "goalObjectIds": [],
             "gridSize": 0.1,
             "logs": True,
             "onlyReturnObjectGoal": False,
             "numberProperty": 1234,
             "renderDepthImage": True,
-            "renderObjectImage": False,
+            "renderObjectImage": True,
             "snapToGrid": False,
             "stringProperty": "test_property",
             "consistentColors": False,
             "recordTopDown": False,
             "topDownImagePath": "path"
         }
         self.assertEqual(actual, expected)
@@ -336,15 +336,15 @@
             "action": "TestAction",
             "continuous": True,
             "disablePosition": True,
             "goalObjectIds": [],
             "gridSize": 0.1,
             "logs": True,
             "numberProperty": 1234,
-            "onlyReturnObjectGoal": False,
+            "onlyReturnObjectGoal": True,
             "renderDepthImage": False,
             "renderObjectImage": False,
             "snapToGrid": False,
             "stringProperty": "test_property",
             "consistentColors": False,
             "recordTopDown": False,
             "topDownImagePath": "path"
@@ -365,22 +365,22 @@
             action="TestAction",
             numberProperty=1234,
             goal_object_ids=[],
             stringProperty="test_property")
         expected = {
             "action": "TestAction",
             "continuous": True,
-            "disablePosition": True,
+            "disablePosition": False,
             "goalObjectIds": [],
             "gridSize": 0.1,
             "logs": True,
             "numberProperty": 1234,
             "onlyReturnObjectGoal": False,
-            "renderDepthImage": False,
-            "renderObjectImage": False,
+            "renderDepthImage": True,
+            "renderObjectImage": True,
             "snapToGrid": False,
             "stringProperty": "test_property",
             "consistentColors": False,
             "recordTopDown": False,
             "topDownImagePath": "path"
         }
         self.assertEqual(actual, expected)
@@ -404,15 +404,15 @@
             "action": "TestAction",
             "continuous": True,
             "disablePosition": True,
             "goalObjectIds": [],
             "gridSize": 0.1,
             "logs": True,
             "numberProperty": 1234,
-            "onlyReturnObjectGoal": False,
+            "onlyReturnObjectGoal": True,
             "renderDepthImage": False,
             "renderObjectImage": False,
             "snapToGrid": False,
             "stringProperty": "test_property",
             "consistentColors": False,
             "recordTopDown": False,
             "topDownImagePath": "path"
```

### Comparing `machine_common_sense-0.6.5/tests/test_plotter.py` & `machine_common_sense-0.7.0/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_recorder.py` & `machine_common_sense-0.7.0/tests/test_recorder.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_reward.py` & `machine_common_sense-0.7.0/tests/test_reward.py`

 * *Files 18% similar despite different names*

```diff
@@ -219,73 +219,187 @@
         self.assertIsInstance(list(polygon.exterior.coords)[0], Tuple)
 
     def test_retrieval_reward(self):
         goal = mcs.GoalMetadata()
         goal.metadata['target'] = {'id': '0'}
         obj_list = []
         for i in range(10):
-            obj = {"objectId": str(i), 'isPickedUp': not i}
+            obj = {"objectId": str(i), 'wasPickedUp': not i}
             obj_list.append(obj)
         reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, agent={},
                                                    performer_reach=1.0)
         self.assertEqual(reward, 1)
         self.assertIsInstance(reward, int)
 
     def test_retrieval_reward_nothing_pickedup(self):
         goal = mcs.GoalMetadata()
         goal.metadata['target'] = {'id': '0'}
         obj_list = []
         for i in range(10):
-            obj = {"objectId": str(i), 'isPickedUp': False}
+            obj = {"objectId": str(i), 'wasPickedUp': False}
             obj_list.append(obj)
         reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, agent={},
                                                    performer_reach=1.0)
         self.assertEqual(reward, 0)
         self.assertIsInstance(reward, int)
 
     def test_retrieval_reward_multi_target(self):
         goal = mcs.GoalMetadata()
         goal.metadata['targets'] = [{'id': '0'}, {'id': '1'}, {'id': '2'}]
         obj_list = []
         for i in range(10):
-            obj_list.append({'objectId': str(i), 'isPickedUp': True})
+            obj_list.append({'objectId': str(i), 'wasPickedUp': True})
         reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, agent={},
                                                    performer_reach=1.0)
         self.assertEqual(reward, 1)
         self.assertIsInstance(reward, int)
 
     def test_retrieval_reward_multi_target_nothing_pickedup(self):
         goal = mcs.GoalMetadata()
         goal.metadata['targets'] = [{'id': '0'}, {'id': '1'}, {'id': '2'}]
         obj_list = []
         for i in range(10):
-            obj_list.append({'objectId': str(i), 'isPickedUp': False})
+            obj_list.append({'objectId': str(i), 'wasPickedUp': False})
         reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, agent={},
                                                    performer_reach=1.0)
         self.assertEqual(reward, 0)
         self.assertIsInstance(reward, int)
 
     def test_retrieval_reward_multi_target_some_pickedup(self):
         goal = mcs.GoalMetadata()
         goal.metadata['targets'] = [{'id': '0'}, {'id': '1'}, {'id': '2'}]
         obj_list = []
         for i in range(10):
-            obj_list.append({'objectId': str(i), 'isPickedUp': (i == 0)})
+            obj_list.append({'objectId': str(i), 'wasPickedUp': (i == 0)})
         reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, agent={},
                                                    performer_reach=1.0)
         self.assertEqual(reward, 0)
         self.assertIsInstance(reward, int)
 
     def test_retrieval_reward_multi_target_more_pickedup(self):
         goal = mcs.GoalMetadata()
         goal.metadata['targets'] = [{'id': '0'}, {'id': '1'}, {'id': '2'}]
         obj_list = []
         for i in range(10):
-            obj_list.append({'objectId': str(i), 'isPickedUp': (i != 0)})
+            obj_list.append({'objectId': str(i), 'wasPickedUp': (i != 0)})
         reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, agent={},
                                                    performer_reach=1.0)
         self.assertEqual(reward, 0)
         self.assertIsInstance(reward, int)
 
+    def test_retrieval_reward_multi_target_pickup_one_of_two(self):
+        goal = mcs.GoalMetadata()
+        goal.metadata['targets'] = [{'id': '0'}, {'id': '1'}]
+        goal.metadata['pickup_number'] = 1
+
+        # Test: Picking up no targets should return a reward of 0
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': False},
+            {'objectId': '1', 'wasPickedUp': False}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 0)
+
+        # Test: Picking up only the 1st target should return a reward of 1
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': True},
+            {'objectId': '1', 'wasPickedUp': False}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 1)
+
+        # Test: Picking up only the 2nd target should return a reward of 1
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': False},
+            {'objectId': '1', 'wasPickedUp': True}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 1)
+
+        # Test: Picking up all targets should return a reward of 1
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': True},
+            {'objectId': '1', 'wasPickedUp': True}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 1)
+
+    def test_retrieval_reward_multi_target_pickup_two_of_three(self):
+        goal = mcs.GoalMetadata()
+        goal.metadata['targets'] = [{'id': '0'}, {'id': '1'}, {'id': '2'}]
+        goal.metadata['pickup_number'] = 2
+
+        # Test: Picking up no targets should return a reward of 0
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': False},
+            {'objectId': '1', 'wasPickedUp': False},
+            {'objectId': '2', 'wasPickedUp': False}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 0)
+
+        # Test: Picking up only the 1st target should return a reward of 0
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': True},
+            {'objectId': '1', 'wasPickedUp': False},
+            {'objectId': '2', 'wasPickedUp': False}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 0)
+
+        # Test: Picking up only the 2nd target should return a reward of 0
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': False},
+            {'objectId': '1', 'wasPickedUp': True},
+            {'objectId': '2', 'wasPickedUp': False}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 0)
+
+        # Test: Picking up only the 3rd target should return a reward of 0
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': False},
+            {'objectId': '1', 'wasPickedUp': False},
+            {'objectId': '2', 'wasPickedUp': True}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 0)
+
+        # Test: Picking up the 1st and 2nd targets should return a reward of 1
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': True},
+            {'objectId': '1', 'wasPickedUp': True},
+            {'objectId': '2', 'wasPickedUp': False}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 1)
+
+        # Test: Picking up the 1st and 3rd targets should return a reward of 1
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': True},
+            {'objectId': '1', 'wasPickedUp': False},
+            {'objectId': '2', 'wasPickedUp': True}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 1)
+
+        # Test: Picking up the 2nd and 3rd targets should return a reward of 1
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': False},
+            {'objectId': '1', 'wasPickedUp': True},
+            {'objectId': '2', 'wasPickedUp': True}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 1)
+
+        # Test: Picking up all targets should return a reward of 1
+        obj_list = [
+            {'objectId': '0', 'wasPickedUp': True},
+            {'objectId': '1', 'wasPickedUp': True},
+            {'objectId': '2', 'wasPickedUp': True}
+        ]
+        reward = mcs.Reward._calc_retrieval_reward(goal, obj_list, {}, 1.0)
+        self.assertEqual(reward, 1)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `machine_common_sense-0.6.5/tests/test_serializer.py` & `machine_common_sense-0.7.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_step_metadata.py` & `machine_common_sense-0.7.0/tests/test_step_metadata.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_stringifier.py` & `machine_common_sense-0.7.0/tests/test_stringifier.py`

 * *Files identical despite different names*

### Comparing `machine_common_sense-0.6.5/tests/test_unity_executable_provider.py` & `machine_common_sense-0.7.0/tests/test_unity_executable_provider.py`

 * *Files identical despite different names*

