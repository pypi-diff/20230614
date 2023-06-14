# Comparing `tmp/trajdata-1.3.1.tar.gz` & `tmp/trajdata-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajdata-1.3.1.tar", last modified: Sat Apr 22 06:24:18 2023, max compression
+gzip compressed data, was "trajdata-1.3.2.tar", last modified: Wed Jun 14 07:04:47 2023, max compression
```

## Comparing `trajdata-1.3.1.tar` & `trajdata-1.3.2.tar`

### file list

```diff
@@ -1,115 +1,122 @@
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.484937 trajdata-1.3.1/
--rw-r--r--   0 bivanovic (41443) dip         (30)    11357 2022-07-10 04:26:11.000000 trajdata-1.3.1/LICENSE
--rw-r--r--   0 bivanovic (41443) dip         (30)    11821 2023-04-22 06:24:18.484937 trajdata-1.3.1/PKG-INFO
--rw-r--r--   0 bivanovic (41443) dip         (30)    11195 2023-04-22 06:23:41.000000 trajdata-1.3.1/README.md
--rw-r--r--   0 bivanovic (41443) dip         (30)      135 2022-07-10 04:26:11.000000 trajdata-1.3.1/pyproject.toml
--rw-r--r--   0 bivanovic (41443) dip         (30)     1059 2023-04-22 06:24:18.484937 trajdata-1.3.1/setup.cfg
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.476937 trajdata-1.3.1/src/
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.476937 trajdata-1.3.1/src/trajdata/
--rw-r--r--   0 bivanovic (41443) dip         (30)      135 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/__init__.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.476937 trajdata-1.3.1/src/trajdata/augmentation/
--rw-r--r--   0 bivanovic (41443) dip         (30)      181 2022-11-12 07:40:30.000000 trajdata-1.3.1/src/trajdata/augmentation/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      548 2022-07-30 07:42:53.000000 trajdata-1.3.1/src/trajdata/augmentation/augmentation.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1786 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/augmentation/low_vel_yaw_correction.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1785 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/augmentation/noise_histories.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.476937 trajdata-1.3.1/src/trajdata/caching/
--rw-r--r--   0 bivanovic (41443) dip         (30)       68 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/caching/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    35798 2023-04-22 06:23:41.000000 trajdata-1.3.1/src/trajdata/caching/df_cache.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2311 2022-11-12 07:57:45.000000 trajdata-1.3.1/src/trajdata/caching/env_cache.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     6507 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/caching/scene_cache.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/data_structures/
--rw-r--r--   0 bivanovic (41443) dip         (30)      551 2023-02-01 00:28:01.000000 trajdata-1.3.1/src/trajdata/data_structures/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1944 2023-02-15 17:46:18.000000 trajdata-1.3.1/src/trajdata/data_structures/agent.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    13883 2023-02-11 07:41:45.000000 trajdata-1.3.1/src/trajdata/data_structures/batch.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    22665 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/data_structures/batch_element.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    36157 2023-02-11 07:41:45.000000 trajdata-1.3.1/src/trajdata/data_structures/collation.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3965 2022-07-20 07:32:10.000000 trajdata-1.3.1/src/trajdata/data_structures/data_index.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      841 2023-02-15 17:47:17.000000 trajdata-1.3.1/src/trajdata/data_structures/environment.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3570 2023-02-01 00:28:01.000000 trajdata-1.3.1/src/trajdata/data_structures/scene.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1865 2023-02-15 17:46:08.000000 trajdata-1.3.1/src/trajdata/data_structures/scene_metadata.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      411 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/data_structures/scene_tag.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    15442 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/data_structures/state.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    41903 2023-04-22 06:23:41.000000 trajdata-1.3.1/src/trajdata/dataset.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/dataset_specific/
--rw-r--r--   0 bivanovic (41443) dip         (30)      110 2022-11-12 07:42:49.000000 trajdata-1.3.1/src/trajdata/dataset_specific/__init__.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/dataset_specific/eth_ucy_peds/
--rw-r--r--   0 bivanovic (41443) dip         (30)       42 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/dataset_specific/eth_ucy_peds/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    12036 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/dataset_specific/lyft/
--rw-r--r--   0 bivanovic (41443) dip         (30)       38 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/dataset_specific/lyft/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    12667 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/dataset_specific/lyft/lyft_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     6613 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/dataset_specific/lyft/lyft_utils.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/dataset_specific/nuplan/
--rw-r--r--   0 bivanovic (41443) dip         (30)       42 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/dataset_specific/nuplan/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    15566 2023-02-15 17:41:49.000000 trajdata-1.3.1/src/trajdata/dataset_specific/nuplan/nuplan_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    14656 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/dataset_specific/nuplan/nuplan_utils.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/dataset_specific/nusc/
--rw-r--r--   0 bivanovic (41443) dip         (30)       38 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/dataset_specific/nusc/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    12101 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/dataset_specific/nusc/nusc_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    19061 2023-02-11 07:41:45.000000 trajdata-1.3.1/src/trajdata/dataset_specific/nusc/nusc_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3310 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/dataset_specific/raw_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      569 2023-04-22 06:23:41.000000 trajdata-1.3.1/src/trajdata/dataset_specific/scene_records.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/dataset_specific/waymo/
--rw-r--r--   0 bivanovic (41443) dip         (30)       40 2023-04-22 06:23:41.000000 trajdata-1.3.1/src/trajdata/dataset_specific/waymo/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    12977 2023-04-22 06:23:41.000000 trajdata-1.3.1/src/trajdata/dataset_specific/waymo/waymo_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    20306 2023-04-22 06:23:41.000000 trajdata-1.3.1/src/trajdata/dataset_specific/waymo/waymo_utils.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/filtering/
--rw-r--r--   0 bivanovic (41443) dip         (30)       23 2022-11-12 07:42:55.000000 trajdata-1.3.1/src/trajdata/filtering/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3659 2023-02-11 07:41:45.000000 trajdata-1.3.1/src/trajdata/filtering/filters.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/maps/
--rw-r--r--   0 bivanovic (41443) dip         (30)      193 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/maps/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      111 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/maps/lane_route.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1483 2023-01-05 00:00:22.000000 trajdata-1.3.1/src/trajdata/maps/map_api.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     6780 2023-04-22 06:23:41.000000 trajdata-1.3.1/src/trajdata/maps/map_kdtree.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2116 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/maps/raster_map.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      121 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/maps/traffic_light_status.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    21905 2023-02-10 07:47:20.000000 trajdata-1.3.1/src/trajdata/maps/vec_map.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     5194 2023-01-05 00:04:06.000000 trajdata-1.3.1/src/trajdata/maps/vec_map_elements.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/parallel/
--rw-r--r--   0 bivanovic (41443) dip         (30)       83 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/parallel/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3423 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/parallel/data_preprocessor.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/proto/
--rw-r--r--   0 bivanovic (41443) dip         (30)        0 2022-10-24 06:19:35.000000 trajdata-1.3.1/src/trajdata/proto/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     5969 2023-04-07 21:05:44.000000 trajdata-1.3.1/src/trajdata/proto/vectorized_map_pb2.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/simulation/
--rw-r--r--   0 bivanovic (41443) dip         (30)       39 2022-11-12 06:09:23.000000 trajdata-1.3.1/src/trajdata/simulation/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1056 2023-02-11 07:41:45.000000 trajdata-1.3.1/src/trajdata/simulation/sim_cache.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    10217 2023-02-11 07:41:45.000000 trajdata-1.3.1/src/trajdata/simulation/sim_df_cache.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1077 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/simulation/sim_metrics.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     8635 2023-02-11 07:41:45.000000 trajdata-1.3.1/src/trajdata/simulation/sim_scene.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3872 2022-10-24 06:19:35.000000 trajdata-1.3.1/src/trajdata/simulation/sim_stats.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      786 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/simulation/sim_vis.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.480937 trajdata-1.3.1/src/trajdata/utils/
--rw-r--r--   0 bivanovic (41443) dip         (30)        0 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/utils/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2724 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/utils/agent_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    10314 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/utils/arr_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     7225 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/utils/batch_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3204 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/utils/df_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2011 2023-04-22 06:23:41.000000 trajdata-1.3.1/src/trajdata/utils/env_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    10518 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/utils/map_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1843 2022-11-18 01:28:43.000000 trajdata-1.3.1/src/trajdata/utils/parallel_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     8175 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/utils/raster_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3520 2022-11-12 08:23:30.000000 trajdata-1.3.1/src/trajdata/utils/scene_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     5684 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/utils/state_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      186 2022-07-10 04:26:11.000000 trajdata-1.3.1/src/trajdata/utils/string_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    19023 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/utils/vis_utils.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.484937 trajdata-1.3.1/src/trajdata/visualization/
--rw-r--r--   0 bivanovic (41443) dip         (30)      160 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/visualization/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    17001 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/visualization/interactive_animation.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     5798 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/visualization/interactive_figure.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     7029 2023-04-21 23:35:15.000000 trajdata-1.3.1/src/trajdata/visualization/interactive_vis.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    13225 2023-02-04 18:48:20.000000 trajdata-1.3.1/src/trajdata/visualization/vis.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.476937 trajdata-1.3.1/src/trajdata.egg-info/
--rw-r--r--   0 bivanovic (41443) dip         (30)    11821 2023-04-22 06:24:18.000000 trajdata-1.3.1/src/trajdata.egg-info/PKG-INFO
--rw-r--r--   0 bivanovic (41443) dip         (30)     3472 2023-04-22 06:24:18.000000 trajdata-1.3.1/src/trajdata.egg-info/SOURCES.txt
--rw-r--r--   0 bivanovic (41443) dip         (30)        1 2023-04-22 06:24:18.000000 trajdata-1.3.1/src/trajdata.egg-info/dependency_links.txt
--rw-r--r--   0 bivanovic (41443) dip         (30)      338 2023-04-22 06:24:18.000000 trajdata-1.3.1/src/trajdata.egg-info/requires.txt
--rw-r--r--   0 bivanovic (41443) dip         (30)        9 2023-04-22 06:24:18.000000 trajdata-1.3.1/src/trajdata.egg-info/top_level.txt
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-22 06:24:18.484937 trajdata-1.3.1/tests/
--rw-r--r--   0 bivanovic (41443) dip         (30)    10463 2023-04-21 23:35:15.000000 trajdata-1.3.1/tests/test_batch_conversion.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     7443 2023-02-11 07:41:45.000000 trajdata-1.3.1/tests/test_collation.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     7569 2023-02-11 07:41:45.000000 trajdata-1.3.1/tests/test_datasizes.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      992 2022-11-17 10:42:27.000000 trajdata-1.3.1/tests/test_description_matching.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    13585 2023-02-11 07:41:45.000000 trajdata-1.3.1/tests/test_state.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     6304 2023-02-04 18:48:52.000000 trajdata-1.3.1/tests/test_traffic_data.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2068 2023-01-05 00:04:06.000000 trajdata-1.3.1/tests/test_vec_map.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.227769 trajdata-1.3.2/
+-rw-r--r--   0 bivanovic (41443) dip         (30)    11357 2022-07-10 04:26:11.000000 trajdata-1.3.2/LICENSE
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12764 2023-06-14 07:04:47.227769 trajdata-1.3.2/PKG-INFO
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12110 2023-06-14 07:04:31.000000 trajdata-1.3.2/README.md
+-rw-r--r--   0 bivanovic (41443) dip         (30)      135 2022-07-10 04:26:11.000000 trajdata-1.3.2/pyproject.toml
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1091 2023-06-14 07:04:47.227769 trajdata-1.3.2/setup.cfg
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.219769 trajdata-1.3.2/src/
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.219769 trajdata-1.3.2/src/trajdata/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      135 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/__init__.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.219769 trajdata-1.3.2/src/trajdata/augmentation/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      181 2022-11-12 07:40:30.000000 trajdata-1.3.2/src/trajdata/augmentation/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      548 2022-07-30 07:42:53.000000 trajdata-1.3.2/src/trajdata/augmentation/augmentation.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1786 2022-07-10 04:26:11.000000 trajdata-1.3.2/src/trajdata/augmentation/low_vel_yaw_correction.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1785 2023-02-04 18:48:20.000000 trajdata-1.3.2/src/trajdata/augmentation/noise_histories.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/caching/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       68 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/caching/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    35798 2023-04-22 23:20:08.000000 trajdata-1.3.2/src/trajdata/caching/df_cache.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2738 2023-06-14 07:04:31.000000 trajdata-1.3.2/src/trajdata/caching/env_cache.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     6507 2023-02-04 18:48:20.000000 trajdata-1.3.2/src/trajdata/caching/scene_cache.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/data_structures/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      551 2023-02-01 00:28:01.000000 trajdata-1.3.2/src/trajdata/data_structures/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1944 2023-04-26 07:43:53.000000 trajdata-1.3.2/src/trajdata/data_structures/agent.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    13883 2023-02-11 07:41:45.000000 trajdata-1.3.2/src/trajdata/data_structures/batch.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    22665 2023-04-21 23:35:15.000000 trajdata-1.3.2/src/trajdata/data_structures/batch_element.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    36157 2023-02-11 07:41:45.000000 trajdata-1.3.2/src/trajdata/data_structures/collation.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3965 2022-07-20 07:32:10.000000 trajdata-1.3.2/src/trajdata/data_structures/data_index.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      841 2023-02-15 17:47:17.000000 trajdata-1.3.2/src/trajdata/data_structures/environment.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3570 2023-02-01 00:28:01.000000 trajdata-1.3.2/src/trajdata/data_structures/scene.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1865 2023-02-15 17:46:08.000000 trajdata-1.3.2/src/trajdata/data_structures/scene_metadata.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      411 2022-07-10 04:26:11.000000 trajdata-1.3.2/src/trajdata/data_structures/scene_tag.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    15442 2023-04-22 23:20:08.000000 trajdata-1.3.2/src/trajdata/data_structures/state.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    42193 2023-06-14 07:04:31.000000 trajdata-1.3.2/src/trajdata/dataset.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/dataset_specific/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       36 2023-04-26 10:37:57.000000 trajdata-1.3.2/src/trajdata/dataset_specific/__init__.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/dataset_specific/eth_ucy_peds/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       42 2023-04-26 00:49:36.000000 trajdata-1.3.2/src/trajdata/dataset_specific/eth_ucy_peds/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12036 2023-04-26 05:58:40.000000 trajdata-1.3.2/src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/dataset_specific/interaction/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       52 2023-06-14 07:04:31.000000 trajdata-1.3.2/src/trajdata/dataset_specific/interaction/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    18800 2023-06-14 07:04:31.000000 trajdata-1.3.2/src/trajdata/dataset_specific/interaction/interaction_dataset.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/dataset_specific/lyft/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       38 2022-07-10 04:26:11.000000 trajdata-1.3.2/src/trajdata/dataset_specific/lyft/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12667 2023-02-04 18:48:20.000000 trajdata-1.3.2/src/trajdata/dataset_specific/lyft/lyft_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     6613 2023-02-04 18:48:20.000000 trajdata-1.3.2/src/trajdata/dataset_specific/lyft/lyft_utils.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/dataset_specific/nuplan/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       42 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/dataset_specific/nuplan/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    15566 2023-02-15 17:41:49.000000 trajdata-1.3.2/src/trajdata/dataset_specific/nuplan/nuplan_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    14656 2023-02-04 18:48:20.000000 trajdata-1.3.2/src/trajdata/dataset_specific/nuplan/nuplan_utils.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/dataset_specific/nusc/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       38 2022-07-10 04:26:11.000000 trajdata-1.3.2/src/trajdata/dataset_specific/nusc/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12101 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/dataset_specific/nusc/nusc_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    19061 2023-02-11 07:41:45.000000 trajdata-1.3.2/src/trajdata/dataset_specific/nusc/nusc_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3310 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/dataset_specific/raw_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      739 2023-06-14 07:04:31.000000 trajdata-1.3.2/src/trajdata/dataset_specific/scene_records.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/dataset_specific/sdd_peds/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       44 2023-04-26 10:37:57.000000 trajdata-1.3.2/src/trajdata/dataset_specific/sdd_peds/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3919 2023-04-26 10:37:57.000000 trajdata-1.3.2/src/trajdata/dataset_specific/sdd_peds/estimated_homography.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12254 2023-04-26 10:37:57.000000 trajdata-1.3.2/src/trajdata/dataset_specific/sdd_peds/sddpeds_dataset.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/dataset_specific/waymo/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       40 2023-04-22 23:20:08.000000 trajdata-1.3.2/src/trajdata/dataset_specific/waymo/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12977 2023-04-22 23:20:08.000000 trajdata-1.3.2/src/trajdata/dataset_specific/waymo/waymo_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    20306 2023-04-22 23:20:08.000000 trajdata-1.3.2/src/trajdata/dataset_specific/waymo/waymo_utils.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/filtering/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       23 2022-11-12 07:42:55.000000 trajdata-1.3.2/src/trajdata/filtering/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3659 2023-02-11 07:41:45.000000 trajdata-1.3.2/src/trajdata/filtering/filters.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/maps/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      193 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/maps/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      111 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/maps/lane_route.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1483 2023-01-05 00:00:22.000000 trajdata-1.3.2/src/trajdata/maps/map_api.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     6780 2023-04-22 23:20:08.000000 trajdata-1.3.2/src/trajdata/maps/map_kdtree.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2116 2023-02-04 18:48:20.000000 trajdata-1.3.2/src/trajdata/maps/raster_map.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      121 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/maps/traffic_light_status.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    21905 2023-02-10 07:47:20.000000 trajdata-1.3.2/src/trajdata/maps/vec_map.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     5194 2023-01-05 00:04:06.000000 trajdata-1.3.2/src/trajdata/maps/vec_map_elements.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/parallel/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       83 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/parallel/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3464 2023-06-14 07:04:31.000000 trajdata-1.3.2/src/trajdata/parallel/data_preprocessor.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.223769 trajdata-1.3.2/src/trajdata/proto/
+-rw-r--r--   0 bivanovic (41443) dip         (30)        0 2022-10-24 06:19:35.000000 trajdata-1.3.2/src/trajdata/proto/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     5969 2023-04-22 23:48:38.000000 trajdata-1.3.2/src/trajdata/proto/vectorized_map_pb2.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.227769 trajdata-1.3.2/src/trajdata/simulation/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       39 2022-11-12 06:09:23.000000 trajdata-1.3.2/src/trajdata/simulation/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1056 2023-02-11 07:41:45.000000 trajdata-1.3.2/src/trajdata/simulation/sim_cache.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10217 2023-02-11 07:41:45.000000 trajdata-1.3.2/src/trajdata/simulation/sim_df_cache.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1077 2022-07-10 04:26:11.000000 trajdata-1.3.2/src/trajdata/simulation/sim_metrics.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     8635 2023-02-11 07:41:45.000000 trajdata-1.3.2/src/trajdata/simulation/sim_scene.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3872 2022-10-24 06:19:35.000000 trajdata-1.3.2/src/trajdata/simulation/sim_stats.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      786 2022-07-10 04:26:11.000000 trajdata-1.3.2/src/trajdata/simulation/sim_vis.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.227769 trajdata-1.3.2/src/trajdata/utils/
+-rw-r--r--   0 bivanovic (41443) dip         (30)        0 2022-07-10 04:26:11.000000 trajdata-1.3.2/src/trajdata/utils/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2724 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/utils/agent_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10314 2023-04-21 23:35:15.000000 trajdata-1.3.2/src/trajdata/utils/arr_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     7225 2023-04-21 23:35:15.000000 trajdata-1.3.2/src/trajdata/utils/batch_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3204 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/utils/df_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2441 2023-06-14 07:04:31.000000 trajdata-1.3.2/src/trajdata/utils/env_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10518 2023-04-22 23:48:38.000000 trajdata-1.3.2/src/trajdata/utils/map_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1843 2022-11-18 01:28:43.000000 trajdata-1.3.2/src/trajdata/utils/parallel_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     8175 2023-02-04 18:48:20.000000 trajdata-1.3.2/src/trajdata/utils/raster_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3520 2022-11-12 08:23:30.000000 trajdata-1.3.2/src/trajdata/utils/scene_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     5684 2023-04-21 23:35:15.000000 trajdata-1.3.2/src/trajdata/utils/state_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      186 2022-07-10 04:26:11.000000 trajdata-1.3.2/src/trajdata/utils/string_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    19023 2023-04-21 23:35:15.000000 trajdata-1.3.2/src/trajdata/utils/vis_utils.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.227769 trajdata-1.3.2/src/trajdata/visualization/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      160 2023-04-21 23:35:15.000000 trajdata-1.3.2/src/trajdata/visualization/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    17001 2023-05-20 19:20:13.000000 trajdata-1.3.2/src/trajdata/visualization/interactive_animation.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     5798 2023-04-21 23:35:15.000000 trajdata-1.3.2/src/trajdata/visualization/interactive_figure.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     7029 2023-04-21 23:35:15.000000 trajdata-1.3.2/src/trajdata/visualization/interactive_vis.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    13231 2023-06-14 07:04:31.000000 trajdata-1.3.2/src/trajdata/visualization/vis.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.219769 trajdata-1.3.2/src/trajdata.egg-info/
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12764 2023-06-14 07:04:47.000000 trajdata-1.3.2/src/trajdata.egg-info/PKG-INFO
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3763 2023-06-14 07:04:47.000000 trajdata-1.3.2/src/trajdata.egg-info/SOURCES.txt
+-rw-r--r--   0 bivanovic (41443) dip         (30)        1 2023-06-14 07:04:47.000000 trajdata-1.3.2/src/trajdata.egg-info/dependency_links.txt
+-rw-r--r--   0 bivanovic (41443) dip         (30)      369 2023-06-14 07:04:47.000000 trajdata-1.3.2/src/trajdata.egg-info/requires.txt
+-rw-r--r--   0 bivanovic (41443) dip         (30)        9 2023-06-14 07:04:47.000000 trajdata-1.3.2/src/trajdata.egg-info/top_level.txt
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-06-14 07:04:47.227769 trajdata-1.3.2/tests/
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10463 2023-04-21 23:35:15.000000 trajdata-1.3.2/tests/test_batch_conversion.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     7443 2023-02-11 07:41:45.000000 trajdata-1.3.2/tests/test_collation.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     7569 2023-02-11 07:41:45.000000 trajdata-1.3.2/tests/test_datasizes.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      992 2022-11-17 10:42:27.000000 trajdata-1.3.2/tests/test_description_matching.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    13585 2023-02-11 07:41:45.000000 trajdata-1.3.2/tests/test_state.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     6304 2023-02-04 18:48:52.000000 trajdata-1.3.2/tests/test_traffic_data.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2068 2023-01-05 00:04:06.000000 trajdata-1.3.2/tests/test_vec_map.py
```

### Comparing `trajdata-1.3.1/LICENSE` & `trajdata-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/PKG-INFO` & `trajdata-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajdata
-Version: 1.3.1
+Version: 1.3.2
 Summary: A unified interface to many trajectory forecasting datasets.
 Home-page: https://github.com/nvr-avg/trajdata
 Author: Boris Ivanovic
 Author-email: bivanovic@nvidia.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: nusc
 Provides-Extra: lyft
 Provides-Extra: waymo
+Provides-Extra: interaction
 License-File: LICENSE
 
 # Unified Trajectory Data Loader
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -29,29 +30,32 @@
 ## Installation
 
 The easiest way to install trajdata is through PyPI with
 ```sh
 pip install trajdata
 ```
 
-In case you would also like to use datasets such as nuScenes, Lyft Level 5, or Waymo Open Motion Dataset (which require their own devkits to access raw data), the following will also install the respective devkits.
+In case you would also like to use datasets such as nuScenes, Lyft Level 5, or Waymo Open Motion Dataset (which require their own devkits to access raw data or additional package dependencies), the following will also install the respective devkits and/or package dependencies.
 ```sh
 # For nuScenes
 pip install "trajdata[nusc]"
 
 # For Lyft
 pip install "trajdata[lyft]"
 
 # For Waymo
 pip install "trajdata[waymo]"
 
+# For INTERACTION
+pip install "trajdata[interaction]"
+
 # All
-pip install "trajdata[nusc,lyft,waymo]"
+pip install "trajdata[nusc,lyft,waymo,interaction]"
 ```
-Then, download the raw datasets (nuScenes, Lyft Level 5, ETH/UCY, etc) in case you do not already have them. For more information about how to structure dataset folders/files, please see [`DATASETS.md`](./DATASETS.md).
+Then, download the raw datasets (nuScenes, Lyft Level 5, ETH/UCY, etc.) in case you do not already have them. For more information about how to structure dataset folders/files, please see [`DATASETS.md`](./DATASETS.md).
 
 ### Package Developer Installation
 
 First, in whichever environment you would like to use (conda, venv, ...), make sure to install all required dependencies with
 ```
 pip install -r requirements.txt
 ```
@@ -100,32 +104,35 @@
 For a more comprehensive example, please see `examples/batch_example.py`.
 
 For more information on all of the possible `UnifiedDataset` constructor arguments, please see `src/trajdata/dataset.py`.
 
 ## Supported Datasets
 Currently, the dataloader supports interfacing with the following datasets:
 
-| Dataset | ID | Splits | Add'l Tags | Description | dt | Maps |
+| Dataset | ID | Splits | Locations | Description | dt | Maps |
 |---------|----|--------|------------|-------------|----|------|
 | nuScenes Train/TrainVal/Val | `nusc_trainval` | `train`, `train_val`, `val` | `boston`, `singapore` | nuScenes prediction challenge training/validation/test splits (500/200/150 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuScenes Test | `nusc_test` | `test` | `boston`, `singapore` | nuScenes test split, no annotations (150 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuScenes Mini | `nusc_mini` | `mini_train`, `mini_val` | `boston`, `singapore` | nuScenes mini training/validation splits (8/2 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuPlan Mini | `nuplan_mini` | `mini_train`, `mini_val`, `mini_test` | `boston`, `singapore`, `pittsburgh`, `las_vegas` | nuPlan mini training/validation/test splits (942/197/224 scenes) | 0.05s (20Hz) | :white_check_mark: |
 | Waymo Open Motion Training | `waymo_train` | `train` | N/A | Waymo Open Motion Dataset `training` split | 0.1s (10Hz) | :white_check_mark: |
 | Waymo Open Motion Validation | `waymo_val` | `val` | N/A | Waymo Open Motion Dataset `validation` split | 0.1s (10Hz) | :white_check_mark: |
 | Waymo Open Motion Testing | `waymo_test` | `test` | N/A | Waymo Open Motion Dataset `testing` split | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Train | `lyft_train` | `train` | `palo_alto` | Lyft Level 5 training data - part 1/2 (8.4 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Train Full | `lyft_train_full` | `train` | `palo_alto` | Lyft Level 5 training data - part 2/2 (70 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Validation | `lyft_val` | `val` | `palo_alto` | Lyft Level 5 validation data (8.2 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Sample | `lyft_sample` | `mini_train`, `mini_val` | `palo_alto` | Lyft Level 5 sample data (100 scenes, randomly split 80/20 for training/validation) | 0.1s (10Hz) | :white_check_mark: |
+| INTERACTION Dataset Single-Agent | `interaction_single` | `train`, `val`, `test`, `test_conditional` | `usa`, `china`, `germany`, `bulgaria` | Single-agent split of the INTERACTION Dataset (where the goal is to predict one target agents' future motion) | 0.1s (10Hz) | :white_check_mark: |
+| INTERACTION Dataset Multi-Agent | `interaction_multi` | `train`, `val`, `test`, `test_conditional` | `usa`, `china`, `germany`, `bulgaria` | Multi-agent split of the INTERACTION Dataset (where the goal is to jointly predict multiple agents' future motion) | 0.1s (10Hz) | :white_check_mark: |
 | ETH - Univ | `eupeds_eth` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `zurich` | The ETH (University) scene from the ETH BIWI Walking Pedestrians dataset | 0.4s (2.5Hz) | |
 | ETH - Hotel | `eupeds_hotel` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `zurich` | The Hotel scene from the ETH BIWI Walking Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Univ | `eupeds_univ` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The University scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Zara1 | `eupeds_zara1` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The Zara1 scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Zara2 | `eupeds_zara2` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The Zara2 scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
+| Stanford Drone Dataset | `sdd` | `train`, `val`, `test` | `stanford` | Stanford Drone Dataset (60 scenes, randomly split 42/9/9 (70%/15%/15%) for training/validation/test) | 0.0333...s (30Hz) | |
 
 ### Adding New Datasets
 The code that interfaces the original datasets (dealing with their unique formats) can be found in `src/trajdata/dataset_specific`.
 
 To add a new dataset, one needs to:
 - Create a new folder under `src/trajdata/dataset_specific` which will contain all the code specific to a particular dataset (e.g., for extracting data into our canonical format). In particular, there must be:
   - An `__init__.py` file.
```

### Comparing `trajdata-1.3.1/README.md` & `trajdata-1.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 ## Installation
 
 The easiest way to install trajdata is through PyPI with
 ```sh
 pip install trajdata
 ```
 
-In case you would also like to use datasets such as nuScenes, Lyft Level 5, or Waymo Open Motion Dataset (which require their own devkits to access raw data), the following will also install the respective devkits.
+In case you would also like to use datasets such as nuScenes, Lyft Level 5, or Waymo Open Motion Dataset (which require their own devkits to access raw data or additional package dependencies), the following will also install the respective devkits and/or package dependencies.
 ```sh
 # For nuScenes
 pip install "trajdata[nusc]"
 
 # For Lyft
 pip install "trajdata[lyft]"
 
 # For Waymo
 pip install "trajdata[waymo]"
 
+# For INTERACTION
+pip install "trajdata[interaction]"
+
 # All
-pip install "trajdata[nusc,lyft,waymo]"
+pip install "trajdata[nusc,lyft,waymo,interaction]"
 ```
-Then, download the raw datasets (nuScenes, Lyft Level 5, ETH/UCY, etc) in case you do not already have them. For more information about how to structure dataset folders/files, please see [`DATASETS.md`](./DATASETS.md).
+Then, download the raw datasets (nuScenes, Lyft Level 5, ETH/UCY, etc.) in case you do not already have them. For more information about how to structure dataset folders/files, please see [`DATASETS.md`](./DATASETS.md).
 
 ### Package Developer Installation
 
 First, in whichever environment you would like to use (conda, venv, ...), make sure to install all required dependencies with
 ```
 pip install -r requirements.txt
 ```
@@ -80,32 +83,35 @@
 For a more comprehensive example, please see `examples/batch_example.py`.
 
 For more information on all of the possible `UnifiedDataset` constructor arguments, please see `src/trajdata/dataset.py`.
 
 ## Supported Datasets
 Currently, the dataloader supports interfacing with the following datasets:
 
-| Dataset | ID | Splits | Add'l Tags | Description | dt | Maps |
+| Dataset | ID | Splits | Locations | Description | dt | Maps |
 |---------|----|--------|------------|-------------|----|------|
 | nuScenes Train/TrainVal/Val | `nusc_trainval` | `train`, `train_val`, `val` | `boston`, `singapore` | nuScenes prediction challenge training/validation/test splits (500/200/150 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuScenes Test | `nusc_test` | `test` | `boston`, `singapore` | nuScenes test split, no annotations (150 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuScenes Mini | `nusc_mini` | `mini_train`, `mini_val` | `boston`, `singapore` | nuScenes mini training/validation splits (8/2 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuPlan Mini | `nuplan_mini` | `mini_train`, `mini_val`, `mini_test` | `boston`, `singapore`, `pittsburgh`, `las_vegas` | nuPlan mini training/validation/test splits (942/197/224 scenes) | 0.05s (20Hz) | :white_check_mark: |
 | Waymo Open Motion Training | `waymo_train` | `train` | N/A | Waymo Open Motion Dataset `training` split | 0.1s (10Hz) | :white_check_mark: |
 | Waymo Open Motion Validation | `waymo_val` | `val` | N/A | Waymo Open Motion Dataset `validation` split | 0.1s (10Hz) | :white_check_mark: |
 | Waymo Open Motion Testing | `waymo_test` | `test` | N/A | Waymo Open Motion Dataset `testing` split | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Train | `lyft_train` | `train` | `palo_alto` | Lyft Level 5 training data - part 1/2 (8.4 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Train Full | `lyft_train_full` | `train` | `palo_alto` | Lyft Level 5 training data - part 2/2 (70 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Validation | `lyft_val` | `val` | `palo_alto` | Lyft Level 5 validation data (8.2 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Sample | `lyft_sample` | `mini_train`, `mini_val` | `palo_alto` | Lyft Level 5 sample data (100 scenes, randomly split 80/20 for training/validation) | 0.1s (10Hz) | :white_check_mark: |
+| INTERACTION Dataset Single-Agent | `interaction_single` | `train`, `val`, `test`, `test_conditional` | `usa`, `china`, `germany`, `bulgaria` | Single-agent split of the INTERACTION Dataset (where the goal is to predict one target agents' future motion) | 0.1s (10Hz) | :white_check_mark: |
+| INTERACTION Dataset Multi-Agent | `interaction_multi` | `train`, `val`, `test`, `test_conditional` | `usa`, `china`, `germany`, `bulgaria` | Multi-agent split of the INTERACTION Dataset (where the goal is to jointly predict multiple agents' future motion) | 0.1s (10Hz) | :white_check_mark: |
 | ETH - Univ | `eupeds_eth` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `zurich` | The ETH (University) scene from the ETH BIWI Walking Pedestrians dataset | 0.4s (2.5Hz) | |
 | ETH - Hotel | `eupeds_hotel` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `zurich` | The Hotel scene from the ETH BIWI Walking Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Univ | `eupeds_univ` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The University scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Zara1 | `eupeds_zara1` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The Zara1 scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Zara2 | `eupeds_zara2` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The Zara2 scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
+| Stanford Drone Dataset | `sdd` | `train`, `val`, `test` | `stanford` | Stanford Drone Dataset (60 scenes, randomly split 42/9/9 (70%/15%/15%) for training/validation/test) | 0.0333...s (30Hz) | |
 
 ### Adding New Datasets
 The code that interfaces the original datasets (dealing with their unique formats) can be found in `src/trajdata/dataset_specific`.
 
 To add a new dataset, one needs to:
 - Create a new folder under `src/trajdata/dataset_specific` which will contain all the code specific to a particular dataset (e.g., for extracting data into our canonical format). In particular, there must be:
   - An `__init__.py` file.
```

### Comparing `trajdata-1.3.1/setup.cfg` & `trajdata-1.3.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trajdata
-version = 1.3.1
+version = 1.3.2
 author = Boris Ivanovic
 author_email = bivanovic@nvidia.com
 description = A unified interface to many trajectory forecasting datasets.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
 url = https://github.com/nvr-avg/trajdata
@@ -48,12 +48,14 @@
 lyft = 
 	protobuf==3.19.4
 	l5kit==1.5.0
 waymo = 
 	tensorflow==2.11.0
 	waymo-open-dataset-tf-2-11-0
 	intervaltree
+interaction = 
+	lanelet2==1.2.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trajdata-1.3.1/src/trajdata/augmentation/augmentation.py` & `trajdata-1.3.2/src/trajdata/augmentation/augmentation.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/augmentation/low_vel_yaw_correction.py` & `trajdata-1.3.2/src/trajdata/augmentation/low_vel_yaw_correction.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/augmentation/noise_histories.py` & `trajdata-1.3.2/src/trajdata/augmentation/noise_histories.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/caching/df_cache.py` & `trajdata-1.3.2/src/trajdata/caching/df_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/caching/env_cache.py` & `trajdata-1.3.2/src/trajdata/caching/env_cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,28 @@
         scene_cache_dir.mkdir(parents=True, exist_ok=True)
 
         with open(scene_file, "wb") as f:
             dill.dump(scene, f)
 
         return scene_file
 
+    @staticmethod
+    def save_scene_with_path(base_path: Path, scene: Scene) -> Path:
+        scene_file: Path = EnvCache.scene_metadata_path(
+            base_path, scene.env_name, scene.name, scene.dt
+        )
+
+        scene_cache_dir: Path = scene_file.parent
+        scene_cache_dir.mkdir(parents=True, exist_ok=True)
+
+        with open(scene_file, "wb") as f:
+            dill.dump(scene, f)
+
+        return scene_file
+
     def load_env_scenes_list(self, env_name: str) -> List[NamedTuple]:
         env_cache_dir: Path = self.path / env_name
         with open(env_cache_dir / "scenes_list.dill", "rb") as f:
             scenes_list: List[NamedTuple] = dill.load(f)
 
         return scenes_list
```

### Comparing `trajdata-1.3.1/src/trajdata/caching/scene_cache.py` & `trajdata-1.3.2/src/trajdata/caching/scene_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/__init__.py` & `trajdata-1.3.2/src/trajdata/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/agent.py` & `trajdata-1.3.2/src/trajdata/data_structures/agent.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/batch.py` & `trajdata-1.3.2/src/trajdata/data_structures/batch.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/batch_element.py` & `trajdata-1.3.2/src/trajdata/data_structures/batch_element.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/collation.py` & `trajdata-1.3.2/src/trajdata/data_structures/collation.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/data_index.py` & `trajdata-1.3.2/src/trajdata/data_structures/data_index.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/environment.py` & `trajdata-1.3.2/src/trajdata/data_structures/environment.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/scene.py` & `trajdata-1.3.2/src/trajdata/data_structures/scene.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/scene_metadata.py` & `trajdata-1.3.2/src/trajdata/data_structures/scene_metadata.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/data_structures/state.py` & `trajdata-1.3.2/src/trajdata/data_structures/state.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset.py` & `trajdata-1.3.2/src/trajdata/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import gc
+import random
 import time
 from collections import defaultdict
 from functools import partial
 from itertools import chain
 from os.path import isfile
 from pathlib import Path
 from typing import (
@@ -700,15 +701,17 @@
     def get_desired_scenes_from_env(
         self,
         scene_tags: List[SceneTag],
         scene_description_contains: Optional[List[str]],
         env: RawDataset,
     ) -> Union[List[Scene], List[SceneMetadata]]:
         scenes_list: Union[List[Scene], List[SceneMetadata]] = list()
-        for scene_tag in scene_tags:
+        for scene_tag in tqdm(
+            scene_tags, desc=f"Getting Scenes from {env.name}", disable=not self.verbose
+        ):
             if env.name in scene_tag:
                 scenes_list += env.get_matching_scenes(
                     scene_tag,
                     scene_description_contains,
                     self.env_cache,
                     self.rebuild_cache,
                 )
@@ -738,14 +741,18 @@
                 if not self.envs_dict[scene_info.env_name].parallelizable
             ]
             parallel_scenes = [
                 scene_info
                 for scene_info in scenes_list
                 if self.envs_dict[scene_info.env_name].parallelizable
             ]
+
+            # Fixing the seed for random suffling (for debugging and reproducibility).
+            shuffle_rng = random.Random(123)
+            shuffle_rng.shuffle(parallel_scenes)
         else:
             serial_scenes = scenes_list
             parallel_scenes = list()
 
         # List of (Original cached path, Temporary cached path)
         scene_paths: List[Path] = list()
         if serial_scenes:
```

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/lyft/lyft_dataset.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/lyft/lyft_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/lyft/lyft_utils.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/lyft/lyft_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/nuplan/nuplan_dataset.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/nuplan/nuplan_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/nuplan/nuplan_utils.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/nuplan/nuplan_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/nusc/nusc_dataset.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/nusc/nusc_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/nusc/nusc_utils.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/nusc/nusc_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/raw_dataset.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/raw_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/scene_records.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/scene_records.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,26 @@
     name: str
     location: str
     length: str
     split: str
     data_idx: int
 
 
+class SDDPedsRecord(NamedTuple):
+    name: str
+    length: str
+    data_idx: int
+
+
+class InteractionRecord(NamedTuple):
+    name: str
+    length: str
+    data_idx: int
+
+
 class NuscSceneRecord(NamedTuple):
     name: str
     location: str
     length: str
     desc: str
     data_idx: int
```

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/waymo/waymo_dataset.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/waymo/waymo_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/dataset_specific/waymo/waymo_utils.py` & `trajdata-1.3.2/src/trajdata/dataset_specific/waymo/waymo_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/filtering/filters.py` & `trajdata-1.3.2/src/trajdata/filtering/filters.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/maps/map_api.py` & `trajdata-1.3.2/src/trajdata/maps/map_api.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/maps/map_kdtree.py` & `trajdata-1.3.2/src/trajdata/maps/map_kdtree.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/maps/raster_map.py` & `trajdata-1.3.2/src/trajdata/maps/raster_map.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/maps/vec_map.py` & `trajdata-1.3.2/src/trajdata/maps/vec_map.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/maps/vec_map_elements.py` & `trajdata-1.3.2/src/trajdata/maps/vec_map_elements.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/parallel/data_preprocessor.py` & `trajdata-1.3.2/src/trajdata/parallel/data_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Dict, List, Optional, Type
+from typing import Dict, List, Optional, Tuple, Type
 
 import numpy as np
 from torch.utils.data import Dataset
 
 from trajdata.caching import EnvCache, SceneCache
 from trajdata.data_structures import Scene, SceneMetadata
 from trajdata.utils import agent_utils, env_utils
@@ -25,28 +25,28 @@
     ) -> None:
         self.env_cache_path = np.array(env_cache_path).astype(np.string_)
         self.desired_dt = desired_dt
         self.cache_class = cache_class
         self.rebuild_cache = rebuild_cache
 
         env_names: List[str] = list(envs_dir_dict.keys())
-        scene_names: List[str] = [scene_info.name for scene_info in scene_info_list]
+        scene_idxs_names: List[Tuple[int, str]] = [
+            (idx, scene_info.name) for idx, scene_info in enumerate(scene_info_list)
+        ]
+        scene_name_idxs, scene_names = zip(*scene_idxs_names)
 
         self.scene_idxs = np.array(
             [scene_info.raw_data_idx for scene_info in scene_info_list], dtype=int
         )
         self.env_name_idxs = np.array(
             [env_names.index(scene_info.env_name) for scene_info in scene_info_list],
             dtype=int,
         )
-        self.scene_name_idxs = np.array(
-            [scene_names.index(scene_info.name) for scene_info in scene_info_list],
-            dtype=int,
-        )
 
+        self.scene_name_idxs = np.array(scene_name_idxs, dtype=int)
         self.env_names_arr = np.array(env_names).astype(np.string_)
         self.scene_names_arr = np.array(scene_names).astype(np.string_)
         self.data_dir_arr = np.array(list(envs_dir_dict.values())).astype(np.string_)
 
         self.data_len: int = len(scene_info_list)
 
     def __len__(self) -> int:
```

### Comparing `trajdata-1.3.1/src/trajdata/proto/vectorized_map_pb2.py` & `trajdata-1.3.2/src/trajdata/proto/vectorized_map_pb2.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/simulation/sim_cache.py` & `trajdata-1.3.2/src/trajdata/simulation/sim_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/simulation/sim_df_cache.py` & `trajdata-1.3.2/src/trajdata/simulation/sim_df_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/simulation/sim_metrics.py` & `trajdata-1.3.2/src/trajdata/simulation/sim_metrics.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/simulation/sim_scene.py` & `trajdata-1.3.2/src/trajdata/simulation/sim_scene.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/simulation/sim_stats.py` & `trajdata-1.3.2/src/trajdata/simulation/sim_stats.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/simulation/sim_vis.py` & `trajdata-1.3.2/src/trajdata/simulation/sim_vis.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/agent_utils.py` & `trajdata-1.3.2/src/trajdata/utils/agent_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/arr_utils.py` & `trajdata-1.3.2/src/trajdata/utils/arr_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/batch_utils.py` & `trajdata-1.3.2/src/trajdata/utils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/df_utils.py` & `trajdata-1.3.2/src/trajdata/utils/df_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/env_utils.py` & `trajdata-1.3.2/src/trajdata/utils/env_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import Dict, List
 
 from trajdata.dataset_specific.eth_ucy_peds import EUPedsDataset
+from trajdata.dataset_specific.interaction import InteractionDataset
 from trajdata.dataset_specific.raw_dataset import RawDataset
+from trajdata.dataset_specific.sdd_peds import SDDPedsDataset
 
 try:
     from trajdata.dataset_specific.lyft import LyftDataset
 except ModuleNotFoundError:
     # This can happen if the user did not install trajdata
     # with the "trajdata[lyft]" option.
     pass
@@ -41,20 +43,30 @@
         return LyftDataset(dataset_name, data_dir, parallelizable=True, has_maps=True)
 
     if "eupeds" in dataset_name:
         return EUPedsDataset(
             dataset_name, data_dir, parallelizable=True, has_maps=False
         )
 
+    if "sdd" in dataset_name:
+        return SDDPedsDataset(
+            dataset_name, data_dir, parallelizable=True, has_maps=False
+        )
+
     if "nuplan" in dataset_name:
         return NuplanDataset(dataset_name, data_dir, parallelizable=True, has_maps=True)
 
     if "waymo" in dataset_name:
         return WaymoDataset(dataset_name, data_dir, parallelizable=True, has_maps=True)
 
+    if "interaction" in dataset_name:
+        return InteractionDataset(
+            dataset_name, data_dir, parallelizable=True, has_maps=True
+        )
+
     raise ValueError(f"Dataset with name '{dataset_name}' is not supported")
 
 
 def get_raw_datasets(data_dirs: Dict[str, str]) -> List[RawDataset]:
     raw_datasets: List[RawDataset] = list()
 
     for dataset_name, data_dir in data_dirs.items():
```

### Comparing `trajdata-1.3.1/src/trajdata/utils/map_utils.py` & `trajdata-1.3.2/src/trajdata/utils/map_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/parallel_utils.py` & `trajdata-1.3.2/src/trajdata/utils/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/raster_utils.py` & `trajdata-1.3.2/src/trajdata/utils/raster_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/scene_utils.py` & `trajdata-1.3.2/src/trajdata/utils/scene_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/state_utils.py` & `trajdata-1.3.2/src/trajdata/utils/state_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/utils/vis_utils.py` & `trajdata-1.3.2/src/trajdata/utils/vis_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/visualization/interactive_animation.py` & `trajdata-1.3.2/src/trajdata/visualization/interactive_animation.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/visualization/interactive_figure.py` & `trajdata-1.3.2/src/trajdata/visualization/interactive_figure.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/visualization/interactive_vis.py` & `trajdata-1.3.2/src/trajdata/visualization/interactive_vis.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/src/trajdata/visualization/vis.py` & `trajdata-1.3.2/src/trajdata/visualization/vis.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     close: bool = True,
 ) -> None:
     if ax is None:
         _, ax = plt.subplots()
 
     agent_name: str = batch.agent_name[batch_idx]
     agent_type: AgentType = AgentType(batch.agent_type[batch_idx].item())
-    current_state = batch.curr_agent_state[batch_idx].numpy()
+    current_state = batch.curr_agent_state[batch_idx].cpu().numpy()
     ax.set_title(
         f"{str(agent_type)}/{agent_name}\nat x={current_state[0]:.2f},y={current_state[1]:.2f},h={current_state[-1]:.2f}"
     )
 
     agent_from_world_tf: Tensor = batch.agents_from_world_tf[batch_idx].cpu()
 
     if batch.maps is not None:
```

### Comparing `trajdata-1.3.1/src/trajdata.egg-info/PKG-INFO` & `trajdata-1.3.2/src/trajdata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajdata
-Version: 1.3.1
+Version: 1.3.2
 Summary: A unified interface to many trajectory forecasting datasets.
 Home-page: https://github.com/nvr-avg/trajdata
 Author: Boris Ivanovic
 Author-email: bivanovic@nvidia.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: nusc
 Provides-Extra: lyft
 Provides-Extra: waymo
+Provides-Extra: interaction
 License-File: LICENSE
 
 # Unified Trajectory Data Loader
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
@@ -29,29 +30,32 @@
 ## Installation
 
 The easiest way to install trajdata is through PyPI with
 ```sh
 pip install trajdata
 ```
 
-In case you would also like to use datasets such as nuScenes, Lyft Level 5, or Waymo Open Motion Dataset (which require their own devkits to access raw data), the following will also install the respective devkits.
+In case you would also like to use datasets such as nuScenes, Lyft Level 5, or Waymo Open Motion Dataset (which require their own devkits to access raw data or additional package dependencies), the following will also install the respective devkits and/or package dependencies.
 ```sh
 # For nuScenes
 pip install "trajdata[nusc]"
 
 # For Lyft
 pip install "trajdata[lyft]"
 
 # For Waymo
 pip install "trajdata[waymo]"
 
+# For INTERACTION
+pip install "trajdata[interaction]"
+
 # All
-pip install "trajdata[nusc,lyft,waymo]"
+pip install "trajdata[nusc,lyft,waymo,interaction]"
 ```
-Then, download the raw datasets (nuScenes, Lyft Level 5, ETH/UCY, etc) in case you do not already have them. For more information about how to structure dataset folders/files, please see [`DATASETS.md`](./DATASETS.md).
+Then, download the raw datasets (nuScenes, Lyft Level 5, ETH/UCY, etc.) in case you do not already have them. For more information about how to structure dataset folders/files, please see [`DATASETS.md`](./DATASETS.md).
 
 ### Package Developer Installation
 
 First, in whichever environment you would like to use (conda, venv, ...), make sure to install all required dependencies with
 ```
 pip install -r requirements.txt
 ```
@@ -100,32 +104,35 @@
 For a more comprehensive example, please see `examples/batch_example.py`.
 
 For more information on all of the possible `UnifiedDataset` constructor arguments, please see `src/trajdata/dataset.py`.
 
 ## Supported Datasets
 Currently, the dataloader supports interfacing with the following datasets:
 
-| Dataset | ID | Splits | Add'l Tags | Description | dt | Maps |
+| Dataset | ID | Splits | Locations | Description | dt | Maps |
 |---------|----|--------|------------|-------------|----|------|
 | nuScenes Train/TrainVal/Val | `nusc_trainval` | `train`, `train_val`, `val` | `boston`, `singapore` | nuScenes prediction challenge training/validation/test splits (500/200/150 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuScenes Test | `nusc_test` | `test` | `boston`, `singapore` | nuScenes test split, no annotations (150 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuScenes Mini | `nusc_mini` | `mini_train`, `mini_val` | `boston`, `singapore` | nuScenes mini training/validation splits (8/2 scenes) | 0.5s (2Hz) | :white_check_mark: |
 | nuPlan Mini | `nuplan_mini` | `mini_train`, `mini_val`, `mini_test` | `boston`, `singapore`, `pittsburgh`, `las_vegas` | nuPlan mini training/validation/test splits (942/197/224 scenes) | 0.05s (20Hz) | :white_check_mark: |
 | Waymo Open Motion Training | `waymo_train` | `train` | N/A | Waymo Open Motion Dataset `training` split | 0.1s (10Hz) | :white_check_mark: |
 | Waymo Open Motion Validation | `waymo_val` | `val` | N/A | Waymo Open Motion Dataset `validation` split | 0.1s (10Hz) | :white_check_mark: |
 | Waymo Open Motion Testing | `waymo_test` | `test` | N/A | Waymo Open Motion Dataset `testing` split | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Train | `lyft_train` | `train` | `palo_alto` | Lyft Level 5 training data - part 1/2 (8.4 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Train Full | `lyft_train_full` | `train` | `palo_alto` | Lyft Level 5 training data - part 2/2 (70 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Validation | `lyft_val` | `val` | `palo_alto` | Lyft Level 5 validation data (8.2 GB) | 0.1s (10Hz) | :white_check_mark: |
 | Lyft Level 5 Sample | `lyft_sample` | `mini_train`, `mini_val` | `palo_alto` | Lyft Level 5 sample data (100 scenes, randomly split 80/20 for training/validation) | 0.1s (10Hz) | :white_check_mark: |
+| INTERACTION Dataset Single-Agent | `interaction_single` | `train`, `val`, `test`, `test_conditional` | `usa`, `china`, `germany`, `bulgaria` | Single-agent split of the INTERACTION Dataset (where the goal is to predict one target agents' future motion) | 0.1s (10Hz) | :white_check_mark: |
+| INTERACTION Dataset Multi-Agent | `interaction_multi` | `train`, `val`, `test`, `test_conditional` | `usa`, `china`, `germany`, `bulgaria` | Multi-agent split of the INTERACTION Dataset (where the goal is to jointly predict multiple agents' future motion) | 0.1s (10Hz) | :white_check_mark: |
 | ETH - Univ | `eupeds_eth` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `zurich` | The ETH (University) scene from the ETH BIWI Walking Pedestrians dataset | 0.4s (2.5Hz) | |
 | ETH - Hotel | `eupeds_hotel` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `zurich` | The Hotel scene from the ETH BIWI Walking Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Univ | `eupeds_univ` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The University scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Zara1 | `eupeds_zara1` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The Zara1 scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
 | UCY - Zara2 | `eupeds_zara2` | `train`, `val`, `train_loo`, `val_loo`, `test_loo` | `cyprus` | The Zara2 scene from the UCY Pedestrians dataset | 0.4s (2.5Hz) | |
+| Stanford Drone Dataset | `sdd` | `train`, `val`, `test` | `stanford` | Stanford Drone Dataset (60 scenes, randomly split 42/9/9 (70%/15%/15%) for training/validation/test) | 0.0333...s (30Hz) | |
 
 ### Adding New Datasets
 The code that interfaces the original datasets (dealing with their unique formats) can be found in `src/trajdata/dataset_specific`.
 
 To add a new dataset, one needs to:
 - Create a new folder under `src/trajdata/dataset_specific` which will contain all the code specific to a particular dataset (e.g., for extracting data into our canonical format). In particular, there must be:
   - An `__init__.py` file.
```

### Comparing `trajdata-1.3.1/src/trajdata.egg-info/SOURCES.txt` & `trajdata-1.3.2/src/trajdata.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,23 +29,28 @@
 src/trajdata/data_structures/scene_tag.py
 src/trajdata/data_structures/state.py
 src/trajdata/dataset_specific/__init__.py
 src/trajdata/dataset_specific/raw_dataset.py
 src/trajdata/dataset_specific/scene_records.py
 src/trajdata/dataset_specific/eth_ucy_peds/__init__.py
 src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py
+src/trajdata/dataset_specific/interaction/__init__.py
+src/trajdata/dataset_specific/interaction/interaction_dataset.py
 src/trajdata/dataset_specific/lyft/__init__.py
 src/trajdata/dataset_specific/lyft/lyft_dataset.py
 src/trajdata/dataset_specific/lyft/lyft_utils.py
 src/trajdata/dataset_specific/nuplan/__init__.py
 src/trajdata/dataset_specific/nuplan/nuplan_dataset.py
 src/trajdata/dataset_specific/nuplan/nuplan_utils.py
 src/trajdata/dataset_specific/nusc/__init__.py
 src/trajdata/dataset_specific/nusc/nusc_dataset.py
 src/trajdata/dataset_specific/nusc/nusc_utils.py
+src/trajdata/dataset_specific/sdd_peds/__init__.py
+src/trajdata/dataset_specific/sdd_peds/estimated_homography.py
+src/trajdata/dataset_specific/sdd_peds/sddpeds_dataset.py
 src/trajdata/dataset_specific/waymo/__init__.py
 src/trajdata/dataset_specific/waymo/waymo_dataset.py
 src/trajdata/dataset_specific/waymo/waymo_utils.py
 src/trajdata/filtering/__init__.py
 src/trajdata/filtering/filters.py
 src/trajdata/maps/__init__.py
 src/trajdata/maps/lane_route.py
```

### Comparing `trajdata-1.3.1/tests/test_batch_conversion.py` & `trajdata-1.3.2/tests/test_batch_conversion.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/tests/test_collation.py` & `trajdata-1.3.2/tests/test_collation.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/tests/test_datasizes.py` & `trajdata-1.3.2/tests/test_datasizes.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/tests/test_description_matching.py` & `trajdata-1.3.2/tests/test_description_matching.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/tests/test_state.py` & `trajdata-1.3.2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/tests/test_traffic_data.py` & `trajdata-1.3.2/tests/test_traffic_data.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.3.1/tests/test_vec_map.py` & `trajdata-1.3.2/tests/test_vec_map.py`

 * *Files identical despite different names*

