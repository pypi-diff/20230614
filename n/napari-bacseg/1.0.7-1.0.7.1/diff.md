# Comparing `tmp/napari-bacseg-1.0.7.tar.gz` & `tmp/napari-bacseg-1.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-bacseg-1.0.7.tar", last modified: Tue Jun 13 16:26:18 2023, max compression
+gzip compressed data, was "napari-bacseg-1.0.7.1.tar", last modified: Tue Jun 13 16:49:52 2023, max compression
```

## Comparing `napari-bacseg-1.0.7.tar` & `napari-bacseg-1.0.7.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.249218 napari-bacseg-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:17.997889 napari-bacseg-1.0.7/.github/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.033792 napari-bacseg-1.0.7/.github/workflows/
--rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.7/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.037782 napari-bacseg-1.0.7/.napari-hub/
--rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/.napari-hub/DESCRIPTION.md
--rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/.napari-hub/config.yml
--rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.7/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4732 2023-06-13 16:26:18.249218 napari-bacseg-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/README.md
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/bacseg_ui.py
--rw-rw-rw-   0        0        0      988 2023-06-13 16:26:05.000000 napari-bacseg-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0     2035 2023-06-13 16:26:18.252210 napari-bacseg-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:17.998886 napari-bacseg-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.181398 napari-bacseg-1.0.7/src/_dev/
--rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.7/src/_dev/Export Masks to AKSEG v5 dev.py
--rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7/src/_dev/ScanR dev.py
--rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.7/src/_dev/Troodos dev.py
--rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.7/src/_dev/__init__.py
--rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.7/src/_dev/akseg_db_stats.py
--rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/akseg_dev.py
--rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/akseg_dev2.py
--rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.7/src/_dev/akseg_txt_metadata.py
--rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/align_alex_datadump.py
--rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/alison_datadump.py
--rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7/src/_dev/autocontast_dev.py
--rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/cellposedev.py
--rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.7/src/_dev/cellposeshapely.py
--rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.7/src/_dev/chatGPT_midlines.py
--rw-rw-rw-   0        0        0     6105 2023-05-05 10:49:23.000000 napari-bacseg-1.0.7/src/_dev/check_AluGasketv12_DFP.py
--rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/check_metadata.py
--rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7/src/_dev/colicoords_cellldist_dev.py
--rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7/src/_dev/colicoords_ldist_dev.py
--rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.7/src/_dev/database_dev.py
--rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.7/src/_dev/deepsegmattest.py
--rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.7/src/_dev/edit_database_columns.py
--rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.7/src/_dev/fits_dev.py
--rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/fix_alison_missing_file_list.py
--rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/generate_scanr_movie.py
--rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/get_akseg_stats.py
--rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.7/src/_dev/get_species_info.py
--rw-rw-rw-   0        0        0     1991 2023-06-13 13:41:08.000000 napari-bacseg-1.0.7/src/_dev/imagej_dev.py
--rw-rw-rw-   0        0        0     5034 2023-06-13 08:40:50.000000 napari-bacseg-1.0.7/src/_dev/json_nuclei_dev.py
--rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/luke__script.py
--rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.7/src/_dev/matplotlib_Events.py
--rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.7/src/_dev/move_AluGasketDFP.py
--rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.7/src/_dev/move_AluGasketDFP_poster.py
--rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.7/src/_dev/move_AluGasketv12_DFP.py
--rw-rw-rw-   0        0        0    46551 2023-05-05 08:15:07.000000 napari-bacseg-1.0.7/src/_dev/move_AluGasketv12_DFP_Titration.py
--rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.7/src/_dev/move_conor_nim_dfp_data.py
--rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.7/src/_dev/move_pillar_data.py
--rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/move_pillar_zstack_data.py
--rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7/src/_dev/move_unlearning_files.py
--rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.7/src/_dev/new_metadata2.pickle.py
--rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7/src/_dev/new_read_akseg_directory.py
--rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/nim_dev.py
--rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/omnipose_dev.py
--rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7/src/_dev/omnipose_midlines.py
--rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7/src/_dev/omnipose_train.py
--rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7/src/_dev/oufti_dilate.py
--rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.7/src/_dev/oufti_dilate_with_midlines.py
--rw-rw-rw-   0        0        0     4449 2023-05-04 09:42:23.000000 napari-bacseg-1.0.7/src/_dev/pandas_speed.py
--rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/process_alex_datadump.py
--rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/process_alex_datadump_clinical.py
--rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/process_conor_datadump.py
--rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/process_gramstain_datadump.py
--rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.7/src/_dev/read_non_tif.py
--rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/rebuild_usermeta.py
--rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/rebuild_usermeta_2.py
--rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.7/src/_dev/recreate_user_metadata.py
--rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.7/src/_dev/scalebar_dev.py
--rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/sort_midlines.py
--rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/stelios_stats.py
--rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/tile_meta_check.py
--rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.7/src/_dev/tiler_dev.py
--rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7/src/_dev/updade_akseg_metadata.py
--rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.7/src/_dev/update_img_metadata.py
--rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7/src/_dev/video_iamges.py
--rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.7/src/_dev/zooniverse.py
--rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_move.py
--rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_move_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_titration_upload.py
--rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_titrations.py
--rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.7/src/_dev/zooniverse_upload.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.221292 napari-bacseg-1.0.7/src/napari_bacseg/
--rw-rw-rw-   0        0        0      155 2023-06-13 16:18:00.000000 napari-bacseg-1.0.7/src/napari_bacseg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.247223 napari-bacseg-1.0.7/src/napari_bacseg/_tests/
--rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/src/napari_bacseg/_tests/__init__.py
--rw-rw-rw-   0        0        0    26817 2023-06-13 13:36:57.000000 napari-bacseg-1.0.7/src/napari_bacseg/_tests/test_bacseg.py
--rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_tests/test_widget.py
--rw-rw-rw-   0        0        0    90731 2023-06-13 16:07:22.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils.py
--rw-rw-rw-   0        0        0    14723 2023-06-13 08:44:12.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_cellpose.py
--rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_colicoords.py
--rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_database.py
--rw-rw-rw-   0        0        0    47487 2023-06-13 09:49:45.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_database_IO.py
--rw-rw-rw-   0        0        0     1670 2023-06-13 13:50:19.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_imagej.py
--rw-rw-rw-   0        0        0    40215 2023-06-13 08:44:13.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_interface_events.py
--rw-rw-rw-   0        0        0     6485 2023-06-13 08:44:12.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_json.py
--rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_oufti.py
--rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_refine.py
--rw-rw-rw-   0        0        0    22517 2023-06-09 14:18:42.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_statistics.py
--rw-rw-rw-   0        0        0     7837 2023-06-09 14:18:42.000000 napari-bacseg-1.0.7/src/napari_bacseg/_utils_tiler.py
--rw-rw-rw-   0        0        0      218 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg/_version.py
--rw-rw-rw-   0        0        0    83296 2023-06-13 15:33:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/_widget.py
--rw-rw-rw-   0        0        0   172700 2023-06-13 16:10:14.000000 napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.py
--rw-rw-rw-   0        0        0   172251 2023-06-13 16:10:08.000000 napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.ui
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/gapseq_ui.py
--rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.7/src/napari_bacseg/napari.yaml
--rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7/src/napari_bacseg/napari_ui.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:26:18.242236 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/
--rw-rw-rw-   0        0        0     4732 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      352 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-13 16:26:17.000000 napari-bacseg-1.0.7/src/napari_bacseg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7/tox.ini
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.450077 napari-bacseg-1.0.7.1/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.249487 napari-bacseg-1.0.7.1/.github/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.268898 napari-bacseg-1.0.7.1/.github/workflows/
+-rw-rw-rw-   0        0        0     2904 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7.1/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1239 2023-03-08 16:30:28.000000 napari-bacseg-1.0.7.1/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.271890 napari-bacseg-1.0.7.1/.napari-hub/
+-rw-rw-rw-   0        0        0      472 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7.1/.napari-hub/DESCRIPTION.md
+-rw-rw-rw-   0        0        0      551 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7.1/.napari-hub/config.yml
+-rw-rw-rw-   0        0        0     1211 2023-02-24 11:01:10.000000 napari-bacseg-1.0.7.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1515 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7.1/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4734 2023-06-13 16:49:52.451074 napari-bacseg-1.0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3859 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7.1/README.md
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7.1/bacseg_ui.py
+-rw-rw-rw-   0        0        0      990 2023-06-13 16:48:48.000000 napari-bacseg-1.0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2035 2023-06-13 16:49:52.453069 napari-bacseg-1.0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.251588 napari-bacseg-1.0.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.392231 napari-bacseg-1.0.7.1/src/_dev/
+-rw-rw-rw-   0        0        0      560 2022-10-16 10:26:58.000000 napari-bacseg-1.0.7.1/src/_dev/Export Masks to AKSEG v5 dev.py
+-rw-rw-rw-   0        0        0     8279 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7.1/src/_dev/ScanR dev.py
+-rw-rw-rw-   0        0        0      482 2022-05-26 11:42:59.000000 napari-bacseg-1.0.7.1/src/_dev/Troodos dev.py
+-rw-rw-rw-   0        0        0        0 2022-04-28 17:23:51.000000 napari-bacseg-1.0.7.1/src/_dev/__init__.py
+-rw-rw-rw-   0        0        0     1878 2023-02-24 12:15:54.000000 napari-bacseg-1.0.7.1/src/_dev/akseg_db_stats.py
+-rw-rw-rw-   0        0        0    11262 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/akseg_dev.py
+-rw-rw-rw-   0        0        0     4463 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/akseg_dev2.py
+-rw-rw-rw-   0        0        0    10114 2023-02-24 14:36:34.000000 napari-bacseg-1.0.7.1/src/_dev/akseg_txt_metadata.py
+-rw-rw-rw-   0        0        0    10960 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/align_alex_datadump.py
+-rw-rw-rw-   0        0        0    28052 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/alison_datadump.py
+-rw-rw-rw-   0        0        0     4168 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7.1/src/_dev/autocontast_dev.py
+-rw-rw-rw-   0        0        0      454 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/cellposedev.py
+-rw-rw-rw-   0        0        0      367 2022-09-22 16:01:43.000000 napari-bacseg-1.0.7.1/src/_dev/cellposeshapely.py
+-rw-rw-rw-   0        0        0     1279 2023-03-27 16:45:42.000000 napari-bacseg-1.0.7.1/src/_dev/chatGPT_midlines.py
+-rw-rw-rw-   0        0        0     6105 2023-05-05 10:49:23.000000 napari-bacseg-1.0.7.1/src/_dev/check_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0     6452 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/check_metadata.py
+-rw-rw-rw-   0        0        0     1650 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7.1/src/_dev/colicoords_cellldist_dev.py
+-rw-rw-rw-   0        0        0     3442 2023-02-24 14:19:11.000000 napari-bacseg-1.0.7.1/src/_dev/colicoords_ldist_dev.py
+-rw-rw-rw-   0        0        0    11185 2023-02-24 14:36:34.000000 napari-bacseg-1.0.7.1/src/_dev/database_dev.py
+-rw-rw-rw-   0        0        0     1023 2023-03-23 14:05:20.000000 napari-bacseg-1.0.7.1/src/_dev/deepsegmattest.py
+-rw-rw-rw-   0        0        0      666 2023-03-22 14:37:10.000000 napari-bacseg-1.0.7.1/src/_dev/edit_database_columns.py
+-rw-rw-rw-   0        0        0     1701 2023-02-24 12:15:54.000000 napari-bacseg-1.0.7.1/src/_dev/fits_dev.py
+-rw-rw-rw-   0        0        0     7216 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/fix_alison_missing_file_list.py
+-rw-rw-rw-   0        0        0     1126 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/generate_scanr_movie.py
+-rw-rw-rw-   0        0        0    24393 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/get_akseg_stats.py
+-rw-rw-rw-   0        0        0     2623 2022-11-14 15:25:24.000000 napari-bacseg-1.0.7.1/src/_dev/get_species_info.py
+-rw-rw-rw-   0        0        0     1991 2023-06-13 13:41:08.000000 napari-bacseg-1.0.7.1/src/_dev/imagej_dev.py
+-rw-rw-rw-   0        0        0     5034 2023-06-13 08:40:50.000000 napari-bacseg-1.0.7.1/src/_dev/json_nuclei_dev.py
+-rw-rw-rw-   0        0        0     4255 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/luke__script.py
+-rw-rw-rw-   0        0        0     5550 2023-02-24 14:21:12.000000 napari-bacseg-1.0.7.1/src/_dev/matplotlib_Events.py
+-rw-rw-rw-   0        0        0    40825 2023-03-22 17:47:52.000000 napari-bacseg-1.0.7.1/src/_dev/move_AluGasketDFP.py
+-rw-rw-rw-   0        0        0    44028 2023-04-04 10:28:53.000000 napari-bacseg-1.0.7.1/src/_dev/move_AluGasketDFP_poster.py
+-rw-rw-rw-   0        0        0    48241 2023-04-26 15:22:38.000000 napari-bacseg-1.0.7.1/src/_dev/move_AluGasketv12_DFP.py
+-rw-rw-rw-   0        0        0    46551 2023-05-05 08:15:07.000000 napari-bacseg-1.0.7.1/src/_dev/move_AluGasketv12_DFP_Titration.py
+-rw-rw-rw-   0        0        0    35330 2023-03-13 15:20:23.000000 napari-bacseg-1.0.7.1/src/_dev/move_conor_nim_dfp_data.py
+-rw-rw-rw-   0        0        0    34295 2023-03-08 10:06:11.000000 napari-bacseg-1.0.7.1/src/_dev/move_pillar_data.py
+-rw-rw-rw-   0        0        0    37169 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/move_pillar_zstack_data.py
+-rw-rw-rw-   0        0        0    57720 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7.1/src/_dev/move_unlearning_files.py
+-rw-rw-rw-   0        0        0      686 2023-02-14 15:45:10.000000 napari-bacseg-1.0.7.1/src/_dev/new_metadata2.pickle.py
+-rw-rw-rw-   0        0        0     5989 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7.1/src/_dev/new_read_akseg_directory.py
+-rw-rw-rw-   0        0        0     7222 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/nim_dev.py
+-rw-rw-rw-   0        0        0     3173 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/omnipose_dev.py
+-rw-rw-rw-   0        0        0     4398 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7.1/src/_dev/omnipose_midlines.py
+-rw-rw-rw-   0        0        0     3032 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7.1/src/_dev/omnipose_train.py
+-rw-rw-rw-   0        0        0    33520 2023-02-24 14:29:03.000000 napari-bacseg-1.0.7.1/src/_dev/oufti_dilate.py
+-rw-rw-rw-   0        0        0    37571 2023-03-06 10:55:01.000000 napari-bacseg-1.0.7.1/src/_dev/oufti_dilate_with_midlines.py
+-rw-rw-rw-   0        0        0     4449 2023-05-04 09:42:23.000000 napari-bacseg-1.0.7.1/src/_dev/pandas_speed.py
+-rw-rw-rw-   0        0        0    32011 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/process_alex_datadump.py
+-rw-rw-rw-   0        0        0    32643 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/process_alex_datadump_clinical.py
+-rw-rw-rw-   0        0        0    28804 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/process_conor_datadump.py
+-rw-rw-rw-   0        0        0    30160 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/process_gramstain_datadump.py
+-rw-rw-rw-   0        0        0      576 2022-08-16 09:34:20.000000 napari-bacseg-1.0.7.1/src/_dev/read_non_tif.py
+-rw-rw-rw-   0        0        0     7794 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/rebuild_usermeta.py
+-rw-rw-rw-   0        0        0    10440 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/rebuild_usermeta_2.py
+-rw-rw-rw-   0        0        0     3034 2023-03-23 13:58:59.000000 napari-bacseg-1.0.7.1/src/_dev/recreate_user_metadata.py
+-rw-rw-rw-   0        0        0     2117 2023-04-20 14:14:30.000000 napari-bacseg-1.0.7.1/src/_dev/scalebar_dev.py
+-rw-rw-rw-   0        0        0    25122 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/sort_midlines.py
+-rw-rw-rw-   0        0        0     9633 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/stelios_stats.py
+-rw-rw-rw-   0        0        0      644 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/tile_meta_check.py
+-rw-rw-rw-   0        0        0     1615 2022-07-22 11:43:30.000000 napari-bacseg-1.0.7.1/src/_dev/tiler_dev.py
+-rw-rw-rw-   0        0        0     3064 2023-02-24 14:29:04.000000 napari-bacseg-1.0.7.1/src/_dev/updade_akseg_metadata.py
+-rw-rw-rw-   0        0        0     2057 2023-02-24 12:22:32.000000 napari-bacseg-1.0.7.1/src/_dev/update_img_metadata.py
+-rw-rw-rw-   0        0        0     6859 2023-02-24 14:19:52.000000 napari-bacseg-1.0.7.1/src/_dev/video_iamges.py
+-rw-rw-rw-   0        0        0     7767 2023-03-13 16:18:11.000000 napari-bacseg-1.0.7.1/src/_dev/zooniverse.py
+-rw-rw-rw-   0        0        0     5624 2023-02-24 14:21:12.000000 napari-bacseg-1.0.7.1/src/_dev/zooniverse_move.py
+-rw-rw-rw-   0        0        0     5742 2023-03-15 10:15:29.000000 napari-bacseg-1.0.7.1/src/_dev/zooniverse_move_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:29:04.000000 napari-bacseg-1.0.7.1/src/_dev/zooniverse_titration_upload.py
+-rw-rw-rw-   0        0        0     7503 2023-03-13 17:00:21.000000 napari-bacseg-1.0.7.1/src/_dev/zooniverse_titrations.py
+-rw-rw-rw-   0        0        0    30267 2023-03-13 16:09:34.000000 napari-bacseg-1.0.7.1/src/_dev/zooniverse_upload.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.427138 napari-bacseg-1.0.7.1/src/napari_bacseg/
+-rw-rw-rw-   0        0        0      157 2023-06-13 16:48:48.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.449080 napari-bacseg-1.0.7.1/src/napari_bacseg/_tests/
+-rw-rw-rw-   0        0        0        0 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_tests/__init__.py
+-rw-rw-rw-   0        0        0    26817 2023-06-13 13:36:57.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_tests/test_bacseg.py
+-rw-rw-rw-   0        0        0     1276 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    90731 2023-06-13 16:07:22.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils.py
+-rw-rw-rw-   0        0        0    14723 2023-06-13 08:44:12.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_cellpose.py
+-rw-rw-rw-   0        0        0    17465 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_colicoords.py
+-rw-rw-rw-   0        0        0    20495 2023-05-03 08:53:54.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_database.py
+-rw-rw-rw-   0        0        0    47487 2023-06-13 09:49:45.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_database_IO.py
+-rw-rw-rw-   0        0        0     1670 2023-06-13 13:50:19.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_imagej.py
+-rw-rw-rw-   0        0        0    40215 2023-06-13 08:44:13.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_interface_events.py
+-rw-rw-rw-   0        0        0     6485 2023-06-13 08:44:12.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_json.py
+-rw-rw-rw-   0        0        0    34168 2023-03-07 17:38:57.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_oufti.py
+-rw-rw-rw-   0        0        0     2132 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_refine.py
+-rw-rw-rw-   0        0        0    22517 2023-06-09 14:18:42.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_statistics.py
+-rw-rw-rw-   0        0        0     7837 2023-06-09 14:18:42.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_tiler.py
+-rw-rw-rw-   0        0        0      169 2023-06-13 16:49:51.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_version.py
+-rw-rw-rw-   0        0        0    97800 2023-06-13 16:49:02.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/_widget.py
+-rw-rw-rw-   0        0        0   172700 2023-06-13 16:10:14.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/bacseg_ui.py
+-rw-rw-rw-   0        0        0   172251 2023-06-13 16:10:08.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/bacseg_ui.ui
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/gapseq_ui.py
+-rw-rw-rw-   0        0        0      501 2023-03-07 17:38:57.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/napari.yaml
+-rw-rw-rw-   0        0        0      271 2023-02-27 13:15:54.000000 napari-bacseg-1.0.7.1/src/napari_bacseg/napari_ui.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:49:52.445090 napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/
+-rw-rw-rw-   0        0        0     4734 2023-06-13 16:49:52.000000 napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2023-06-13 16:49:52.000000 napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:49:52.000000 napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-13 16:49:52.000000 napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      352 2023-06-13 16:49:52.000000 napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-13 16:49:52.000000 napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2023-02-24 11:00:35.000000 napari-bacseg-1.0.7.1/tox.ini
```

### Comparing `napari-bacseg-1.0.7/.github/workflows/test_and_deploy.yml` & `napari-bacseg-1.0.7.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/.gitignore` & `napari-bacseg-1.0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/.napari-hub/config.yml` & `napari-bacseg-1.0.7.1/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/.pre-commit-config.yaml` & `napari-bacseg-1.0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/LICENSE` & `napari-bacseg-1.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/PKG-INFO` & `napari-bacseg-1.0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.7
+Version: 1.0.7.1
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.7/README.md` & `napari-bacseg-1.0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/pyproject.toml` & `napari-bacseg-1.0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [project]
 name = "napari-bacseg"
-version = "1.0.7"
+version = "1.0.7.1"
 authors = [
   { name="Piers Turner", email="piers.turner@physics.ox.ac.uk"},
 ]
 description = "Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `napari-bacseg-1.0.7/setup.cfg` & `napari-bacseg-1.0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/Export Masks to AKSEG v5 dev.py` & `napari-bacseg-1.0.7.1/src/_dev/Export Masks to AKSEG v5 dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/ScanR dev.py` & `napari-bacseg-1.0.7.1/src/_dev/ScanR dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/akseg_db_stats.py` & `napari-bacseg-1.0.7.1/src/_dev/akseg_db_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/akseg_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/akseg_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/akseg_dev2.py` & `napari-bacseg-1.0.7.1/src/_dev/akseg_dev2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/akseg_txt_metadata.py` & `napari-bacseg-1.0.7.1/src/_dev/akseg_txt_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/align_alex_datadump.py` & `napari-bacseg-1.0.7.1/src/_dev/align_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/alison_datadump.py` & `napari-bacseg-1.0.7.1/src/_dev/alison_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/autocontast_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/autocontast_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/chatGPT_midlines.py` & `napari-bacseg-1.0.7.1/src/_dev/chatGPT_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/check_AluGasketv12_DFP.py` & `napari-bacseg-1.0.7.1/src/_dev/check_AluGasketv12_DFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/check_metadata.py` & `napari-bacseg-1.0.7.1/src/_dev/check_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/colicoords_cellldist_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/colicoords_cellldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/colicoords_ldist_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/colicoords_ldist_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/database_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/database_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/deepsegmattest.py` & `napari-bacseg-1.0.7.1/src/_dev/deepsegmattest.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/edit_database_columns.py` & `napari-bacseg-1.0.7.1/src/_dev/edit_database_columns.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/fits_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/fits_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/fix_alison_missing_file_list.py` & `napari-bacseg-1.0.7.1/src/_dev/fix_alison_missing_file_list.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/generate_scanr_movie.py` & `napari-bacseg-1.0.7.1/src/_dev/generate_scanr_movie.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/get_akseg_stats.py` & `napari-bacseg-1.0.7.1/src/_dev/get_akseg_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/get_species_info.py` & `napari-bacseg-1.0.7.1/src/_dev/get_species_info.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/imagej_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/imagej_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/json_nuclei_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/json_nuclei_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/luke__script.py` & `napari-bacseg-1.0.7.1/src/_dev/luke__script.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/matplotlib_Events.py` & `napari-bacseg-1.0.7.1/src/_dev/matplotlib_Events.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/move_AluGasketDFP.py` & `napari-bacseg-1.0.7.1/src/_dev/move_AluGasketDFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/move_AluGasketDFP_poster.py` & `napari-bacseg-1.0.7.1/src/_dev/move_AluGasketDFP_poster.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/move_AluGasketv12_DFP.py` & `napari-bacseg-1.0.7.1/src/_dev/move_AluGasketv12_DFP.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/move_AluGasketv12_DFP_Titration.py` & `napari-bacseg-1.0.7.1/src/_dev/move_AluGasketv12_DFP_Titration.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/move_conor_nim_dfp_data.py` & `napari-bacseg-1.0.7.1/src/_dev/move_conor_nim_dfp_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/move_pillar_data.py` & `napari-bacseg-1.0.7.1/src/_dev/move_pillar_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/move_pillar_zstack_data.py` & `napari-bacseg-1.0.7.1/src/_dev/move_pillar_zstack_data.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/move_unlearning_files.py` & `napari-bacseg-1.0.7.1/src/_dev/move_unlearning_files.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/new_metadata2.pickle.py` & `napari-bacseg-1.0.7.1/src/_dev/new_metadata2.pickle.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/new_read_akseg_directory.py` & `napari-bacseg-1.0.7.1/src/_dev/new_read_akseg_directory.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/nim_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/nim_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/omnipose_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/omnipose_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/omnipose_midlines.py` & `napari-bacseg-1.0.7.1/src/_dev/omnipose_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/omnipose_train.py` & `napari-bacseg-1.0.7.1/src/_dev/omnipose_train.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/oufti_dilate.py` & `napari-bacseg-1.0.7.1/src/_dev/oufti_dilate.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/oufti_dilate_with_midlines.py` & `napari-bacseg-1.0.7.1/src/_dev/oufti_dilate_with_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/pandas_speed.py` & `napari-bacseg-1.0.7.1/src/_dev/pandas_speed.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/process_alex_datadump.py` & `napari-bacseg-1.0.7.1/src/_dev/process_alex_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/process_alex_datadump_clinical.py` & `napari-bacseg-1.0.7.1/src/_dev/process_alex_datadump_clinical.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/process_conor_datadump.py` & `napari-bacseg-1.0.7.1/src/_dev/process_conor_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/process_gramstain_datadump.py` & `napari-bacseg-1.0.7.1/src/_dev/process_gramstain_datadump.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/read_non_tif.py` & `napari-bacseg-1.0.7.1/src/_dev/read_non_tif.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/rebuild_usermeta.py` & `napari-bacseg-1.0.7.1/src/_dev/rebuild_usermeta.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/rebuild_usermeta_2.py` & `napari-bacseg-1.0.7.1/src/_dev/rebuild_usermeta_2.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/recreate_user_metadata.py` & `napari-bacseg-1.0.7.1/src/_dev/recreate_user_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/scalebar_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/scalebar_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/sort_midlines.py` & `napari-bacseg-1.0.7.1/src/_dev/sort_midlines.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/stelios_stats.py` & `napari-bacseg-1.0.7.1/src/_dev/stelios_stats.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/tile_meta_check.py` & `napari-bacseg-1.0.7.1/src/_dev/tile_meta_check.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/tiler_dev.py` & `napari-bacseg-1.0.7.1/src/_dev/tiler_dev.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/updade_akseg_metadata.py` & `napari-bacseg-1.0.7.1/src/_dev/updade_akseg_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/update_img_metadata.py` & `napari-bacseg-1.0.7.1/src/_dev/update_img_metadata.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/video_iamges.py` & `napari-bacseg-1.0.7.1/src/_dev/video_iamges.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/zooniverse.py` & `napari-bacseg-1.0.7.1/src/_dev/zooniverse.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/zooniverse_move.py` & `napari-bacseg-1.0.7.1/src/_dev/zooniverse_move.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/zooniverse_move_titrations.py` & `napari-bacseg-1.0.7.1/src/_dev/zooniverse_move_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/zooniverse_titration_upload.py` & `napari-bacseg-1.0.7.1/src/_dev/zooniverse_titration_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/zooniverse_titrations.py` & `napari-bacseg-1.0.7.1/src/_dev/zooniverse_titrations.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/_dev/zooniverse_upload.py` & `napari-bacseg-1.0.7.1/src/_dev/zooniverse_upload.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_tests/test_bacseg.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_tests/test_bacseg.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_tests/test_widget.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_cellpose.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_cellpose.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_colicoords.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_colicoords.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_database.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_database.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_database_IO.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_database_IO.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_imagej.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_imagej.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_interface_events.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_interface_events.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_json.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_json.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_oufti.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_oufti.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_refine.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_refine.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_statistics.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_statistics.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_utils_tiler.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_utils_tiler.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/_widget.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,30 @@
 
 import cv2
 import napari
 import numpy as np
 from napari.utils.notifications import show_info
 from PyQt5.QtCore import pyqtSignal, pyqtSlot
 from qtpy.QtCore import QObject, QRunnable, QThreadPool
-from qtpy.QtWidgets import (QCheckBox, QComboBox, QFileDialog, QFormLayout, QHBoxLayout, QLabel, QLineEdit, QProgressBar, QPushButton, QRadioButton, QSlider, QTabWidget, QVBoxLayout, QWidget, )
+from qtpy.QtWidgets import (
+    QCheckBox,
+    QComboBox,
+    QFileDialog,
+    QFormLayout,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QProgressBar,
+    QPushButton,
+    QRadioButton,
+    QSlider,
+    QTabWidget,
+    QVBoxLayout,
+    QWidget,
+)
 
 import napari_bacseg._utils
 from napari_bacseg._utils import align_image_channels, unstack_images
 
 os.environ["QT_AUTO_SCREEN_SCALE_FACTOR"] = "1"
 
 
@@ -91,15 +106,17 @@
         try:
             result = self.fn(*self.args, **self.kwargs)
         except:
             traceback.print_exc()
             exctype, value = sys.exc_info()[:2]
             self.signals.error.emit((exctype, value, traceback.format_exc()))
         else:
-            self.signals.result.emit(result)  # Return the result of the processing
+            self.signals.result.emit(
+                result
+            )  # Return the result of the processing
         finally:
             self.signals.finished.emit()  # Done
 
     def result(self):
         return self.fn(*self.args, **self.kwargs)
 
 
@@ -140,20 +157,53 @@
     def __init__(self, viewer: napari.Viewer):
         """Initialize widget with two layer combo boxes and a run button"""
 
         super().__init__()
 
         # import functions
         from napari_bacseg._utils import _manualImport, stack_images
-        from napari_bacseg._utils_cellpose import (_initialise_cellpose_model, _select_cellpose_save_directory, _select_cellpose_save_path, _select_custom_cellpose_model, train_cellpose_model, )
-        from napari_bacseg._utils_database import (_create_bacseg_database, _load_bacseg_database, _populateUSERMETA, _show_database_controls, populate_upload_combos, update_database_metadata, )
-        from napari_bacseg._utils_interface_events import (_copymasktoall, _delete_active_image, _deleteallmasks, _doubeClickEvents, _imageControls, _modify_channel_changed, _modifyMode, _segmentationEvents, _viewerControls, )
-        from napari_bacseg._utils_oufti import (_update_active_midlines, centre_oufti_midlines, generate_midlines, midline_edit_toggle, update_midlines, )
+        from napari_bacseg._utils_cellpose import (
+            _initialise_cellpose_model,
+            _select_cellpose_save_directory,
+            _select_cellpose_save_path,
+            _select_custom_cellpose_model,
+            train_cellpose_model,
+        )
+        from napari_bacseg._utils_database import (
+            _create_bacseg_database,
+            _load_bacseg_database,
+            _populateUSERMETA,
+            _show_database_controls,
+            populate_upload_combos,
+            update_database_metadata,
+        )
+        from napari_bacseg._utils_interface_events import (
+            _copymasktoall,
+            _delete_active_image,
+            _deleteallmasks,
+            _doubeClickEvents,
+            _imageControls,
+            _modify_channel_changed,
+            _modifyMode,
+            _segmentationEvents,
+            _viewerControls,
+        )
+        from napari_bacseg._utils_oufti import (
+            _update_active_midlines,
+            centre_oufti_midlines,
+            generate_midlines,
+            midline_edit_toggle,
+            update_midlines,
+        )
         from napari_bacseg._utils_statistics import _compute_simple_cell_stats
-        from napari_bacseg._utils_tiler import (fold_images, unfold_images, update_image_folds, )
+        from napari_bacseg._utils_tiler import (
+            fold_images,
+            unfold_images,
+            update_image_folds,
+        )
         from napari_bacseg.bacseg_ui import Ui_tab_widget
 
         self.populate_upload_combos = self.wrapper(populate_upload_combos)
         self.update_database_metadata = self.wrapper(update_database_metadata)
         self.stack_image = self.wrapper(stack_images)
         self._modifyMode = self.wrapper(_modifyMode)
         self._viewerControls = self.wrapper(_viewerControls)
@@ -162,31 +212,41 @@
         self._delete_active_image = self.wrapper(_delete_active_image)
         self._populateUSERMETA = self.wrapper(_populateUSERMETA)
         self._imageControls = self.wrapper(_imageControls)
         self._segmentationEvents = self.wrapper(_segmentationEvents)
         self._modify_channel_changed = self.wrapper(_modify_channel_changed)
         self._manualImport = self.wrapper(_manualImport)
         self.train_cellpose_model = self.wrapper(train_cellpose_model)
-        self._initialise_cellpose_model = self.wrapper(_initialise_cellpose_model)
-        self._select_custom_cellpose_model = self.wrapper(_select_custom_cellpose_model)
-        self._select_cellpose_save_directory = self.wrapper(_select_cellpose_save_directory)
-        self._select_cellpose_save_path = self.wrapper(_select_cellpose_save_path)
+        self._initialise_cellpose_model = self.wrapper(
+            _initialise_cellpose_model
+        )
+        self._select_custom_cellpose_model = self.wrapper(
+            _select_custom_cellpose_model
+        )
+        self._select_cellpose_save_directory = self.wrapper(
+            _select_cellpose_save_directory
+        )
+        self._select_cellpose_save_path = self.wrapper(
+            _select_cellpose_save_path
+        )
         self.unfold_images = self.wrapper(unfold_images)
         self.fold_images = self.wrapper(fold_images)
         self.update_image_folds = self.wrapper(update_image_folds)
         self.midline_edit_toggle = self.wrapper(midline_edit_toggle)
         self.centre_oufti_midlines = self.wrapper(centre_oufti_midlines)
         self.generate_midlines = self.wrapper(generate_midlines)
         self.update_midlines = self.wrapper(update_midlines)
         self._update_active_midlines = self.wrapper(_update_active_midlines)
         self._create_bacseg_database = self.wrapper(_create_bacseg_database)
         self._load_bacseg_database = self.wrapper(_load_bacseg_database)
         self._show_database_controls = self.wrapper(_show_database_controls)
         self._doubeClickEvents = self.wrapper(_doubeClickEvents)
-        self._compute_simple_cell_stats = self.wrapper(_compute_simple_cell_stats)
+        self._compute_simple_cell_stats = self.wrapper(
+            _compute_simple_cell_stats
+        )
 
         application_path = os.path.dirname(sys.executable)
         self.viewer = viewer
         self.setLayout(QVBoxLayout())
 
         # ui_path = os.path.abspath(r"C:\napari-bacseg\src\napari_bacseg\bacseg_ui.ui")
         # self.bacseg_ui = uic.loadUi(ui_path)
@@ -207,129 +267,215 @@
         self.active_import_mode = ""
         self.import_mode = self.findChild(QComboBox, "import_mode")
         self.import_filemode = self.findChild(QComboBox, "import_filemode")
         self.import_precision = self.findChild(QComboBox, "import_precision")
         self.import_import = self.findChild(QPushButton, "import_import")
         self.import_limit = self.findChild(QComboBox, "import_limit")
         self.import_limit_label = self.findChild(QLabel, "import_limit_label")
-        self.clear_previous = self.findChild(QCheckBox, "import_clear_previous")
+        self.clear_previous = self.findChild(
+            QCheckBox, "import_clear_previous"
+        )
         self.autocontrast = self.findChild(QCheckBox, "import_auto_contrast")
-        self.import_multiframe_mode = self.findChild(QComboBox, "import_multiframe_mode")
+        self.import_multiframe_mode = self.findChild(
+            QComboBox, "import_multiframe_mode"
+        )
         self.import_crop_mode = self.findChild(QComboBox, "import_crop_mode")
         self.channel_mode = self.findChild(QComboBox, "nim_channel_mode")
-        self.import_progressbar = self.findChild(QProgressBar, "import_progressbar")
+        self.import_progressbar = self.findChild(
+            QProgressBar, "import_progressbar"
+        )
         self.import_align = self.findChild(QCheckBox, "import_align")
         self.label_modality = self.findChild(QComboBox, "label_modality")
         self.label_stain = self.findChild(QComboBox, "label_stain")
-        self.label_stain_target = self.findChild(QComboBox, "label_stain_target")
+        self.label_stain_target = self.findChild(
+            QComboBox, "label_stain_target"
+        )
         self.label_overwrite = self.findChild(QPushButton, "label_overwrite")
-        self.label_light_source = self.findChild(QComboBox, "label_light_source")
+        self.label_light_source = self.findChild(
+            QComboBox, "label_light_source"
+        )
 
         # view tab controls + variables from Qt Desinger References
         self.unfold_tile_size = self.findChild(QComboBox, "unfold_tile_size")
-        self.unfold_tile_overlap = self.findChild(QComboBox, "unfold_tile_overlap")
+        self.unfold_tile_overlap = self.findChild(
+            QComboBox, "unfold_tile_overlap"
+        )
         self.unfold_mode = self.findChild(QComboBox, "unfold_mode")
         self.fold = self.findChild(QPushButton, "fold")
         self.unfold = self.findChild(QPushButton, "unfold")
-        self.unfold_progressbar = self.findChild(QPushButton, "unfold_progressbar")
+        self.unfold_progressbar = self.findChild(
+            QPushButton, "unfold_progressbar"
+        )
         self.alignment_channel = self.findChild(QComboBox, "alignment_channel")
-        self.align_active_image = self.findChild(QPushButton, "align_active_image")
+        self.align_active_image = self.findChild(
+            QPushButton, "align_active_image"
+        )
         self.align_all_images = self.findChild(QPushButton, "align_all_images")
 
         self.overlay_filename = self.findChild(QCheckBox, "overlay_filename")
         self.overlay_folder = self.findChild(QCheckBox, "overlay_folder")
-        self.overlay_microscope = self.findChild(QCheckBox, "overlay_microscope")
-        self.overlay_datemodified = self.findChild(QCheckBox, "overlay_datemodified")
+        self.overlay_microscope = self.findChild(
+            QCheckBox, "overlay_microscope"
+        )
+        self.overlay_datemodified = self.findChild(
+            QCheckBox, "overlay_datemodified"
+        )
         self.overlay_content = self.findChild(QCheckBox, "overlay_content")
         self.overlay_phenotype = self.findChild(QCheckBox, "overlay_phenotype")
         self.overlay_strain = self.findChild(QCheckBox, "overlay_strain")
-        self.overlay_staintarget = self.findChild(QCheckBox, "overlay_staintarget")
-        self.overlay_antibiotic = self.findChild(QCheckBox, "overlay_antibiotic")
+        self.overlay_staintarget = self.findChild(
+            QCheckBox, "overlay_staintarget"
+        )
+        self.overlay_antibiotic = self.findChild(
+            QCheckBox, "overlay_antibiotic"
+        )
         self.overlay_stain = self.findChild(QCheckBox, "overlay_stain")
         self.overlay_modality = self.findChild(QCheckBox, "overlay_modality")
-        self.overlay_lightsource = self.findChild(QCheckBox, "overlay_lightsource")
+        self.overlay_lightsource = self.findChild(
+            QCheckBox, "overlay_lightsource"
+        )
         self.overlay_focus = self.findChild(QCheckBox, "overlay_focus")
         self.overlay_debris = self.findChild(QCheckBox, "overlay_debris")
         self.overlay_laplacian = self.findChild(QCheckBox, "overlay_laplacian")
         self.overlay_range = self.findChild(QCheckBox, "overlay_range")
 
-        self.zoom_magnification = self.findChild(QComboBox, "zoom_magnification")
+        self.zoom_magnification = self.findChild(
+            QComboBox, "zoom_magnification"
+        )
         self.zoom_apply = self.findChild(QPushButton, "zoom_apply")
 
         # cellpose controls + variables from Qt Desinger References
         self.cellpose_segmentation = False
         self.cellpose_model = None
         self.cellpose_custom_model_path = ""
         self.cellpose_train_model_path = ""
         self.cellpose_log_file = None
-        self.cellpose_select_custom_model = self.findChild(QPushButton, "cellpose_select_custom_model")
+        self.cellpose_select_custom_model = self.findChild(
+            QPushButton, "cellpose_select_custom_model"
+        )
         self.cellpose_segmodel = self.findChild(QComboBox, "cellpose_segmodel")
-        self.cellpose_trainmodel = self.findChild(QComboBox, "cellpose_trainmodel")
-        self.cellpose_segchannel = self.findChild(QComboBox, "cellpose_segchannel")
-        self.cellpose_flowthresh = self.findChild(QSlider, "cellpose_flowthresh")
-        self.cellpose_flowthresh_label = self.findChild(QLabel, "cellpose_flowthresh_label")
-        self.cellpose_maskthresh = self.findChild(QSlider, "cellpose_maskthresh")
-        self.cellpose_maskthresh_label = self.findChild(QLabel, "cellpose_maskthresh_label")
+        self.cellpose_trainmodel = self.findChild(
+            QComboBox, "cellpose_trainmodel"
+        )
+        self.cellpose_segchannel = self.findChild(
+            QComboBox, "cellpose_segchannel"
+        )
+        self.cellpose_flowthresh = self.findChild(
+            QSlider, "cellpose_flowthresh"
+        )
+        self.cellpose_flowthresh_label = self.findChild(
+            QLabel, "cellpose_flowthresh_label"
+        )
+        self.cellpose_maskthresh = self.findChild(
+            QSlider, "cellpose_maskthresh"
+        )
+        self.cellpose_maskthresh_label = self.findChild(
+            QLabel, "cellpose_maskthresh_label"
+        )
         self.cellpose_minsize = self.findChild(QSlider, "cellpose_minsize")
-        self.cellpose_minsize_label = self.findChild(QLabel, "cellpose_minsize_label")
+        self.cellpose_minsize_label = self.findChild(
+            QLabel, "cellpose_minsize_label"
+        )
         self.cellpose_diameter = self.findChild(QSlider, "cellpose_diameter")
-        self.cellpose_diameter_label = self.findChild(QLabel, "cellpose_diameter_label")
-        self.cellpose_segment_active = self.findChild(QPushButton, "cellpose_segment_active")
-        self.cellpose_segment_all = self.findChild(QPushButton, "cellpose_segment_all")
-        self.cellpose_clear_previous = self.findChild(QCheckBox, "cellpose_clear_previous")
+        self.cellpose_diameter_label = self.findChild(
+            QLabel, "cellpose_diameter_label"
+        )
+        self.cellpose_segment_active = self.findChild(
+            QPushButton, "cellpose_segment_active"
+        )
+        self.cellpose_segment_all = self.findChild(
+            QPushButton, "cellpose_segment_all"
+        )
+        self.cellpose_clear_previous = self.findChild(
+            QCheckBox, "cellpose_clear_previous"
+        )
         self.cellpose_usegpu = self.findChild(QCheckBox, "cellpose_usegpu")
-        self.cellpose_resetimage = self.findChild(QCheckBox, "cellpose_resetimage")
-        self.cellpose_progressbar = self.findChild(QProgressBar, "cellpose_progressbar")
-        self.cellpose_train_model = self.findChild(QPushButton, "cellpose_train_model")
-        self.cellpose_save_dir = self.findChild(QPushButton, "cellpose_save_dir")
-        self.cellpose_trainchannel = self.findChild(QComboBox, "cellpose_trainchannel")
+        self.cellpose_resetimage = self.findChild(
+            QCheckBox, "cellpose_resetimage"
+        )
+        self.cellpose_progressbar = self.findChild(
+            QProgressBar, "cellpose_progressbar"
+        )
+        self.cellpose_train_model = self.findChild(
+            QPushButton, "cellpose_train_model"
+        )
+        self.cellpose_save_dir = self.findChild(
+            QPushButton, "cellpose_save_dir"
+        )
+        self.cellpose_trainchannel = self.findChild(
+            QComboBox, "cellpose_trainchannel"
+        )
         self.cellpose_nepochs = self.findChild(QComboBox, "cellpose_nepochs")
-        self.cellpose_batchsize = self.findChild(QComboBox, "cellpose_batchsize")
-        self.cellpose_min_seg_size = self.findChild(QComboBox, "cellpose_min_seg_size")
+        self.cellpose_batchsize = self.findChild(
+            QComboBox, "cellpose_batchsize"
+        )
+        self.cellpose_min_seg_size = self.findChild(
+            QComboBox, "cellpose_min_seg_size"
+        )
         self.cellpose_seg_mode = self.findChild(QComboBox, "cellpose_seg_mode")
 
         # modify tab controls + variables from Qt Desinger References
         self.interface_mode = "panzoom"
         self.segmentation_mode = "add"
         self.class_mode = "single"
         self.class_colour = 1
         self.modify_panzoom = self.findChild(QPushButton, "modify_panzoom")
         self.modify_segment = self.findChild(QPushButton, "modify_segment")
         self.modify_classify = self.findChild(QPushButton, "modify_classify")
         self.modify_refine = self.findChild(QPushButton, "modify_refine")
         self.refine_channel = self.findChild(QComboBox, "refine_channel")
         self.refine_all = self.findChild(QPushButton, "refine_all")
-        self.modify_copymasktoall = self.findChild(QPushButton, "modify_copymasktoall")
-        self.modify_deleteallmasks = self.findChild(QPushButton, "modify_deleteallmasks")
-        self.modify_deleteactivemasks = self.findChild(QPushButton, "modify_deleteactivemasks")
-        self.modify_deleteactiveimage = self.findChild(QPushButton, "modify_deleteactiveimage")
-        self.modify_deleteotherimages = self.findChild(QPushButton, "modify_deleteotherimages")
-        self.modify_progressbar = self.findChild(QProgressBar, "modify_progressbar")
+        self.modify_copymasktoall = self.findChild(
+            QPushButton, "modify_copymasktoall"
+        )
+        self.modify_deleteallmasks = self.findChild(
+            QPushButton, "modify_deleteallmasks"
+        )
+        self.modify_deleteactivemasks = self.findChild(
+            QPushButton, "modify_deleteactivemasks"
+        )
+        self.modify_deleteactiveimage = self.findChild(
+            QPushButton, "modify_deleteactiveimage"
+        )
+        self.modify_deleteotherimages = self.findChild(
+            QPushButton, "modify_deleteotherimages"
+        )
+        self.modify_progressbar = self.findChild(
+            QProgressBar, "modify_progressbar"
+        )
         self.modify_channel = self.findChild(QComboBox, "modify_channel")
 
-        self.modify_auto_panzoom = self.findChild(QCheckBox, "modify_auto_panzoom")
+        self.modify_auto_panzoom = self.findChild(
+            QCheckBox, "modify_auto_panzoom"
+        )
         self.modify_add = self.findChild(QPushButton, "modify_add")
         self.modify_extend = self.findChild(QPushButton, "modify_extend")
         self.modify_split = self.findChild(QPushButton, "modify_split")
         self.modify_join = self.findChild(QPushButton, "modify_join")
         self.modify_delete = self.findChild(QPushButton, "modify_delete")
         self.classify_single = self.findChild(QPushButton, "classify_single")
-        self.classify_dividing = self.findChild(QPushButton, "classify_dividing")
+        self.classify_dividing = self.findChild(
+            QPushButton, "classify_dividing"
+        )
         self.classify_divided = self.findChild(QPushButton, "classify_divided")
-        self.classify_vertical = self.findChild(QPushButton, "classify_vertical")
+        self.classify_vertical = self.findChild(
+            QPushButton, "classify_vertical"
+        )
         self.classify_broken = self.findChild(QPushButton, "classify_broken")
         self.classify_edge = self.findChild(QPushButton, "classify_edge")
         self.modify_viewmasks = self.findChild(QCheckBox, "modify_viewmasks")
         self.modify_viewlabels = self.findChild(QCheckBox, "modify_viewlabels")
         self.find_next = self.findChild(QPushButton, "find_next")
         self.find_previous = self.findChild(QPushButton, "find_previous")
         self.find_criterion = self.findChild(QComboBox, "find_criterion")
         self.find_mode = self.findChild(QComboBox, "find_mode")
         self.scalebar_show = self.findChild(QCheckBox, "scalebar_show")
-        self.scalebar_resolution = self.findChild(QLineEdit, "scalebar_resolution")
+        self.scalebar_resolution = self.findChild(
+            QLineEdit, "scalebar_resolution"
+        )
         self.scalebar_units = self.findChild(QComboBox, "scalebar_units")
 
         self.set_quality_mode = self.findChild(QComboBox, "set_quality_mode")
         self.set_focus_0 = self.findChild(QPushButton, "set_focus_0")
         self.set_focus_1 = self.findChild(QPushButton, "set_focus_1")
         self.set_focus_2 = self.findChild(QPushButton, "set_focus_2")
         self.set_focus_3 = self.findChild(QPushButton, "set_focus_3")
@@ -342,134 +488,281 @@
         self.set_debris_4 = self.findChild(QPushButton, "set_debris_4")
         self.set_debris_5 = self.findChild(QPushButton, "set_debris_5")
 
         # upload tab controls from Qt Desinger References
         self.database_path = ""
         self.user_metadata_keys = 6
 
-        self.metadata_columns = ["date_uploaded", "date_created", "date_modified", "file_name", "channel", "file_list", "channel_list", "segmentation_file", "segmentation_channel", "akseg_hash",
-            "user_initial", "content", "microscope", "modality", "source", "strain", "phenotype", "stain", "stain_target", "antibiotic", "treatment time (mins)", "antibiotic concentration",
-            "mounting method", "protocol", "folder", "parent_folder", "num_segmentations", "image_laplacian", "image_focus", "image_debris", "segmented", "labelled", "segmentation_curated",
-            "label_curated", "posX", "posY", "posZ", "image_load_path", "image_save_path", "mask_load_path", "mask_save_path", "label_load_path", "label_save_path", ]
+        self.metadata_columns = [
+            "date_uploaded",
+            "date_created",
+            "date_modified",
+            "file_name",
+            "channel",
+            "file_list",
+            "channel_list",
+            "segmentation_file",
+            "segmentation_channel",
+            "akseg_hash",
+            "user_initial",
+            "content",
+            "microscope",
+            "modality",
+            "source",
+            "strain",
+            "phenotype",
+            "stain",
+            "stain_target",
+            "antibiotic",
+            "treatment time (mins)",
+            "antibiotic concentration",
+            "mounting method",
+            "protocol",
+            "folder",
+            "parent_folder",
+            "num_segmentations",
+            "image_laplacian",
+            "image_focus",
+            "image_debris",
+            "segmented",
+            "labelled",
+            "segmentation_curated",
+            "label_curated",
+            "posX",
+            "posY",
+            "posZ",
+            "image_load_path",
+            "image_save_path",
+            "mask_load_path",
+            "mask_save_path",
+            "label_load_path",
+            "label_save_path",
+        ]
 
         user_key_list = np.arange(1, self.user_metadata_keys + 1).tolist()
         user_key_list.reverse()
 
         for key in user_key_list:
             user_key = f"user_meta{key}"
             self.metadata_columns.insert(22, str(user_key))
-            setattr(self, f"upload_usermeta{key}", self.findChild(QComboBox, f"upload_usermeta{key}"), )
+            setattr(
+                self,
+                f"upload_usermeta{key}",
+                self.findChild(QComboBox, f"upload_usermeta{key}"),
+            )
 
         self.upload_initial = self.findChild(QComboBox, "upload_initial")
         self.upload_content = self.findChild(QComboBox, "upload_content")
         self.upload_microscope = self.findChild(QComboBox, "upload_microscope")
         self.upload_antibiotic = self.findChild(QComboBox, "upload_antibiotic")
         self.upload_phenotype = self.findChild(QComboBox, "upload_phenotype")
         self.upload_strain = self.findChild(QComboBox, "upload_strain")
-        self.upload_abxconcentration = self.findChild(QComboBox, "upload_abxconcentration")
-        self.upload_treatmenttime = self.findChild(QComboBox, "upload_treatmenttime")
+        self.upload_abxconcentration = self.findChild(
+            QComboBox, "upload_abxconcentration"
+        )
+        self.upload_treatmenttime = self.findChild(
+            QComboBox, "upload_treatmenttime"
+        )
         self.upload_mount = self.findChild(QComboBox, "upload_mount")
         self.upload_protocol = self.findChild(QComboBox, "upload_protocol")
-        self.upload_overwrite_images = self.findChild(QCheckBox, "upload_overwrite_images")
-        self.upload_overwrite_masks = self.findChild(QCheckBox, "upload_overwrite_masks")
-        self.overwrite_selected_metadata = self.findChild(QCheckBox, "overwrite_selected_metadata")
-        self.overwrite_all_metadata = self.findChild(QCheckBox, "overwrite_all_metadata")
+        self.upload_overwrite_images = self.findChild(
+            QCheckBox, "upload_overwrite_images"
+        )
+        self.upload_overwrite_masks = self.findChild(
+            QCheckBox, "upload_overwrite_masks"
+        )
+        self.overwrite_selected_metadata = self.findChild(
+            QCheckBox, "overwrite_selected_metadata"
+        )
+        self.overwrite_all_metadata = self.findChild(
+            QCheckBox, "overwrite_all_metadata"
+        )
         self.upload_all = self.findChild(QPushButton, "upload_all")
         self.upload_active = self.findChild(QPushButton, "upload_active")
-        self.database_download = self.findChild(QPushButton, "database_download")
-        self.database_download_limit = self.findChild(QComboBox, "database_download_limit")
+        self.database_download = self.findChild(
+            QPushButton, "database_download"
+        )
+        self.database_download_limit = self.findChild(
+            QComboBox, "database_download_limit"
+        )
         self.create_database = self.findChild(QPushButton, "create_database")
         self.load_database = self.findChild(QPushButton, "load_database")
-        self.display_database_path = self.findChild(QLineEdit, "display_database_path")
-        self.upload_progressbar = self.findChild(QProgressBar, "upload_progressbar")
+        self.display_database_path = self.findChild(
+            QLineEdit, "display_database_path"
+        )
+        self.upload_progressbar = self.findChild(
+            QProgressBar, "upload_progressbar"
+        )
         self.upload_tab = self.findChild(QWidget, "upload_tab")
-        self.upload_segmentation_combo = self.findChild(QComboBox, "upload_segmentation_combo")
-        self.upload_label_combo = self.findChild(QComboBox, "upload_label_combo")
-        self.download_sort_order_1 = self.findChild(QComboBox, "download_sort_order_1")
-        self.download_sort_order_2 = self.findChild(QComboBox, "download_sort_order_2")
-        self.download_sort_direction_1 = self.findChild(QComboBox, "download_sort_direction_1")
-        self.download_sort_direction_2 = self.findChild(QComboBox, "download_sort_direction_2")
+        self.upload_segmentation_combo = self.findChild(
+            QComboBox, "upload_segmentation_combo"
+        )
+        self.upload_label_combo = self.findChild(
+            QComboBox, "upload_label_combo"
+        )
+        self.download_sort_order_1 = self.findChild(
+            QComboBox, "download_sort_order_1"
+        )
+        self.download_sort_order_2 = self.findChild(
+            QComboBox, "download_sort_order_2"
+        )
+        self.download_sort_direction_1 = self.findChild(
+            QComboBox, "download_sort_direction_1"
+        )
+        self.download_sort_direction_2 = self.findChild(
+            QComboBox, "download_sort_direction_2"
+        )
         self.update_metadata = self.findChild(QPushButton, "update_metadata")
-        self.upload_images_setting = self.findChild(QCheckBox, "upload_images_setting")
-        self.upload_segmentations_setting = self.findChild(QCheckBox, "upload_segmentations_setting")
-        self.upload_metadata_setting = self.findChild(QCheckBox, "upload_metadata_setting")
-
-        self.image_metadata_controls = self.findChild(QFormLayout, "image_metadata_controls")
+        self.upload_images_setting = self.findChild(
+            QCheckBox, "upload_images_setting"
+        )
+        self.upload_segmentations_setting = self.findChild(
+            QCheckBox, "upload_segmentations_setting"
+        )
+        self.upload_metadata_setting = self.findChild(
+            QCheckBox, "upload_metadata_setting"
+        )
+
+        self.image_metadata_controls = self.findChild(
+            QFormLayout, "image_metadata_controls"
+        )
 
         self._show_database_controls(False)
 
         # oufti tab controls
-        self.oufti_generate_all_midlines = self.findChild(QPushButton, "oufti_generate_all_midlines")
-        self.oufti_generate_active_midlines = self.findChild(QPushButton, "oufti_generate_active_midlines")
-        self.oufti_panzoom_mode = self.findChild(QRadioButton, "oufti_panzoom_mode")
+        self.oufti_generate_all_midlines = self.findChild(
+            QPushButton, "oufti_generate_all_midlines"
+        )
+        self.oufti_generate_active_midlines = self.findChild(
+            QPushButton, "oufti_generate_active_midlines"
+        )
+        self.oufti_panzoom_mode = self.findChild(
+            QRadioButton, "oufti_panzoom_mode"
+        )
         self.oufti_edit_mode = self.findChild(QRadioButton, "oufti_edit_mode")
-        self.oufti_midline_vertexes = self.findChild(QComboBox, "oufti_midline_vertexes")
-        self.oufti_centre_all_midlines = self.findChild(QPushButton, "oufti_centre_all_midlines")
-        self.oufti_centre_active_midlines = self.findChild(QPushButton, "oufti_centre_active_midlines")
+        self.oufti_midline_vertexes = self.findChild(
+            QComboBox, "oufti_midline_vertexes"
+        )
+        self.oufti_centre_all_midlines = self.findChild(
+            QPushButton, "oufti_centre_all_midlines"
+        )
+        self.oufti_centre_active_midlines = self.findChild(
+            QPushButton, "oufti_centre_active_midlines"
+        )
         self.oufti_mesh_length = self.findChild(QComboBox, "oufti_mesh_length")
-        self.oufti_mesh_dilation = self.findChild(QComboBox, "oufti_mesh_dilation")
+        self.oufti_mesh_dilation = self.findChild(
+            QComboBox, "oufti_mesh_dilation"
+        )
 
         # export tab controls from Qt Desinger References
         self.export_channel = self.findChild(QComboBox, "export_channel")
         self.export_mode = self.findChild(QComboBox, "export_mode")
         self.export_location = self.findChild(QComboBox, "export_location")
         self.export_modifier = self.findChild(QLineEdit, "export_modifier")
         self.export_single = self.findChild(QCheckBox, "export_single")
         self.export_dividing = self.findChild(QCheckBox, "export_dividing")
         self.export_divided = self.findChild(QCheckBox, "export_divided")
         self.export_vertical = self.findChild(QCheckBox, "export_vertical")
         self.export_broken = self.findChild(QCheckBox, "export_broken")
         self.export_edge = self.findChild(QCheckBox, "export_edge")
-        self.export_statistics_multithreaded = self.findChild(QCheckBox, "export_statistics_multithreaded")
+        self.export_statistics_multithreaded = self.findChild(
+            QCheckBox, "export_statistics_multithreaded"
+        )
         self.export_active = self.findChild(QPushButton, "export_active")
         self.export_all = self.findChild(QPushButton, "export_all")
         self.export_normalise = self.findChild(QCheckBox, "export_normalise")
         self.export_invert = self.findChild(QCheckBox, "export_invert")
         self.export_scalebar = self.findChild(QCheckBox, "export_scalebar")
-        self.export_scalebar_resolution = self.findChild(QLineEdit, "export_scalebar_resolution")
-        self.export_scalebar_resolution_units = self.findChild(QComboBox, "export_scalebar_resolution_units")
-        self.export_scalebar_size = self.findChild(QLineEdit, "export_scalebar_size")
-        self.export_scalebar_size_units = self.findChild(QComboBox, "export_scalebar_size_units")
-        self.export_scalebar_colour = self.findChild(QComboBox, "export_scalebar_colour")
-        self.export_scalebar_thickness = self.findChild(QComboBox, "export_scalebar_thickness")
+        self.export_scalebar_resolution = self.findChild(
+            QLineEdit, "export_scalebar_resolution"
+        )
+        self.export_scalebar_resolution_units = self.findChild(
+            QComboBox, "export_scalebar_resolution_units"
+        )
+        self.export_scalebar_size = self.findChild(
+            QLineEdit, "export_scalebar_size"
+        )
+        self.export_scalebar_size_units = self.findChild(
+            QComboBox, "export_scalebar_size_units"
+        )
+        self.export_scalebar_colour = self.findChild(
+            QComboBox, "export_scalebar_colour"
+        )
+        self.export_scalebar_thickness = self.findChild(
+            QComboBox, "export_scalebar_thickness"
+        )
         self.export_cropzoom = self.findChild(QCheckBox, "export_crop_zoom")
-        self.export_mask_background = self.findChild(QCheckBox, "export_mask_background")
-
-        self.export_stack_channel = self.findChild(QComboBox, "export_stack_channel")
+        self.export_mask_background = self.findChild(
+            QCheckBox, "export_mask_background"
+        )
+
+        self.export_stack_channel = self.findChild(
+            QComboBox, "export_stack_channel"
+        )
         self.export_stack_mode = self.findChild(QComboBox, "export_stack_mode")
-        self.export_stack_location = self.findChild(QComboBox, "export_stack_location")
-        self.export_stack_modifier = self.findChild(QLineEdit, "export_stack_modifier")
-        self.export_stack_image_setting = self.findChild(QCheckBox, "export_stack_image_setting")
-        self.export_stack_overwrite_setting = self.findChild(QCheckBox, "export_stack_overwrite_setting")
-        self.export_stack_active = self.findChild(QPushButton, "export_stack_active")
+        self.export_stack_location = self.findChild(
+            QComboBox, "export_stack_location"
+        )
+        self.export_stack_modifier = self.findChild(
+            QLineEdit, "export_stack_modifier"
+        )
+        self.export_stack_image_setting = self.findChild(
+            QCheckBox, "export_stack_image_setting"
+        )
+        self.export_stack_overwrite_setting = self.findChild(
+            QCheckBox, "export_stack_overwrite_setting"
+        )
+        self.export_stack_active = self.findChild(
+            QPushButton, "export_stack_active"
+        )
         self.export_stack_all = self.findChild(QPushButton, "export_stack_all")
 
-        self.export_autocontrast = self.findChild(QCheckBox, "export_autocontrast")
-        self.export_statistics_pixelsize = self.findChild(QLineEdit, "export_statistics_pixelsize")
-        self.export_statistics_active = self.findChild(QPushButton, "export_statistics_active")
-        self.export_statistics_all = self.findChild(QPushButton, "export_statistics_all")
-        self.export_colicoords_mode = self.findChild(QComboBox, "export_colicoords_mode")
-        self.export_progressbar = self.findChild(QProgressBar, "export_progressbar")
-        self.export_image_setting = self.findChild(QCheckBox, "export_image_setting")
-        self.export_overwrite_setting = self.findChild(QCheckBox, "export_overwrite_setting")
+        self.export_autocontrast = self.findChild(
+            QCheckBox, "export_autocontrast"
+        )
+        self.export_statistics_pixelsize = self.findChild(
+            QLineEdit, "export_statistics_pixelsize"
+        )
+        self.export_statistics_active = self.findChild(
+            QPushButton, "export_statistics_active"
+        )
+        self.export_statistics_all = self.findChild(
+            QPushButton, "export_statistics_all"
+        )
+        self.export_colicoords_mode = self.findChild(
+            QComboBox, "export_colicoords_mode"
+        )
+        self.export_progressbar = self.findChild(
+            QProgressBar, "export_progressbar"
+        )
+        self.export_image_setting = self.findChild(
+            QCheckBox, "export_image_setting"
+        )
+        self.export_overwrite_setting = self.findChild(
+            QCheckBox, "export_overwrite_setting"
+        )
         self.export_directory = ""
 
         # import events
         self.autocontrast.stateChanged.connect(self._autoContrast)
         self.import_import.clicked.connect(self._importDialog)
         self.label_overwrite.clicked.connect(self.overwrite_channel_info)
 
         # view events
         self.fold.clicked.connect(self.fold_images)
         self.unfold.clicked.connect(self.unfold_images)
         self.tiler_object = None
         self.tile_dict = {"Segmentations": [], "Classes": [], "Nucleoid": []}
         self.unfolded = False
-        self.align_active_image.clicked.connect(partial(self._align_images, mode="active"))
-        self.align_all_images.clicked.connect(partial(self._align_images, mode="all"))
+        self.align_active_image.clicked.connect(
+            partial(self._align_images, mode="active")
+        )
+        self.align_all_images.clicked.connect(
+            partial(self._align_images, mode="all")
+        )
         self.scalebar_show.stateChanged.connect(self._updateScaleBar)
         self.scalebar_resolution.textChanged.connect(self._updateScaleBar)
         self.scalebar_units.currentTextChanged.connect(self._updateScaleBar)
         self.overlay_filename.stateChanged.connect(self._updateFileName)
         self.overlay_folder.stateChanged.connect(self._updateFileName)
         self.overlay_microscope.stateChanged.connect(self._updateFileName)
         self.overlay_datemodified.stateChanged.connect(self._updateFileName)
@@ -484,85 +777,159 @@
         self.overlay_focus.stateChanged.connect(self._updateFileName)
         self.overlay_debris.stateChanged.connect(self._updateFileName)
         self.overlay_laplacian.stateChanged.connect(self._updateFileName)
         self.overlay_range.stateChanged.connect(self._updateFileName)
         self.zoom_apply.clicked.connect(self._applyZoom)
 
         # cellpose events
-        self.cellpose_flowthresh.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_flowthresh", "cellpose_flowthresh_label"))
-        self.cellpose_maskthresh.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_maskthresh", "cellpose_maskthresh_label"))
-        self.cellpose_minsize.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_minsize", "cellpose_minsize_label"))
-        self.cellpose_diameter.valueChanged.connect(lambda: self._updateSliderLabel("cellpose_diameter", "cellpose_diameter_label"))
-
-        self.cellpose_select_custom_model.clicked.connect(self._select_custom_cellpose_model)
-        self.cellpose_save_dir.clicked.connect(self._select_cellpose_save_directory)
+        self.cellpose_flowthresh.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_flowthresh", "cellpose_flowthresh_label"
+            )
+        )
+        self.cellpose_maskthresh.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_maskthresh", "cellpose_maskthresh_label"
+            )
+        )
+        self.cellpose_minsize.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_minsize", "cellpose_minsize_label"
+            )
+        )
+        self.cellpose_diameter.valueChanged.connect(
+            lambda: self._updateSliderLabel(
+                "cellpose_diameter", "cellpose_diameter_label"
+            )
+        )
+
+        self.cellpose_select_custom_model.clicked.connect(
+            self._select_custom_cellpose_model
+        )
+        self.cellpose_save_dir.clicked.connect(
+            self._select_cellpose_save_directory
+        )
         self.cellpose_segment_all.clicked.connect(self._segmentAll)
         self.cellpose_segment_active.clicked.connect(self._segmentActive)
         self.cellpose_train_model.clicked.connect(self._trainCellpose)
-        self.cellpose_segchannel.currentTextChanged.connect(self._updateSegChannels)
+        self.cellpose_segchannel.currentTextChanged.connect(
+            self._updateSegChannels
+        )
 
         # modify tab events
         self.modify_panzoom.clicked.connect(self._modifyMode(mode="panzoom"))
         self.modify_segment.clicked.connect(self._modifyMode(mode="segment"))
         self.modify_classify.clicked.connect(self._modifyMode(mode="classify"))
         self.modify_refine.clicked.connect(self._modifyMode(mode="refine"))
         self.modify_add.clicked.connect(self._modifyMode(mode="add"))
         self.modify_extend.clicked.connect(self._modifyMode(mode="extend"))
         self.modify_join.clicked.connect(self._modifyMode(mode="join"))
         self.modify_split.clicked.connect(self._modifyMode(mode="split"))
         self.modify_delete.clicked.connect(self._modifyMode(mode="delete"))
         self.classify_single.clicked.connect(self._modifyMode(mode="single"))
-        self.classify_dividing.clicked.connect(self._modifyMode(mode="dividing"))
+        self.classify_dividing.clicked.connect(
+            self._modifyMode(mode="dividing")
+        )
         self.classify_divided.clicked.connect(self._modifyMode(mode="divided"))
-        self.classify_vertical.clicked.connect(self._modifyMode(mode="vertical"))
+        self.classify_vertical.clicked.connect(
+            self._modifyMode(mode="vertical")
+        )
         self.classify_broken.clicked.connect(self._modifyMode(mode="broken"))
         self.classify_edge.clicked.connect(self._modifyMode(mode="edge"))
 
         self.viewer.bind_key(key="b", func=self.set_blurred, overwrite=True)
-        self.set_focus_1.clicked.connect(partial(self.set_image_quality, mode="focus", value=1))
-        self.set_focus_2.clicked.connect(partial(self.set_image_quality, mode="focus", value=2))
-        self.set_focus_3.clicked.connect(partial(self.set_image_quality, mode="focus", value=3))
-        self.set_focus_4.clicked.connect(partial(self.set_image_quality, mode="focus", value=4))
-        self.set_focus_5.clicked.connect(partial(self.set_image_quality, mode="focus", value=5))
+        self.set_focus_1.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=1)
+        )
+        self.set_focus_2.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=2)
+        )
+        self.set_focus_3.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=3)
+        )
+        self.set_focus_4.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=4)
+        )
+        self.set_focus_5.clicked.connect(
+            partial(self.set_image_quality, mode="focus", value=5)
+        )
         self.viewer.bind_key(key="f", func=self.set_focused, overwrite=True)
 
-        self.set_debris_1.clicked.connect(partial(self.set_image_quality, mode="debris", value=1))
-        self.set_debris_2.clicked.connect(partial(self.set_image_quality, mode="debris", value=2))
-        self.set_debris_3.clicked.connect(partial(self.set_image_quality, mode="debris", value=3))
-        self.set_debris_4.clicked.connect(partial(self.set_image_quality, mode="debris", value=4))
-        self.set_debris_5.clicked.connect(partial(self.set_image_quality, mode="debris", value=5))
-
-        self.modify_viewmasks.stateChanged.connect(self._viewerControls("viewmasks"))
-        self.modify_viewlabels.stateChanged.connect(self._viewerControls("viewlabels"))
+        self.set_debris_1.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=1)
+        )
+        self.set_debris_2.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=2)
+        )
+        self.set_debris_3.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=3)
+        )
+        self.set_debris_4.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=4)
+        )
+        self.set_debris_5.clicked.connect(
+            partial(self.set_image_quality, mode="debris", value=5)
+        )
+
+        self.modify_viewmasks.stateChanged.connect(
+            self._viewerControls("viewmasks")
+        )
+        self.modify_viewlabels.stateChanged.connect(
+            self._viewerControls("viewlabels")
+        )
         self.refine_all.clicked.connect(self._refine_bacseg)
         self.modify_copymasktoall.clicked.connect(self._copymasktoall)
-        self.modify_deleteallmasks.clicked.connect(self._deleteallmasks(mode="all"))
-        self.modify_deleteactivemasks.clicked.connect(self._deleteallmasks(mode="active"))
-        self.modify_deleteactiveimage.clicked.connect(self._delete_active_image(mode="active"))
-        self.modify_deleteotherimages.clicked.connect(self._delete_active_image(mode="other"))
+        self.modify_deleteallmasks.clicked.connect(
+            self._deleteallmasks(mode="all")
+        )
+        self.modify_deleteactivemasks.clicked.connect(
+            self._deleteallmasks(mode="active")
+        )
+        self.modify_deleteactiveimage.clicked.connect(
+            self._delete_active_image(mode="active")
+        )
+        self.modify_deleteotherimages.clicked.connect(
+            self._delete_active_image(mode="other")
+        )
         self.find_next.clicked.connect(self._sort_cells("next"))
         self.find_previous.clicked.connect(self._sort_cells("previous"))
-        self.modify_channel.currentTextChanged.connect(self._modify_channel_changed)
+        self.modify_channel.currentTextChanged.connect(
+            self._modify_channel_changed
+        )
 
         # export events
         self.export_active.clicked.connect(self._export("active"))
         self.export_all.clicked.connect(self._export("all"))
         self.export_stack_active.clicked.connect(self._export_stack("active"))
         self.export_stack_all.clicked.connect(self._export_stack("all"))
-        self.export_statistics_active.clicked.connect(self._export_statistics("active"))
-        self.export_statistics_all.clicked.connect(self._export_statistics("all"))
+        self.export_statistics_active.clicked.connect(
+            self._export_statistics("active")
+        )
+        self.export_statistics_all.clicked.connect(
+            self._export_statistics("all")
+        )
 
         # oufti events
-        self.oufti_generate_all_midlines.clicked.connect(self.generate_midlines(mode="all"))
-        self.oufti_generate_active_midlines.clicked.connect(self.generate_midlines(mode="active"))
-        self.viewer.bind_key(key="m", func=self.midline_edit_toggle, overwrite=True)
+        self.oufti_generate_all_midlines.clicked.connect(
+            self.generate_midlines(mode="all")
+        )
+        self.oufti_generate_active_midlines.clicked.connect(
+            self.generate_midlines(mode="active")
+        )
+        self.viewer.bind_key(
+            key="m", func=self.midline_edit_toggle, overwrite=True
+        )
         self.oufti_edit_mode.clicked.connect(self.midline_edit_toggle)
         self.oufti_panzoom_mode.clicked.connect(self.midline_edit_toggle)
-        self.oufti_centre_all_midlines.clicked.connect(self.centre_oufti_midlines(mode="all"))
-        self.oufti_centre_active_midlines.clicked.connect(self.centre_oufti_midlines(mode="active"))
+        self.oufti_centre_all_midlines.clicked.connect(
+            self.centre_oufti_midlines(mode="all")
+        )
+        self.oufti_centre_active_midlines.clicked.connect(
+            self.centre_oufti_midlines(mode="active")
+        )
 
         # upload tab events
         self.upload_all.clicked.connect(self._uploadDatabase(mode="all"))
         self.upload_active.clicked.connect(self._uploadDatabase(mode="active"))
         self.database_download.clicked.connect(self._downloadDatabase)
         self.create_database.clicked.connect(self._create_bacseg_database)
         self.load_database.clicked.connect(self._load_bacseg_database)
@@ -571,160 +938,334 @@
         self.update_metadata.clicked.connect(self.update_database_metadata)
 
         # viewer event that call updateFileName when the slider is modified
         self.contours = []
         self.viewer.dims.events.current_step.connect(self._sliderEvent)
 
         # self.segImage = self.viewer.add_image(np.zeros((1,100,100),dtype=np.uint16),name="Image")
-        self.class_colours = {1: (255 / 255, 255 / 255, 255 / 255, 1), 2: (0 / 255, 255 / 255, 0 / 255, 1), 3: (0 / 255, 170 / 255, 255 / 255, 1), 4: (170 / 255, 0 / 255, 255 / 255, 1), 5: (
-        255 / 255, 170 / 255, 0 / 255, 1), 6: (255 / 255, 0 / 255, 0 / 255, 1), }
-
-        self.classLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=0.25, name="Classes", color=self.class_colours, metadata={0: {"image_name": ""}}, visible=False, )
-        self.nucLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=1, name="Nucleoid", metadata={0: {"image_name": ""}}, )
-        self.segLayer = self.viewer.add_labels(np.zeros((1, 100, 100), dtype=np.uint16), opacity=1, name="Segmentations", metadata={0: {"image_name": ""}}, )
+        self.class_colours = {
+            1: (255 / 255, 255 / 255, 255 / 255, 1),
+            2: (0 / 255, 255 / 255, 0 / 255, 1),
+            3: (0 / 255, 170 / 255, 255 / 255, 1),
+            4: (170 / 255, 0 / 255, 255 / 255, 1),
+            5: (255 / 255, 170 / 255, 0 / 255, 1),
+            6: (255 / 255, 0 / 255, 0 / 255, 1),
+        }
+
+        self.classLayer = self.viewer.add_labels(
+            np.zeros((1, 100, 100), dtype=np.uint16),
+            opacity=0.25,
+            name="Classes",
+            color=self.class_colours,
+            metadata={0: {"image_name": ""}},
+            visible=False,
+        )
+        self.nucLayer = self.viewer.add_labels(
+            np.zeros((1, 100, 100), dtype=np.uint16),
+            opacity=1,
+            name="Nucleoid",
+            metadata={0: {"image_name": ""}},
+        )
+        self.segLayer = self.viewer.add_labels(
+            np.zeros((1, 100, 100), dtype=np.uint16),
+            opacity=1,
+            name="Segmentations",
+            metadata={0: {"image_name": ""}},
+        )
 
         self.segLayer.contour = 1
 
         # keyboard events, only triggered when viewer is not empty (an image is loaded/active)
-        self.viewer.bind_key(key="a", func=self._modifyMode(mode="add"), overwrite=True)
-        self.viewer.bind_key(key="e", func=self._modifyMode(mode="extend"), overwrite=True)
-        self.viewer.bind_key(key="j", func=self._modifyMode(mode="join"), overwrite=True)
-        self.viewer.bind_key(key="s", func=self._modifyMode(mode="split"), overwrite=True)
-        self.viewer.bind_key(key="d", func=self._modifyMode(mode="delete"), overwrite=True)
-        self.viewer.bind_key(key="r", func=self._modifyMode(mode="refine"), overwrite=True)
-        self.viewer.bind_key(key="k", func=self._modifyMode(mode="clicktozoom"), overwrite=True)
-        self.viewer.bind_key(key="Control-1", func=self._modifyMode(mode="single"), overwrite=True, )
-        self.viewer.bind_key(key="Control-2", func=self._modifyMode(mode="dividing"), overwrite=True, )
-        self.viewer.bind_key(key="Control-3", func=self._modifyMode(mode="divided"), overwrite=True, )
-        self.viewer.bind_key(key="Control-4", func=self._modifyMode(mode="vertical"), overwrite=True, )
-        self.viewer.bind_key(key="Control-5", func=self._modifyMode(mode="broken"), overwrite=True, )
-        self.viewer.bind_key(key="Control-6", func=self._modifyMode(mode="edge"), overwrite=True)
-        self.viewer.bind_key(key="F1", func=self._modifyMode(mode="panzoom"), overwrite=True)
-        self.viewer.bind_key(key="F2", func=self._modifyMode(mode="segment"), overwrite=True)
-        self.viewer.bind_key(key="F3", func=self._modifyMode(mode="classify"), overwrite=True)
-        self.viewer.bind_key(key="h", func=self._viewerControls("h"), overwrite=True)
-        self.viewer.bind_key(key="i", func=self._viewerControls("i"), overwrite=True)
-        self.viewer.bind_key(key="o", func=self._viewerControls("o"), overwrite=True)
-        self.viewer.bind_key(key="x", func=self._viewerControls("x"), overwrite=True)
-        self.viewer.bind_key(key="z", func=self._viewerControls("z"), overwrite=True)
-        self.viewer.bind_key(key="c", func=self._viewerControls("c"), overwrite=True)
-        self.viewer.bind_key(key="Right", func=self._imageControls("Right"), overwrite=True)
-        self.viewer.bind_key(key="Left", func=self._imageControls("Left"), overwrite=True)
-        self.viewer.bind_key(key="u", func=self._imageControls("Upload"), overwrite=True)
-        self.viewer.bind_key(key="Control-d", func=self._deleteallmasks(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-d", func=self._deleteallmasks(mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Control-i", func=self._delete_active_image(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-i", func=self._delete_active_image(mode="other"), overwrite=True, )
-
-        self.viewer.bind_key(key="Control-l", func=self._downloadDatabase(), overwrite=True)
-        self.viewer.bind_key(key="Control-u", func=self._uploadDatabase(mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Shift-u", func=self._uploadDatabase(mode="all"), overwrite=True, )
+        self.viewer.bind_key(
+            key="a", func=self._modifyMode(mode="add"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="e", func=self._modifyMode(mode="extend"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="j", func=self._modifyMode(mode="join"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="s", func=self._modifyMode(mode="split"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="d", func=self._modifyMode(mode="delete"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="r", func=self._modifyMode(mode="refine"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="k", func=self._modifyMode(mode="clicktozoom"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-1",
+            func=self._modifyMode(mode="single"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-2",
+            func=self._modifyMode(mode="dividing"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-3",
+            func=self._modifyMode(mode="divided"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-4",
+            func=self._modifyMode(mode="vertical"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-5",
+            func=self._modifyMode(mode="broken"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-6", func=self._modifyMode(mode="edge"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F1", func=self._modifyMode(mode="panzoom"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F2", func=self._modifyMode(mode="segment"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="F3", func=self._modifyMode(mode="classify"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="h", func=self._viewerControls("h"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="i", func=self._viewerControls("i"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="o", func=self._viewerControls("o"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="x", func=self._viewerControls("x"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="z", func=self._viewerControls("z"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="c", func=self._viewerControls("c"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Right", func=self._imageControls("Right"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Left", func=self._imageControls("Left"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="u", func=self._imageControls("Upload"), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-d",
+            func=self._deleteallmasks(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-d",
+            func=self._deleteallmasks(mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-i",
+            func=self._delete_active_image(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-i",
+            func=self._delete_active_image(mode="other"),
+            overwrite=True,
+        )
+
+        self.viewer.bind_key(
+            key="Control-l", func=self._downloadDatabase(), overwrite=True
+        )
+        self.viewer.bind_key(
+            key="Control-u",
+            func=self._uploadDatabase(mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Shift-u",
+            func=self._uploadDatabase(mode="all"),
+            overwrite=True,
+        )
         #
-        self.viewer.bind_key(key="Control-Left", func=self._manual_align_channels("left", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Right", func=self._manual_align_channels("right", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Up", func=self._manual_align_channels("up", mode="active"), overwrite=True, )
-        self.viewer.bind_key(key="Control-Down", func=self._manual_align_channels("down", mode="active"), overwrite=True, )
-
-        self.viewer.bind_key(key="Alt-Left", func=self._manual_align_channels("left", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Right", func=self._manual_align_channels("right", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Up", func=self._manual_align_channels("up", mode="all"), overwrite=True, )
-        self.viewer.bind_key(key="Alt-Down", func=self._manual_align_channels("down", mode="all"), overwrite=True, )
-
-        self.import_filemode.currentIndexChanged.connect(self.update_import_limit)
+        self.viewer.bind_key(
+            key="Control-Left",
+            func=self._manual_align_channels("left", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Right",
+            func=self._manual_align_channels("right", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Up",
+            func=self._manual_align_channels("up", mode="active"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Control-Down",
+            func=self._manual_align_channels("down", mode="active"),
+            overwrite=True,
+        )
+
+        self.viewer.bind_key(
+            key="Alt-Left",
+            func=self._manual_align_channels("left", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Right",
+            func=self._manual_align_channels("right", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Up",
+            func=self._manual_align_channels("up", mode="all"),
+            overwrite=True,
+        )
+        self.viewer.bind_key(
+            key="Alt-Down",
+            func=self._manual_align_channels("down", mode="all"),
+            overwrite=True,
+        )
+
+        self.import_filemode.currentIndexChanged.connect(
+            self.update_import_limit
+        )
         self.update_import_limit()
 
         # mouse events
         self.segLayer.mouse_drag_callbacks.append(self._segmentationEvents)
         self.nucLayer.mouse_drag_callbacks.append(self._segmentationEvents)
 
         # self.segLayer.mouse_move_callbac1ks.append(self._zoomEvents)
-        self.segLayer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+        self.segLayer.mouse_double_click_callbacks.append(
+            self._doubeClickEvents
+        )
 
         # viewer events
         self.viewer.layers.events.inserted.connect(self._manualImport)
-        self.viewer.layers.events.removed.connect(self._updateSegmentationCombo)
-        self.viewer.layers.selection.events.changed.connect(self._updateFileName)
+        self.viewer.layers.events.removed.connect(
+            self._updateSegmentationCombo
+        )
+        self.viewer.layers.selection.events.changed.connect(
+            self._updateFileName
+        )
 
         self.threadpool = QThreadPool()  # self.load_dev_data()
 
         self.widget_notifications = True
 
     def _applyZoom(self):
         try:
             import re
 
             magnification = self.zoom_magnification.currentText()
             pixel_resolution = float(self.scalebar_resolution.text())
-            magnification = (magnification.lower().replace("x", "").replace("%", ""))
+            magnification = (
+                magnification.lower().replace("x", "").replace("%", "")
+            )
 
             magnification = re.findall(r"\b\d+\b", magnification)[0]
 
             if magnification.isdigit():
                 magnification = int(magnification)
 
                 if magnification == 0:
                     self.viewer.reset_view()
                 elif magnification > 0:
                     magnification = 1 + magnification / 100
 
-                    self.viewer.camera.zoom = magnification * (1 / pixel_resolution)
+                    self.viewer.camera.zoom = magnification * (
+                        1 / pixel_resolution
+                    )
 
         except:
             print(traceback.format_exc())
 
     def _align_images(self, viewer=None, mode="active"):
         import scipy
         from skimage.registration import phase_cross_correlation
 
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+            ]
 
             if len(layer_names) > 2:
                 num_images = self.viewer.layers[layer_names[0]].data.shape[0]
 
                 if mode == "active":
                     fov_list = [self.viewer.dims.current_step[0]]
                 else:
                     fov_list = range(num_images)
 
                 alignment_channel = self.alignment_channel.currentText()
                 current_fov = self.viewer.dims.current_step[0]
 
-                target_channels = [layer for layer in layer_names if layer != alignment_channel]
+                target_channels = [
+                    layer
+                    for layer in layer_names
+                    if layer != alignment_channel
+                ]
 
                 for channel in target_channels:
                     image_stack = self.viewer.layers[channel].data.copy()
-                    target_image_stack = self.viewer.layers[alignment_channel].data.copy()
+                    target_image_stack = self.viewer.layers[
+                        alignment_channel
+                    ].data.copy()
 
                     for fov in fov_list:
                         target_image = image_stack[fov, :, :]
                         alignment_image = target_image_stack[fov, :, :]
 
-                        shift, error, diffphase = phase_cross_correlation(alignment_image, target_image, upsample_factor=100)
+                        shift, error, diffphase = phase_cross_correlation(
+                            alignment_image, target_image, upsample_factor=100
+                        )
 
                         shifted_img = scipy.ndimage.shift(target_image, shift)
 
                         image_stack[fov, :, :] = shifted_img
 
                     self.viewer.layers[channel].data = image_stack
 
-                show_info(f"{len(fov_list)} Image(s) aligned to channel: " + alignment_channel)
+                show_info(
+                    f"{len(fov_list)} Image(s) aligned to channel: "
+                    + alignment_channel
+                )
 
         except:
             pass
 
     def set_blurred(self, viewer=None):
         self.set_image_quality(mode="focus", value=1)
 
     def set_focused(self, viewer=None):
         self.set_image_quality(mode="focus", value=5)
 
     def set_image_quality(self, mode="", value=""):
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+            ]
 
             update_mode = self.set_quality_mode.currentIndex()
 
             if len(layer_names) > 0:
                 current_fov = self.viewer.dims.current_step[0]
                 n_frames = self.viewer.dims.nsteps[0]
                 active_layer = self.viewer.layers.selection.active.name
@@ -767,21 +1308,28 @@
         except:
             pass
 
         return func
 
     def overwrite_channel_info(self):
         all_layers = [layer.name for layer in self.viewer.layers]
-        selected_layers = [layer.name for layer in self.viewer.layers.selection]
+        selected_layers = [
+            layer.name for layer in self.viewer.layers.selection
+        ]
 
         if len(selected_layers) == 1:
             selected_layer = selected_layers[0]
             all_layers.pop(all_layers.index(selected_layer))
 
-            if selected_layer not in ["Segmentations", "Nucleoid", "Classes", "center_lines", ]:
+            if selected_layer not in [
+                "Segmentations",
+                "Nucleoid",
+                "Classes",
+                "center_lines",
+            ]:
                 metadata = self.viewer.layers[selected_layer].metadata.copy()
 
                 label_modality = self.label_modality.currentText()
                 label_light_source = self.label_light_source.currentText()
                 label_stain = self.label_stain.currentText()
                 label_stain_target = self.label_stain_target.currentText()
 
@@ -821,47 +1369,74 @@
             colicoords_channel = colicoords_channel.replace("Mask + ", "")
 
             if pixel_size <= 0:
                 pixel_size = 1
 
             desktop = os.path.expanduser("~/Desktop")
 
-            path = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+            path = QFileDialog.getExistingDirectory(
+                self, "Select Directory", desktop
+            )
 
             colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
 
             if os.path.isdir(colicoords_dir) != True:
                 os.mkdir(colicoords_dir)
             else:
                 shutil.rmtree(colicoords_dir)
                 os.mkdir(colicoords_dir)
 
             if os.path.isdir(path):
                 path = os.path.abspath(path)
 
-                from napari_bacseg._utils_statistics import (get_cell_statistics, process_cell_statistics, )
+                from napari_bacseg._utils_statistics import (
+                    get_cell_statistics,
+                    process_cell_statistics,
+                )
 
                 self.get_cell_statistics = self.wrapper(get_cell_statistics)
-                self.process_cell_statistics = self.wrapper(process_cell_statistics)
-
-                worker = Worker(self.get_cell_statistics, mode=mode, pixel_size=pixel_size, colicoords_dir=colicoords_dir, )
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
-                worker.signals.result.connect(self.process_cell_statistics(path=path))
+                self.process_cell_statistics = self.wrapper(
+                    process_cell_statistics
+                )
+
+                worker = Worker(
+                    self.get_cell_statistics,
+                    mode=mode,
+                    pixel_size=pixel_size,
+                    colicoords_dir=colicoords_dir,
+                )
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="export")
+                )
+                worker.signals.result.connect(
+                    self.process_cell_statistics(path=path)
+                )
                 self.threadpool.start(worker)
                 cell_data = worker.result()
 
                 if self.export_colicoords_mode.currentIndex() != 0:
                     from napari_bacseg._utils_colicoords import run_colicoords
 
                     self.run_colicoords = self.wrapper(run_colicoords)
 
-                    worker = Worker(self.run_colicoords, cell_data=cell_data, colicoords_channel=colicoords_channel, pixel_size=pixel_size, statistics=True, multithreaded=multithreaded, )
-
-                    worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
-                    worker.signals.result.connect(self.process_cell_statistics(path=path))
+                    worker = Worker(
+                        self.run_colicoords,
+                        cell_data=cell_data,
+                        colicoords_channel=colicoords_channel,
+                        pixel_size=pixel_size,
+                        statistics=True,
+                        multithreaded=multithreaded,
+                    )
+
+                    worker.signals.progress.connect(
+                        partial(self._Progresbar, progressbar="export")
+                    )
+                    worker.signals.result.connect(
+                        self.process_cell_statistics(path=path)
+                    )
                     self.threadpool.start(worker)
 
         return _event
 
     def update_import_limit(self):
         if self.import_filemode.currentIndex() == 0:
             self.import_limit.setEnabled(False)
@@ -896,34 +1471,49 @@
                     criterion = meta["simple_cell_stats"]["cell_area"]
                 if find_criterion == "Cell Solidity":
                     criterion = meta["simple_cell_stats"]["cell_solidity"]
                 if find_criterion == "Cell Aspect Ratio":
                     criterion = meta["simple_cell_stats"]["cell_aspect_ratio"]
 
                 if find_mode == "Ascending":
-                    criterion, cell_centre, cell_zoom = zip(*sorted(zip(criterion, cell_centre, cell_zoom), key=lambda x: x[0], ))
+                    criterion, cell_centre, cell_zoom = zip(
+                        *sorted(
+                            zip(criterion, cell_centre, cell_zoom),
+                            key=lambda x: x[0],
+                        )
+                    )
                 else:
-                    criterion, cell_centre, cell_zoom = zip(*sorted(zip(criterion, cell_centre, cell_zoom), key=lambda x: x[0], reverse=True, ))
-
-                current_position = tuple(np.array(self.viewer.camera.center).round())
+                    criterion, cell_centre, cell_zoom = zip(
+                        *sorted(
+                            zip(criterion, cell_centre, cell_zoom),
+                            key=lambda x: x[0],
+                            reverse=True,
+                        )
+                    )
+
+                current_position = tuple(
+                    np.array(self.viewer.camera.center).round()
+                )
 
                 if current_position not in cell_centre:
                     self.viewer.camera.center = cell_centre[0]
                     self.viewer.camera.zoom = cell_zoom[0]
 
                 else:
                     current_index = cell_centre.index(current_position)
 
                     if order == "next":
                         new_index = current_index + 1
 
                     if order == "previous":
                         new_index = current_index - 1
 
-                    new_index = max(current_fov, min(new_index, len(cell_centre) - 1))
+                    new_index = max(
+                        current_fov, min(new_index, len(cell_centre) - 1)
+                    )
 
                     self.viewer.camera.center = cell_centre[new_index]
                     self.viewer.camera.zoom = cell_zoom[new_index]
 
             except:
                 pass
 
@@ -948,15 +1538,19 @@
             elif key == "right":
                 shift_vector = [0.0, 1.0]
             else:
                 shift_vector = [0.0, 0.0]
 
             shift_image = False
             if active_layer != None:
-                if active_layer.name not in ["Segmentations", "Classes", "center_lines", ]:
+                if active_layer.name not in [
+                    "Segmentations",
+                    "Classes",
+                    "center_lines",
+                ]:
                     shift_image = True
 
             if shift_image is True:
                 if mode == "active":
                     image_stack = active_layer.data.copy()
                     image = image_stack[current_fov, :, :]
                     image = shift(image, shift=shift_vector)
@@ -1004,90 +1598,146 @@
 
         channel = self.refine_channel.currentText()
         colicoords_channel = channel.replace("Mask + ", "")
 
         mask_stack = self.segLayer.data
         mask = mask_stack[current_fov, :, :].copy()
 
-        from napari_bacseg._utils_colicoords import (process_colicoords, run_colicoords, )
+        from napari_bacseg._utils_colicoords import (
+            process_colicoords,
+            run_colicoords,
+        )
         from napari_bacseg._utils_statistics import get_cell_statistics
 
         self.get_cell_statistics = self.wrapper(get_cell_statistics)
         self.run_colicoords = self.wrapper(run_colicoords)
         self.process_colicoords = self.wrapper(process_colicoords)
 
         colicoords_dir = os.path.join(tempfile.gettempdir(), "colicoords")
 
-        worker = Worker(self.get_cell_statistics, mode="active", pixel_size=pixel_size, colicoords_dir=colicoords_dir, )
+        worker = Worker(
+            self.get_cell_statistics,
+            mode="active",
+            pixel_size=pixel_size,
+            colicoords_dir=colicoords_dir,
+        )
 
         self.threadpool.start(worker)
         cell_data = worker.result()
 
-        worker = Worker(self.run_colicoords, cell_data=cell_data, colicoords_channel=colicoords_channel, pixel_size=pixel_size, multithreaded=True, )
-
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="modify"))
+        worker = Worker(
+            self.run_colicoords,
+            cell_data=cell_data,
+            colicoords_channel=colicoords_channel,
+            pixel_size=pixel_size,
+            multithreaded=True,
+        )
+
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="modify")
+        )
         worker.signals.result.connect(self.process_colicoords)
         self.threadpool.start(worker)
 
     def _uploadDatabase(self, viewer=None, mode=""):
         def _event(viewer):
             try:
-                if (self.database_path != "" and os.path.exists(self.database_path) == True):
+                if (
+                    self.database_path != ""
+                    and os.path.exists(self.database_path) == True
+                ):
                     if self.unfolded == True:
                         self.fold_images()
 
-                    if self.upload_initial.currentText() in ["", "Required for upload", ]:
+                    if self.upload_initial.currentText() in [
+                        "",
+                        "Required for upload",
+                    ]:
                         show_info("Please select the user initial.")
                     else:
-                        from napari_bacseg._utils_database_IO import (_upload_bacseg_database, )
-
-                        self._upload_bacseg_database = self.wrapper(_upload_bacseg_database)
-
-                        worker = Worker(self._upload_bacseg_database, mode=mode)
-                        worker.signals.progress.connect(partial(self._Progresbar, progressbar="database"))
+                        from napari_bacseg._utils_database_IO import (
+                            _upload_bacseg_database,
+                        )
+
+                        self._upload_bacseg_database = self.wrapper(
+                            _upload_bacseg_database
+                        )
+
+                        worker = Worker(
+                            self._upload_bacseg_database, mode=mode
+                        )
+                        worker.signals.progress.connect(
+                            partial(self._Progresbar, progressbar="database")
+                        )
                         self.threadpool.start(worker)
             except:
                 pass
 
         return _event
 
     def _downloadDatabase(self, viewer=None):
         try:
-            if (self.database_path != "" and os.path.exists(self.database_path) == True):
+            if (
+                self.database_path != ""
+                and os.path.exists(self.database_path) == True
+            ):
                 if self.unfolded == True:
                     self.fold_images()
 
-                if self.upload_initial.currentText() in ["", "Required for upload", ]:
+                if self.upload_initial.currentText() in [
+                    "",
+                    "Required for upload",
+                ]:
                     show_info("Please select the user initial.")
 
                 else:
-                    from napari_bacseg._utils_database_IO import (get_filtered_database_metadata, read_bacseg_images, )
-
-                    self.get_filtered_database_metadata = self.wrapper(get_filtered_database_metadata)
+                    from napari_bacseg._utils_database_IO import (
+                        get_filtered_database_metadata,
+                        read_bacseg_images,
+                    )
+
+                    self.get_filtered_database_metadata = self.wrapper(
+                        get_filtered_database_metadata
+                    )
                     self.read_bacseg_images = self.wrapper(read_bacseg_images)
 
                     self.active_import_mode = "BacSeg"
 
-                    (measurements, file_paths, channels,) = self.get_filtered_database_metadata()
+                    (
+                        measurements,
+                        file_paths,
+                        channels,
+                    ) = self.get_filtered_database_metadata()
 
                     if len(file_paths) == 0:
                         if self.widget_notifications:
                             show_info("no matching database files found")
 
                     else:
-                        worker = Worker(self.read_bacseg_images, measurements=measurements, channels=channels, )
+                        worker = Worker(
+                            self.read_bacseg_images,
+                            measurements=measurements,
+                            channels=channels,
+                        )
                         worker.signals.result.connect(self._process_import)
-                        worker.signals.progress.connect(partial(self._Progresbar, progressbar="database"))
+                        worker.signals.progress.connect(
+                            partial(self._Progresbar, progressbar="database")
+                        )
                         self.threadpool.start(worker)
 
         except:
             print(traceback.format_exc())
 
     def _updateSegChannels(self):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name
+            not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+        ]
 
         segChannel = self.cellpose_segchannel.currentText()
 
         self.export_channel.setCurrentText(segChannel)
 
     def _Progresbar(self, progress, progressbar):
         if progressbar == "import":
@@ -1127,225 +1777,301 @@
         if import_mode == "JSON (.txt) Segmentation(s)":
             file_extension = "*.txt"
 
         desktop = os.path.expanduser("~/Desktop")
 
         if type(paths) is not list:
             if import_filemode == "Import File(s)":
-                paths, _ = QFileDialog.getOpenFileNames(self, "Open Files", desktop, f"Files ({file_extension})")
+                paths, _ = QFileDialog.getOpenFileNames(
+                    self, "Open Files", desktop, f"Files ({file_extension})"
+                )
 
             if import_filemode == "Import Directory":
-                path = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+                path = QFileDialog.getExistingDirectory(
+                    self, "Select Directory", desktop
+                )
 
                 paths = [path]
 
         if "" in paths or paths == [] or type(paths) is not list:
             if self.widget_notifications:
                 show_info("No file/folder selected")
 
         else:
             if import_mode == "Images":
-                self.import_images = self.wrapper(napari_bacseg._utils.import_images)
+                self.import_images = self.wrapper(
+                    napari_bacseg._utils.import_images
+                )
 
                 worker = Worker(self.import_images, file_paths=paths)
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "NanoImager Data":
-                self.read_nim_directory = self.wrapper(napari_bacseg._utils.read_nim_directory)
-                self.read_nim_images = self.wrapper(napari_bacseg._utils.read_nim_images)
-
-                measurements, file_paths, channels = self.read_nim_directory(paths)
-
-                worker = Worker(self.read_nim_images, measurements=measurements, channels=channels, )
+                self.read_nim_directory = self.wrapper(
+                    napari_bacseg._utils.read_nim_directory
+                )
+                self.read_nim_images = self.wrapper(
+                    napari_bacseg._utils.read_nim_images
+                )
+
+                measurements, file_paths, channels = self.read_nim_directory(
+                    paths
+                )
+
+                worker = Worker(
+                    self.read_nim_images,
+                    measurements=measurements,
+                    channels=channels,
+                )
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "Mask (.tif) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".tif")
                 self._autoClassify()
 
             if import_mode == "Cellpose (.npy) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".npy")
                 self._autoClassify()
 
             if import_mode == "Oufti (.mat) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".mat")
                 self._autoClassify()
 
             if import_mode == "JSON (.txt) Segmentation(s)":
-                self.import_masks = self.wrapper(napari_bacseg._utils.import_masks)
+                self.import_masks = self.wrapper(
+                    napari_bacseg._utils.import_masks
+                )
                 self.import_masks(paths, file_extension=".txt")
                 self._autoClassify()
 
             if import_mode == "ImageJ files(s)":
-                self.import_imagej = self.wrapper(napari_bacseg._utils.import_imagej)
+                self.import_imagej = self.wrapper(
+                    napari_bacseg._utils.import_imagej
+                )
 
                 worker = Worker(self.import_imagej, paths=paths)
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
             if import_mode == "ScanR Data":
-                from napari_bacseg._utils import (read_scanr_directory, read_scanr_images, )
+                from napari_bacseg._utils import (
+                    read_scanr_directory,
+                    read_scanr_images,
+                )
 
                 self.read_scanr_images = self.wrapper(read_scanr_images)
 
-                measurements, file_paths, channels = read_scanr_directory(self, paths)
-
-                worker = Worker(self.read_scanr_images, measurements=measurements, channels=channels, )
+                measurements, file_paths, channels = read_scanr_directory(
+                    self, paths
+                )
+
+                worker = Worker(
+                    self.read_scanr_images,
+                    measurements=measurements,
+                    channels=channels,
+                )
                 worker.signals.result.connect(self._process_import)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="import"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="import")
+                )
                 self.threadpool.start(worker)
 
     def _export_stack(self, mode, viewer=None):
-
         def _event(viewer):
-
             execute_export = True
 
             if self.export_location.currentIndex() == 1:
                 desktop = os.path.expanduser("~/Desktop")
-                self.export_directory = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+                self.export_directory = QFileDialog.getExistingDirectory(
+                    self, "Select Directory", desktop
+                )
 
                 if self.export_directory == "":
                     execute_export = False
 
             if execute_export == True:
-                self.export_stacks = self.wrapper(napari_bacseg._utils.export_stacks)
+                self.export_stacks = self.wrapper(
+                    napari_bacseg._utils.export_stacks
+                )
 
                 worker = Worker(self.export_stacks, mode=mode)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="export")
+                )
                 self.threadpool.start(worker)
 
         return _event
 
-
     def _export(self, mode, viewer=None):
         def _event(viewer):
             # if self.unfolded == True:
             #     self.fold_images()
 
             execute_export = True
 
             if self.export_location.currentIndex() == 1:
                 desktop = os.path.expanduser("~/Desktop")
-                self.export_directory = QFileDialog.getExistingDirectory(self, "Select Directory", desktop)
+                self.export_directory = QFileDialog.getExistingDirectory(
+                    self, "Select Directory", desktop
+                )
 
                 if self.export_directory == "":
                     execute_export = False
 
             if execute_export == True:
-                self.export_files = self.wrapper(napari_bacseg._utils.export_files)
+                self.export_files = self.wrapper(
+                    napari_bacseg._utils.export_files
+                )
 
                 worker = Worker(self.export_files, mode=mode)
-                worker.signals.progress.connect(partial(self._Progresbar, progressbar="export"))
+                worker.signals.progress.connect(
+                    partial(self._Progresbar, progressbar="export")
+                )
                 self.threadpool.start(worker)
 
         return _event
 
     def _trainCellpose(self):
         if self.unfolded == True:
             self.fold_images()
 
         from napari_bacseg._utils_cellpose import train_cellpose_model
 
         self.train_cellpose_model = self.wrapper(train_cellpose_model)
 
         worker = Worker(self.train_cellpose_model)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose_train"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose_train")
+        )
         self.threadpool.start(worker)
 
     def _segmentActive(self):
         if self.unfolded == True:
             self.fold_images()
 
-        from napari_bacseg._utils_cellpose import (_process_cellpose, _run_cellpose, )
+        from napari_bacseg._utils_cellpose import (
+            _process_cellpose,
+            _run_cellpose,
+        )
 
         self._run_cellpose = self.wrapper(_run_cellpose)
         self._process_cellpose = self.wrapper(_process_cellpose)
 
         current_fov = self.viewer.dims.current_step[0]
         chanel = self.cellpose_segchannel.currentText()
 
         images = self.viewer.layers[chanel].data
 
         image = [images[current_fov, :, :]]
 
         worker = Worker(self._run_cellpose, images=image)
         worker.signals.result.connect(self._process_cellpose)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose")
+        )
         self.threadpool.start(worker)
 
     def _segmentAll(self):
         if self.unfolded == True:
             self.fold_images()
 
-        from napari_bacseg._utils_cellpose import (_process_cellpose, _run_cellpose, )
+        from napari_bacseg._utils_cellpose import (
+            _process_cellpose,
+            _run_cellpose,
+        )
 
         self._run_cellpose = self.wrapper(_run_cellpose)
         self._process_cellpose = self.wrapper(_process_cellpose)
 
         channel = self.cellpose_segchannel.currentText()
 
         images = self.viewer.layers[channel].data
 
         images = unstack_images(images)
 
         worker = Worker(self._run_cellpose, images=images)
         worker.signals.result.connect(self._process_cellpose)
-        worker.signals.progress.connect(partial(self._Progresbar, progressbar="cellpose"))
+        worker.signals.progress.connect(
+            partial(self._Progresbar, progressbar="cellpose")
+        )
         self.threadpool.start(worker)
 
     def _updateSliderLabel(self, slider_name, label_name):
         self.slider = self.findChild(QSlider, slider_name)
         self.label = self.findChild(QLabel, label_name)
 
         slider_value = self.slider.value()
 
-        if (slider_name == "cellpose_flowthresh" or slider_name == "cellpose_maskthresh"):
+        if (
+            slider_name == "cellpose_flowthresh"
+            or slider_name == "cellpose_maskthresh"
+        ):
             self.label.setText(str(slider_value / 100))
         else:
             self.label.setText(str(slider_value))
 
     def _updateSegmentationCombo(self):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name
+            not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+        ]
 
         self.cellpose_segchannel.clear()
         self.cellpose_segchannel.addItems(layer_names)
 
         self.cellpose_trainchannel.clear()
         self.cellpose_trainchannel.addItems(layer_names)
 
         self.cellpose_trainchannel.clear()
         self.cellpose_trainchannel.addItems(layer_names)
 
         self.alignment_channel.clear()
         self.alignment_channel.addItems(layer_names)
 
+        self.export_stack_channel.clear()
+        self.export_stack_channel.addItems(layer_names)
+
         self.export_channel.clear()
         export_layers = layer_names
-        export_layers.extend(["All Channels (Stack)", "First Three Channels (RGB)"])
+        export_layers.extend(
+            ["All Channels (Stack)", "First Three Channels (RGB)"]
+        )
         self.export_channel.addItems(export_layers)
 
-        self.export_stack_channel.clear()
-        self.export_stack_channel.addItems(layer_names)
-
         self.refine_channel.clear()
         refine_layers = ["Mask + " + layer for layer in layer_names]
         self.refine_channel.addItems(["Mask"] + refine_layers)
 
         self.export_colicoords_mode.clear()
         refine_layers = ["Mask + " + layer for layer in layer_names]
-        self.export_colicoords_mode.addItems(["None (OpenCV Stats)", "Mask"] + refine_layers)
+        self.export_colicoords_mode.addItems(
+            ["None (OpenCV Stats)", "Mask"] + refine_layers
+        )
 
     def _sliderEvent(self, current_step):
         try:
             active_layer = self.viewer.layers.selection.active
 
             crop = active_layer.corner_pixels.T
 
@@ -1365,93 +2091,176 @@
         try:
             if self.scalebar_show.isChecked() and len(layer_names) > 0:
                 pixel_resolution = float(self.scalebar_resolution.text())
                 scalebar_units = self.scalebar_units.currentText()
 
                 if pixel_resolution > 0:
                     for layer in layer_names:
-                        self.viewer.layers[layer].scale = [1, pixel_resolution, pixel_resolution, ]
+                        self.viewer.layers[layer].scale = [
+                            1,
+                            pixel_resolution,
+                            pixel_resolution,
+                        ]
 
                         self.viewer.scale_bar.visible = True
                         self.viewer.scale_bar.unit = scalebar_units
                         self.viewer.reset_view()
 
             else:
                 self.viewer.scale_bar.visible = False
 
         except:
             self.viewer.scale_bar.visible = False
 
     def _autoContrast(self):
         try:
             if self.autocontrast.isChecked():
-                layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines", ]]
+                layer_names = [
+                    layer.name
+                    for layer in self.viewer.layers
+                    if layer.name
+                    not in [
+                        "Segmentations",
+                        "Nucleoid",
+                        "Classes",
+                        "center_lines",
+                    ]
+                ]
 
                 if len(layer_names) != 0:
                     active_layer = layer_names[-1]
 
-                    image_dims = tuple(list(self.viewer.dims.current_step[:-2]) + [...])
-
-                    image = (self.viewer.layers[str(active_layer)].data[image_dims].copy())
-
-                    crop = self.viewer.layers[str(active_layer)].corner_pixels[:, -2:]
+                    image_dims = tuple(
+                        list(self.viewer.dims.current_step[:-2]) + [...]
+                    )
+
+                    image = (
+                        self.viewer.layers[str(active_layer)]
+                        .data[image_dims]
+                        .copy()
+                    )
+
+                    crop = self.viewer.layers[str(active_layer)].corner_pixels[
+                        :, -2:
+                    ]
 
                     [[y1, x1], [y2, x2]] = crop
 
                     image_crop = image[y1:y2, x1:x2]
 
-                    contrast_limit = np.percentile(image_crop[image_crop != 0], (1, 99))
-                    contrast_limit = [int(contrast_limit[0] * 0.5), int(contrast_limit[1] * 2), ]
+                    contrast_limit = np.percentile(
+                        image_crop[image_crop != 0], (1, 99)
+                    )
+                    contrast_limit = [
+                        int(contrast_limit[0] * 0.5),
+                        int(contrast_limit[1] * 2),
+                    ]
 
                     if contrast_limit[1] > contrast_limit[0]:
-                        self.viewer.layers[str(active_layer)].contrast_limits = contrast_limit
+                        self.viewer.layers[
+                            str(active_layer)
+                        ].contrast_limits = contrast_limit
 
         except:
             pass
 
     def _updateFileName(self):
         try:
             current_fov = self.viewer.dims.current_step[0]
             active_layer = self.viewer.layers.selection.active
 
             image = self.viewer.layers[str(active_layer)].data[current_fov]
-            metadata = self.viewer.layers[str(active_layer)].metadata[current_fov]
+            metadata = self.viewer.layers[str(active_layer)].metadata[
+                current_fov
+            ]
 
             viewer_text = ""
 
             # print(metadata['image_name'])
 
-            if (self.overlay_filename.isChecked() and "image_name" in metadata.keys()):
+            if (
+                self.overlay_filename.isChecked()
+                and "image_name" in metadata.keys()
+            ):
                 viewer_text = f"File Name: {metadata['image_name']}"
             if self.overlay_folder.isChecked() and "folder" in metadata.keys():
                 viewer_text = viewer_text + f"\nFolder: {metadata['folder']}"
-            if (self.overlay_microscope.isChecked() and "microscope" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nMicroscope: {metadata['microscope']}")
-            if (self.overlay_datemodified.isChecked() and "date_modified" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nDate Modified: {metadata['date_modified']}")
-            if (self.overlay_content.isChecked() and "content" in metadata.keys()):
+            if (
+                self.overlay_microscope.isChecked()
+                and "microscope" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nMicroscope: {metadata['microscope']}"
+                )
+            if (
+                self.overlay_datemodified.isChecked()
+                and "date_modified" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text
+                    + f"\nDate Modified: {metadata['date_modified']}"
+                )
+            if (
+                self.overlay_content.isChecked()
+                and "content" in metadata.keys()
+            ):
                 viewer_text = viewer_text + f"\nContent: {metadata['content']}"
             if self.overlay_strain.isChecked() and "strain" in metadata.keys():
                 viewer_text = viewer_text + f"\nStrain: {metadata['strain']}"
-            if (self.overlay_phenotype.isChecked() and "phenotype" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nPhenotype: {metadata['phenotype']}")
-            if (self.overlay_antibiotic.isChecked() and "antibiotic" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nAntibiotic: {metadata['antibiotic']}")
+            if (
+                self.overlay_phenotype.isChecked()
+                and "phenotype" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nPhenotype: {metadata['phenotype']}"
+                )
+            if (
+                self.overlay_antibiotic.isChecked()
+                and "antibiotic" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nAntibiotic: {metadata['antibiotic']}"
+                )
             if self.overlay_stain.isChecked() and "stain" in metadata.keys():
                 viewer_text = viewer_text + f"\nStain: {metadata['stain']}"
-            if (self.overlay_staintarget.isChecked() and "stain_target" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nStain Target: {metadata['stain_target']}")
-            if (self.overlay_modality.isChecked() and "modality" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nModality: {metadata['modality']}")
-            if (self.overlay_lightsource.isChecked() and "source" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nLight Source: {metadata['source']}")
-            if (self.overlay_focus.isChecked() and "image_focus" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nImage Focus: {metadata['image_focus']}")
-            if (self.overlay_debris.isChecked() and "image_debris" in metadata.keys()):
-                viewer_text = (viewer_text + f"\nImage Debris: {metadata['image_debris']}")
+            if (
+                self.overlay_staintarget.isChecked()
+                and "stain_target" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nStain Target: {metadata['stain_target']}"
+                )
+            if (
+                self.overlay_modality.isChecked()
+                and "modality" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nModality: {metadata['modality']}"
+                )
+            if (
+                self.overlay_lightsource.isChecked()
+                and "source" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nLight Source: {metadata['source']}"
+                )
+            if (
+                self.overlay_focus.isChecked()
+                and "image_focus" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nImage Focus: {metadata['image_focus']}"
+                )
+            if (
+                self.overlay_debris.isChecked()
+                and "image_debris" in metadata.keys()
+            ):
+                viewer_text = (
+                    viewer_text + f"\nImage Debris: {metadata['image_debris']}"
+                )
             if self.overlay_laplacian.isChecked():
                 image_laplacian = np.mean(cv2.Laplacian(image, cv2.CV_64F))
                 viewer_text = viewer_text + f"\nLaplacian: {image_laplacian}"
             if self.overlay_range.isChecked():
                 image_range = np.max(image) - np.min(image)
                 viewer_text = viewer_text + f"\nRange: {image_range}"
 
@@ -1461,15 +2270,20 @@
             else:
                 self.viewer.text_overlay.visible = False
 
         except:
             pass
 
     def _process_import(self, imported_data, rearrange=True):
-        layer_names = [layer.name for layer in self.viewer.layers if layer.name not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
+        layer_names = [
+            layer.name
+            for layer in self.viewer.layers
+            if layer.name
+            not in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+        ]
 
         if self.clear_previous.isChecked() == True:
             # removes all layers (except segmentation layer)
             for layer_name in layer_names:
                 self.viewer.layers.remove(self.viewer.layers[layer_name])
             # reset segmentation and class layers
             self.segLayer.data = np.zeros((1, 100, 100), dtype=np.uint16)
@@ -1498,82 +2312,165 @@
 
             new_image_stack, new_metadata = stack_images(images, metadata)
             new_mask_stack, new_metadata = stack_images(masks, metadata)
             new_nmask_stack, new_metadata = stack_images(nmasks, metadata)
             new_class_stack, new_metadata = stack_images(classes, metadata)
 
             if len(new_mask_stack) == 0:
-                new_mask_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+                new_mask_stack = np.zeros(
+                    new_image_stack.shape, dtype=np.uint16
+                )
 
             if len(new_nmask_stack) == 0:
-                new_nmask_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+                new_nmask_stack = np.zeros(
+                    new_image_stack.shape, dtype=np.uint16
+                )
 
             if len(new_class_stack) == 0:
-                new_class_stack = np.zeros(new_image_stack.shape, dtype=np.uint16)
+                new_class_stack = np.zeros(
+                    new_image_stack.shape, dtype=np.uint16
+                )
 
             colormap = "gray"
 
             if layer_name == "405":
                 colormap = "green"
             if layer_name == "532":
                 colormap = "red"
             if layer_name == "Cy3":
                 colormap = "red"
             if layer_name == "DAPI":
                 colormap = "green"
 
-            if (self.clear_previous.isChecked() == False and layer_name in layer_names):
+            if (
+                self.clear_previous.isChecked() == False
+                and layer_name in layer_names
+            ):
                 current_image_stack = self.viewer.layers[layer_name].data
                 current_metadata = self.viewer.layers[layer_name].metadata
                 current_mask_stack = self.segLayer.data
                 current_nmask_stack = self.nucLayer.data
                 current_class_stack = self.classLayer.data
 
                 if len(current_image_stack) == 0:
-                    setattr(self, layer_name, self.viewer.add_image(new_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=new_metadata, ), )
+                    setattr(
+                        self,
+                        layer_name,
+                        self.viewer.add_image(
+                            new_image_stack,
+                            name=layer_name,
+                            colormap=colormap,
+                            gamma=0.8,
+                            metadata=new_metadata,
+                        ),
+                    )
 
                     image_layer = getattr(self, layer_name)
-                    image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                    image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                    image_layer.mouse_drag_callbacks.append(
+                        self._segmentationEvents
+                    )
+                    image_layer.mouse_double_click_callbacks.append(
+                        self._doubeClickEvents
+                    )
 
                     self.segLayer.data = new_mask_stack
                     self.nucLayer.data = new_nmask_stack
                     self.classLayer.data = new_class_stack
                     self.segLayer.metadata = new_metadata
 
                 else:
                     from napari_bacseg._utils import append_image_stacks
 
-                    (appended_image_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_image_stack, new_image_stack, )
-
-                    (appended_mask_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_mask_stack, new_mask_stack, )
-
-                    (appended_nmask_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_nmask_stack, new_nmask_stack, )
-
-                    (appended_class_stack, appended_metadata,) = append_image_stacks(current_metadata, new_metadata, current_class_stack, new_class_stack, )
+                    (
+                        appended_image_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_image_stack,
+                        new_image_stack,
+                    )
+
+                    (
+                        appended_mask_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_mask_stack,
+                        new_mask_stack,
+                    )
+
+                    (
+                        appended_nmask_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_nmask_stack,
+                        new_nmask_stack,
+                    )
+
+                    (
+                        appended_class_stack,
+                        appended_metadata,
+                    ) = append_image_stacks(
+                        current_metadata,
+                        new_metadata,
+                        current_class_stack,
+                        new_class_stack,
+                    )
 
                     self.viewer.layers.remove(self.viewer.layers[layer_name])
 
-                    setattr(self, layer_name, self.viewer.add_image(appended_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=appended_metadata, ), )
+                    setattr(
+                        self,
+                        layer_name,
+                        self.viewer.add_image(
+                            appended_image_stack,
+                            name=layer_name,
+                            colormap=colormap,
+                            gamma=0.8,
+                            metadata=appended_metadata,
+                        ),
+                    )
 
                     image_layer = getattr(self, layer_name)
-                    image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                    image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                    image_layer.mouse_drag_callbacks.append(
+                        self._segmentationEvents
+                    )
+                    image_layer.mouse_double_click_callbacks.append(
+                        self._doubeClickEvents
+                    )
 
                     self.segLayer.data = appended_mask_stack
                     self.nucLayer.data = appended_nmask_stack
                     self.classLayer.data = appended_class_stack
                     self.segLayer.metadata = appended_metadata
 
             else:
-                setattr(self, layer_name, self.viewer.add_image(new_image_stack, name=layer_name, colormap=colormap, gamma=0.8, metadata=new_metadata, ), )
+                setattr(
+                    self,
+                    layer_name,
+                    self.viewer.add_image(
+                        new_image_stack,
+                        name=layer_name,
+                        colormap=colormap,
+                        gamma=0.8,
+                        metadata=new_metadata,
+                    ),
+                )
 
                 image_layer = getattr(self, layer_name)
-                image_layer.mouse_drag_callbacks.append(self._segmentationEvents)
-                image_layer.mouse_double_click_callbacks.append(self._doubeClickEvents)
+                image_layer.mouse_drag_callbacks.append(
+                    self._segmentationEvents
+                )
+                image_layer.mouse_double_click_callbacks.append(
+                    self._doubeClickEvents
+                )
 
                 self.segLayer.data = new_mask_stack
                 self.nucLayer.data = new_nmask_stack
                 self.classLayer.data = new_class_stack
                 self.segLayer.metadata = new_metadata
 
         # sets labels such that only label contours are shown
@@ -1591,17 +2488,27 @@
         self._autoClassify()
         align_image_channels(self)
         self._autoContrast()
         self._updateScaleBar()
 
     def _reorderLayers(self):
         try:
-            layer_names = [layer.name for layer in self.viewer.layers if layer.name in ["Segmentations", "Nucleoid", "Classes", "center_lines"]]
-
-            for layer in ["center_lines", "Classes", "Nucleoid", "Segmentations", ]:
+            layer_names = [
+                layer.name
+                for layer in self.viewer.layers
+                if layer.name
+                in ["Segmentations", "Nucleoid", "Classes", "center_lines"]
+            ]
+
+            for layer in [
+                "center_lines",
+                "Classes",
+                "Nucleoid",
+                "Segmentations",
+            ]:
                 if layer in layer_names:
                     layer_index = self.viewer.layers.index(layer)
                     self.viewer.layers.move(layer_index, -1)
 
         except:
             pass
 
@@ -1620,21 +2527,30 @@
                 label = np.zeros(label.shape, dtype=np.uint16)
 
                 for mask_id in mask_ids:
                     if mask_id != 0:
                         cnt_mask = np.zeros(label.shape, dtype=np.uint8)
                         cnt_mask[mask == mask_id] = 255
 
-                        cnt, _ = cv2.findContours(cnt_mask.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE, )
+                        cnt, _ = cv2.findContours(
+                            cnt_mask.astype(np.uint8),
+                            cv2.RETR_EXTERNAL,
+                            cv2.CHAIN_APPROX_NONE,
+                        )
 
                         x, y, w, h = cv2.boundingRect(cnt[0])
                         y1, y2, x1, x2 = y, (y + h), x, (x + w)
 
                         # appends contour to list if the bounding coordinates are along the edge of the image
-                        if (y1 > 0 and y2 < cnt_mask.shape[0] and x1 > 0 and x2 < cnt_mask.shape[1]):
+                        if (
+                            y1 > 0
+                            and y2 < cnt_mask.shape[0]
+                            and x1 > 0
+                            and x2 < cnt_mask.shape[1]
+                        ):
                             label[mask == mask_id] = 1
 
                         else:
                             label[mask == mask_id] = 6
 
             label_stack[i, :, :] = label
```

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.py` & `napari-bacseg-1.0.7.1/src/napari_bacseg/bacseg_ui.py`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg/bacseg_ui.ui` & `napari-bacseg-1.0.7.1/src/napari_bacseg/bacseg_ui.ui`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg.egg-info/PKG-INFO` & `napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bacseg
-Version: 1.0.7
+Version: 1.0.7.1
 Summary: Bacterial segmentation and analysis platform than can inport/export files in multiple formats. Integrating many tools such as Cellpose, ColiCoords, Oufti/MicrobeTracker.
 Home-page: https://github.com/piedrro/napari-bacseg
 Author: Piers Turner
 Author-email: Piers Turner <piers.turner@physics.ox.ac.uk>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/piedrro/napari-bacseg
 Project-URL: Bug Tracker, https://github.com/piedrro/napari-bacseg/issues
```

### Comparing `napari-bacseg-1.0.7/src/napari_bacseg.egg-info/SOURCES.txt` & `napari-bacseg-1.0.7.1/src/napari_bacseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-bacseg-1.0.7/tox.ini` & `napari-bacseg-1.0.7.1/tox.ini`

 * *Files identical despite different names*

