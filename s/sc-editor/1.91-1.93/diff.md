# Comparing `tmp/sc-editor-1.91.tar.gz` & `tmp/sc-editor-1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-editor-1.91.tar", last modified: Tue Jun 13 01:09:55 2023, max compression
+gzip compressed data, was "sc-editor-1.93.tar", last modified: Wed Jun 14 00:20:46 2023, max compression
```

## Comparing `sc-editor-1.91.tar` & `sc-editor-1.93.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.384950 sc-editor-1.91/
--rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-06-08 17:53:44.000000 sc-editor-1.91/LICENSE
--rw-r--r--   0 hayun      (502) staff       (20)      120 2023-06-12 05:42:31.000000 sc-editor-1.91/MANIFEST.in
--rw-r--r--   0 hayun      (502) staff       (20)    10977 2023-06-13 01:09:55.384426 sc-editor-1.91/PKG-INFO
--rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-06-08 17:53:44.000000 sc-editor-1.91/README.md
--rw-rw-r--   0 hayun      (502) staff       (20)        0 2023-06-12 03:06:57.000000 sc-editor-1.91/pyproject.toml
--rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-13 01:09:55.385093 sc-editor-1.91/setup.cfg
--rw-rw-r--   0 hayun      (502) staff       (20)     1085 2023-06-13 01:09:46.000000 sc-editor-1.91/setup.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:54.937079 sc-editor-1.91/src/
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.168105 sc-editor-1.91/src/SC_Editor/
--rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    15733 2023-06-13 01:01:02.000000 sc-editor-1.91/src/SC_Editor/__main__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/adb_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    13743 2023-06-12 02:58:41.000000 sc-editor-1.91/src/SC_Editor/config_manager.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/csv_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.173633 sc-editor-1.91/src/SC_Editor/edits/
--rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/__init__.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.218573 sc-editor-1.91/src/SC_Editor/edits/basic/
--rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8987 2023-06-13 01:09:41.000000 sc-editor-1.91/src/SC_Editor/edits/basic/basic_items.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/catfruit.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/catseyes.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/ototo_base_mats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/talent_orbs.py
--rw-rw-r--   0 hayun      (502) staff       (20)    16530 2023-06-12 02:58:44.000000 sc-editor-1.91/src/SC_Editor/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.283862 sc-editor-1.91/src/SC_Editor/edits/cats/
--rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/cat_helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/cat_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/chara_drop.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/clear_cat_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/evolve_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/get_remove_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/talents.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/upgrade_blue.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.288700 sc-editor-1.91/src/SC_Editor/edits/gamototo/
--rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/fix_gamatoto.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/gamatoto_xp.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/helpers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.321785 sc-editor-1.91/src/SC_Editor/edits/levels/
--rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/aku.py
--rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/allow_filibuster_clearing.py
--rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/behemoth_culling.py
--rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/clear_tutorial.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/enigma_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/event_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/gauntlet.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/itf_timed_scores.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/legend_quest.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/main_story.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/outbreaks.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/story_level_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/towers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/treasures.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/uncanny.py
--rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.366259 sc-editor-1.91/src/SC_Editor/edits/other/
--rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/cat_shrine.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/claim_user_rank_rewards.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/create_new_account.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/fix_elsewhere.py
--rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/fix_time_issues.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/get_gold_pass.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7138 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/meow_medals.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/missions.py
--rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/play_time.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/scheme_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/trade_progress.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/unlock_enemy_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.378980 sc-editor-1.91/src/SC_Editor/edits/save_management/
--rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/convert.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/load.py
--rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/other.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/edits/save_management/server_upload.py
--rw-rw-r--   0 hayun      (502) staff       (20)    12771 2023-06-13 01:06:35.000000 sc-editor-1.91/src/SC_Editor/feature_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4822 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/game_data_getter.py
--rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/locale_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/managed_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/parse_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/patcher.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/root_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/serialise_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/server_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3494 2023-06-13 00:01:03.000000 sc-editor-1.91/src/SC_Editor/updater.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/user_info.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-06-08 17:53:44.000000 sc-editor-1.91/src/SC_Editor/user_input_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-13 01:09:55.383093 sc-editor-1.91/src/sc_editor.egg-info/
--rw-r--r--   0 hayun      (502) staff       (20)    10977 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)     3354 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/SOURCES.txt
--rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/dependency_links.txt
--rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/requires.txt
--rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-13 01:09:54.000000 sc-editor-1.91/src/sc_editor.egg-info/top_level.txt
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.611367 sc-editor-1.93/
+-rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-06-08 17:53:44.000000 sc-editor-1.93/LICENSE
+-rw-r--r--   0 hayun      (502) staff       (20)      120 2023-06-12 05:42:31.000000 sc-editor-1.93/MANIFEST.in
+-rw-r--r--   0 hayun      (502) staff       (20)    10977 2023-06-14 00:20:46.609662 sc-editor-1.93/PKG-INFO
+-rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-06-08 17:53:44.000000 sc-editor-1.93/README.md
+-rw-rw-r--   0 hayun      (502) staff       (20)        0 2023-06-12 03:06:57.000000 sc-editor-1.93/pyproject.toml
+-rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-14 00:20:46.611545 sc-editor-1.93/setup.cfg
+-rw-rw-r--   0 hayun      (502) staff       (20)     1085 2023-06-14 00:20:01.000000 sc-editor-1.93/setup.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.186047 sc-editor-1.93/src/
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.248994 sc-editor-1.93/src/SC_Editor/
+-rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    15733 2023-06-13 01:01:02.000000 sc-editor-1.93/src/SC_Editor/__main__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/adb_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    13743 2023-06-12 02:58:41.000000 sc-editor-1.93/src/SC_Editor/config_manager.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/csv_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.249499 sc-editor-1.93/src/SC_Editor/edits/
+-rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/__init__.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.265284 sc-editor-1.93/src/SC_Editor/edits/basic/
+-rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/basic/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8867 2023-06-14 00:19:57.000000 sc-editor-1.93/src/SC_Editor/edits/basic/basic_items.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/basic/catfruit.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/basic/catseyes.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/basic/ototo_base_mats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/basic/talent_orbs.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    16530 2023-06-12 02:58:44.000000 sc-editor-1.93/src/SC_Editor/edits/basic/talent_orbs_new.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.435037 sc-editor-1.93/src/SC_Editor/edits/cats/
+-rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/cat_helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/cat_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/chara_drop.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/clear_cat_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/evolve_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/get_remove_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/talents.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/upgrade_blue.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.445214 sc-editor-1.93/src/SC_Editor/edits/gamototo/
+-rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/gamototo/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/gamototo/fix_gamatoto.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/gamototo/gamatoto_xp.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/gamototo/helpers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.495094 sc-editor-1.93/src/SC_Editor/edits/levels/
+-rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/aku.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/allow_filibuster_clearing.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/behemoth_culling.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/clear_tutorial.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/enigma_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/event_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/gauntlet.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/itf_timed_scores.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/legend_quest.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/main_story.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/outbreaks.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/story_level_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/towers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/treasures.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/uncanny.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.584176 sc-editor-1.93/src/SC_Editor/edits/other/
+-rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/cat_shrine.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/claim_user_rank_rewards.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/create_new_account.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/fix_elsewhere.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/fix_time_issues.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/get_gold_pass.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7138 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/meow_medals.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/missions.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/play_time.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/scheme_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/trade_progress.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/unlock_enemy_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.590541 sc-editor-1.93/src/SC_Editor/edits/save_management/
+-rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/save_management/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/save_management/convert.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/save_management/load.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/save_management/other.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/save_management/save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/edits/save_management/server_upload.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    12538 2023-06-14 00:18:46.000000 sc-editor-1.93/src/SC_Editor/feature_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4822 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/game_data_getter.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/locale_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/managed_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/parse_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/patcher.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/root_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/serialise_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/server_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3494 2023-06-13 00:01:03.000000 sc-editor-1.93/src/SC_Editor/updater.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/user_info.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-06-08 17:53:44.000000 sc-editor-1.93/src/SC_Editor/user_input_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-14 00:20:46.604204 sc-editor-1.93/src/sc_editor.egg-info/
+-rw-r--r--   0 hayun      (502) staff       (20)    10977 2023-06-14 00:20:46.000000 sc-editor-1.93/src/sc_editor.egg-info/PKG-INFO
+-rw-r--r--   0 hayun      (502) staff       (20)     3354 2023-06-14 00:20:46.000000 sc-editor-1.93/src/sc_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-14 00:20:46.000000 sc-editor-1.93/src/sc_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-14 00:20:46.000000 sc-editor-1.93/src/sc_editor.egg-info/requires.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-14 00:20:46.000000 sc-editor-1.93/src/sc_editor.egg-info/top_level.txt
```

### Comparing `sc-editor-1.91/LICENSE` & `sc-editor-1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/PKG-INFO` & `sc-editor-1.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-editor
-Version: 1.91
+Version: 1.93
 Summary: A battle cats save file editor korean version
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: cintagramabp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sc-editor-1.91/README.md` & `sc-editor-1.93/README.md`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/setup.py` & `sc-editor-1.93/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
 setuptools.setup(
     name="sc-editor",
-    version="1.91",
+    version="1.93",
     author="cintagramabp",
     description="A battle cats save file editor korean version",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fieryhenry/BCSFE-Python",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `sc-editor-1.91/src/SC_Editor/__main__.py` & `sc-editor-1.93/src/SC_Editor/__main__.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/adb_handler.py` & `sc-editor-1.93/src/SC_Editor/adb_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/config_manager.py` & `sc-editor-1.93/src/SC_Editor/config_manager.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/csv_handler.py` & `sc-editor-1.93/src/SC_Editor/csv_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/basic/basic_items.py` & `sc-editor-1.93/src/SC_Editor/edits/basic/basic_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     rare_tickets = item.IntItem(
         name="레어 티켓",
         value=item.Int(save_stats["rare_tickets"]["Value"]),
         max_value=299,
         bannable=item.Bannable(
             inquiry_code=save_stats["inquiry_code"],
-            work_around='&Instead of editing rare tickets directly, use the "Normal Ticket Max Trade Progress" conversion feature instead! It is much more safe.',
+            work_around='밴 위험이 높으니 신중히 사용하세요.',
             type=managed_item.ManagedItemType.RARE_TICKET,
         ),
     )
     rare_tickets.edit()
     save_stats["rare_tickets"]["Value"] = rare_tickets.get_value()
     return save_stats
 
@@ -68,15 +68,15 @@
 
     platinum_tickets = item.IntItem(
         name="플래티넘 티켓",
         value=item.Int(save_stats["platinum_tickets"]["Value"]),
         max_value=9,
         bannable=item.Bannable(
             inquiry_code=save_stats["inquiry_code"],
-            work_around="&Instead of editing platinum tickets, edit platinum shards instead! They are much more safe. 10 platinum shards = 1 platinum ticket",
+            work_around="밴 위험이 높으니 신중히 사용하세요.",
             type=managed_item.ManagedItemType.PLATINUM_TICKET,
         ),
     )
     platinum_tickets.edit()
     save_stats["platinum_tickets"]["Value"] = platinum_tickets.get_value()
     return save_stats
 
@@ -190,44 +190,44 @@
     return save_stats
 
 
 def edit_rare_gacha_seed(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the rare gacha seed"""
 
     rare_gacha_seed = item.IntItem(
-        name="Rare Gacha Seed",
+        name="레어 뽑기 시드",
         value=item.Int(save_stats["rare_gacha_seed"]["Value"], signed=False),
         max_value=None,
     )
     rare_gacha_seed.edit()
     save_stats["rare_gacha_seed"]["Value"] = rare_gacha_seed.get_value()
     return save_stats
 
 
 def edit_unlocked_slots(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the amount of unlocked slots"""
 
     unlocked_slots = item.IntItem(
-        name="Unlocked Slots",
+        name="캐릭터 편성",
         value=item.Int(save_stats["unlocked_slots"]["Value"]),
         max_value=len(save_stats["slots"]),
     )
     unlocked_slots.edit()
     save_stats["unlocked_slots"]["Value"] = unlocked_slots.get_value()
     return save_stats
 
 
 def edit_token(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the password-refresh-token"""
 
     print(
-        "WARNING: Editing your token should only be done if you know what you are doing! Because it will lead to an elsewhere error in-game if not done correctly!"
+        "경고: 토큰 편집은 수행 중인 작업을 알고 있는 경우에만 수행해야 합니다! 올바르게 수행하지 않으면 게임 내에서 다른 오류가 발생합니다!"
     )
     token = item.StrItem(
-        name="Token",
+        name="토큰",
         value=save_stats["token"],
     )
     token.edit()
     save_stats["token"] = token.get_value()
     return save_stats
 
 
@@ -239,29 +239,29 @@
     return save_stats
 
 
 def edit_challenge_battle(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the score of the challenge battle"""
 
     challenge_battle = item.IntItem(
-        name="Challenge Battle",
+        name="챌린지 배틀",
         value=item.Int(save_stats["challenge"]["Score"]["Value"]),
         max_value=None,
     )
     challenge_battle.edit()
     save_stats["challenge"]["Score"]["Value"] = challenge_battle.get_value()
     save_stats["challenge"]["Cleared"]["Value"] = 1
     return save_stats
 
 
 def edit_legend_tickets(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing legend tickets"""
 
     legend_tickets = item.IntItem(
-        name="Legend Tickets",
+        name="레전드 티켓",
         value=item.Int(save_stats["legend_tickets"]["Value"]),
         max_value=4,
         bannable=item.Bannable(
             inquiry_code=save_stats["inquiry_code"],
             type=managed_item.ManagedItemType.LEGEND_TICKET,
         ),
     )
@@ -273,14 +273,14 @@
 def edit_dojo_score(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editing the dojo score"""
 
     if not save_stats["dojo_data"]:
         save_stats["dojo_data"] = {0: {0: 0}}
 
     dojo_score = item.IntItem(
-        name="Dojo Score",
+        name="도장 점수",
         value=item.Int(save_stats["dojo_data"][0][0]),
         max_value=None,
     )
     dojo_score.edit()
     save_stats["dojo_data"][0][0] = dojo_score.get_value()
     return save_stats
```

### Comparing `sc-editor-1.91/src/SC_Editor/edits/basic/catfruit.py` & `sc-editor-1.93/src/SC_Editor/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/basic/catseyes.py` & `sc-editor-1.93/src/SC_Editor/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/basic/ototo_base_mats.py` & `sc-editor-1.93/src/SC_Editor/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/basic/talent_orbs.py` & `sc-editor-1.93/src/SC_Editor/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/basic/talent_orbs_new.py` & `sc-editor-1.93/src/SC_Editor/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/cat_helper.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/cat_id_selector.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/chara_drop.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/clear_cat_guide.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/evolve_cats.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/get_remove_cats.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/talents.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/upgrade_blue.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/cats/upgrade_cats.py` & `sc-editor-1.93/src/SC_Editor/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/gamototo/gamatoto_xp.py` & `sc-editor-1.93/src/SC_Editor/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/gamototo/helpers.py` & `sc-editor-1.93/src/SC_Editor/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py` & `sc-editor-1.93/src/SC_Editor/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/aku.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/behemoth_culling.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/clear_tutorial.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/enigma_stages.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/event_stages.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/gauntlet.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/itf_timed_scores.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/legend_quest.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/main_story.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/outbreaks.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/story_level_id_selector.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/towers.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/treasures.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/uncanny.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/levels/unlock_aku_realm.py` & `sc-editor-1.93/src/SC_Editor/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/cat_shrine.py` & `sc-editor-1.93/src/SC_Editor/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/claim_user_rank_rewards.py` & `sc-editor-1.93/src/SC_Editor/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/create_new_account.py` & `sc-editor-1.93/src/SC_Editor/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/fix_elsewhere.py` & `sc-editor-1.93/src/SC_Editor/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/fix_time_issues.py` & `sc-editor-1.93/src/SC_Editor/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/get_gold_pass.py` & `sc-editor-1.93/src/SC_Editor/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/meow_medals.py` & `sc-editor-1.93/src/SC_Editor/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/missions.py` & `sc-editor-1.93/src/SC_Editor/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/play_time.py` & `sc-editor-1.93/src/SC_Editor/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/scheme_item.py` & `sc-editor-1.93/src/SC_Editor/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/trade_progress.py` & `sc-editor-1.93/src/SC_Editor/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/other/unlock_enemy_guide.py` & `sc-editor-1.93/src/SC_Editor/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/save_management/convert.py` & `sc-editor-1.93/src/SC_Editor/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/save_management/load.py` & `sc-editor-1.93/src/SC_Editor/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/save_management/other.py` & `sc-editor-1.93/src/SC_Editor/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/save_management/save.py` & `sc-editor-1.93/src/SC_Editor/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/edits/save_management/server_upload.py` & `sc-editor-1.93/src/SC_Editor/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/feature_handler.py` & `sc-editor-1.93/src/SC_Editor/feature_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,19 +42,19 @@
 FEATURES: dict[str, Any] = {
     "세이브 관리": {
         "세이브 저장": save_management.save.save_save,
         "세이브 저장후 기종변경 코드 받기": save_management.server_upload.save_and_upload,
         "파일에 저장하기": save_management.save.save,
         "Save changes and push save data to the game with adb (don't re-open game)": save_management.save.save_and_push,
         "Save changes and push save data to the game with adb (re-open game)": save_management.save.save_and_push_rerun,
-        "Export save data as json": save_management.other.export,
+        "세이브 데이터를 JSON으로 컴파일": save_management.other.export,
         "Clear save data with adb (used to generate a new account without re-installing the game)": save_management.other.clear_data,
         "Upload tracked bannable items (This is done automatically when saving or exiting)": save_management.server_upload.upload_metadata,
-        "Load save data": save_management.load.select,
-        "Convert save data to to a different version": save_management.convert.convert_save,
+        "새로운 세이브 데이터 로딩": save_management.load.select,
+        "세이브 데이터 국가 변경": save_management.convert.convert_save,
         # "Manage Presets": preset_handler.preset_manager,
     },
     "아이템": {
         "통조림": basic.basic_items.edit_cat_food,
         "XP": basic.basic_items.edit_xp,
         "티켓": {
             "냥코 티켓": basic.basic_items.edit_normal_tickets,
@@ -92,89 +92,89 @@
             "3단 진화 제거": cats.evolve_cats.remove_evolve,
             "강제 3단 진화 (3단 진화가 없는 고양이의 경우 빈 고양이로 채워짐)": cats.evolve_cats.get_evolve_forced,
         },
         "본능": {
             "선택한 각 고양이의 본능을 개별적으로 설정": cats.talents.edit_talents_individual,
             "선택된 모든 고양이 본능 만렙 / 제거": cats.talents.max_all_talents,
         },
-        "Collect / Remove Cat Guide": {
-            "Set Cat Guide Entries (does not give cf)": cats.clear_cat_guide.collect_cat_guide,
-            "Unclaim Cat Guide Entries": cats.clear_cat_guide.remove_cat_guide,
-        },
-        'Get stage unit drops - removes the "Clear this stage to get special cat" dialog': cats.chara_drop.get_character_drops,
-        "Upgrade special skills / abilities": cats.upgrade_blue.upgrade_blue,
-    },
-    "Levels / Treasures": {
-        "Main Story Chapters Clear / Unclear": {
-            "Clear each stage in every chapter for all selected chapters": levels.main_story.clear_all,
-            "Clear each stage in every chapter for each selected chapter": levels.main_story.clear_each,
-        },
-        "Treasures": {
-            "Treasure Groups (e.g energy drink, aqua crystal, etc)": levels.treasures.treasure_groups,
-            "Specific stages and specific chapters individually": levels.treasures.specific_stages,
-            "Specific stages and chapters all at once": levels.treasures.specific_stages_all_chapters,
-        },
-        "Zombie Stages / Outbreaks": levels.outbreaks.edit_outbreaks,
-        "Event Stages": levels.event_stages.event_stages,
-        "Stories of Legend": levels.event_stages.stories_of_legend,
-        "Uncanny Legends": levels.uncanny.edit_uncanny,
-        "Aku Realm/Gates Clearing": levels.aku.edit_aku,
-        "Unlock the Aku Realm/Gates": levels.unlock_aku_realm.unlock_aku_realm,
-        "Gauntlets": levels.gauntlet.edit_gauntlet,
-        "Collab Gauntlets": levels.gauntlet.edit_collab_gauntlet,
-        "Towers": levels.towers.edit_tower,
-        "Behemoth Culling": levels.behemoth_culling.edit_behemoth_culling,
-        "Into the Future Timed Scores": levels.itf_timed_scores.timed_scores,
-        "Challenge Battle Score": basic.basic_items.edit_challenge_battle,
-        "Clear Tutorial": levels.clear_tutorial.clear_tutorial,
-        "Catclaw Dojo Score (Hall of Initiates)": basic.basic_items.edit_dojo_score,
-        "Add Enigma Stages": levels.enigma_stages.edit_enigma_stages,
-        "Allow the filibuster stage to be recleared": levels.allow_filibuster_clearing.allow_filibuster_clearing,
-        "Legend Quest": levels.legend_quest.edit_legend_quest,
-    },
-    "Inquiry Code / Token / Account": {
-        "Inquiry Code": basic.basic_items.edit_inquiry_code,
-        "Token": basic.basic_items.edit_token,
-        "Fix elsewhere error / Unban account": other.fix_elsewhere.fix_elsewhere,
-        "Old Fix elsewhere error / Unban account (needs 2 save files)": fix_elsewhere_old,
-        "Generate a new inquiry code and token": other.create_new_account.create_new_account,
-    },
-    "Other": {
-        "Rare Gacha Seed": basic.basic_items.edit_rare_gacha_seed,
-        "Unlocked Equip Slots": basic.basic_items.edit_unlocked_slots,
-        "Get Restart Pack / Returner Mode": basic.basic_items.edit_restart_pack,
-        "Meow Medals": other.meow_medals.medals,
-        "Play Time": other.play_time.edit_play_time,
-        "Unlock / Remove Enemy Guide Entries": other.unlock_enemy_guide.enemy_guide,
-        "Catnip Challenges / Missions": other.missions.edit_missions,
-        "Normal Ticket Max Trade Progress (allows for unbannable rare tickets)": other.trade_progress.set_trade_progress,
-        "Get / Remove Gold Pass": other.get_gold_pass.get_gold_pass,
-        "Claim / Remove all user rank rewards (does not give any items)": other.claim_user_rank_rewards.edit_rewards,
-        "Cat Shrine Level / XP": other.cat_shrine.edit_shrine_xp,
-    },
-    "Fixes": {
-        "Fix time errors": other.fix_time_issues.fix_time_issues,
-        "Unlock the Equip Menu": other.unlock_equip_menu.unlock_equip,
-        "Clear Tutorial": levels.clear_tutorial.clear_tutorial,
-        "Fix elsewhere error / Unban account": other.fix_elsewhere.fix_elsewhere,
-        "Old Fix elsewhere error / Unban account (needs 2 save files)": fix_elsewhere_old,
-        "Fix gamatoto from crashing the game": gamototo.fix_gamatoto.fix_gamatoto,
+        "캐릭터 도감": {
+            "캐릭터 도감 획득 (통조림 X)": cats.clear_cat_guide.collect_cat_guide,
+            "캐릭터 도감 미확인 상태": cats.clear_cat_guide.remove_cat_guide,
+        },
+        '스테이지 드롭 보상 받기 (보수 상태 획득)': cats.chara_drop.get_character_drops,
+        "특능 편집": cats.upgrade_blue.upgrade_blue,
+    },
+    "스테이지 / 보물": {
+        "스테이지 클리어 / 언클리어": {
+            "선택한 모든 챕터의 모든 챕터에서 각 스테이지 클리어": levels.main_story.clear_all,
+            "선택한 각 챕터의 모든 챕터에서 각 스테이지 클리어": levels.main_story.clear_each,
+        },
+        "보물": {
+            "보물 그룹으로 설정": levels.treasures.treasure_groups,
+            "모든 보물을 따로따로 설정": levels.treasures.specific_stages,
+            "각 장별로 한번에 설정": levels.treasures.specific_stages_all_chapters,
+        },
+        "좀비스테이지": levels.outbreaks.edit_outbreaks,
+        "이벤트 스테이지": levels.event_stages.event_stages,
+        "구레전드 스테이지": levels.event_stages.stories_of_legend,
+        "신레전드 스테이지": levels.uncanny.edit_uncanny,
+        "마계편 클리어": levels.aku.edit_aku,
+        "마계의 문 열기": levels.unlock_aku_realm.unlock_aku_realm,
+        #"Gauntlets": levels.gauntlet.edit_gauntlet,
+        #"Collab Gauntlets": levels.gauntlet.edit_collab_gauntlet,
+        "탑": levels.towers.edit_tower,
+        "초수 스테이지": levels.behemoth_culling.edit_behemoth_culling,
+        "미래편 시간 점수": levels.itf_timed_scores.timed_scores,
+        "챌린지 배틀 점수": basic.basic_items.edit_challenge_battle,
+        "튜토리얼 클리어": levels.clear_tutorial.clear_tutorial,
+        "냥코 도장 점수": basic.basic_items.edit_dojo_score,
+        "발굴 스테이지 추가": levels.enigma_stages.edit_enigma_stages,
+        "필리버스터 스테이지 언클리어": levels.allow_filibuster_clearing.allow_filibuster_clearing,
+        "레전드 퀘스트": levels.legend_quest.edit_legend_quest,
+    },
+    "문의코드 / 토큰 / 계정": {
+        "문의코드": basic.basic_items.edit_inquiry_code,
+        "토큰": basic.basic_items.edit_token,
+        "언밴 / 오류 해결": other.fix_elsewhere.fix_elsewhere,
+        #"Old Fix elsewhere error / Unban account (needs 2 save files)": fix_elsewhere_old,
+        "새 문의코드와 토큰 생성": other.create_new_account.create_new_account,
+    },
+    "기타": {
+        "레어 뽑기 시드": basic.basic_items.edit_rare_gacha_seed,
+        "캐릭터 편성": basic.basic_items.edit_unlocked_slots,
+        "리스타트팩 설정": basic.basic_items.edit_restart_pack,
+        "냥코 메달 설정": other.meow_medals.medals,
+        "플레이타임 설정": other.play_time.edit_play_time,
+        "적 도감 설정": other.unlock_enemy_guide.enemy_guide,
+        "미션 설정": other.missions.edit_missions,
+        "일반 티켓 최대 거래 진행률(금지할 수 없는 희귀 티켓 허용)": other.trade_progress.set_trade_progress,
+        "골드패스 설정": other.get_gold_pass.get_gold_pass,
+        "모든 유저 랭크 보상 제거 / 획득 (아이템을 주지 않음)": other.claim_user_rank_rewards.edit_rewards,
+        "냥코 사당 레벨 / XP": other.cat_shrine.edit_shrine_xp,
+    },
+    "오류해결": {
+        "시간 오류 해결": other.fix_time_issues.fix_time_issues,
+        "캐릭터 편성 오류 해결": other.unlock_equip_menu.unlock_equip,
+        "튜토리얼 클리어": levels.clear_tutorial.clear_tutorial,
+        "언밴 / 오류 해결": other.fix_elsewhere.fix_elsewhere,
+        #"Old Fix elsewhere error / Unban account (needs 2 save files)": fix_elsewhere_old,
+        "가마토토 / 오토토 오류 해결": gamototo.fix_gamatoto.fix_gamatoto,
     },
-    "Edit Config": {
+    "에디터 설정 (사용 X)": {
         "Edit LOCALIZATION": config_manager.edit_locale,
         "Edit DEFAULT_COUNTRY_CODE": config_manager.edit_default_gv,
         "Edit DEFAULT_SAVE_PATH": config_manager.edit_default_save_file_path,
         "Edit FIXED_SAVE_PATH": config_manager.edit_fixed_save_path,
         "Edit EDITOR settings": config_manager.edit_editor_settings,
         "Edit START_UP settings": config_manager.edit_start_up_settings,
         "Edit SAVE_CHANGES settings": config_manager.edit_save_changes_settings,
         "Edit SERVER settings": config_manager.edit_server_settings,
         "Edit config path": config_manager.edit_config_path,
     },
-    "Exit": helper.exit_check_changes,
+    "종료": helper.exit_check_changes,
 }
 
 
 def get_feature(
     selected_features: Any, search_string: str, results: dict[str, Any]
 ) -> dict[str, Any]:
     """Search for a feature if the feature name contains the search string"""
@@ -196,52 +196,52 @@
     if (
         not config_manager.get_config_value_category("EDITOR", "SHOW_CATEGORIES")
         and FEATURES == features_to_use
     ):
         user_input = ""
     else:
         prompt = (
-            "What do you want to edit (some options contain other features within them)"
+            "에딧할 것을 선택하세요."
         )
         if config_manager.get_config_value_category(
             "EDITOR", "SHOW_FEATURE_SELECT_EXPLANATION"
         ):
-            prompt += "\nYou can enter a number to run a feature or a word to search for that feature (e.g entering catfood will run the Cat Food feature, and entering tickets will show you all the features that edit tickets)\nYou can press enter to see a list of all of the features"
+            prompt += "\n원하시는 메뉴의 번호를 입력해주세요"
         user_input = user_input_handler.colored_input(f"{prompt}:\n")
     user_int = helper.check_int(user_input)
     results = []
     if user_int is None:
         results = get_feature(features_to_use, user_input, {})
     else:
         if user_int < 1 or user_int > len(features_to_use) + 1:
-            helper.colored_text("Value out of range", helper.RED)
+            helper.colored_text("번호가 메뉴에 없습니다.", helper.RED)
             return show_options(save_stats, features_to_use)
         if FEATURES != features_to_use:
             if user_int - 2 < 0:
                 return menu(save_stats)
             results = features_to_use[list(features_to_use)[user_int - 2]]
         else:
             results = features_to_use[list(features_to_use)[user_int - 1]]
     if not isinstance(results, dict):
         save_stats_return = results(save_stats)
         if save_stats_return is None:
             return save_stats
         return save_stats_return
     if len(results) == 0:
-        helper.colored_text("No feature found with that name.", helper.RED)
+        helper.colored_text("해당 메뉴가 없습니다.", helper.RED)
         return menu(save_stats)
     if len(results) == 1 and isinstance(list(results.values())[0], dict):
         results = results[list(results)[0]]
     if len(results) == 1:
         save_stats_return = results[list(results)[0]](save_stats)
         if save_stats_return is None:
             return save_stats
         return save_stats_return
 
-    helper.colored_list(["Go Back"] + list(results))
+    helper.colored_list(["뒤로가기"] + list(results))
     return show_options(save_stats, results)
 
 
 def menu(
     save_stats: dict[str, Any], path_save: Union[str, None] = None
 ) -> dict[str, Any]:
     """Show the menu and allow the user to select a feature to edit"""
```

### Comparing `sc-editor-1.91/src/SC_Editor/game_data_getter.py` & `sc-editor-1.93/src/SC_Editor/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/helper.py` & `sc-editor-1.93/src/SC_Editor/helper.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/item.py` & `sc-editor-1.93/src/SC_Editor/item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/locale_handler.py` & `sc-editor-1.93/src/SC_Editor/locale_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/managed_item.py` & `sc-editor-1.93/src/SC_Editor/managed_item.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/parse_save.py` & `sc-editor-1.93/src/SC_Editor/parse_save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/patcher.py` & `sc-editor-1.93/src/SC_Editor/patcher.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/root_handler.py` & `sc-editor-1.93/src/SC_Editor/root_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/serialise_save.py` & `sc-editor-1.93/src/SC_Editor/serialise_save.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/server_handler.py` & `sc-editor-1.93/src/SC_Editor/server_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/updater.py` & `sc-editor-1.93/src/SC_Editor/updater.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/user_info.py` & `sc-editor-1.93/src/SC_Editor/user_info.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/SC_Editor/user_input_handler.py` & `sc-editor-1.93/src/SC_Editor/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `sc-editor-1.91/src/sc_editor.egg-info/PKG-INFO` & `sc-editor-1.93/src/sc_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-editor
-Version: 1.91
+Version: 1.93
 Summary: A battle cats save file editor korean version
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: cintagramabp
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sc-editor-1.91/src/sc_editor.egg-info/SOURCES.txt` & `sc-editor-1.93/src/sc_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

