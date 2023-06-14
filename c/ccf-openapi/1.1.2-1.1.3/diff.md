# Comparing `tmp/ccf-openapi-1.1.2.tar.gz` & `tmp/ccf-openapi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccf-openapi-1.1.2.tar", last modified: Tue Jun  6 19:49:55 2023, max compression
+gzip compressed data, was "ccf-openapi-1.1.3.tar", last modified: Wed Jun 14 15:26:58 2023, max compression
```

## Comparing `ccf-openapi-1.1.2.tar` & `ccf-openapi-1.1.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/PKG-INFO
--rw-r--r--   0 bherr     (1000) bherr     (1000)     9274 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/README.md
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/ccf_openapi.egg-info/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-06-06 19:49:55.000000 ccf-openapi-1.1.2/ccf_openapi.egg-info/PKG-INFO
--rw-r--r--   0 bherr     (1000) bherr     (1000)     2880 2023-06-06 19:49:55.000000 ccf-openapi-1.1.2/ccf_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 bherr     (1000) bherr     (1000)        1 2023-06-06 19:49:55.000000 ccf-openapi-1.1.2/ccf_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 bherr     (1000) bherr     (1000)       32 2023-06-06 19:49:55.000000 ccf-openapi-1.1.2/ccf_openapi.egg-info/requires.txt
--rw-r--r--   0 bherr     (1000) bherr     (1000)       19 2023-06-06 19:49:55.000000 ccf-openapi-1.1.2/ccf_openapi.egg-info/top_level.txt
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/ccf_openapi_client/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      850 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/__init__.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/ccf_openapi_client/api/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      222 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/api/__init__.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)   104876 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/api/default_api.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    37737 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/api_client.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/ccf_openapi_client/apis/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      471 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/apis/__init__.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16559 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/configuration.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     5140 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/exceptions.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/ccf_openapi_client/model/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      348 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/__init__.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11524 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/aggregate_count.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12078 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/database_status.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11108 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/error_message.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16430 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/flat_spatial_placement.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11732 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/get_spatial_placement_request.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    10915 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/json_ld_object.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11255 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/min_max.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11747 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/ontology_tree.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    14194 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/ontology_tree_node.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11443 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/rgba.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11164 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/sparql_query_request.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    19757 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_entity.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12267 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_entity_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12072 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_entity_creator.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12370 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_entity_dimensions.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    13671 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_object_reference.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16736 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16857 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12287 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement_rotation.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12190 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement_scaling.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    12474 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement_translation.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    18061 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_scene_node.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11807 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_search.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    16469 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_block.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11549 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    14011 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_dataset.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    13866 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_donor.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    11680 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_sample_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    14674 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_section.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    82158 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/model_utils.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/ccf_openapi_client/models/
--rw-r--r--   0 bherr     (1000) bherr     (1000)     2495 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/models/__init__.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)    14268 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/ccf_openapi_client/rest.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)       69 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/setup.cfg
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1181 2023-06-06 19:49:43.000000 ccf-openapi-1.1.2/setup.py
-drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-06 19:49:55.517773 ccf-openapi-1.1.2/test/
--rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_aggregate_count.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_database_status.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     3580 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_default_api.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_error_message.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1029 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_flat_spatial_placement.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1035 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_get_spatial_placement_request.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      827 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_json_ld_object.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      784 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_min_max.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      948 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_ontology_tree.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      961 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_ontology_tree_node.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      769 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_rgba.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      869 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_sparql_query_request.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1579 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_entity.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      876 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_entity_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      883 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_entity_creator.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_entity_dimensions.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1003 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_object_reference.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1109 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_placement.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1473 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_placement_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      911 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_placement_rotation.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_placement_scaling.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      932 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_placement_translation.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1167 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_scene_node.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      833 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_spatial_search.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1479 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_tissue_block.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_tissue_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1044 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_tissue_dataset.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1030 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_tissue_donor.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)      978 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_tissue_sample_common.py
--rw-r--r--   0 bherr     (1000) bherr     (1000)     1283 2023-06-06 19:46:32.000000 ccf-openapi-1.1.2/test/test_tissue_section.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.989572 ccf-openapi-1.1.3/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-06-14 15:26:58.989572 ccf-openapi-1.1.3/PKG-INFO
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     9274 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/README.md
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.969572 ccf-openapi-1.1.3/ccf_openapi.egg-info/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     2880 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)        1 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       32 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/requires.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       19 2023-06-14 15:26:58.000000 ccf-openapi-1.1.3/ccf_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      850 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/__init__.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/api/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      222 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/api/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)   104876 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/api/default_api.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    37737 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/api_client.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/apis/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      471 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/apis/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16559 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/configuration.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     5140 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/exceptions.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/model/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      348 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11524 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/aggregate_count.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12078 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/database_status.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11108 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/error_message.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16430 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/flat_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11732 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/get_spatial_placement_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    10915 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/json_ld_object.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11255 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/min_max.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11747 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/ontology_tree.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14402 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/ontology_tree_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11443 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/rgba.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11164 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/sparql_query_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    19757 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12267 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12072 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_creator.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12370 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_dimensions.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    13721 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_object_reference.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16736 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16857 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12287 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_rotation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12190 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_scaling.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12474 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_translation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    18061 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_scene_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11807 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_search.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16643 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_block.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11549 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14111 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_dataset.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    13916 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_donor.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11680 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_sample_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14726 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_section.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    82158 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/model_utils.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.979572 ccf-openapi-1.1.3/ccf_openapi_client/models/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     2495 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/models/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14268 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/ccf_openapi_client/rest.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       69 2023-06-14 15:26:58.989572 ccf-openapi-1.1.3/setup.cfg
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1181 2023-06-14 15:26:54.000000 ccf-openapi-1.1.3/setup.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-06-14 15:26:58.989572 ccf-openapi-1.1.3/test/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_aggregate_count.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_database_status.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     3580 2023-06-14 15:21:34.000000 ccf-openapi-1.1.3/test/test_default_api.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_error_message.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1029 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_flat_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1035 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_get_spatial_placement_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      827 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_json_ld_object.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      784 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_min_max.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      948 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_ontology_tree.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      961 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_ontology_tree_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      769 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_rgba.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      869 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_sparql_query_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1579 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_entity.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      876 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_entity_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      883 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_entity_creator.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_entity_dimensions.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1003 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_object_reference.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1109 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1473 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      911 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement_rotation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement_scaling.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      932 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_placement_translation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1167 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_scene_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      833 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_spatial_search.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1479 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_block.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1044 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_dataset.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1030 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_donor.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      978 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_sample_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1283 2023-06-14 15:21:33.000000 ccf-openapi-1.1.3/test/test_tissue_section.py
```

### Comparing `ccf-openapi-1.1.2/README.md` & `ccf-openapi-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi.egg-info/SOURCES.txt` & `ccf-openapi-1.1.3/ccf_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/__init__.py` & `ccf-openapi-1.1.3/ccf_openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/api/default_api.py` & `ccf-openapi-1.1.3/ccf_openapi_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/api_client.py` & `ccf-openapi-1.1.3/ccf_openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/configuration.py` & `ccf-openapi-1.1.3/ccf_openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/exceptions.py` & `ccf-openapi-1.1.3/ccf_openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/aggregate_count.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/aggregate_count.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/database_status.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/database_status.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/error_message.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/error_message.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/flat_spatial_placement.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/flat_spatial_placement.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/get_spatial_placement_request.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/get_spatial_placement_request.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/json_ld_object.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/json_ld_object.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/min_max.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/min_max.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/ontology_tree.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/ontology_tree.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/ontology_tree_node.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/ontology_tree_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,47 +83,43 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'id': (str,),  # noqa: E501
             'label': (str,),  # noqa: E501
             'synonym_labels': ([str],),  # noqa: E501
             'parent': (str,),  # noqa: E501
             'children': ([str],),  # noqa: E501
-            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'id': 'id',  # noqa: E501
         'label': 'label',  # noqa: E501
         'synonym_labels': 'synonymLabels',  # noqa: E501
         'parent': 'parent',  # noqa: E501
         'children': 'children',  # noqa: E501
-        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """OntologyTreeNode - a model defined in OpenAPI
 
         Keyword Args:
-            label (str): Main descriptive label for the node.
-            synonym_labels ([str]): Additional label for the node.
-            parent (str): Reference to the parent node.
-            children ([str]): References to all child nodes.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -147,14 +143,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Unique identifier for the node.. [optional]  # noqa: E501
+            label (str): Main descriptive label for the node.. [optional]  # noqa: E501
+            synonym_labels ([str]): Additional label for the node.. [optional]  # noqa: E501
+            parent (str): Reference to the parent node.. [optional]  # noqa: E501
+            children ([str]): References to all child nodes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -216,18 +216,14 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """OntologyTreeNode - a model defined in OpenAPI
 
         Keyword Args:
-            label (str): Main descriptive label for the node.
-            synonym_labels ([str]): Additional label for the node.
-            parent (str): Reference to the parent node.
-            children ([str]): References to all child nodes.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -251,14 +247,18 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Unique identifier for the node.. [optional]  # noqa: E501
+            label (str): Main descriptive label for the node.. [optional]  # noqa: E501
+            synonym_labels ([str]): Additional label for the node.. [optional]  # noqa: E501
+            parent (str): Reference to the parent node.. [optional]  # noqa: E501
+            children ([str]): References to all child nodes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/rgba.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/rgba.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/sparql_query_request.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/sparql_query_request.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_entity.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_entity_common.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_entity_creator.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_creator.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_entity_dimensions.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_entity_dimensions.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_object_reference.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_object_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,40 +83,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'file_format': (str,),  # noqa: E501
             'file': (str,),  # noqa: E501
+            'file_format': (str,),  # noqa: E501
             'file_subpath': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'file_format': 'file_format',  # noqa: E501
         'file': 'file',  # noqa: E501
+        'file_format': 'file_format',  # noqa: E501
         'file_subpath': 'file_subpath',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """SpatialObjectReference - a model defined in OpenAPI
 
         Keyword Args:
-            file_format (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -140,14 +139,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             file (str): [optional]  # noqa: E501
+            file_format (str): [optional]  # noqa: E501
             file_subpath (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -210,15 +210,14 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """SpatialObjectReference - a model defined in OpenAPI
 
         Keyword Args:
-            file_format (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -242,14 +241,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             file (str): [optional]  # noqa: E501
+            file_format (str): [optional]  # noqa: E501
             file_subpath (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement_common.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement_rotation.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_rotation.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement_scaling.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_scaling.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_placement_translation.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_placement_translation.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_scene_node.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_scene_node.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/spatial_search.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/spatial_search.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_block.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,60 +100,55 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'sample_type': (str,),  # noqa: E501
+            'label': (str,),  # noqa: E501
+            'link': (str,),  # noqa: E501
+            'datasets': ([TissueDataset],),  # noqa: E501
+            'spatial_entity_id': (str,),  # noqa: E501
             'donor': (TissueDonor,),  # noqa: E501
             'section_count': (int,),  # noqa: E501
             'section_size': (float,),  # noqa: E501
             'section_units': (str,),  # noqa: E501
             'sections': ([TissueSection],),  # noqa: E501
-            'label': (str,),  # noqa: E501
-            'link': (str,),  # noqa: E501
-            'datasets': ([TissueDataset],),  # noqa: E501
-            'spatial_entity_id': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'sample_type': 'sampleType',  # noqa: E501
+        'label': 'label',  # noqa: E501
+        'link': 'link',  # noqa: E501
+        'datasets': 'datasets',  # noqa: E501
+        'spatial_entity_id': 'spatialEntityId',  # noqa: E501
         'donor': 'donor',  # noqa: E501
         'section_count': 'sectionCount',  # noqa: E501
         'section_size': 'sectionSize',  # noqa: E501
         'section_units': 'sectionUnits',  # noqa: E501
         'sections': 'sections',  # noqa: E501
-        'label': 'label',  # noqa: E501
-        'link': 'link',  # noqa: E501
-        'datasets': 'datasets',  # noqa: E501
-        'spatial_entity_id': 'spatialEntityId',  # noqa: E501
         'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """TissueBlock - a model defined in OpenAPI
 
         Keyword Args:
             sample_type (str):
-            donor (TissueDonor):
-            section_count (int): Number of sections contained in the block.
-            section_size (float): Size of each section in the block.
-            section_units (str): Length unit `sectionSize` is in (generally, millimeters). defaults to "millimeters"  # noqa: E501
-            sections ([TissueSection]): All sections in the block.
             label (str):
             link (str):
             datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -180,18 +175,22 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             spatial_entity_id (str): The associated spatial entity (rui_location) for the block.. [optional]  # noqa: E501
+            donor (TissueDonor): [optional]  # noqa: E501
+            section_count (int): Number of sections contained in the block.. [optional]  # noqa: E501
+            section_size (float): Size of each section in the block.. [optional]  # noqa: E501
+            section_units (str): Length unit `sectionSize` is in (generally, millimeters). [optional] if omitted the server will use the default value of "millimeters"  # noqa: E501
+            sections ([TissueSection]): All sections in the block.. [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
         """
 
-        section_units = kwargs.get('section_units', "millimeters")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         self = super(OpenApiModel, cls).__new__(cls)
@@ -252,19 +251,14 @@
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """TissueBlock - a model defined in OpenAPI
 
         Keyword Args:
             sample_type (str):
-            donor (TissueDonor):
-            section_count (int): Number of sections contained in the block.
-            section_size (float): Size of each section in the block.
-            section_units (str): Length unit `sectionSize` is in (generally, millimeters). defaults to "millimeters"  # noqa: E501
-            sections ([TissueSection]): All sections in the block.
             label (str):
             link (str):
             datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -291,18 +285,22 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             spatial_entity_id (str): The associated spatial entity (rui_location) for the block.. [optional]  # noqa: E501
+            donor (TissueDonor): [optional]  # noqa: E501
+            section_count (int): Number of sections contained in the block.. [optional]  # noqa: E501
+            section_size (float): Size of each section in the block.. [optional]  # noqa: E501
+            section_units (str): Length unit `sectionSize` is in (generally, millimeters). [optional] if omitted the server will use the default value of "millimeters"  # noqa: E501
+            sections ([TissueSection]): All sections in the block.. [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
         """
 
-        section_units = kwargs.get('section_units', "millimeters")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
```

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_common.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_dataset.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_donor.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def lazy_import():
     from ccf_openapi_client.model.json_ld_object import JsonLdObject
     from ccf_openapi_client.model.tissue_common import TissueCommon
     globals()['JsonLdObject'] = JsonLdObject
     globals()['TissueCommon'] = TissueCommon
 
 
-class TissueDataset(ModelComposed):
+class TissueDonor(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,45 +85,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'technology': (str,),  # noqa: E501
-            'thumbnail': (str,),  # noqa: E501
             'label': (str,),  # noqa: E501
             'link': (str,),  # noqa: E501
+            'provider_name': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'technology': 'technology',  # noqa: E501
-        'thumbnail': 'thumbnail',  # noqa: E501
         'label': 'label',  # noqa: E501
         'link': 'link',  # noqa: E501
+        'provider_name': 'providerName',  # noqa: E501
         'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TissueDataset - a model defined in OpenAPI
+        """TissueDonor - a model defined in OpenAPI
 
         Keyword Args:
-            technology (str):
-            thumbnail (str):
             label (str):
             link (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -148,14 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            provider_name (str): [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -215,19 +212,17 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TissueDataset - a model defined in OpenAPI
+        """TissueDonor - a model defined in OpenAPI
 
         Keyword Args:
-            technology (str):
-            thumbnail (str):
             label (str):
             link (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -252,14 +247,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            provider_name (str): [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_donor.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_section.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,19 +28,23 @@
 )
 from ccf_openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ccf_openapi_client.model.json_ld_object import JsonLdObject
     from ccf_openapi_client.model.tissue_common import TissueCommon
+    from ccf_openapi_client.model.tissue_dataset import TissueDataset
+    from ccf_openapi_client.model.tissue_sample_common import TissueSampleCommon
     globals()['JsonLdObject'] = JsonLdObject
     globals()['TissueCommon'] = TissueCommon
+    globals()['TissueDataset'] = TissueDataset
+    globals()['TissueSampleCommon'] = TissueSampleCommon
 
 
-class TissueDonor(ModelComposed):
+class TissueSection(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,14 +64,17 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('section_number',): {
+            'inclusive_minimum': 0,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -85,44 +92,49 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'provider_name': (str,),  # noqa: E501
+            'sample_type': (str,),  # noqa: E501
             'label': (str,),  # noqa: E501
             'link': (str,),  # noqa: E501
+            'datasets': ([TissueDataset],),  # noqa: E501
+            'section_number': (int,),  # noqa: E501
             'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'provider_name': 'providerName',  # noqa: E501
+        'sample_type': 'sampleType',  # noqa: E501
         'label': 'label',  # noqa: E501
         'link': 'link',  # noqa: E501
+        'datasets': 'datasets',  # noqa: E501
+        'section_number': 'sectionNumber',  # noqa: E501
         'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TissueDonor - a model defined in OpenAPI
+        """TissueSection - a model defined in OpenAPI
 
         Keyword Args:
-            provider_name (str):
+            sample_type (str):
             label (str):
             link (str):
+            datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -145,14 +157,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            section_number (int): Index of the section in the parent block.. [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -212,20 +225,21 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TissueDonor - a model defined in OpenAPI
+        """TissueSection - a model defined in OpenAPI
 
         Keyword Args:
-            provider_name (str):
+            sample_type (str):
             label (str):
             link (str):
+            datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -248,14 +262,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            section_number (int): Index of the section in the parent block.. [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -316,11 +331,12 @@
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               JsonLdObject,
               TissueCommon,
+              TissueSampleCommon,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_sample_common.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_sample_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model/tissue_section.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model/tissue_dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,23 +28,19 @@
 )
 from ccf_openapi_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ccf_openapi_client.model.json_ld_object import JsonLdObject
     from ccf_openapi_client.model.tissue_common import TissueCommon
-    from ccf_openapi_client.model.tissue_dataset import TissueDataset
-    from ccf_openapi_client.model.tissue_sample_common import TissueSampleCommon
     globals()['JsonLdObject'] = JsonLdObject
     globals()['TissueCommon'] = TissueCommon
-    globals()['TissueDataset'] = TissueDataset
-    globals()['TissueSampleCommon'] = TissueSampleCommon
 
 
-class TissueSection(ModelComposed):
+class TissueDataset(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -64,17 +60,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('section_number',): {
-            'inclusive_minimum': 0,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -92,50 +85,45 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'sample_type': (str,),  # noqa: E501
-            'section_number': (int,),  # noqa: E501
             'label': (str,),  # noqa: E501
             'link': (str,),  # noqa: E501
-            'datasets': ([TissueDataset],),  # noqa: E501
+            'technology': (str,),  # noqa: E501
+            'thumbnail': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'sample_type': 'sampleType',  # noqa: E501
-        'section_number': 'sectionNumber',  # noqa: E501
         'label': 'label',  # noqa: E501
         'link': 'link',  # noqa: E501
-        'datasets': 'datasets',  # noqa: E501
+        'technology': 'technology',  # noqa: E501
+        'thumbnail': 'thumbnail',  # noqa: E501
         'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TissueSection - a model defined in OpenAPI
+        """TissueDataset - a model defined in OpenAPI
 
         Keyword Args:
-            sample_type (str):
-            section_number (int): Index of the section in the parent block.
             label (str):
             link (str):
-            datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -158,14 +146,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            technology (str): [optional]  # noqa: E501
+            thumbnail (str): [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -225,22 +215,19 @@
         '_composed_instances',
         '_var_name_to_model_instances',
         '_additional_properties_model_instances',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TissueSection - a model defined in OpenAPI
+        """TissueDataset - a model defined in OpenAPI
 
         Keyword Args:
-            sample_type (str):
-            section_number (int): Index of the section in the parent block.
             label (str):
             link (str):
-            datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -263,14 +250,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            technology (str): [optional]  # noqa: E501
+            thumbnail (str): [optional]  # noqa: E501
             description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -331,12 +320,11 @@
         lazy_import()
         return {
           'anyOf': [
           ],
           'allOf': [
               JsonLdObject,
               TissueCommon,
-              TissueSampleCommon,
           ],
           'oneOf': [
           ],
         }
```

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/model_utils.py` & `ccf-openapi-1.1.3/ccf_openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/models/__init__.py` & `ccf-openapi-1.1.3/ccf_openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/ccf_openapi_client/rest.py` & `ccf-openapi-1.1.3/ccf_openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/setup.py` & `ccf-openapi-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
     CCF-API
 
     This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 1.1.3
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ccf-openapi"
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ccf-openapi-1.1.2/test/test_aggregate_count.py` & `ccf-openapi-1.1.3/test/test_aggregate_count.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_database_status.py` & `ccf-openapi-1.1.3/test/test_database_status.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_default_api.py` & `ccf-openapi-1.1.3/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_error_message.py` & `ccf-openapi-1.1.3/test/test_error_message.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_flat_spatial_placement.py` & `ccf-openapi-1.1.3/test/test_flat_spatial_placement.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_get_spatial_placement_request.py` & `ccf-openapi-1.1.3/test/test_get_spatial_placement_request.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_json_ld_object.py` & `ccf-openapi-1.1.3/test/test_json_ld_object.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_min_max.py` & `ccf-openapi-1.1.3/test/test_min_max.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_ontology_tree.py` & `ccf-openapi-1.1.3/test/test_ontology_tree.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_ontology_tree_node.py` & `ccf-openapi-1.1.3/test/test_ontology_tree_node.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_rgba.py` & `ccf-openapi-1.1.3/test/test_rgba.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_sparql_query_request.py` & `ccf-openapi-1.1.3/test/test_sparql_query_request.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_entity.py` & `ccf-openapi-1.1.3/test/test_spatial_entity.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_entity_common.py` & `ccf-openapi-1.1.3/test/test_spatial_entity_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_entity_creator.py` & `ccf-openapi-1.1.3/test/test_spatial_entity_creator.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_entity_dimensions.py` & `ccf-openapi-1.1.3/test/test_spatial_entity_dimensions.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_object_reference.py` & `ccf-openapi-1.1.3/test/test_spatial_object_reference.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_placement.py` & `ccf-openapi-1.1.3/test/test_spatial_placement.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_placement_common.py` & `ccf-openapi-1.1.3/test/test_spatial_placement_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_placement_rotation.py` & `ccf-openapi-1.1.3/test/test_spatial_placement_rotation.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_placement_scaling.py` & `ccf-openapi-1.1.3/test/test_spatial_placement_scaling.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_placement_translation.py` & `ccf-openapi-1.1.3/test/test_spatial_placement_translation.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_scene_node.py` & `ccf-openapi-1.1.3/test/test_spatial_scene_node.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_spatial_search.py` & `ccf-openapi-1.1.3/test/test_spatial_search.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_tissue_block.py` & `ccf-openapi-1.1.3/test/test_tissue_block.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_tissue_common.py` & `ccf-openapi-1.1.3/test/test_tissue_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_tissue_dataset.py` & `ccf-openapi-1.1.3/test/test_tissue_dataset.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_tissue_donor.py` & `ccf-openapi-1.1.3/test/test_tissue_donor.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_tissue_sample_common.py` & `ccf-openapi-1.1.3/test/test_tissue_sample_common.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.2/test/test_tissue_section.py` & `ccf-openapi-1.1.3/test/test_tissue_section.py`

 * *Files identical despite different names*

