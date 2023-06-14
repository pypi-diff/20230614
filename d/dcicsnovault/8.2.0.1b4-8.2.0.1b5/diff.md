# Comparing `tmp/dcicsnovault-8.2.0.1b4.tar.gz` & `tmp/dcicsnovault-8.2.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.2.0.1b4.tar", max compression
+gzip compressed data, was "dcicsnovault-8.2.0.1b5.tar", max compression
```

## Comparing `dcicsnovault-8.2.0.1b4.tar` & `dcicsnovault-8.2.0.1b5.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0     1135 2023-06-01 18:38:04.101679 dcicsnovault-8.2.0.1b4/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-06-01 18:38:04.101679 dcicsnovault-8.2.0.1b4/README.rst
--rw-r--r--   0        0        0     5609 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/pyproject.toml
--rw-r--r--   0        0        0     4907 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/aggregated_items.py
--rw-r--r--   0        0        0     9389 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/app.py
--rw-r--r--   0        0        0      358 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/appdefs.py
--rw-r--r--   0        0        0    11879 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/attachment.py
--rw-r--r--   0        0        0    26351 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/authentication.py
--rw-r--r--   0        0        0     4692 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6876 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     5839 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/list_db_tables.py
--rw-r--r--   0        0        0     6212 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2402 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     5155 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/prepare_template.py
--rw-r--r--   0        0        0     4350 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/custom_embed.py
--rw-r--r--   0        0        0     7282 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0    11599 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/indexing_views.py
--rw-r--r--   0        0        0     6889 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/ingestion/common.py
--rw-r--r--   0        0        0     1294 2023-06-01 18:38:04.109679 dcicsnovault-8.2.0.1b4/snovault/ingestion/exceptions.py
--rw-r--r--   0        0        0    26153 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_listener.py
--rw-r--r--   0        0        0      586 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_listener_base.py
--rw-r--r--   0        0        0      692 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_message.py
--rw-r--r--   0        0        0    12257 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_message_handler_decorator.py
--rw-r--r--   0        0        0     3760 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_message_handler_default.py
--rw-r--r--   0        0        0     1107 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_processor_decorator.py
--rw-r--r--   0        0        0      863 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_processors.py
--rw-r--r--   0        0        0     8586 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/ingestion/queue_utils.py
--rw-r--r--   0        0        0      774 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/jsonld_context.py
--rw-r--r--   0        0        0    32979 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/loadxl.py
--rw-r--r--   0        0        0     2425 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/memlimit.py
--rw-r--r--   0        0        0      895 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/nginx-dev.conf
--rw-r--r--   0        0        0     1165 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/parallel.py
--rw-r--r--   0        0        0      846 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/predicates.py
--rw-r--r--   0        0        0     1520 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/project/authentication.py
--rw-r--r--   0        0        0      378 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/project/authorization.py
--rw-r--r--   0        0        0      289 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/project/ingestion.py
--rw-r--r--   0        0        0      228 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/project/loadxl.py
--rw-r--r--   0        0        0      107 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/project_app.py
--rw-r--r--   0        0        0      575 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/project_defs.py
--rw-r--r--   0        0        0       95 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22128 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/resource_views.py
--rw-r--r--   0        0        0    26122 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/resources.py
--rw-r--r--   0        0        0     9867 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/root.py
--rw-r--r--   0        0        0      986 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schema_formats.py
--rw-r--r--   0        0        0     3450 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schema_graph.py
--rw-r--r--   0        0        0    18330 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0     5407 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schemas/ingestion_submission.json
--rw-r--r--   0        0        0    18744 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/search/search.py
--rw-r--r--   0        0        0    17915 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/search/search_utils.py
--rw-r--r--   0        0        0     4442 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/server_defaults.py
--rw-r--r--   0        0        0      522 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/settings.py
--rw-r--r--   0        0        0     1769 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/sqlalchemy_tools.py
--rw-r--r--   0        0        0     1498 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-06-01 18:38:04.113679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2191 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0        0 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/data/inserts/README.rst
--rw-r--r--   0        0        0        0 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/data/master-inserts/README.rst
--rw-r--r--   0        0        0     3086 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3186 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0     8173 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_ingestion_message_handler_decorator.py
--rw-r--r--   0        0        0      384 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_ingestion_processor.py
--rw-r--r--   0        0        0    28258 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     6782 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_types_access_key.py
--rw-r--r--   0        0        0     1291 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_util.py
--rw-r--r--   0        0        0    19246 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4620 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/types/__init__.py
--rw-r--r--   0        0        0     5101 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/types/access_key.py
--rw-r--r--   0        0        0     8979 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/types/filter_set.py
--rw-r--r--   0        0        0    11559 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/types/ingestion.py
--rw-r--r--   0        0        0     5583 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/upgrader.py
--rw-r--r--   0        0        0    63565 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-06-01 18:38:04.117679 dcicsnovault-8.2.0.1b4/snovault/validators.py
--rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 dcicsnovault-8.2.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-06-01 19:10:13.202015 dcicsnovault-8.2.0.1b5/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-06-01 19:10:13.202015 dcicsnovault-8.2.0.1b5/README.rst
+-rw-r--r--   0        0        0     5609 2023-06-01 19:10:13.206015 dcicsnovault-8.2.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     4907 2023-06-01 19:10:13.206015 dcicsnovault-8.2.0.1b5/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     9389 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/app.py
+-rw-r--r--   0        0        0      358 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/appdefs.py
+-rw-r--r--   0        0        0    11879 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/attachment.py
+-rw-r--r--   0        0        0    26351 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/authentication.py
+-rw-r--r--   0        0        0     4692 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6876 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     5839 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/list_db_tables.py
+-rw-r--r--   0        0        0     6212 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2402 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     5155 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/prepare_template.py
+-rw-r--r--   0        0        0     4350 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7282 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0    11599 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/indexing_views.py
+-rw-r--r--   0        0        0     6889 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/common.py
+-rw-r--r--   0        0        0     1294 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/exceptions.py
+-rw-r--r--   0        0        0    26153 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_listener.py
+-rw-r--r--   0        0        0      586 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_listener_base.py
+-rw-r--r--   0        0        0      692 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message.py
+-rw-r--r--   0        0        0    12257 2023-06-01 19:10:13.210015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message_handler_decorator.py
+-rw-r--r--   0        0        0     3760 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message_handler_default.py
+-rw-r--r--   0        0        0     1107 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_processor_decorator.py
+-rw-r--r--   0        0        0      863 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_processors.py
+-rw-r--r--   0        0        0     8586 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/ingestion/queue_utils.py
+-rw-r--r--   0        0        0      774 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    32979 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/loadxl.py
+-rw-r--r--   0        0        0     2425 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/memlimit.py
+-rw-r--r--   0        0        0      895 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/nginx-dev.conf
+-rw-r--r--   0        0        0     1165 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/predicates.py
+-rw-r--r--   0        0        0     1520 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project/authentication.py
+-rw-r--r--   0        0        0      378 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project/authorization.py
+-rw-r--r--   0        0        0      289 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project/ingestion.py
+-rw-r--r--   0        0        0      228 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project/loadxl.py
+-rw-r--r--   0        0        0      107 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project_app.py
+-rw-r--r--   0        0        0      575 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/project_defs.py
+-rw-r--r--   0        0        0       95 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22128 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/resource_views.py
+-rw-r--r--   0        0        0    26122 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/resources.py
+-rw-r--r--   0        0        0     9867 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/root.py
+-rw-r--r--   0        0        0      986 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schema_formats.py
+-rw-r--r--   0        0        0     3450 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schema_graph.py
+-rw-r--r--   0        0        0    18330 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4358 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schema_views.py
+-rw-r--r--   0        0        0     1855 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5098 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0     5407 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/ingestion_submission.json
+-rw-r--r--   0        0        0    18744 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19600 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/search/search.py
+-rw-r--r--   0        0        0    17915 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     4442 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/server_defaults.py
+-rw-r--r--   0        0        0      522 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/settings.py
+-rw-r--r--   0        0        0     1769 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/sqlalchemy_tools.py
+-rw-r--r--   0        0        0     1498 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-06-01 19:10:13.214015 dcicsnovault-8.2.0.1b5/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      697 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2191 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/data/inserts/README.rst
+-rw-r--r--   0        0        0        0 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/data/master-inserts/README.rst
+-rw-r--r--   0        0        0     3086 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3186 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0     8173 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_ingestion_message_handler_decorator.py
+-rw-r--r--   0        0        0      384 2023-06-01 19:10:13.218015 dcicsnovault-8.2.0.1b5/snovault/tests/test_ingestion_processor.py
+-rw-r--r--   0        0        0    28258 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     6782 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_types_access_key.py
+-rw-r--r--   0        0        0     1291 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    19246 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4620 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34107 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5101 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/access_key.py
+-rw-r--r--   0        0        0     8961 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/filter_set.py
+-rw-r--r--   0        0        0    11559 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/ingestion.py
+-rw-r--r--   0        0        0     5583 2023-06-01 19:10:13.222015 dcicsnovault-8.2.0.1b5/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-06-01 19:10:13.226015 dcicsnovault-8.2.0.1b5/snovault/upgrader.py
+-rw-r--r--   0        0        0    63565 2023-06-01 19:10:13.226015 dcicsnovault-8.2.0.1b5/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-06-01 19:10:13.226015 dcicsnovault-8.2.0.1b5/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-06-01 19:10:13.226015 dcicsnovault-8.2.0.1b5/snovault/validators.py
+-rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 dcicsnovault-8.2.0.1b5/PKG-INFO
```

### Comparing `dcicsnovault-8.2.0.1b4/LICENSE.txt` & `dcicsnovault-8.2.0.1b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/README.rst` & `dcicsnovault-8.2.0.1b5/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/pyproject.toml` & `dcicsnovault-8.2.0.1b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.2.0.1b4"  # to become 8.2.0
+version = "8.2.0.1b5"  # to become 8.2.0
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
```

### Comparing `dcicsnovault-8.2.0.1b4/snovault/__init__.py` & `dcicsnovault-8.2.0.1b5/snovault/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/aggregated_items.py` & `dcicsnovault-8.2.0.1b5/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/app.py` & `dcicsnovault-8.2.0.1b5/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/attachment.py` & `dcicsnovault-8.2.0.1b5/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/authentication.py` & `dcicsnovault-8.2.0.1b5/snovault/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/authorization.py` & `dcicsnovault-8.2.0.1b5/snovault/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/batchupgrade.py` & `dcicsnovault-8.2.0.1b5/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/cache.py` & `dcicsnovault-8.2.0.1b5/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/calculated.py` & `dcicsnovault-8.2.0.1b5/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/check_rendering.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/clear_db_es_contents.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/create_mapping_on_deploy.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/create_mapping_on_deploy.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/es_index_data.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/list_db_tables.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/list_db_tables.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/load_access_keys.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/load_access_keys.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/load_data.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/load_data_by_type.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/load_data_by_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/prepare_template.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/prepare_template.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/profile.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/purge_item_type.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/purge_item_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/run_upgrader_on_inserts.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/run_upgrader_on_inserts.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/update_inserts_from_server.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/update_inserts_from_server.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.2.0.1b5/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/config.py` & `dcicsnovault-8.2.0.1b5/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/connection.py` & `dcicsnovault-8.2.0.1b5/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/crud_views.py` & `dcicsnovault-8.2.0.1b5/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/custom_embed.py` & `dcicsnovault-8.2.0.1b5/snovault/custom_embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/dev_servers.py` & `dcicsnovault-8.2.0.1b5/snovault/dev_servers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/drs.py` & `dcicsnovault-8.2.0.1b5/snovault/drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/edw_hash.py` & `dcicsnovault-8.2.0.1b5/snovault/edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.2.0.1b5/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/embed.py` & `dcicsnovault-8.2.0.1b5/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/etag.py` & `dcicsnovault-8.2.0.1b5/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/indexing_views.py` & `dcicsnovault-8.2.0.1b5/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/common.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/common.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/exceptions.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_listener.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_listener_base.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_listener_base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_message.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_message_handler_decorator.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message_handler_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_message_handler_default.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_message_handler_default.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_processor_decorator.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_processor_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/ingestion_processors.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/ingestion_processors.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/ingestion/queue_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/ingestion/queue_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/interfaces.py` & `dcicsnovault-8.2.0.1b5/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/invalidation.py` & `dcicsnovault-8.2.0.1b5/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/json_renderer.py` & `dcicsnovault-8.2.0.1b5/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/jsongraph.py` & `dcicsnovault-8.2.0.1b5/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/jsonld_context.py` & `dcicsnovault-8.2.0.1b5/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/loadxl.py` & `dcicsnovault-8.2.0.1b5/snovault/loadxl.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/memlimit.py` & `dcicsnovault-8.2.0.1b5/snovault/memlimit.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/nginx-dev.conf` & `dcicsnovault-8.2.0.1b5/snovault/nginx-dev.conf`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/parallel.py` & `dcicsnovault-8.2.0.1b5/snovault/parallel.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/predicates.py` & `dcicsnovault-8.2.0.1b5/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/project/authentication.py` & `dcicsnovault-8.2.0.1b5/snovault/project/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/project_defs.py` & `dcicsnovault-8.2.0.1b5/snovault/project_defs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/redis/redis_connection.py` & `dcicsnovault-8.2.0.1b5/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/renderers.py` & `dcicsnovault-8.2.0.1b5/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/resource_views.py` & `dcicsnovault-8.2.0.1b5/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/resources.py` & `dcicsnovault-8.2.0.1b5/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/root.py` & `dcicsnovault-8.2.0.1b5/snovault/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schema_formats.py` & `dcicsnovault-8.2.0.1b5/snovault/schema_formats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schema_graph.py` & `dcicsnovault-8.2.0.1b5/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schema_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schema_views.py` & `dcicsnovault-8.2.0.1b5/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schemas/access_key.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/access_key.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schemas/filter_set.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/filter_set.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schemas/ingestion_submission.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/ingestion_submission.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schemas/mixins.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/schemas/user.json` & `dcicsnovault-8.2.0.1b5/snovault/schemas/user.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/search/compound_search.py` & `dcicsnovault-8.2.0.1b5/snovault/search/compound_search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/search/lucene_builder.py` & `dcicsnovault-8.2.0.1b5/snovault/search/lucene_builder.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/search/search.py` & `dcicsnovault-8.2.0.1b5/snovault/search/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/search/search_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/search/search_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/server_defaults.py` & `dcicsnovault-8.2.0.1b5/snovault/server_defaults.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/settings.py` & `dcicsnovault-8.2.0.1b5/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/sqlalchemy_tools.py` & `dcicsnovault-8.2.0.1b5/snovault/sqlalchemy_tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/standalone_dev.py` & `dcicsnovault-8.2.0.1b5/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/stats.py` & `dcicsnovault-8.2.0.1b5/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/storage.py` & `dcicsnovault-8.2.0.1b5/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/test_schemas/mixins.json` & `dcicsnovault-8.2.0.1b5/snovault/test_schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/conftest.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/root.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/serverfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_attachment.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_authentication.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_calculated.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_clear_db_es_contents.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_drs.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_edw_hash.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_embedding.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_indexing.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_ingestion_message_handler_decorator.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_ingestion_message_handler_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_key.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_link.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_logging.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_misc.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_schemas.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_stats.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_storage.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_types_access_key.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_types_access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_upgrader.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_util.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/test_views.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/testappfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/testing_views.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tests/toolfixtures.py` & `dcicsnovault-8.2.0.1b5/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/tools.py` & `dcicsnovault-8.2.0.1b5/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/typedsheets.py` & `dcicsnovault-8.2.0.1b5/snovault/typedsheets.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/typeinfo.py` & `dcicsnovault-8.2.0.1b5/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/types/access_key.py` & `dcicsnovault-8.2.0.1b5/snovault/types/access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/types/base.py` & `dcicsnovault-8.2.0.1b5/snovault/types/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     validate_item_content_in_place,
     no_validate_item_content_post,
     no_validate_item_content_put,
     no_validate_item_content_patch
 )
 from ..crud_views import (
     collection_add as sno_collection_add,
-    item_edit as sno_item_edit,
+    item_edit
 )
 from ..interfaces import CONNECTION
 from typing import Any, List, Tuple, Union
 from ..server_defaults import get_userid, add_last_modified
 
 
 Acl = List[Tuple[Any, Any, Union[str, List[str]]]]
```

### Comparing `dcicsnovault-8.2.0.1b4/snovault/types/filter_set.py` & `dcicsnovault-8.2.0.1b5/snovault/types/filter_set.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/types/ingestion.py` & `dcicsnovault-8.2.0.1b5/snovault/types/ingestion.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/types/user.py` & `dcicsnovault-8.2.0.1b5/snovault/types/user.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/upgrader.py` & `dcicsnovault-8.2.0.1b5/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/util.py` & `dcicsnovault-8.2.0.1b5/snovault/util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/validation.py` & `dcicsnovault-8.2.0.1b5/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/snovault/validators.py` & `dcicsnovault-8.2.0.1b5/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.2.0.1b4/PKG-INFO` & `dcicsnovault-8.2.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.2.0.1b4
+Version: 8.2.0.1b5
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
```

