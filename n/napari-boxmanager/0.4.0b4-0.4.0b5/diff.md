# Comparing `tmp/napari_boxmanager-0.4.0b4.tar.gz` & `tmp/napari_boxmanager-0.4.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_boxmanager-0.4.0b4.tar", last modified: Fri Jun  9 09:20:13 2023, max compression
+gzip compressed data, was "napari_boxmanager-0.4.0b5.tar", last modified: Wed Jun 14 09:44:01 2023, max compression
```

## Comparing `napari_boxmanager-0.4.0b4.tar` & `napari_boxmanager-0.4.0b5.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.852164 napari_boxmanager-0.4.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.816164 napari_boxmanager-0.4.0b4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.820164 napari_boxmanager-0.4.0b4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.820164 napari_boxmanager-0.4.0b4/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-09 09:20:13.852164 napari_boxmanager-0.4.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.820164 napari_boxmanager-0.4.0b4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/bin/napari_boxmanager
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.824164 napari_boxmanager-0.4.0b4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.824164 napari_boxmanager-0.4.0b4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/_static/version-alert.js
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.824164 napari_boxmanager-0.4.0b4/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/manual/general.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/manual/manual.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/manual/read.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/manual/write.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.824164 napari_boxmanager-0.4.0b4/reader_backup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.828164 napari_boxmanager-0.4.0b4/reader_backup/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/_tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/_tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/_tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/_tests/test_tlpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/tepkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/tlpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/tmpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/reader_backup/to_napari_backup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-09 09:20:13.852164 napari_boxmanager-0.4.0b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.816164 napari_boxmanager-0.4.0b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.828164 napari_boxmanager-0.4.0b4/src/box_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.828164 napari_boxmanager-0.4.0b4/src/box_manager/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_qt/FilterImage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_qt/OrganizeBox.py
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_qt/OrganizeLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    84364 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_qt/SelectMetric.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.832164 napari_boxmanager-0.4.0b4/src/box_manager/_qt/_icons/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_qt/_icons/checkmark_black.png
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_qt/_icons/checkmark_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.832164 napari_boxmanager-0.4.0b4/src/box_manager/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_tests/_dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.832164 napari_boxmanager-0.4.0b4/src/box_manager/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_utils/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 09:20:13.000000 napari_boxmanager-0.4.0b4/src/box_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.836164 napari_boxmanager-0.4.0b4/src/box_manager/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/star.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/tif.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/io/tloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/src/box_manager/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.836164 napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-09 09:20:13.000000 napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-09 09:20:13.000000 napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:20:13.000000 napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 09:20:13.000000 napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-09 09:20:13.000000 napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 09:20:13.000000 napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.848164 napari_boxmanager-0.4.0b4/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_0_center.box
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_center.box
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_center_float.box
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_corrupt_has_string.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_corrupt_unqual_columns.box
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_empty.box
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_left.box
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/2d_particles.cbox
--rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/3d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/3d.mrci
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/3d_particle.cbox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.852164 napari_boxmanager-0.4.0b4/test_data/box_data/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/create_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_0.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_0_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_1.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_1.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_1_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_1_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_2.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_2.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_2_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_2_new.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_3.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_4.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_4.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_4_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_5.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_5.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_6.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_6.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_6_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_7.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_7_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_7_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_8.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_8.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_8_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_9.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_9.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/box_data/test_9_new.box
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.852164 napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_02885.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_03047.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_03070.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_03211.cbox
--rw-r--r--   0 runner    (1001) docker     (123)    63796 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_04203.cbox
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/empty.cbox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.852164 napari_boxmanager-0.4.0b4/test_data/particle_cbox_2d/
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/valid.tloc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.852164 napari_boxmanager-0.4.0b4/test_data/valid_box/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/valid_box/2d.box
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/valid_box/2d_0.box
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/valid_missing_dim_z.tloc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:20:13.852164 napari_boxmanager-0.4.0b4/test_data/valid_mrc/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/valid_mrc/2d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/test_data/valid_mrc/2d_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-09 09:19:53.000000 napari_boxmanager-0.4.0b4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.100513 napari_boxmanager-0.4.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.068512 napari_boxmanager-0.4.0b5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.072512 napari_boxmanager-0.4.0b5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.072512 napari_boxmanager-0.4.0b5/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-14 09:44:01.100513 napari_boxmanager-0.4.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.072512 napari_boxmanager-0.4.0b5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/bin/napari_boxmanager
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.072512 napari_boxmanager-0.4.0b5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.072512 napari_boxmanager-0.4.0b5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/_static/version-alert.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.076512 napari_boxmanager-0.4.0b5/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/manual/general.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/manual/manual.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/manual/read.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/manual/write.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.076512 napari_boxmanager-0.4.0b5/reader_backup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.076512 napari_boxmanager-0.4.0b5/reader_backup/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/_tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/_tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/_tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/_tests/test_tlpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/tepkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/tlpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/tmpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/reader_backup/to_napari_backup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-14 09:44:01.100513 napari_boxmanager-0.4.0b5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.072512 napari_boxmanager-0.4.0b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.076512 napari_boxmanager-0.4.0b5/src/box_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.076512 napari_boxmanager-0.4.0b5/src/box_manager/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_qt/FilterImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_qt/OrganizeBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_qt/OrganizeLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84364 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_qt/SelectMetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.076512 napari_boxmanager-0.4.0b5/src/box_manager/_qt/_icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_qt/_icons/checkmark_black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_qt/_icons/checkmark_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.080512 napari_boxmanager-0.4.0b5/src/box_manager/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_tests/_dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.080512 napari_boxmanager-0.4.0b5/src/box_manager/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_utils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 09:44:00.000000 napari_boxmanager-0.4.0b5/src/box_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.080512 napari_boxmanager-0.4.0b5/src/box_manager/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20453 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/io/tloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/src/box_manager/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.080512 napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-14 09:44:00.000000 napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-14 09:44:01.000000 napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:44:00.000000 napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 09:44:00.000000 napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 09:44:00.000000 napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 09:44:00.000000 napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.092513 napari_boxmanager-0.4.0b5/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_0_center.box
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_center.box
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_center_float.box
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_corrupt_has_string.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_corrupt_unqual_columns.box
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_empty.box
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_left.box
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/2d_particles.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/3d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/3d.mrci
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/3d_particle.cbox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.100513 napari_boxmanager-0.4.0b5/test_data/box_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/create_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_0.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_0_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_1.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_1.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_1_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_1_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_2.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_2.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_2_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_2_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_3.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_4.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_4.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_4_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_5.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_5.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_6.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_6.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_6_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_7.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_7_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_7_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_8.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_8.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_8_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_9.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_9.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/box_data/test_9_new.box
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.100513 napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_02885.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_03047.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_03070.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_03211.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)    63796 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_04203.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/empty.cbox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.100513 napari_boxmanager-0.4.0b5/test_data/particle_cbox_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/valid.tloc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.100513 napari_boxmanager-0.4.0b5/test_data/valid_box/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/valid_box/2d.box
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/valid_box/2d_0.box
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/valid_missing_dim_z.tloc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:44:01.100513 napari_boxmanager-0.4.0b5/test_data/valid_mrc/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/valid_mrc/2d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/test_data/valid_mrc/2d_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-14 09:43:36.000000 napari_boxmanager-0.4.0b5/tox.ini
```

### Comparing `napari_boxmanager-0.4.0b4/.github/workflows/test_and_deploy.yml` & `napari_boxmanager-0.4.0b5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/.gitignore` & `napari_boxmanager-0.4.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/.napari/DESCRIPTION.md` & `napari_boxmanager-0.4.0b5/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/.pre-commit-config.yaml` & `napari_boxmanager-0.4.0b5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/LICENSE` & `napari_boxmanager-0.4.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/PKG-INFO` & `napari_boxmanager-0.4.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_boxmanager
-Version: 0.4.0b4
+Version: 0.4.0b5
 Summary: Particle selection tool for cryo-em
 Home-page: https://github.com/MPI-Dortmund/napari-boxmanager
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari_boxmanager-0.4.0b4/README.md` & `napari_boxmanager-0.4.0b5/README.md`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/docs/_static/version-alert.js` & `napari_boxmanager-0.4.0b5/docs/_static/version-alert.js`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/docs/changes.rst` & `napari_boxmanager-0.4.0b5/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/docs/conf.py` & `napari_boxmanager-0.4.0b5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/docs/manual/general.rst` & `napari_boxmanager-0.4.0b5/docs/manual/general.rst`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/reader_backup/_tests/test_box.py` & `napari_boxmanager-0.4.0b5/reader_backup/_tests/test_box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/reader_backup/_tests/test_interface.py` & `napari_boxmanager-0.4.0b5/reader_backup/_tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/reader_backup/_tests/test_tlpkl.py` & `napari_boxmanager-0.4.0b5/reader_backup/_tests/test_tlpkl.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/reader_backup/tlpkl.py` & `napari_boxmanager-0.4.0b5/reader_backup/tlpkl.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/reader_backup/to_napari_backup.txt` & `napari_boxmanager-0.4.0b5/reader_backup/to_napari_backup.txt`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/setup.cfg` & `napari_boxmanager-0.4.0b5/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_qt/FilterImage.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_qt/FilterImage.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_qt/OrganizeBox.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_qt/OrganizeBox.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_qt/OrganizeLayer.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_qt/OrganizeLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,30 @@
 
         b1 = QPushButton("Accept", self)
         b1.clicked.connect(self.accept)
         b2 = QPushButton("Reject", self)
         b2.clicked.connect(self.reject)
 
         tmp_layout = QHBoxLayout()
+        tmp_layout.setContentsMargins(0, 0, 0, 0)
         tmp_layout.addWidget(b1)
         tmp_layout.addWidget(b2)
         self.layout().addLayout(tmp_layout)
 
         area = QScrollArea(self)
 
         for l1, l2 in entries:
             tmp_layout = QHBoxLayout()
+            tmp_layout.setContentsMargins(0, 0, 0, 0)
             tmp_layout.addWidget(QLabel(l1, self))
             tmp_layout.addWidget(QLabel(l2, self))
             widget.layout().addLayout(tmp_layout)
 
+        widget.layout().addStretch(1)
+
         area.setWidget(widget)
         self.layout().addWidget(area)
 
 
 class OrganizeLayerWidget(QWidget):
     def __init__(self, napari_viewer: "napari.Viewer"):
         super().__init__()
@@ -88,16 +92,18 @@
         self.saved_dir_path = os.getcwd()
 
     def _link_auto_ui(self):
         inner_layout = QVBoxLayout()
         inner_layout.setContentsMargins(0, 0, 0, 0)
 
         self.link_auto_layers = {
-            "prefix": QLineEdit(self),
-            "suffix": QLineEdit(self),
+            "prefix image": QLineEdit(self),
+            "suffix image": QLineEdit(self),
+            "prefix layer": QLineEdit(self),
+            "suffix layer": QLineEdit(self),
         }
         self.link_run_auto_btn = QPushButton("Link", self)
         layout = QFormLayout()
         for name, widget in self.link_auto_layers.items():
             layout.addRow(name + "(optional)", widget)
 
         self.link_run_auto_btn.clicked.connect(self._link_auto_layers)
@@ -105,31 +111,35 @@
         inner_layout.addWidget(QLabel("Automatic layer linking", self))
         inner_layout.addLayout(layout)
         inner_layout.addWidget(self.link_run_auto_btn)
         self.layout().addLayout(inner_layout)
 
     @Slot()
     def _link_auto_layers(self):
-        prefix = self.link_auto_layers["prefix"].text()
-        suffix = self.link_auto_layers["suffix"].text()
+        prefix_image = self.link_auto_layers["prefix image"].text()
+        suffix_image = self.link_auto_layers["suffix image"].text()
+        prefix_layer = self.link_auto_layers["prefix layer"].text()
+        suffix_layer = self.link_auto_layers["suffix layer"].text()
 
-        def get_unique(path: str):
+        def get_unique(layer: napari.layers.Layer, prefix: str, suffix: str):
             return (
-                os.path.splitext(os.path.basename(path))[0]
+                os.path.splitext(
+                    os.path.basename(layer.metadata["original_path"])
+                )[0]
                 .removeprefix(prefix)
                 .removesuffix(suffix)
             )
 
         image_layers = {
-            get_unique(_.name): _.name
+            get_unique(_, prefix_image, suffix_image): _.name
             for _ in self.napari_viewer.layers
             if isinstance(_, napari.layers.Image)
         }
         layer_layers = {
-            get_unique(_.name): _.name
+            get_unique(_, prefix_layer, suffix_layer): _.name
             for _ in self.napari_viewer.layers
             if not isinstance(_, napari.layers.Image)
         }
 
         data = []
         for abbreviation, name in image_layers.items():
             try:
```

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_qt/SelectMetric.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_qt/SelectMetric.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_qt/_icons/checkmark_black.png` & `napari_boxmanager-0.4.0b5/src/box_manager/_qt/_icons/checkmark_black.png`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_qt/_icons/checkmark_white.png` & `napari_boxmanager-0.4.0b5/src/box_manager/_qt/_icons/checkmark_white.png`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_reader.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_reader.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_box.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_cbox.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_cbox.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_reader.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_tests/test_widget.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_utils/filters.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_utils/general.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_utils/general.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_widget.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/_writer.py` & `napari_boxmanager-0.4.0b5/src/box_manager/_writer.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/__init__.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/box.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/cbox.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/cbox.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/coords.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/coords.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/interface.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/interface.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/io_utils.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/io_utils.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/mrc.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/mrc.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/star.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/star.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/tif.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/tif.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/io/tloc.py` & `napari_boxmanager-0.4.0b5/src/box_manager/io/tloc.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/box_manager/napari.yaml` & `napari_boxmanager-0.4.0b5/src/box_manager/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/PKG-INFO` & `napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-boxmanager
-Version: 0.4.0b4
+Version: 0.4.0b5
 Summary: Particle selection tool for cryo-em
 Home-page: https://github.com/MPI-Dortmund/napari-boxmanager
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari_boxmanager-0.4.0b4/src/napari_boxmanager.egg-info/SOURCES.txt` & `napari_boxmanager-0.4.0b5/src/napari_boxmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/2d.mrc` & `napari_boxmanager-0.4.0b5/test_data/2d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/2d_0.mrc` & `napari_boxmanager-0.4.0b5/test_data/2d_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/2d_particles.cbox` & `napari_boxmanager-0.4.0b5/test_data/2d_particles.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/3d.mrc` & `napari_boxmanager-0.4.0b5/test_data/3d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/3d.mrci` & `napari_boxmanager-0.4.0b5/test_data/3d.mrci`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/3d_particle.cbox` & `napari_boxmanager-0.4.0b5/test_data/3d_particle.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/create_data.py` & `napari_boxmanager-0.4.0b5/test_data/box_data/create_data.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_0.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_1.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_1.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_2.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_2.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_3.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_3.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_4.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_4.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_5.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_5.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_6.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_6.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_7.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_7.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_8.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_8.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/box_data/test_9.mrc` & `napari_boxmanager-0.4.0b5/test_data/box_data/test_9.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_02885.cbox` & `napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_02885.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_03047.cbox` & `napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_03047.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_03070.cbox` & `napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_03070.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_03211.cbox` & `napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_03211.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/filament_cbox_2d/ActLifeact_04203.cbox` & `napari_boxmanager-0.4.0b5/test_data/filament_cbox_2d/ActLifeact_04203.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox` & `napari_boxmanager-0.4.0b5/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox` & `napari_boxmanager-0.4.0b5/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/valid.tloc` & `napari_boxmanager-0.4.0b5/test_data/valid.tloc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/valid_missing_dim_z.tloc` & `napari_boxmanager-0.4.0b5/test_data/valid_missing_dim_z.tloc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/valid_mrc/2d.mrc` & `napari_boxmanager-0.4.0b5/test_data/valid_mrc/2d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/test_data/valid_mrc/2d_0.mrc` & `napari_boxmanager-0.4.0b5/test_data/valid_mrc/2d_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.4.0b4/tox.ini` & `napari_boxmanager-0.4.0b5/tox.ini`

 * *Files identical despite different names*

