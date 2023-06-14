# Comparing `tmp/debater_python_api-5.0.3.tar.gz` & `tmp/debater_python_api-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debater_python_api-5.0.3.tar", last modified: Tue Jun 13 07:10:00 2023, max compression
+gzip compressed data, was "debater_python_api-5.0.4.tar", last modified: Wed Jun 14 16:41:14 2023, max compression
```

## Comparing `debater_python_api-5.0.3.tar` & `debater_python_api-5.0.4.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.434270 debater_python_api-5.0.3/
--rw-r--r--   0 yoavkantor   (501) staff       (20)    11358 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/LICENSE
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-06-13 07:10:00.434076 debater_python_api-5.0.3/PKG-INFO
--rw-r--r--   0 yoavkantor   (501) staff       (20)      169 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/README.md
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.422852 debater_python_api-5.0.3/debater_python_api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.423724 debater_python_api-5.0.3/debater_python_api/api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.425837 debater_python_api-5.0.3/debater_python_api/api/clients/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4503 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/abstract_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1147 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/argument_quality_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1548 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/claim_and_evidence_detection_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      934 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/claim_boundaries_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6203 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/clustering_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3034 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/embedding_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1999 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/index_searcher_client.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.426558 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/
--rw-r--r--   0 yoavkantor   (501) staff       (20)      478 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    37388 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/KpsResult.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    12349 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/docx_generator.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    16293 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/graph_generator.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4239 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/utils.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6969 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_admin_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    38464 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1894 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_pairs_infer_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13830 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/narrative_generation_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1230 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/pro_con_client.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.426802 debater_python_api-5.0.3/debater_python_api/api/clients/response_data/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/response_data/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1597 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/response_data/speech_response.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1790 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/term_relater_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1563 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/term_wikifier_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3394 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/clients/theme_extraction_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3263 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/api/debater_api.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.426950 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.427856 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      142 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     5079 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1001 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1314 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3576 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1516 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.430252 debater_python_api-5.0.3/debater_python_api/examples/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      803 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/argument_quality_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      854 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/claim_boundaries_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1002 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/claim_detection_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      932 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/clustering_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      860 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/embedding_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1014 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/evidence_detection_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    85859 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/example_of_sc_args.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1480 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/index_searcher_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1204 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/examples/keypoints_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1428 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/pro_con_example.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.430708 debater_python_api-5.0.3/debater_python_api/examples/resources/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/resources/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    23817 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/resources/arguments.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.430860 debater_python_api-5.0.3/debater_python_api/examples/resources/filters_output/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/resources/filters_output/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     2530 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/resources/pro_con_scores.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     9581 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/run_all_services.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      870 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/speech_construction_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      480 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/term_relater_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      907 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/term_wikifier_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1154 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/theme_extraction_example.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.431260 debater_python_api-5.0.3/debater_python_api/examples/usecases/
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4943 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/usecases/kp_based_survey.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6036 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/usecases/mining_to_narrative.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    10191 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/examples/usecases/survey.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.431401 debater_python_api-5.0.3/debater_python_api/integration_tests/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.431521 debater_python_api-5.0.3/debater_python_api/integration_tests/api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.433013 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/
--rw-r--r--   0 yoavkantor   (501) staff       (20)     2708 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    11791 2023-06-13 07:07:20.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/ServicesIT.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4630 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/ServicesLoad.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.433821 debater_python_api-5.0.3/debater_python_api/utils/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/utils/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      992 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/utils/clusters_refiner.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1574 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/utils/general_utils.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      604 2022-12-21 08:56:59.000000 debater_python_api-5.0.3/debater_python_api/utils/kp_analysis_conf.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-13 07:10:00.423497 debater_python_api-5.0.3/debater_python_api.egg-info/
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4041 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)        1 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)       96 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/requires.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)       19 2023-06-13 07:10:00.000000 debater_python_api-5.0.3/debater_python_api.egg-info/top_level.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)      895 2023-06-13 07:07:43.000000 debater_python_api-5.0.3/pyproject.toml
--rw-r--r--   0 yoavkantor   (501) staff       (20)       38 2023-06-13 07:10:00.434321 debater_python_api-5.0.3/setup.cfg
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.749070 debater_python_api-5.0.4/
+-rw-r--r--   0 lilache    (501) staff       (20)    11358 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/LICENSE
+-rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-14 16:41:14.748792 debater_python_api-5.0.4/PKG-INFO
+-rw-r--r--   0 lilache    (501) staff       (20)      169 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/README.md
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.730381 debater_python_api-5.0.4/debater_python_api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.731286 debater_python_api-5.0.4/debater_python_api/api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.735453 debater_python_api-5.0.4/debater_python_api/api/clients/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     4503 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/abstract_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1147 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/argument_quality_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1548 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/claim_and_evidence_detection_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)      934 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/claim_boundaries_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6203 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/clustering_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3034 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/embedding_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1999 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/index_searcher_client.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.736719 debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/
+-rw-r--r--   0 lilache    (501) staff       (20)      478 2023-06-05 13:38:02.000000 debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
+-rw-r--r--   0 lilache    (501) staff       (20)    39919 2023-06-14 14:50:25.000000 debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/KpsResult.py
+-rw-r--r--   0 lilache    (501) staff       (20)    12349 2023-06-12 11:19:07.000000 debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/docx_generator.py
+-rw-r--r--   0 lilache    (501) staff       (20)    16293 2023-06-11 10:50:55.000000 debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/graph_generator.py
+-rw-r--r--   0 lilache    (501) staff       (20)     4329 2023-06-14 07:55:39.000000 debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/utils.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6969 2023-06-05 13:38:02.000000 debater_python_api-5.0.4/debater_python_api/api/clients/keypoints_admin_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)    38464 2023-06-14 13:42:24.000000 debater_python_api-5.0.4/debater_python_api/api/clients/keypoints_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1894 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/keypoints_pairs_infer_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)    13830 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/narrative_generation_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1230 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/pro_con_client.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.736981 debater_python_api-5.0.4/debater_python_api/api/clients/response_data/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/response_data/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1597 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/response_data/speech_response.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1790 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/term_relater_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1563 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/term_wikifier_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3394 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/clients/theme_extraction_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3263 2023-06-05 13:38:02.000000 debater_python_api-5.0.4/debater_python_api/api/debater_api.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.737143 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.739377 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      142 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
+-rw-r--r--   0 lilache    (501) staff       (20)     5079 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/elastic_client.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1001 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1314 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
+-rw-r--r--   0 lilache    (501) staff       (20)     3576 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1516 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.744070 debater_python_api-5.0.4/debater_python_api/examples/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      803 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/argument_quality_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      854 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/claim_boundaries_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1002 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/claim_detection_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      932 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/clustering_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      860 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/embedding_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1014 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/evidence_detection_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)    85859 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/example_of_sc_args.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1480 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/index_searcher_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1204 2023-06-05 13:38:02.000000 debater_python_api-5.0.4/debater_python_api/examples/keypoints_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1428 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/pro_con_example.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.744798 debater_python_api-5.0.4/debater_python_api/examples/resources/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/resources/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)    23817 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/resources/arguments.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.745027 debater_python_api-5.0.4/debater_python_api/examples/resources/filters_output/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/resources/filters_output/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)     2530 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/resources/pro_con_scores.py
+-rw-r--r--   0 lilache    (501) staff       (20)     9581 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/run_all_services.py
+-rw-r--r--   0 lilache    (501) staff       (20)      870 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/speech_construction_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      480 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/term_relater_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)      907 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/term_wikifier_example.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1154 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/theme_extraction_example.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.745755 debater_python_api-5.0.4/debater_python_api/examples/usecases/
+-rw-r--r--   0 lilache    (501) staff       (20)     4943 2023-06-12 07:54:01.000000 debater_python_api-5.0.4/debater_python_api/examples/usecases/kp_based_survey.py
+-rw-r--r--   0 lilache    (501) staff       (20)     6036 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/usecases/mining_to_narrative.py
+-rw-r--r--   0 lilache    (501) staff       (20)    10191 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/examples/usecases/survey.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.746016 debater_python_api-5.0.4/debater_python_api/integration_tests/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/integration_tests/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.746260 debater_python_api-5.0.4/debater_python_api/integration_tests/api/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/integration_tests/api/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.747533 debater_python_api-5.0.4/debater_python_api/integration_tests/api/clients/
+-rw-r--r--   0 lilache    (501) staff       (20)     2708 2023-05-22 15:52:47.000000 debater_python_api-5.0.4/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
+-rw-r--r--   0 lilache    (501) staff       (20)    11791 2023-06-05 13:38:02.000000 debater_python_api-5.0.4/debater_python_api/integration_tests/api/clients/ServicesIT.py
+-rw-r--r--   0 lilache    (501) staff       (20)     4630 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/integration_tests/api/clients/ServicesLoad.py
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/integration_tests/api/clients/__init__.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.748391 debater_python_api-5.0.4/debater_python_api/utils/
+-rw-r--r--   0 lilache    (501) staff       (20)        0 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/utils/__init__.py
+-rw-r--r--   0 lilache    (501) staff       (20)      992 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/utils/clusters_refiner.py
+-rw-r--r--   0 lilache    (501) staff       (20)     1574 2022-12-12 10:25:59.000000 debater_python_api-5.0.4/debater_python_api/utils/general_utils.py
+-rw-r--r--   0 lilache    (501) staff       (20)      604 2023-05-22 16:30:58.000000 debater_python_api-5.0.4/debater_python_api/utils/kp_analysis_conf.py
+drwxr-xr-x   0 lilache    (501) staff       (20)        0 2023-06-14 16:41:14.731048 debater_python_api-5.0.4/debater_python_api.egg-info/
+-rw-r--r--   0 lilache    (501) staff       (20)    13508 2023-06-14 16:41:14.000000 debater_python_api-5.0.4/debater_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 lilache    (501) staff       (20)     4041 2023-06-14 16:41:14.000000 debater_python_api-5.0.4/debater_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lilache    (501) staff       (20)        1 2023-06-14 16:41:14.000000 debater_python_api-5.0.4/debater_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lilache    (501) staff       (20)       96 2023-06-14 16:41:14.000000 debater_python_api-5.0.4/debater_python_api.egg-info/requires.txt
+-rw-r--r--   0 lilache    (501) staff       (20)       19 2023-06-14 16:41:14.000000 debater_python_api-5.0.4/debater_python_api.egg-info/top_level.txt
+-rw-r--r--   0 lilache    (501) staff       (20)      895 2023-06-14 16:38:55.000000 debater_python_api-5.0.4/pyproject.toml
+-rw-r--r--   0 lilache    (501) staff       (20)       38 2023-06-14 16:41:14.749122 debater_python_api-5.0.4/setup.cfg
```

### Comparing `debater_python_api-5.0.3/LICENSE` & `debater_python_api-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/PKG-INFO` & `debater_python_api-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater_python_api
-Version: 5.0.3
+Version: 5.0.4
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/abstract_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/abstract_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/argument_quality_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/argument_quality_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/claim_and_evidence_detection_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/claim_and_evidence_detection_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/claim_boundaries_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/claim_boundaries_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/clustering_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/clustering_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/embedding_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/embedding_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/index_searcher_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/index_searcher_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/KpsResult.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/KpsResult.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional, Dict, List
 
 import pandas as pd
 import numpy as np
 
 from debater_python_api.api.clients.key_point_summarization.KpsExceptions import KpsIllegalInputException
 from debater_python_api.api.clients.key_point_summarization.utils import read_dicts_from_df, create_dict_to_list, \
-    write_df_to_file, get_unique_sent_id, filter_dict_by_keys
+    write_df_to_file, get_unique_sent_id, filter_dict_by_keys, update_row_with_stance_data
 from debater_python_api.api.clients.key_point_summarization.docx_generator import save_hierarchical_graph_data_to_docx
 from debater_python_api.api.clients.key_point_summarization.graph_generator import create_graph_data, graph_data_to_hierarchical_graph_data, \
     get_hierarchical_graph_from_tree_and_subset_results, get_hierarchical_kps_data
 import os
 CURR_RESULTS_VERSION = "2.0"
 
 
@@ -33,14 +33,38 @@
         self.result_df = self._create_result_df()
         self.version = CURR_RESULTS_VERSION
         self.stances = set(result_json["job_metadata"]["per_stance"].keys()).difference({"no-stance"})
         self.filter_min_relations = filter_min_relations
         self.kp_id_to_hierarchical_data = self._get_kp_id_to_hierarchical_data()
         self.summary_df = self._result_df_to_summary_df()
 
+    def get_unmapped_sentences_df(self):
+        """
+        return a df with all the sentences not matched during the job (either filtered for length/stance or no matching key point was found).
+        """
+        unmatched_sentences = self.result_json['unmatched_sentences']
+        sentences_data = self.result_json['sentences_data']
+        data_cols = ['span_start', 'span_end', 'num_tokens', 'argument_quality','sentence_text','stance']
+        rows = []
+
+        for s in unmatched_sentences:
+            comment_id = str(s["comment_id"])
+            sent_id_in_comment = str(s["sentence_id"])
+            comment_data = sentences_data[comment_id]
+            sent_data = comment_data["sentences"][sent_id_in_comment]
+            sent_row = [comment_id, sent_id_in_comment, comment_data["sents_in_comment"]] + [sent_data[c] for c in data_cols]
+            rows.append(sent_row)
+
+        cols = ['comment_id', 'sentence_id', "sents_in_comment"] + data_cols
+
+        unmatched_df = pd.DataFrame(rows, columns=cols)
+        unmatched_df = unmatched_df.rename(columns={"stance":"stance_dict"})
+        unmatched_df = unmatched_df.apply(lambda r: update_row_with_stance_data(r), axis=1)
+        return unmatched_df
+
     def get_domain(self):
         return self.result_json["job_metadata"]["general"]["domain"]
 
     def get_stance_to_job_id(self):
         """
         Return a dictionary with the mapping from each stance to its job id
         """
@@ -119,17 +143,16 @@
 
         kp_to_id = {self.kp_id_to_hierarchical_data[id]["kp"]:id for id in self.kp_id_to_hierarchical_data }
         dicts, _ = read_dicts_from_df(self.result_df)
         dicts = list(filter(lambda d: d["kp"]!= "none", dicts))
 
         kp_to_dicts = create_dict_to_list([(d['kp'], d) for d in dicts])
 
-        general_metadata = self.result_json["job_metadata"]["general"]
-        n_total_sentences = general_metadata["n_sentences"]
-        n_total_comments = general_metadata["n_comments"]
+        n_total_sentences = self._get_number_of_unique_sentences()
+        n_total_comments = self._get_number_of_unique_comments()
 
         summary_rows = []
         summary_cols = ["key_point", '#comments', 'comments_coverage', "#sentences", 'sentences_coverage', "stance","kp_id","parent_id", "n_comments_subtree"]
 
         for kp, kp_dicts in kp_to_dicts.items():
 
             n_sentences = len(kp_dicts)
@@ -436,15 +459,16 @@
             if add_change:
                 change_percent = title_to_precent[titles[1]] - title_to_precent[titles[0]]
                 row.append(f'{change_percent:.2f}%')
                 if i == 0:
                     total_row.append("")
 
             rows.append(row)
-        rows.append(total_row)
+        if len(rows) > 0:
+            rows.append(total_row)
         comparison_df = pd.DataFrame(rows, columns=cols)
 
         if len(set(kp_to_stance.values()).difference({"no-stance", None})) == 0:
             comparison_df = comparison_df[[c for c in comparison_df.columns if c != "stance"]]
         return comparison_df
 
     def compare_with_comment_subsets(self, comments_subsets_dict:Dict[str, List[str]], include_full:Optional[bool] = True):
@@ -513,80 +537,103 @@
         none_matchings = []
         for result in [pro_result, con_result]:
             for keypoint_matching in result.result_json["keypoint_matchings"]:
                 if keypoint_matching["keypoint"] == "none":
                     none_matchings.extend(keypoint_matching["matching"])
                 else:
                     keypoint_matchings.append(keypoint_matching)
-        keypoint_matchings.append({'keypoint':'none', 'matching':none_matchings})
+
+        if len(none_matchings) > 0: # if there were non keypoints in original results, for backwards compatibility
+            keypoint_matchings.append({'keypoint':'none', 'matching':none_matchings})
         keypoint_matchings.sort(key=lambda matchings: len(matchings['matching']), reverse=True)
 
         sentences_data = pro_result.result_json['sentences_data']
         for comment_id, comment_data_dict in con_result.result_json["sentences_data"].items():
             if comment_id not in sentences_data:
                  sentences_data[comment_id] = {"sents_in_comment":comment_data_dict["sents_in_comment"], "sentences":{}}
             for sent_id_in_comment, sent_data in comment_data_dict["sentences"].items():
                  sentences_data[comment_id]["sentences"][sent_id_in_comment] = sent_data
 
+        pro_unmatched_sents = set([tuple(d.items()) for d in pro_result.result_json["unmatched_sentences"]])
+        con_unmatched_sents = set([tuple(d.items()) for d in con_result.result_json["unmatched_sentences"]])
+        unmatched_sents = pro_unmatched_sents.intersection(con_unmatched_sents)
+        unmatched_sents = [dict(s_data) for s_data in unmatched_sents]
+
         pro_metadata = pro_result.result_json["job_metadata"]
         con_metadata = con_result.result_json["job_metadata"]
         new_metadata = {"general":pro_metadata["general"],
                         "per_stance":{"pro":pro_metadata["per_stance"]["pro"], "con":con_metadata["per_stance"]["con"]}}
         combined_results_json = {'keypoint_matchings':keypoint_matchings, "sentences_data":sentences_data,
                                  "version":CURR_RESULTS_VERSION,
-                                 "job_metadata":new_metadata}
+                                 "job_metadata":new_metadata, "unmatched_sentences":unmatched_sents}
         filter_min_relations = np.min([pro_result.filter_min_relations, con_result.filter_min_relations])
         return KpsResult.create_from_result_json(combined_results_json, filter_min_relations=filter_min_relations)
 
     @staticmethod
     # If result_json is of the old server version, convert to version 2.0
     # 1.0 - received from the server, must have only one stance (merging pro_con is only on v2)
     def _convert_v1_to_v2(result_json):
         metadata = result_json["job_metadata"]
         kps_stance = KpsResult._get_stance_from_server_stances(metadata["stances"])
         sentences_data = {}
+
+        unmapped_sentences = result_json.get("unused_sentences", []) # for server backward compatibility
+        unmapped_sentences_ids = []
+        for s in unmapped_sentences:
+            KpsResult._add_sentence_to_sentences_data(s, sentences_data)
+            unmapped_sentences_ids.append({"comment_id":s["comment_id"], "sentence_id":str(s["sentence_id"])})
+
         new_matchings = []
         for keypoint_matching in result_json['keypoint_matchings']:
             kp = keypoint_matching['keypoint']
 
             new_kp_matching = {'keypoint': kp, "matching": []}
             if kps_stance != "no-stance":
                 new_kp_matching["stance"] = kps_stance
 
             for match in keypoint_matching['matching']:
+
+                if kp == "none":
+                    unmapped_sentences_ids.append({"comment_id": match["comment_id"], "sentence_id": str(match["sentence_id"])})
+
                 if "kp_quality" not in new_kp_matching:
                     kpq = match.get("kp_quality", 0)
                     new_kp_matching["kp_quality"] = kpq
 
-                comment_id = match["comment_id"]
-                sent_id_in_comment = str(match["sentence_id"])
+                KpsResult._add_sentence_to_sentences_data(match, sentences_data)
 
                 new_kp_matching["matching"].append(
-                    {"comment_id": comment_id, "sentence_id": str(sent_id_in_comment), "score": match["score"]})
-                if comment_id not in sentences_data:
-                    sentences_data[comment_id] = {"sents_in_comment": match["sents_in_comment"], "sentences": {}}
-
-                if sent_id_in_comment not in sentences_data[comment_id]["sentences"]:
-                    sent_data = {c: match[c] for c in
-                                 ["sentence_text", "span_start", "span_end", "num_tokens", "argument_quality","kp_quality"]}
-                    if "stance" in match:
-                        sent_data["stance"] = dict(match["stance"])
-                    sentences_data[comment_id]["sentences"][sent_id_in_comment] = sent_data.copy()
+                    {"comment_id": match["comment_id"], "sentence_id": str(match["sentence_id"]), "score": match["score"]})
 
-            new_matchings.append(new_kp_matching)
+            if kp != 'none':
+                new_matchings.append(new_kp_matching)
 
         per_stance_dict = {kps_stance: filter_dict_by_keys(metadata, ['description', 'run_params', 'job_id',
                                                                       'n_sentences_stance', 'n_comments_stance'])}
 
         metadata_v2 = {"general": filter_dict_by_keys(metadata, ['domain', 'user_id', 'n_sentences',
                                                                  'n_sentences_unfiltered', 'n_comments',
                                                                  'n_comments_unfiltered']),
                        "per_stance": per_stance_dict}
         return {"keypoint_matchings": new_matchings, "sentences_data": sentences_data, "version": CURR_RESULTS_VERSION,
-                "job_metadata": metadata_v2}
+                "job_metadata": metadata_v2, "unmatched_sentences":unmapped_sentences_ids}
+
+    @staticmethod
+    def _add_sentence_to_sentences_data(match, sentences_data):
+        comment_id = match["comment_id"]
+        sent_id_in_comment = str(match["sentence_id"])
+        if comment_id not in sentences_data:
+            sentences_data[comment_id] = {"sents_in_comment": match["sents_in_comment"], "sentences": {}}
+
+        if sent_id_in_comment not in sentences_data[comment_id]["sentences"]:
+            sent_data = {c: match.get(c) for c in
+                         ["sentence_text", "span_start", "span_end", "num_tokens", "argument_quality", "kp_quality"]}
+            if "stance" in match:
+                sent_data["stance"] = dict(match["stance"])
+            sentences_data[comment_id]["sentences"][sent_id_in_comment] = sent_data.copy()
 
     def _get_number_of_unique_comments(self, include_unmatched=True):
         if include_unmatched:
             return self.result_json["job_metadata"]["general"]["n_comments"]
         else:
             total_comments = set()
             for i, keypoint_matching in enumerate(self.result_json['keypoint_matchings']):
@@ -631,16 +678,16 @@
 
     def get_result_with_top_kp_per_sentence(self):
         """
         Return the same KpsResult with up to one matching key point per sentence (the key point with the highest matching score).
         No hierarchy is generated in this setting.
         :return: new KpsResult after choosing the top kp for each sentence.
         """
-        new_results_df = self.result_df.sort_values(by=["sentence_text","match_score"], ascending=[True, False])
-        top_preds_df = pd.concat([group.head(1) for _,group in new_results_df.groupby(by="sentence_text")])
+        new_results_df = self.result_df.sort_values(by=["match_score"], ascending=[False])
+        top_preds_df = pd.concat([group.head(1) for _,group in new_results_df.groupby(by=["comment_id","sentence_id"])])
 
         kp_to_args = list(zip(top_preds_df["kp"],zip(top_preds_df["comment_id"], top_preds_df["sentence_id"])))
         kp_to_args = create_dict_to_list(kp_to_args)
         new_meta_data = self.result_json["job_metadata"].copy()
         new_meta_data["general"]["top_kp_per_sent"] = True
 
         new_keypoint_matchings = []
@@ -650,15 +697,16 @@
             if kp != "none":
                 new_keypoint_matching["matching"] = list(filter(lambda x: (x["comment_id"],int(x["sentence_id"])) in kp_to_args[kp], new_keypoint_matching["matching"]))
             if len(new_keypoint_matching["matching"]) > 0:
                 new_keypoint_matchings.append(new_keypoint_matching)
         new_keypoint_matchings.sort(key=lambda x: len(x["matching"]), reverse=True)
 
         new_json = {"sentences_data": self.result_json["sentences_data"].copy(), "version": self.result_json["version"],
-                    "job_metadata":new_meta_data, "keypoint_matchings":new_keypoint_matchings}
+                    "job_metadata":new_meta_data, "keypoint_matchings":new_keypoint_matchings,
+                    "unmatched_sentences": self.result_json["unmatched_sentences"]}
 
         return KpsResult.create_from_result_json(new_json)
 
     def get_stance_str(self):
         if len(self.stances) == 0:
             return "no-stance"
         elif len(self.stances) == 1:
```

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/docx_generator.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/docx_generator.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/graph_generator.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/graph_generator.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/key_point_summarization/utils.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/key_point_summarization/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,20 +62,21 @@
     if not os.path.exists(file_path.parent):
         logging.info('creating directory: %s' % str(file_path.parent))
         os.makedirs(file_path.parent)
     df.to_csv(file, index=False)
 
 
 def update_row_with_stance_data(r):
-    stance_dict = dict(r["stance_dict"])
-    stance_list = list(stance_dict.items())
-    stance_list = sorted(stance_list, reverse=True, key=lambda item: item[1])
-    stance, conf = stance_list[0]
-    r["stance"] = stance
-    r["stance_conf"] = conf
+    if "stance_dict" in r and len(r["stance_dict"]) > 0:
+        stance_dict = dict(r["stance_dict"])
+        stance_list = list(stance_dict.items())
+        stance_list = sorted(stance_list, reverse=True, key=lambda item: item[1])
+        stance, conf = stance_list[0]
+        r["selected_stance"] = stance
+        r["stance_conf"] = conf
     return r
 
 
 def get_unique_sent_id(sentence_dict):
     return f"{sentence_dict['comment_id']}_{sentence_dict['sentence_id']}"
```

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_admin_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/keypoints_admin_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/keypoints_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/keypoints_pairs_infer_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/keypoints_pairs_infer_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/narrative_generation_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/narrative_generation_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/pro_con_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/pro_con_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/response_data/speech_response.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/response_data/speech_response.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/term_relater_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/term_relater_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/term_wikifier_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/term_wikifier_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/clients/theme_extraction_client.py` & `debater_python_api-5.0.4/debater_python_api/api/clients/theme_extraction_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/debater_api.py` & `debater_python_api-5.0.4/debater_python_api/api/debater_api.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_client.py` & `debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/elastic_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py` & `debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py` & `debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/sentence_query_base.py` & `debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/sentence_query_base.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/api/sentence_level_index/client/sentence_query_request.py` & `debater_python_api-5.0.4/debater_python_api/api/sentence_level_index/client/sentence_query_request.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/argument_quality_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/argument_quality_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/claim_boundaries_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/claim_boundaries_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/claim_detection_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/claim_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/clustering_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/clustering_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/embedding_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/embedding_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/evidence_detection_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/evidence_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/example_of_sc_args.py` & `debater_python_api-5.0.4/debater_python_api/examples/example_of_sc_args.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/index_searcher_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/index_searcher_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/keypoints_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/keypoints_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/pro_con_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/pro_con_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/resources/arguments.py` & `debater_python_api-5.0.4/debater_python_api/examples/resources/arguments.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/resources/pro_con_scores.py` & `debater_python_api-5.0.4/debater_python_api/examples/resources/pro_con_scores.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/run_all_services.py` & `debater_python_api-5.0.4/debater_python_api/examples/run_all_services.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/speech_construction_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/speech_construction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/term_wikifier_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/term_wikifier_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/theme_extraction_example.py` & `debater_python_api-5.0.4/debater_python_api/examples/theme_extraction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/usecases/kp_based_survey.py` & `debater_python_api-5.0.4/debater_python_api/examples/usecases/kp_based_survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/usecases/mining_to_narrative.py` & `debater_python_api-5.0.4/debater_python_api/examples/usecases/mining_to_narrative.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/examples/usecases/survey.py` & `debater_python_api-5.0.4/debater_python_api/examples/usecases/survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py` & `debater_python_api-5.0.4/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/ServicesIT.py` & `debater_python_api-5.0.4/debater_python_api/integration_tests/api/clients/ServicesIT.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/integration_tests/api/clients/ServicesLoad.py` & `debater_python_api-5.0.4/debater_python_api/integration_tests/api/clients/ServicesLoad.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/utils/clusters_refiner.py` & `debater_python_api-5.0.4/debater_python_api/utils/clusters_refiner.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/utils/general_utils.py` & `debater_python_api-5.0.4/debater_python_api/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api/utils/kp_analysis_conf.py` & `debater_python_api-5.0.4/debater_python_api/utils/kp_analysis_conf.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/debater_python_api.egg-info/PKG-INFO` & `debater_python_api-5.0.4/debater_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater-python-api
-Version: 5.0.3
+Version: 5.0.4
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-5.0.3/debater_python_api.egg-info/SOURCES.txt` & `debater_python_api-5.0.4/debater_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debater_python_api-5.0.3/pyproject.toml` & `debater_python_api-5.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debater_python_api"
-version = "5.0.3"
+version = "5.0.4"
 description = "Project Debater Early Access Program API sdk for python"
 readme = "README.md"
 authors = [{ name = "Elad Venezian", email = "eladv@il.ibm.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

