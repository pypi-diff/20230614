# Comparing `tmp/usdm-0.28.0.tar.gz` & `tmp/usdm-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.28.0.tar", last modified: Mon Jun 12 10:42:48 2023, max compression
+gzip compressed data, was "usdm-0.29.0.tar", last modified: Wed Jun 14 09:05:23 2023, max compression
```

## Comparing `usdm-0.28.0.tar` & `usdm-0.29.0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.162775 usdm-0.28.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.28.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    22277 2023-06-12 10:42:48.156309 usdm-0.28.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    21827 2023-06-12 10:01:21.000000 usdm-0.28.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.28.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2023-06-12 10:42:48.162956 usdm-0.28.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.28.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.012282 usdm-0.28.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.016347 usdm-0.28.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    22277 2023-06-12 10:42:47.000000 usdm-0.28.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     4627 2023-06-12 10:42:48.000000 usdm-0.28.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2023-06-12 10:42:47.000000 usdm-0.28.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       45 2023-06-12 10:42:47.000000 usdm-0.28.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       32 2023-06-12 10:42:47.000000 usdm-0.28.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.057627 usdm-0.28.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)     1611 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.28.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)    10753 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4667 2023-05-01 12:04:14.000000 usdm-0.28.0/src/usdm_excel/cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.28.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.28.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)     1564 2023-05-08 13:47:22.000000 usdm-0.28.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.068119 usdm-0.28.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.28.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.28.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.070098 usdm-0.28.0/src/usdm_excel/errors/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.28.0/src/usdm_excel/errors/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      933 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/errors/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      732 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/errors/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.28.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      883 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/iso_8601_duration.py
--rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.28.0/src/usdm_excel/logger.py
--rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.28.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     5641 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/nodes_and_edges.py
--rw-r--r--   0 daveih     (501) staff       (20)      824 2023-05-08 13:47:22.000000 usdm-0.28.0/src/usdm_excel/option_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.071927 usdm-0.28.0/src/usdm_excel/study_design_activity_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.28.0/src/usdm_excel/study_design_activity_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1570 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.073883 usdm-0.28.0/src/usdm_excel/study_design_arm_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.28.0/src/usdm_excel/study_design_arm_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1617 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.075313 usdm-0.28.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2003 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.076968 usdm-0.28.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2503 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.078554 usdm-0.28.0/src/usdm_excel/study_design_epoch_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.28.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1289 2023-06-09 09:44:08.000000 usdm-0.28.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.079826 usdm-0.28.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2794 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.080944 usdm-0.28.0/src/usdm_excel/study_design_ii_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_ii_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1991 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.083977 usdm-0.28.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2475 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.085282 usdm-0.28.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1778 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.086213 usdm-0.28.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1645 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.087235 usdm-0.28.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     6844 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.088829 usdm-0.28.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     3435 2023-05-17 10:35:35.000000 usdm-0.28.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.091987 usdm-0.28.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     7910 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.104242 usdm-0.28.0/src/usdm_excel/study_soa_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     3498 2023-05-09 06:07:57.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/cycle.py
--rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/cycles.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4620 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5070 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoint.py
--rw-r--r--   0 daveih     (501) staff       (20)     2550 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoint_type.py
--rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-13 04:26:45.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoints.py
--rw-r--r--   0 daveih     (501) staff       (20)     2008 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_excel/study_soa_sheet/window_type.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.104590 usdm-0.28.0/src/usdm_info/
--rw-r--r--   0 daveih     (501) staff       (20)       59 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_info/__init__.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.143778 usdm-0.28.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      586 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.28.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      383 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      243 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      151 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      661 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      240 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      195 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      251 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      238 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/investigational_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      289 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      346 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/organisation.py
--rw-r--r--   0 daveih     (501) staff       (20)      339 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      551 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      729 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      676 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      294 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      188 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     1820 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      398 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_design_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      356 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      328 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      250 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.28.0/src/usdm_model/study_protocol_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      492 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      135 2023-06-12 09:18:24.000000 usdm-0.28.0/src/usdm_model/transition_rule.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-12 10:42:48.155436 usdm-0.28.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    14241 2023-05-16 13:26:16.000000 usdm-0.28.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.28.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)     1517 2023-05-08 13:47:22.000000 usdm-0.28.0/tests/test_configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      880 2023-05-17 10:35:35.000000 usdm-0.28.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     2234 2023-05-17 10:35:35.000000 usdm-0.28.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     2466 2023-06-12 09:18:24.000000 usdm-0.28.0/tests/test_integration.py
--rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.28.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)     1763 2023-06-12 09:18:24.000000 usdm-0.28.0/tests/test_iso_8601_duration.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.28.0/tests/test_ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     1098 2023-05-08 13:47:22.000000 usdm-0.28.0/tests/test_option_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)     3199 2023-05-08 14:51:48.000000 usdm-0.28.0/tests/test_study_design_activity_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.28.0/tests/test_study_design_arm_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.28.0/tests/test_study_design_epoch_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4884 2023-05-16 13:26:16.000000 usdm-0.28.0/tests/test_study_identifiers_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4167 2023-06-12 09:18:24.000000 usdm-0.28.0/tests/test_study_soa_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.591907 usdm-0.29.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.29.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    22277 2023-06-14 09:05:23.591660 usdm-0.29.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    21827 2023-06-12 10:01:21.000000 usdm-0.29.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.29.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2023-06-14 09:05:23.591958 usdm-0.29.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.29.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.439371 usdm-0.29.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.445899 usdm-0.29.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    22277 2023-06-14 09:05:23.000000 usdm-0.29.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     4627 2023-06-14 09:05:23.000000 usdm-0.29.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2023-06-14 09:05:23.000000 usdm-0.29.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       45 2023-06-14 09:05:23.000000 usdm-0.29.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       32 2023-06-14 09:05:23.000000 usdm-0.29.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.466251 usdm-0.29.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)     1611 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.29.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)    10753 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4667 2023-05-01 12:04:14.000000 usdm-0.29.0/src/usdm_excel/cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.29.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.29.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1564 2023-05-08 13:47:22.000000 usdm-0.29.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.477431 usdm-0.29.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.29.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.29.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.522542 usdm-0.29.0/src/usdm_excel/errors/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.29.0/src/usdm_excel/errors/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      933 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/errors/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      732 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/errors/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.29.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      883 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_excel/iso_8601_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.29.0/src/usdm_excel/logger.py
+-rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.29.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5641 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_excel/nodes_and_edges.py
+-rw-r--r--   0 daveih     (501) staff       (20)      824 2023-05-08 13:47:22.000000 usdm-0.29.0/src/usdm_excel/option_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.524131 usdm-0.29.0/src/usdm_excel/study_design_activity_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.29.0/src/usdm_excel/study_design_activity_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1570 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.525147 usdm-0.29.0/src/usdm_excel/study_design_arm_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.29.0/src/usdm_excel/study_design_arm_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1617 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.526102 usdm-0.29.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2003 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.527045 usdm-0.29.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2503 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.541660 usdm-0.29.0/src/usdm_excel/study_design_epoch_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.29.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1289 2023-06-09 09:44:08.000000 usdm-0.29.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.543777 usdm-0.29.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2794 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.548739 usdm-0.29.0/src/usdm_excel/study_design_ii_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_design_ii_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1991 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.549785 usdm-0.29.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2475 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.551384 usdm-0.29.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1778 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.552976 usdm-0.29.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1645 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.554132 usdm-0.29.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     6803 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.555237 usdm-0.29.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3435 2023-05-17 10:35:35.000000 usdm-0.29.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.556485 usdm-0.29.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7866 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.562372 usdm-0.29.0/src/usdm_excel/study_soa_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3498 2023-05-09 06:07:57.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/cycle.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/cycles.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4663 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5463 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/timepoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2765 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/timepoint_type.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2145 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/timepoints.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1962 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_excel/study_soa_sheet/window_type.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.562804 usdm-0.29.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       59 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.581436 usdm-0.29.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      586 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.29.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      816 2023-06-14 09:02:56.000000 usdm-0.29.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      383 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      243 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      151 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      661 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      240 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      195 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      251 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      238 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/investigational_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      289 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      346 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/organisation.py
+-rw-r--r--   0 daveih     (501) staff       (20)      339 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      551 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      729 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      676 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      294 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      188 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1820 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      398 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/study_design_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      356 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      328 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      250 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.29.0/src/usdm_model/study_protocol_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      492 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      135 2023-06-12 09:18:24.000000 usdm-0.29.0/src/usdm_model/transition_rule.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-06-14 09:05:23.591047 usdm-0.29.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    14241 2023-05-16 13:26:16.000000 usdm-0.29.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.29.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1517 2023-05-08 13:47:22.000000 usdm-0.29.0/tests/test_configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      880 2023-05-17 10:35:35.000000 usdm-0.29.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2234 2023-05-17 10:35:35.000000 usdm-0.29.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2465 2023-06-14 09:02:56.000000 usdm-0.29.0/tests/test_integration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.29.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1763 2023-06-12 09:18:24.000000 usdm-0.29.0/tests/test_iso_8601_duration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.29.0/tests/test_ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1098 2023-05-08 13:47:22.000000 usdm-0.29.0/tests/test_option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3174 2023-06-14 09:02:56.000000 usdm-0.29.0/tests/test_study_design_activity_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.29.0/tests/test_study_design_arm_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.29.0/tests/test_study_design_epoch_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4884 2023-05-16 13:26:16.000000 usdm-0.29.0/tests/test_study_identifiers_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4531 2023-06-14 09:02:56.000000 usdm-0.29.0/tests/test_study_soa_sheet.py
```

### Comparing `usdm-0.28.0/LICENSE` & `usdm-0.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/PKG-INFO` & `usdm-0.29.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.28.0
+Version: 0.29.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `usdm-0.28.0/README.md` & `usdm-0.29.0/README.md`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/setup.py` & `usdm-0.29.0/setup.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.29.0/src/usdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.28.0
+Version: 0.29.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `usdm-0.28.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.29.0/src/usdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/__init__.py` & `usdm-0.29.0/src/usdm_excel/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/base_sheet.py` & `usdm-0.29.0/src/usdm_excel/base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/cdisc_biomedical_concept.py` & `usdm-0.29.0/src/usdm_excel/cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/cdisc_ct.py` & `usdm-0.29.0/src/usdm_excel/cdisc_ct.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.29.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/configuration_sheet.py` & `usdm-0.29.0/src/usdm_excel/configuration_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.29.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.29.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.29.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/errors/error.py` & `usdm-0.29.0/src/usdm_excel/errors/error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/errors/errors.py` & `usdm-0.29.0/src/usdm_excel/errors/errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/id_manager.py` & `usdm-0.29.0/src/usdm_excel/id_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/iso_3166.py` & `usdm-0.29.0/src/usdm_excel/iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/iso_8601_duration.py` & `usdm-0.29.0/src/usdm_excel/iso_8601_duration.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/nodes_and_edges.py` & `usdm-0.29.0/src/usdm_excel/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/option_manager.py` & `usdm-0.29.0/src/usdm_excel/option_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
       self.intervention_model = None
       self.main_timeline = None
       self.other_timelines = []
       self.process_sheet()
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
-      print(f"{traceback.format_exc()}")
 
   def process_sheet(self):
     for rindex, row in self.sheet.iterrows():
       if rindex == self.NAME_ROW:
         self.name = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif rindex == self.DESCRIPTION_ROW:
         self.description = self.read_cell(rindex, self.PARAMS_DATA_COL)
```

### Comparing `usdm-0.28.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_sheet/study_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_sheet/study_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
         self.phase = Alias().code(phase, [])
       elif rindex == self.ACRONYM_ROW:
         self.acronym = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif rindex == self.RATIONALE_ROW:
         self.rationale = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif rindex == self.TA_ROW:
         self.therapeutic_areas = self.read_other_code_cell_mutiple(rindex, self.PARAMS_DATA_COL)
-        #print("8", self.therapeutic_areas)
       elif rindex >= self.PROTOCOL_DATA_ROW:
         record = {}
         for cindex in range(0, len(self.sheet.columns)):
           field = fields[cindex]
           if field == 'protocolStatus':
             record[field] = self.read_cdisc_klass_attribute_cell('StudyProtocolVersion', 'protocolStatus', rindex, cindex) 
           elif field == 'protocolEffectiveDate':
```

### Comparing `usdm-0.28.0/src/usdm_excel/study_soa_sheet/activities.py` & `usdm-0.29.0/src/usdm_excel/study_soa_sheet/activities.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_soa_sheet/activity.py` & `usdm-0.29.0/src/usdm_excel/study_soa_sheet/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_soa_sheet/cycle.py` & `usdm-0.29.0/src/usdm_excel/study_soa_sheet/cycle.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_soa_sheet/cycles.py` & `usdm-0.29.0/src/usdm_excel/study_soa_sheet/cycles.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py` & `usdm-0.29.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
         if prev_instance is not None:
           prev_instance.defaultConditionId = instance.scheduledInstanceId
         prev_instance = instance
       exit = self._add_exit()
       self.timeline = self._add_timeline(self.name, self.description, self.condition, instances, exit)
 
     except Exception as e:
-      print(f"Exception [{e}] raised reading sheet")
+      #print(f"Exception [{e}] raised reading sheet")
+      #print(f"{traceback.format_exc()}")
       self._general_error(f"Exception [{e}] raised reading sheet")
       self._traceback(f"{traceback.format_exc()}")
 
   def _process_sheet(self):
     for rindex in range(self.NAME_ROW, self.CONDITION_ROW + 1):
       if rindex == self.NAME_ROW:
         self.name = self.read_cell(rindex, self.PARAMS_DATA_COL)
```

### Comparing `usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoint.py` & `usdm-0.29.0/src/usdm_excel/study_soa_sheet/timepoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from usdm_excel.cdisc_ct import CDISCCT
 from usdm_model.timing import Timing
 from usdm_model.scheduled_instance import ScheduledActivityInstance, ScheduledDecisionInstance
 
 class Timepoint():
   
   def __init__(self, parent, activity_names, col_index, type="", value="", cycle=None, additional=False):
+    epoch_ref = None
     self.parent = parent
     self.col_index = col_index
     if col_index == None:
       self._position_key = None
     else:
       self._position_key = col_index - SoAColumnRows.FIRST_VISIT_COL
     self.encounter_xref = ""
@@ -26,21 +27,22 @@
         self.has_encounter = True
       self.epoch = self.parent.read_cell_with_previous(SoAColumnRows.EPOCH_ROW, col_index, SoAColumnRows.FIRST_VISIT_COL)
       epoch_ref = cross_references.get(self.epoch)
     self.activities = []
     self.activity_map = {}
     self.__timepoint_type = None
     self.reference = None
-    #self.timing_type = type
-    #self.timing_value = value
+    self.timing_value = ""
     self.__window = None
     self.cycle = cycle
     if not additional:
       self._process_timepoint()
       self._add_activities(activity_names)
+    else:
+      self._synthetic_timepoint(type, value, cycle)
     self.usdm_timepoint = self._as_usdm()
     if self.has_encounter:
       encounter = cross_references.get(self.encounter_xref)
       self.usdm_timepoint.scheduledActivityInstanceEncounterId = encounter.encounterId
     if epoch_ref is not None:
       self.usdm_timepoint.epochId = epoch_ref.studyEpochId
 
@@ -51,14 +53,21 @@
     self.usdm_timepoint.activityIds.append(activity.usdm_activity.activityId)
 
   def _process_timepoint(self):
     self.__timepoint_type = TimepointType(self.parent, SoAColumnRows.TIMING_ROW, self.col_index)
     self.reference = self.col_index - SoAColumnRows.FIRST_VISIT_COL + self.__timepoint_type.relative_ref
     self.__window = WindowType(self.parent, SoAColumnRows.VISIT_WINDOW_ROW, self.col_index)
 
+  def _synthetic_timepoint(self, type, value, cycle):
+    self.__timepoint_type = TimepointType(None, 0, 0)
+    self.__timepoint_type.set_type(type, value, cycle)
+    self.timing_value = value
+    #self.reference = self.col_index - SoAColumnRows.FIRST_VISIT_COL + self.__timepoint_type.relative_ref
+    self.__window = WindowType(None, 0, 0)
+
   def _as_usdm(self):
     instance = None
     if self.__timepoint_type.timing_type in ["anchor", "next", "previous", "cycle start"]:
       timing = self._to_timing()
       instance = ScheduledActivityInstance(
         scheduledInstanceId=id_manager.build_id(ScheduledActivityInstance),
         scheduledInstanceType='ACTIVITY',
```

### Comparing `usdm-0.28.0/src/usdm_excel/study_soa_sheet/timepoint_type.py` & `usdm-0.29.0/src/usdm_excel/study_soa_sheet/timepoint_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 import re
 from usdm_excel.iso_8601_duration import ISO8601Duration
 
 class TimepointType():
 
   def __init__(self, parent, row_index, col_index):
-    self.__parent = parent
-    self.__row = row_index
-    self.__col = col_index
     self.timing_type = None
     self.relative_ref = 0
     self.description = None
     self.value = ISO8601Duration.ZERO_DURATION
-    timing_info = self.__parent.read_cell(row_index, col_index)
-    if timing_info:
-      timing_parts = timing_info.split(":")
-      if len(timing_parts) == 2:
-        if timing_parts[0].upper()[0] == "A":
-          self.timing_type = "anchor"
-          self.relative_ref = 0
-        if timing_parts[0].upper()[0] == "P":
-          self.timing_type = "previous"
-          self.relative_ref = self._get_relative_ref(timing_parts[0]) * -1
-          self._set_text_and_encoded(timing_parts[1])
-        elif timing_parts[0].upper()[0] == "N":
-          self.timing_type = "next"
-          self.relative_ref = self._get_relative_ref(timing_parts[0])
-          self._set_text_and_encoded(timing_parts[1])
-        elif timing_parts[0].upper()[0] == "C":
-          self.timing_type = "cycle start"
-          self.relative_ref = self._get_relative_ref(timing_parts[0])
-          self._set_text_and_encoded(timing_parts[1])
+    if parent is not None:
+      self.__parent = parent
+      self.__row = row_index
+      self.__col = col_index
+      timing_info = self.__parent.read_cell(row_index, col_index)
+      if timing_info:
+        timing_parts = timing_info.split(":")
+        if len(timing_parts) == 2:
+          if timing_parts[0].upper()[0] == "A":
+            self.timing_type = "anchor"
+            self.relative_ref = 0
+          if timing_parts[0].upper()[0] == "P":
+            self.timing_type = "previous"
+            self.relative_ref = self._get_relative_ref(timing_parts[0]) * -1
+            self._set_text_and_encoded(timing_parts[1])
+          elif timing_parts[0].upper()[0] == "N":
+            self.timing_type = "next"
+            self.relative_ref = self._get_relative_ref(timing_parts[0])
+            self._set_text_and_encoded(timing_parts[1])
+          elif timing_parts[0].upper()[0] == "C":
+            self.timing_type = "cycle start"
+            self.relative_ref = self._get_relative_ref(timing_parts[0])
+            self._set_text_and_encoded(timing_parts[1])
+        else:
+          self._log_error(f"Could not decode the timing value, no ':' detected in '{timing_info}'")
       else:
-        self._log_error(f"Could not decode the timing value, no ':' detected in '{timing_info}'")
-    else:
-      self._log_error(f"Could not decode the timing value, cell was empty")
- 
+        self._log_error(f"Could not decode the timing value, cell was empty")
+    
+  def set_type(self, type, value, cycle):
+    #print(f"SET TYPE: T='{type}', V='{value}', C='{cycle}'")
+    self.timing_type = type
+
   def _set_text_and_encoded(self, duration):
     the_duration = duration.strip()
     original_duration = the_duration
     for char in ['+', '-']:
       if char in the_duration:
         the_duration = the_duration.replace(char, "")
         self._log_warning(f"Ignoring '{char}' in {original_duration}")
```

### Comparing `usdm-0.28.0/src/usdm_excel/study_soa_sheet/window_type.py` & `usdm-0.29.0/src/usdm_excel/study_soa_sheet/window_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import re
 from usdm_excel.iso_8601_duration import ISO8601Duration
 
 class WindowType():
 
   def __init__(self, parent, row_index, col_index):
-    self.__parent = parent
-    self.__row = row_index
-    self.__col = col_index
     self.description = None
     self.upper = None
     self.lower = None
-    timing_info = self.__parent.read_cell(row_index, col_index)
-    if timing_info:
-      self.description = timing_info.strip()
-      match = re.match(r"(?P<lower>[+|-]*\d+)\s*\.\.\s*(?P<upper>[+|-]*\d+) \s*(?P<units>.+)", self.description)
-      if match is not None:
-        timing_parts = match.groupdict()
-        self.lower = self._set_encoded(f"{timing_parts['lower']}{timing_parts['units']}")
-        self.upper = self._set_encoded(f"{timing_parts['upper']}{timing_parts['units']}")     
+    if parent is not None:
+      self.__parent = parent
+      self.__row = row_index
+      self.__col = col_index
+      timing_info = self.__parent.read_cell(row_index, col_index)
+      if timing_info:
+        self.description = timing_info.strip()
+        match = re.match(r"(?P<lower>[+|-]*\d+)\s*\.\.\s*(?P<upper>[+|-]*\d+) \s*(?P<units>.+)", self.description)
+        if match is not None:
+          timing_parts = match.groupdict()
+          self.lower = self._set_encoded(f"{timing_parts['lower']}{timing_parts['units']}")
+          self.upper = self._set_encoded(f"{timing_parts['upper']}{timing_parts['units']}")     
+        else:
+          self._log_error(f"Could not decode the window value, not all required parts detected in '{timing_info}'")
       else:
-        self._log_error(f"Could not decode the window value, not all required parts detected in '{timing_info}'")
-    else:
-      pass
-      #self._log_error(f"Could not decode the window value, cell was empty") # <<< Window can be empty
+        pass
  
   def _set_encoded(self, duration):
     the_duration = duration.strip()
     original_duration = the_duration
     for char in ['+', '-']:
       if char in the_duration:
         the_duration = the_duration.replace(char, "")
```

### Comparing `usdm-0.28.0/src/usdm_model/__init__.py` & `usdm-0.29.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_model/activity.py` & `usdm-0.29.0/src/usdm_model/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_model/api_base_model.py` & `usdm-0.29.0/src/usdm_model/api_base_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pydantic import BaseModel
 import json
 import enum
 import datetime
 
 def _serialize_as_json(obj):
-  #print("OBJ:", type(obj))
   if isinstance(obj, enum.Enum):
     return obj.value
   elif isinstance(obj, datetime.date):
     return obj.isoformat()
   else:
     return obj.__dict__
```

### Comparing `usdm-0.28.0/src/usdm_model/encounter.py` & `usdm-0.29.0/src/usdm_model/encounter.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_model/estimand.py` & `usdm-0.29.0/src/usdm_model/estimand.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_model/schedule_timeline.py` & `usdm-0.29.0/src/usdm_model/schedule_timeline.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_model/scheduled_instance.py` & `usdm-0.29.0/src/usdm_model/scheduled_instance.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_model/study.py` & `usdm-0.29.0/src/usdm_model/study.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/src/usdm_model/study_design.py` & `usdm-0.29.0/src/usdm_model/study_design.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_base_sheet.py` & `usdm-0.29.0/tests/test_base_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.29.0/tests/test_cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_configuration_sheet.py` & `usdm-0.29.0/tests/test_configuration_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_error.py` & `usdm-0.29.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_errors.py` & `usdm-0.29.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_integration.py` & `usdm-0.29.0/tests/test_integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,25 +14,22 @@
   items = list(reader)
   for item in items:
     item['row'] = int(item['row'])
     item['column'] = int(item['column'])
   return items
 
 def run_test(filename, save=False):
-  print(f"RUN: S={save}")
   excel = USDMExcel(f"tests/integration_test_files/{filename}.xlsx")
   result = excel.to_json()
   errors = excel.errors()
 
   # Useful if you want to see the results.
-  print(f"ERRORS: S={save} E={errors}")
   if save or SAVE_ALL:
     with open(f"tests/integration_test_files/{filename}.json", 'w', encoding='utf-8') as f:
       f.write(json.dumps(json.loads(result), indent=2))
-    print(f"ERRORS: {errors}")
     with open(f"tests/integration_test_files/{filename}_errors.csv", 'w',newline='') as f:
       save_error_csv(f, errors) 
   
   with open(f"tests/integration_test_files/{filename}.json", 'r') as f:
     expected = json.dumps(json.load(f)) # Odd, but doing it for consistency of processing
   assert result == expected
   with open(f"tests/integration_test_files/{filename}_errors.csv", 'r') as f:
@@ -79,7 +76,13 @@
   run_test_ne('complex_1')
 
 def test_arms_epochs_1():
   run_test('arms_epochs')
 
 def test_arms_epochs_1_ne():
   run_test_ne('arms_epochs')
+
+def test_cycles_1():
+  run_test('cycles_1')
+
+def test_cycles_1_ne():
+  run_test_ne('cycles_1')
```

### Comparing `usdm-0.28.0/tests/test_iso_3166.py` & `usdm-0.29.0/tests/test_iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_iso_8601_duration.py` & `usdm-0.29.0/tests/test_iso_8601_duration.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_option_manager.py` & `usdm-0.29.0/tests/test_option_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_study_design_activity_sheet.py` & `usdm-0.29.0/tests/test_study_design_activity_sheet.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,13 +55,12 @@
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   data = [['Activity 1', 'Activity One']]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['activityName', 'activityDescription'])
   activities = StudyDesignActivitySheet("")
   mock_error.assert_called()
-  print(call_parameters)
   assert call_parameters == [
     ("studyDesignActivities", 1, -1, "Error ('activityIsConditional') reading cell", 10),
     ("studyDesignActivities", 1, -1, "Error ('activityIsConditionalReason') reading cell", 10),
   ]
```

### Comparing `usdm-0.28.0/tests/test_study_design_arm_sheet.py` & `usdm-0.29.0/tests/test_study_design_arm_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_study_design_epoch_sheet.py` & `usdm-0.29.0/tests/test_study_design_epoch_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_study_identifiers_sheet.py` & `usdm-0.29.0/tests/test_study_identifiers_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.28.0/tests/test_study_soa_sheet.py` & `usdm-0.29.0/tests/test_study_soa_sheet.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,21 +20,27 @@
     (2,0,'previous', -2, "2D", "P2D"),
     (3,0,'cycle start', 1, None, ISO8601Duration.ZERO_DURATION),
     (4,0,'next', 3, "3 weeks", "P3W"),
     (5,0,'next', 1, "+2 days", "P2D"),
     (6,0,'previous', -1, "-3 hrs", "PT3H"),
   ]
   for index, test in enumerate(test_data):
-    print(f"IDX {index}")
     item = TimepointType(parent, test[0], test[1])
     assert(item.timing_type) == test[2]
     assert(item.relative_ref) == test[3]
     assert(item.description) == test[4]
     assert(item.value) == test[5]
 
+def test_synthetic_timepoint_type():
+  item = TimepointType(None, 0, 0)
+  assert(item.timing_type) == None
+  assert(item.relative_ref) == 0
+  assert(item.description) == None
+  assert(item.value) == ISO8601Duration.ZERO_DURATION
+
 def test_timepoint_type_error(mocker):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   mock_read = mocker.patch("pandas.read_excel")
   data = { 'col_1': [ 'A', 'P: 2 ', '', 'P2: 2 decades' ] }
   mock_read.return_value = pd.DataFrame.from_dict(data)
   parent = BaseSheet("", "Sheet X")
@@ -67,14 +73,20 @@
   ]
   for index, test in enumerate(test_data):
     item = WindowType(parent, test[0], test[1])
     assert(item.description) == test[2]
     assert(item.lower) == test[3]
     assert(item.upper) == test[4]
 
+def test_synthetic_window_type():
+  item = WindowType(None, 0, 0)
+  assert(item.description) == None
+  assert(item.lower) == None
+  assert(item.upper) == None
+
 def test_window_type_error(mocker):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
   mock_read = mocker.patch("pandas.read_excel")
   data = { 'col_1': [ '1.. Days', '-1.1 days', '-1 .. 1', '.. 1 Weeks', '' ] }
   mock_read.return_value = pd.DataFrame.from_dict(data)
   parent = BaseSheet("", "Sheet X")
```

