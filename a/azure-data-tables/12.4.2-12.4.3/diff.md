# Comparing `tmp/azure-data-tables-12.4.2.zip` & `tmp/azure-data-tables-12.4.3.zip`

## zipinfo {}

```diff
@@ -1,146 +1,147 @@
-Zip file size: 315127 bytes, number of entries: 144
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure_data_tables.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/tests/
--rw-rw-r--  2.0 unx    11073 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/migration_guide.md
--rw-rw-r--  2.0 unx    33029 b- defN 23-Feb-07 21:07 azure-data-tables-12.4.2/PKG-INFO
--rw-rw-r--  2.0 unx     2555 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/setup.py
--rw-rw-r--  2.0 unx       38 b- defN 23-Feb-07 21:07 azure-data-tables-12.4.2/setup.cfg
--rw-rw-r--  2.0 unx     1073 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/LICENSE
--rw-rw-r--  2.0 unx      222 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/MANIFEST.in
--rw-rw-r--  2.0 unx    22810 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/README.md
--rw-rw-r--  2.0 unx     9321 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/CHANGELOG.md
--rw-rw-r--  2.0 unx    33029 b- defN 23-Feb-07 21:07 azure-data-tables-12.4.2/azure_data_tables.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Feb-07 21:07 azure-data-tables-12.4.2/azure_data_tables.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     4657 b- defN 23-Feb-07 21:07 azure-data-tables-12.4.2/azure_data_tables.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Feb-07 21:07 azure-data-tables-12.4.2/azure_data_tables.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx       81 b- defN 23-Feb-07 21:07 azure-data-tables-12.4.2/azure_data_tables.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Feb-07 21:07 azure-data-tables-12.4.2/azure_data_tables.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/data/
--rw-rw-r--  2.0 unx       81 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/data/tables/
--rw-rw-r--  2.0 unx       81 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/data/tables/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/data/tables/_generated/
--rw-rw-r--  2.0 unx    11948 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_shared_access_signature.py
--rw-rw-r--  2.0 unx    29209 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_table_batch.py
--rw-rw-r--  2.0 unx     9600 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_authentication.py
--rw-rw-r--  2.0 unx    30261 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_table_client.py
--rw-rw-r--  2.0 unx     7846 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_deserialize.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/py.typed
--rw-rw-r--  2.0 unx      799 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_constants.py
--rw-rw-r--  2.0 unx     1492 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/__init__.py
--rw-rw-r--  2.0 unx      546 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_sdk_moniker.py
--rw-rw-r--  2.0 unx     2730 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_common_conversion.py
--rw-rw-r--  2.0 unx    28180 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_models.py
--rw-rw-r--  2.0 unx    15181 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_error.py
--rw-rw-r--  2.0 unx    14121 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_table_service_client.py
--rw-rw-r--  2.0 unx      330 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_version.py
--rw-rw-r--  2.0 unx     2571 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_entity.py
--rw-rw-r--  2.0 unx     9297 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_serialize.py
--rw-rw-r--  2.0 unx    17756 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_base_client.py
--rw-rw-r--  2.0 unx    10781 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_policies.py
--rw-rw-r--  2.0 unx    14596 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_table_shared_access_signature.py
--rw-rw-r--  2.0 unx    27390 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/aio/_table_batch_async.py
--rw-rw-r--  2.0 unx     8105 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/aio/_base_client_async.py
--rw-rw-r--  2.0 unx      518 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/aio/__init__.py
--rw-rw-r--  2.0 unx     7408 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/aio/_policies_async.py
--rw-rw-r--  2.0 unx     3518 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/aio/_authentication_async.py
--rw-rw-r--  2.0 unx     4676 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/aio/_models.py
--rw-rw-r--  2.0 unx    30936 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/aio/_table_client_async.py
--rw-rw-r--  2.0 unx    14528 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/aio/_table_service_client_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/data/tables/_generated/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/data/tables/_generated/operations/
--rw-rw-r--  2.0 unx     3763 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/_client.py
--rw-rw-r--  2.0 unx      843 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/_vendor.py
--rw-rw-r--  2.0 unx     2813 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/_configuration.py
--rw-rw-r--  2.0 unx      864 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/__init__.py
--rw-rw-r--  2.0 unx    77872 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/_serialization.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/_patch.py
--rw-rw-r--  2.0 unx      491 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/_version.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/
--rw-rw-r--  2.0 unx     3871 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_client.py
--rw-rw-r--  2.0 unx     2824 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx      811 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx      839 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    79632 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     1814 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/models/__init__.py
--rw-rw-r--  2.0 unx     1272 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/models/_enums.py
--rw-rw-r--  2.0 unx    24470 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/models/_models.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/models/_patch.py
--rw-rw-r--  2.0 unx      839 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx   104301 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/operations/_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/azure/data/tables/_generated/operations/_patch.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/samples/async_samples/
--rw-rw-r--  2.0 unx     4144 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_create_delete_table.py
--rw-rw-r--  2.0 unx     5487 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_query_table.py
--rw-rw-r--  2.0 unx     6721 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_copy_table.py
--rw-rw-r--  2.0 unx     3255 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_query_tables.py
--rw-rw-r--  2.0 unx     3757 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_insert_delete_entities.py
--rw-rw-r--  2.0 unx     5626 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_conditional_update.py
--rw-rw-r--  2.0 unx     4228 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_authentication.py
--rw-rw-r--  2.0 unx     3309 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_batching.py
--rw-rw-r--  2.0 unx     7027 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_update_upsert_merge_entities.py
--rw-rw-r--  2.0 unx     8630 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/README.md
--rw-rw-r--  2.0 unx     2671 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/sample_create_client.py
--rw-rw-r--  2.0 unx     2800 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_create_client_async.py
--rw-rw-r--  2.0 unx     5593 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_query_table_async.py
--rw-rw-r--  2.0 unx     3788 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_batching_async.py
--rw-rw-r--  2.0 unx     5805 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_conditional_update_async.py
--rw-rw-r--  2.0 unx     4374 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_create_delete_table_async.py
--rw-rw-r--  2.0 unx     7200 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_update_upsert_merge_entities_async.py
--rw-rw-r--  2.0 unx     4208 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_authentication_async.py
--rw-rw-r--  2.0 unx     6957 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_copy_table_async.py
--rw-rw-r--  2.0 unx     4222 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_insert_delete_entities_async.py
--rw-rw-r--  2.0 unx     3218 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/samples/async_samples/sample_query_tables_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/tests/_shared/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 21:07 azure-data-tables-12.4.2/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     3097 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/preparers.py
--rw-rw-r--  2.0 unx     2686 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_service_stats_cosmos.py
--rw-rw-r--  2.0 unx     6049 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_retry.py
--rw-rw-r--  2.0 unx     4094 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_service_properties_cosmos_async.py
--rw-rw-r--  2.0 unx    51952 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_batch.py
--rw-rw-r--  2.0 unx    10471 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_cosmos_async.py
--rw-rw-r--  2.0 unx     5617 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_retry_async.py
--rw-rw-r--  2.0 unx    84574 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_entity_cosmos_async.py
--rw-rw-r--  2.0 unx    17523 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_challenge_auth_async.py
--rw-rw-r--  2.0 unx     2649 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_service_stats_async.py
--rw-rw-r--  2.0 unx     3761 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_service_properties_cosmos.py
--rw-rw-r--  2.0 unx     1739 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_service_stats.py
--rw-rw-r--  2.0 unx    13235 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_aad_async.py
--rw-rw-r--  2.0 unx    32717 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_client.py
--rw-rw-r--  2.0 unx    32438 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_client_async.py
--rw-rw-r--  2.0 unx     7939 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_service_properties.py
--rw-rw-r--  2.0 unx    18694 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table.py
--rw-rw-r--  2.0 unx    79522 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_entity_cosmos.py
--rw-rw-r--  2.0 unx    74557 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_encoder.py
--rw-rw-r--  2.0 unx    30706 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_batch_cosmos.py
--rw-rw-r--  2.0 unx    17339 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_async.py
--rw-rw-r--  2.0 unx     8390 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_service_properties_async.py
--rw-rw-r--  2.0 unx     2744 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/conftest.py
--rw-rw-r--  2.0 unx     2202 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/async_preparers.py
--rw-rw-r--  2.0 unx    91566 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_entity_async.py
--rw-rw-r--  2.0 unx     2666 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_service_stats_cosmos_async.py
--rw-rw-r--  2.0 unx    12537 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_aad.py
--rw-rw-r--  2.0 unx    36163 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_batch_cosmos_async.py
--rw-rw-r--  2.0 unx    49989 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_batch_async.py
--rw-rw-r--  2.0 unx     9740 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_cosmos.py
--rw-rw-r--  2.0 unx    17277 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_challenge_auth.py
--rw-rw-r--  2.0 unx    87278 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_entity.py
--rw-rw-r--  2.0 unx    30324 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_client_cosmos_async.py
--rw-rw-r--  2.0 unx    30637 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/test_table_client_cosmos.py
--rw-rw-r--  2.0 unx     4956 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/_shared/asynctestcase.py
--rw-rw-r--  2.0 unx     4871 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/_shared/cosmos_testcase.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/_shared/__init__.py
--rw-rw-r--  2.0 unx    21084 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/_shared/testcase.py
--rw-rw-r--  2.0 unx      879 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/perfstress_tests/create_entity.py
--rw-rw-r--  2.0 unx     1894 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/perfstress_tests/create_entity_batch.py
--rw-rw-r--  2.0 unx     4009 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/perfstress_tests/_base.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     1643 b- defN 23-Feb-07 21:05 azure-data-tables-12.4.2/tests/perfstress_tests/list_entities.py
-144 files, 1758324 bytes uncompressed, 287185 bytes compressed:  83.7%
+Zip file size: 315421 bytes, number of entries: 145
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure_data_tables.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/
+-rw-rw-r--  2.0 unx       59 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/pyproject.toml
+-rw-rw-r--  2.0 unx     2562 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/setup.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/LICENSE
+-rw-rw-r--  2.0 unx    33358 b- defN 23-Jun-13 22:15 azure-data-tables-12.4.3/PKG-INFO
+-rw-rw-r--  2.0 unx    22881 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/README.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jun-13 22:15 azure-data-tables-12.4.3/setup.cfg
+-rw-rw-r--  2.0 unx     9579 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/CHANGELOG.md
+-rw-rw-r--  2.0 unx    11073 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/migration_guide.md
+-rw-rw-r--  2.0 unx      222 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/MANIFEST.in
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/tests/perfstress_tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/tests/_shared/
+-rw-rw-r--  2.0 unx    13235 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_aad_async.py
+-rw-rw-r--  2.0 unx    10471 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_cosmos_async.py
+-rw-rw-r--  2.0 unx    79522 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_entity_cosmos.py
+-rw-rw-r--  2.0 unx     2202 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/async_preparers.py
+-rw-rw-r--  2.0 unx    17277 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_challenge_auth.py
+-rw-rw-r--  2.0 unx    51952 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_batch.py
+-rw-rw-r--  2.0 unx     1739 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_service_stats.py
+-rw-rw-r--  2.0 unx     3761 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_service_properties_cosmos.py
+-rw-rw-r--  2.0 unx     2666 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_service_stats_cosmos_async.py
+-rw-rw-r--  2.0 unx    33487 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_client.py
+-rw-rw-r--  2.0 unx    91566 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_entity_async.py
+-rw-rw-r--  2.0 unx     4094 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_service_properties_cosmos_async.py
+-rw-rw-r--  2.0 unx    30637 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_client_cosmos.py
+-rw-rw-r--  2.0 unx    17339 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_async.py
+-rw-rw-r--  2.0 unx     5617 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_retry_async.py
+-rw-rw-r--  2.0 unx     2686 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_service_stats_cosmos.py
+-rw-rw-r--  2.0 unx    30706 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_batch_cosmos.py
+-rw-rw-r--  2.0 unx     2744 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/conftest.py
+-rw-rw-r--  2.0 unx     2649 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_service_stats_async.py
+-rw-rw-r--  2.0 unx    12537 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_aad.py
+-rw-rw-r--  2.0 unx    87278 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_entity.py
+-rw-rw-r--  2.0 unx     7939 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_service_properties.py
+-rw-rw-r--  2.0 unx    17523 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_challenge_auth_async.py
+-rw-rw-r--  2.0 unx    84574 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_entity_cosmos_async.py
+-rw-rw-r--  2.0 unx    33242 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_client_async.py
+-rw-rw-r--  2.0 unx    18694 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table.py
+-rw-rw-r--  2.0 unx    49989 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_batch_async.py
+-rw-rw-r--  2.0 unx    74557 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_encoder.py
+-rw-rw-r--  2.0 unx     6049 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_retry.py
+-rw-rw-r--  2.0 unx    36163 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_batch_cosmos_async.py
+-rw-rw-r--  2.0 unx     8390 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_service_properties_async.py
+-rw-rw-r--  2.0 unx     9740 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_cosmos.py
+-rw-rw-r--  2.0 unx     3097 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/preparers.py
+-rw-rw-r--  2.0 unx    30324 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/test_table_client_cosmos_async.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx     1643 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/perfstress_tests/list_entities.py
+-rw-rw-r--  2.0 unx     1894 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/perfstress_tests/create_entity_batch.py
+-rw-rw-r--  2.0 unx      879 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/perfstress_tests/create_entity.py
+-rw-rw-r--  2.0 unx     4009 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/perfstress_tests/_base.py
+-rw-rw-r--  2.0 unx     4871 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/_shared/cosmos_testcase.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/_shared/__init__.py
+-rw-rw-r--  2.0 unx    21084 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/_shared/testcase.py
+-rw-rw-r--  2.0 unx     4956 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/tests/_shared/asynctestcase.py
+-rw-rw-r--  2.0 unx       88 b- defN 23-Jun-13 22:15 azure-data-tables-12.4.3/azure_data_tables.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-13 22:15 azure-data-tables-12.4.3/azure_data_tables.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-13 22:15 azure-data-tables-12.4.3/azure_data_tables.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx    33358 b- defN 23-Jun-13 22:15 azure-data-tables-12.4.3/azure_data_tables.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-13 22:15 azure-data-tables-12.4.3/azure_data_tables.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     4672 b- defN 23-Jun-13 22:15 azure-data-tables-12.4.3/azure_data_tables.egg-info/SOURCES.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/samples/async_samples/
+-rw-rw-r--  2.0 unx     4228 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_authentication.py
+-rw-rw-r--  2.0 unx     5487 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_query_table.py
+-rw-rw-r--  2.0 unx     3309 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_batching.py
+-rw-rw-r--  2.0 unx     5626 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_conditional_update.py
+-rw-rw-r--  2.0 unx     2671 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_create_client.py
+-rw-rw-r--  2.0 unx     4144 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_create_delete_table.py
+-rw-rw-r--  2.0 unx     8630 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/README.md
+-rw-rw-r--  2.0 unx     7027 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_update_upsert_merge_entities.py
+-rw-rw-r--  2.0 unx     3255 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_query_tables.py
+-rw-rw-r--  2.0 unx     6721 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_copy_table.py
+-rw-rw-r--  2.0 unx     3757 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/sample_insert_delete_entities.py
+-rw-rw-r--  2.0 unx     7200 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_update_upsert_merge_entities_async.py
+-rw-rw-r--  2.0 unx     4222 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_insert_delete_entities_async.py
+-rw-rw-r--  2.0 unx     6957 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_copy_table_async.py
+-rw-rw-r--  2.0 unx     5811 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_conditional_update_async.py
+-rw-rw-r--  2.0 unx     3788 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_batching_async.py
+-rw-rw-r--  2.0 unx     3218 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_query_tables_async.py
+-rw-rw-r--  2.0 unx     5593 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_query_table_async.py
+-rw-rw-r--  2.0 unx     4208 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_authentication_async.py
+-rw-rw-r--  2.0 unx     4374 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_create_delete_table_async.py
+-rw-rw-r--  2.0 unx     2800 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/samples/async_samples/sample_create_client_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/data/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/data/tables/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/data/tables/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/data/tables/_generated/
+-rw-rw-r--  2.0 unx     1492 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/__init__.py
+-rw-rw-r--  2.0 unx    10679 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_policies.py
+-rw-rw-r--  2.0 unx      330 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_version.py
+-rw-rw-r--  2.0 unx    13771 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_table_service_client.py
+-rw-rw-r--  2.0 unx    29409 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_table_client.py
+-rw-rw-r--  2.0 unx     7774 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_deserialize.py
+-rw-rw-r--  2.0 unx    15357 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_error.py
+-rw-rw-r--  2.0 unx     2552 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_entity.py
+-rw-rw-r--  2.0 unx     2730 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_common_conversion.py
+-rw-rw-r--  2.0 unx    16595 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_base_client.py
+-rw-rw-r--  2.0 unx    27334 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_models.py
+-rw-rw-r--  2.0 unx    11743 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_shared_access_signature.py
+-rw-rw-r--  2.0 unx     9284 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_serialize.py
+-rw-rw-r--  2.0 unx      546 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_sdk_moniker.py
+-rw-rw-r--  2.0 unx    28344 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_table_batch.py
+-rw-rw-r--  2.0 unx      799 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_constants.py
+-rw-rw-r--  2.0 unx    14442 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_table_shared_access_signature.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/py.typed
+-rw-rw-r--  2.0 unx    11099 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_authentication.py
+-rw-rw-r--  2.0 unx      518 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/aio/__init__.py
+-rw-rw-r--  2.0 unx    14450 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/aio/_table_service_client_async.py
+-rw-rw-r--  2.0 unx    30933 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/aio/_table_client_async.py
+-rw-rw-r--  2.0 unx    27311 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/aio/_table_batch_async.py
+-rw-rw-r--  2.0 unx     7408 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/aio/_policies_async.py
+-rw-rw-r--  2.0 unx     4676 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/aio/_models.py
+-rw-rw-r--  2.0 unx     7180 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/aio/_base_client_async.py
+-rw-rw-r--  2.0 unx     5122 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/aio/_authentication_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/data/tables/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/data/tables/_generated/models/
+-rw-rw-r--  2.0 unx      843 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/_vendor.py
+-rw-rw-r--  2.0 unx      864 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/__init__.py
+-rw-rw-r--  2.0 unx      491 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/_version.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/_patch.py
+-rw-rw-r--  2.0 unx     3763 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/_client.py
+-rw-rw-r--  2.0 unx    77872 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/_serialization.py
+-rw-rw-r--  2.0 unx     2813 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/_configuration.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-13 22:15 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/
+-rw-rw-r--  2.0 unx      811 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx     3871 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_client.py
+-rw-rw-r--  2.0 unx     2824 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx      839 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    79632 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx      839 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx   104301 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/operations/_operations.py
+-rw-rw-r--  2.0 unx     1814 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/models/_patch.py
+-rw-rw-r--  2.0 unx    24470 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/models/_models.py
+-rw-rw-r--  2.0 unx     1272 b- defN 23-Jun-13 22:14 azure-data-tables-12.4.3/azure/data/tables/_generated/models/_enums.py
+145 files, 1758534 bytes uncompressed, 287325 bytes compressed:  83.7%
```

## zipnote {}

```diff
@@ -1,433 +1,436 @@
-Filename: azure-data-tables-12.4.2/
+Filename: azure-data-tables-12.4.3/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure_data_tables.egg-info/
+Filename: azure-data-tables-12.4.3/tests/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/
+Filename: azure-data-tables-12.4.3/azure_data_tables.egg-info/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/
+Filename: azure-data-tables-12.4.3/samples/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/
+Filename: azure-data-tables-12.4.3/azure/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/migration_guide.md
+Filename: azure-data-tables-12.4.3/pyproject.toml
 Comment: 
 
-Filename: azure-data-tables-12.4.2/PKG-INFO
+Filename: azure-data-tables-12.4.3/setup.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/setup.py
+Filename: azure-data-tables-12.4.3/LICENSE
 Comment: 
 
-Filename: azure-data-tables-12.4.2/setup.cfg
+Filename: azure-data-tables-12.4.3/PKG-INFO
 Comment: 
 
-Filename: azure-data-tables-12.4.2/LICENSE
+Filename: azure-data-tables-12.4.3/README.md
 Comment: 
 
-Filename: azure-data-tables-12.4.2/MANIFEST.in
+Filename: azure-data-tables-12.4.3/setup.cfg
 Comment: 
 
-Filename: azure-data-tables-12.4.2/README.md
+Filename: azure-data-tables-12.4.3/CHANGELOG.md
 Comment: 
 
-Filename: azure-data-tables-12.4.2/CHANGELOG.md
+Filename: azure-data-tables-12.4.3/migration_guide.md
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure_data_tables.egg-info/PKG-INFO
+Filename: azure-data-tables-12.4.3/MANIFEST.in
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure_data_tables.egg-info/not-zip-safe
+Filename: azure-data-tables-12.4.3/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure_data_tables.egg-info/SOURCES.txt
+Filename: azure-data-tables-12.4.3/tests/_shared/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure_data_tables.egg-info/dependency_links.txt
+Filename: azure-data-tables-12.4.3/tests/test_table_aad_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure_data_tables.egg-info/requires.txt
+Filename: azure-data-tables-12.4.3/tests/test_table_cosmos_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure_data_tables.egg-info/top_level.txt
+Filename: azure-data-tables-12.4.3/tests/test_table_entity_cosmos.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/
+Filename: azure-data-tables-12.4.3/tests/async_preparers.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/__init__.py
+Filename: azure-data-tables-12.4.3/tests/test_challenge_auth.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/
+Filename: azure-data-tables-12.4.3/tests/test_table_batch.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/__init__.py
+Filename: azure-data-tables-12.4.3/tests/test_table_service_stats.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/
+Filename: azure-data-tables-12.4.3/tests/test_table_service_properties_cosmos.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/
+Filename: azure-data-tables-12.4.3/tests/test_table_service_stats_cosmos_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_shared_access_signature.py
+Filename: azure-data-tables-12.4.3/tests/test_table_client.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_table_batch.py
+Filename: azure-data-tables-12.4.3/tests/test_table_entity_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_authentication.py
+Filename: azure-data-tables-12.4.3/tests/test_table_service_properties_cosmos_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_table_client.py
+Filename: azure-data-tables-12.4.3/tests/test_table_client_cosmos.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_deserialize.py
+Filename: azure-data-tables-12.4.3/tests/test_table_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/py.typed
+Filename: azure-data-tables-12.4.3/tests/test_retry_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_constants.py
+Filename: azure-data-tables-12.4.3/tests/test_table_service_stats_cosmos.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/__init__.py
+Filename: azure-data-tables-12.4.3/tests/test_table_batch_cosmos.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_sdk_moniker.py
+Filename: azure-data-tables-12.4.3/tests/conftest.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_common_conversion.py
+Filename: azure-data-tables-12.4.3/tests/test_table_service_stats_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_models.py
+Filename: azure-data-tables-12.4.3/tests/test_table_aad.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_error.py
+Filename: azure-data-tables-12.4.3/tests/test_table_entity.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_table_service_client.py
+Filename: azure-data-tables-12.4.3/tests/test_table_service_properties.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_version.py
+Filename: azure-data-tables-12.4.3/tests/test_challenge_auth_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_entity.py
+Filename: azure-data-tables-12.4.3/tests/test_table_entity_cosmos_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_serialize.py
+Filename: azure-data-tables-12.4.3/tests/test_table_client_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_base_client.py
+Filename: azure-data-tables-12.4.3/tests/test_table.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_policies.py
+Filename: azure-data-tables-12.4.3/tests/test_table_batch_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_table_shared_access_signature.py
+Filename: azure-data-tables-12.4.3/tests/test_encoder.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/_table_batch_async.py
+Filename: azure-data-tables-12.4.3/tests/test_retry.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/_base_client_async.py
+Filename: azure-data-tables-12.4.3/tests/test_table_batch_cosmos_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/__init__.py
+Filename: azure-data-tables-12.4.3/tests/test_table_service_properties_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/_policies_async.py
+Filename: azure-data-tables-12.4.3/tests/test_table_cosmos.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/_authentication_async.py
+Filename: azure-data-tables-12.4.3/tests/preparers.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/_models.py
+Filename: azure-data-tables-12.4.3/tests/test_table_client_cosmos_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/_table_client_async.py
+Filename: azure-data-tables-12.4.3/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/aio/_table_service_client_async.py
+Filename: azure-data-tables-12.4.3/tests/perfstress_tests/list_entities.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/
+Filename: azure-data-tables-12.4.3/tests/perfstress_tests/create_entity_batch.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/models/
+Filename: azure-data-tables-12.4.3/tests/perfstress_tests/create_entity.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/operations/
+Filename: azure-data-tables-12.4.3/tests/perfstress_tests/_base.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/_client.py
+Filename: azure-data-tables-12.4.3/tests/_shared/cosmos_testcase.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/_vendor.py
+Filename: azure-data-tables-12.4.3/tests/_shared/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/_configuration.py
+Filename: azure-data-tables-12.4.3/tests/_shared/testcase.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/__init__.py
+Filename: azure-data-tables-12.4.3/tests/_shared/asynctestcase.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/_serialization.py
+Filename: azure-data-tables-12.4.3/azure_data_tables.egg-info/requires.txt
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/_patch.py
+Filename: azure-data-tables-12.4.3/azure_data_tables.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/_version.py
+Filename: azure-data-tables-12.4.3/azure_data_tables.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/
+Filename: azure-data-tables-12.4.3/azure_data_tables.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_client.py
+Filename: azure-data-tables-12.4.3/azure_data_tables.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_configuration.py
+Filename: azure-data-tables-12.4.3/azure_data_tables.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/__init__.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_patch.py
+Filename: azure-data-tables-12.4.3/samples/sample_authentication.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/__init__.py
+Filename: azure-data-tables-12.4.3/samples/sample_query_table.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/_operations.py
+Filename: azure-data-tables-12.4.3/samples/sample_batching.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/_patch.py
+Filename: azure-data-tables-12.4.3/samples/sample_conditional_update.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/models/__init__.py
+Filename: azure-data-tables-12.4.3/samples/sample_create_client.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/models/_enums.py
+Filename: azure-data-tables-12.4.3/samples/sample_create_delete_table.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/models/_models.py
+Filename: azure-data-tables-12.4.3/samples/README.md
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/models/_patch.py
+Filename: azure-data-tables-12.4.3/samples/sample_update_upsert_merge_entities.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/operations/__init__.py
+Filename: azure-data-tables-12.4.3/samples/sample_query_tables.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/operations/_operations.py
+Filename: azure-data-tables-12.4.3/samples/sample_copy_table.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/azure/data/tables/_generated/operations/_patch.py
+Filename: azure-data-tables-12.4.3/samples/sample_insert_delete_entities.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_update_upsert_merge_entities_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_create_delete_table.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_insert_delete_entities_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_query_table.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_copy_table_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_copy_table.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_conditional_update_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_query_tables.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_batching_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_insert_delete_entities.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_query_tables_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_conditional_update.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_query_table_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_authentication.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_authentication_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_batching.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_create_delete_table_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_update_upsert_merge_entities.py
+Filename: azure-data-tables-12.4.3/samples/async_samples/sample_create_client_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/README.md
+Filename: azure-data-tables-12.4.3/azure/data/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/sample_create_client.py
+Filename: azure-data-tables-12.4.3/azure/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_create_client_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_query_table_async.py
+Filename: azure-data-tables-12.4.3/azure/data/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_batching_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_conditional_update_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_create_delete_table_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_update_upsert_merge_entities_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_policies.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_authentication_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_version.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_copy_table_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_table_service_client.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_insert_delete_entities_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_table_client.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/samples/async_samples/sample_query_tables_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_deserialize.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/_shared/
+Filename: azure-data-tables-12.4.3/azure/data/tables/_error.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/perfstress_tests/
+Filename: azure-data-tables-12.4.3/azure/data/tables/_entity.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/preparers.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_common_conversion.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_service_stats_cosmos.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_base_client.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_retry.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_models.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_service_properties_cosmos_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_shared_access_signature.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_batch.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_serialize.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_cosmos_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_sdk_moniker.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_retry_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_table_batch.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_entity_cosmos_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_constants.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_challenge_auth_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_table_shared_access_signature.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_service_stats_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/py.typed
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_service_properties_cosmos.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_authentication.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_service_stats.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_aad_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/_table_service_client_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_client.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/_table_client_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_client_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/_table_batch_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_service_properties.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/_policies_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/_models.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_entity_cosmos.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/_base_client_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_encoder.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/aio/_authentication_async.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_batch_cosmos.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/operations/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_service_properties_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/models/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/conftest.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/_vendor.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/async_preparers.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_entity_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/_version.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_service_stats_cosmos_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/_patch.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_aad.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/_client.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_batch_cosmos_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/_serialization.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_batch_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/_configuration.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_cosmos.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_challenge_auth.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_entity.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_client_cosmos_async.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_client.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/test_table_client_cosmos.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/_shared/asynctestcase.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/_shared/cosmos_testcase.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/_shared/__init__.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/_shared/testcase.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/perfstress_tests/create_entity.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/perfstress_tests/create_entity_batch.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/operations/_operations.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/perfstress_tests/_base.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/perfstress_tests/__init__.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/models/_patch.py
 Comment: 
 
-Filename: azure-data-tables-12.4.2/tests/perfstress_tests/list_entities.py
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/models/_models.py
+Comment: 
+
+Filename: azure-data-tables-12.4.3/azure/data/tables/_generated/models/_enums.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-data-tables-12.4.2/migration_guide.md` & `azure-data-tables-12.4.3/migration_guide.md`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/PKG-INFO` & `azure-data-tables-12.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-data-tables
-Version: 12.4.2
+Version: 12.4.3
 Summary: Microsoft Azure Azure Data Tables Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/table/azure-table
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -24,15 +24,19 @@
 
 Azure Tables is a NoSQL data storage service that can be accessed from anywhere in the world via authenticated calls using HTTP or HTTPS.
 Tables scales as needed to support the amount of data inserted, and allow for the storing of data with non-complex accessing.
 The Azure Tables client can be used to access Azure Storage or Cosmos accounts. This document covers [`azure-data-tables`][Tables_pypi].
 
 Please note, this package is a replacement for [`azure-cosmosdb-tables`](https://github.com/Azure/azure-cosmos-table-python/tree/master/azure-cosmosdb-table) which is now deprecated. See the [migration guide][migration_guide] for more details.
 
-[Source code][source_code] | [Package (PyPI)][Tables_pypi] | [API reference documentation][Tables_ref_docs] | [Samples][Tables_samples]
+[Source code][source_code]
+| [Package (PyPI)][Tables_pypi]
+| [Package (Conda)](https://anaconda.org/microsoft/azure-data-tables/)
+| [API reference documentation][Tables_ref_docs]
+| [Samples][Tables_samples]
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 _Python 3.7 or later is required to use this package. For more details, please refer to [Azure SDK for Python version support policy](https://github.com/Azure/azure-sdk-for-python/wiki/Azure-SDKs-Python-version-support-policy)._
 
 ## Getting started
@@ -409,14 +413,22 @@
 [upsert_entity]:https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/tables/azure-data-tables/samples/sample_update_upsert_merge_entities.py#L155-L163
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python/sdk/tables/azure-data-tables/README.png)
 
 
 # Release History
 
+## 12.4.3 (2023-06-13)
+
+### Bugs Fixed
+* Fixed a bug in getting error attribute values when operations failed. ([#27410](https://github.com/Azure/azure-sdk-for-python/issues/27410))
+
+### Other Changes
+* Adjusted dependency on `isodate` to `<1.0.0,>=0.6.1`.
+
 ## 12.4.2 (2023-02-07)
 
 ### Bugs Fixed
 * Fixed a bug when deleting an entity with partition key or row key in empty string.([#24480](https://github.com/Azure/azure-sdk-for-python/issues/24480))
 
 ### Other Changes
 * Added support for Python 3.11.
```

## Comparing `azure-data-tables-12.4.2/setup.py` & `azure-data-tables-12.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,11 +63,11 @@
         'tests',
         'azure.data',
     ]),
     python_requires=">=3.7",
     install_requires=[
         "azure-core<2.0.0,>=1.24.0",
         "yarl<2.0,>=1.0",
-        "isodate>=0.6.0",
+        "isodate<1.0.0,>=0.6.1",
         "typing-extensions>=4.3.0"
     ],
 )
```

## Comparing `azure-data-tables-12.4.2/LICENSE` & `azure-data-tables-12.4.3/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/README.md` & `azure-data-tables-12.4.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 Azure Tables is a NoSQL data storage service that can be accessed from anywhere in the world via authenticated calls using HTTP or HTTPS.
 Tables scales as needed to support the amount of data inserted, and allow for the storing of data with non-complex accessing.
 The Azure Tables client can be used to access Azure Storage or Cosmos accounts. This document covers [`azure-data-tables`][Tables_pypi].
 
 Please note, this package is a replacement for [`azure-cosmosdb-tables`](https://github.com/Azure/azure-cosmos-table-python/tree/master/azure-cosmosdb-table) which is now deprecated. See the [migration guide][migration_guide] for more details.
 
-[Source code][source_code] | [Package (PyPI)][Tables_pypi] | [API reference documentation][Tables_ref_docs] | [Samples][Tables_samples]
+[Source code][source_code]
+| [Package (PyPI)][Tables_pypi]
+| [Package (Conda)](https://anaconda.org/microsoft/azure-data-tables/)
+| [API reference documentation][Tables_ref_docs]
+| [Samples][Tables_samples]
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 _Python 3.7 or later is required to use this package. For more details, please refer to [Azure SDK for Python version support policy](https://github.com/Azure/azure-sdk-for-python/wiki/Azure-SDKs-Python-version-support-policy)._
 
 ## Getting started
```

## Comparing `azure-data-tables-12.4.2/CHANGELOG.md` & `azure-data-tables-12.4.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Release History
 
+## 12.4.3 (2023-06-13)
+
+### Bugs Fixed
+* Fixed a bug in getting error attribute values when operations failed. ([#27410](https://github.com/Azure/azure-sdk-for-python/issues/27410))
+
+### Other Changes
+* Adjusted dependency on `isodate` to `<1.0.0,>=0.6.1`.
+
 ## 12.4.2 (2023-02-07)
 
 ### Bugs Fixed
 * Fixed a bug when deleting an entity with partition key or row key in empty string.([#24480](https://github.com/Azure/azure-sdk-for-python/issues/24480))
 
 ### Other Changes
 * Added support for Python 3.11.
```

## Comparing `azure-data-tables-12.4.2/azure_data_tables.egg-info/PKG-INFO` & `azure-data-tables-12.4.3/azure_data_tables.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-data-tables
-Version: 12.4.2
+Version: 12.4.3
 Summary: Microsoft Azure Azure Data Tables Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/table/azure-table
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -24,15 +24,19 @@
 
 Azure Tables is a NoSQL data storage service that can be accessed from anywhere in the world via authenticated calls using HTTP or HTTPS.
 Tables scales as needed to support the amount of data inserted, and allow for the storing of data with non-complex accessing.
 The Azure Tables client can be used to access Azure Storage or Cosmos accounts. This document covers [`azure-data-tables`][Tables_pypi].
 
 Please note, this package is a replacement for [`azure-cosmosdb-tables`](https://github.com/Azure/azure-cosmos-table-python/tree/master/azure-cosmosdb-table) which is now deprecated. See the [migration guide][migration_guide] for more details.
 
-[Source code][source_code] | [Package (PyPI)][Tables_pypi] | [API reference documentation][Tables_ref_docs] | [Samples][Tables_samples]
+[Source code][source_code]
+| [Package (PyPI)][Tables_pypi]
+| [Package (Conda)](https://anaconda.org/microsoft/azure-data-tables/)
+| [API reference documentation][Tables_ref_docs]
+| [Samples][Tables_samples]
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 _Python 3.7 or later is required to use this package. For more details, please refer to [Azure SDK for Python version support policy](https://github.com/Azure/azure-sdk-for-python/wiki/Azure-SDKs-Python-version-support-policy)._
 
 ## Getting started
@@ -409,14 +413,22 @@
 [upsert_entity]:https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/tables/azure-data-tables/samples/sample_update_upsert_merge_entities.py#L155-L163
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python/sdk/tables/azure-data-tables/README.png)
 
 
 # Release History
 
+## 12.4.3 (2023-06-13)
+
+### Bugs Fixed
+* Fixed a bug in getting error attribute values when operations failed. ([#27410](https://github.com/Azure/azure-sdk-for-python/issues/27410))
+
+### Other Changes
+* Adjusted dependency on `isodate` to `<1.0.0,>=0.6.1`.
+
 ## 12.4.2 (2023-02-07)
 
 ### Bugs Fixed
 * Fixed a bug when deleting an entity with partition key or row key in empty string.([#24480](https://github.com/Azure/azure-sdk-for-python/issues/24480))
 
 ### Other Changes
 * Added support for Python 3.11.
```

## Comparing `azure-data-tables-12.4.2/azure_data_tables.egg-info/SOURCES.txt` & `azure-data-tables-12.4.3/azure_data_tables.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 migration_guide.md
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/data/__init__.py
 azure/data/tables/__init__.py
 azure/data/tables/_authentication.py
 azure/data/tables/_base_client.py
 azure/data/tables/_common_conversion.py
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_shared_access_signature.py` & `azure-data-tables-12.4.3/azure/data/tables/_shared_access_signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-from datetime import date
-from typing import Optional, Union, TYPE_CHECKING
+from datetime import date, datetime
+from typing import Optional, Union
 
 from ._deserialize import url_quote
-
-
+from ._models import AccountSasPermissions, ResourceTypes, SASProtocol
 from ._common_conversion import (
     _sign_string,
     _to_str,
 )
 from ._constants import DEFAULT_X_MS_VERSION
 
-if TYPE_CHECKING:
-    from datetime import datetime  # pylint: disable=ungrouped-imports
-    from ._models import AccountSasPermissions, ResourceTypes, SASProtocol
-
 
 def _to_utc_datetime(value):
     # This is for SAS where milliseconds are not supported
     return value.strftime("%Y-%m-%dT%H:%M:%SZ")
 
 
 class SharedAccessSignature(object):
@@ -42,23 +37,22 @@
         """
         self.account_name = credential.named_key.name
         self.account_key = credential.named_key.key
         self.x_ms_version = x_ms_version
 
     def generate_account(
         self,
-        services,  # type: str
-        resource_types,  # type: ResourceTypes
-        permission,  # type: Union[AccountSasPermissions, str]
-        expiry,  # type: Union[datetime, str]
-        start=None,  # type: Optional[Union[datetime, str]]
-        ip_address_or_range=None,  # type: Optional[str]
-        protocol=None,  # type: Optional[Union[str, SASProtocol]]
-    ):
-    # type: (...) -> str
+        services: str,
+        resource_types: ResourceTypes,
+        permission: Union[AccountSasPermissions, str],
+        expiry: Union[datetime, str],
+        start: Optional[Union[datetime, str]] = None,
+        ip_address_or_range: Optional[str] = None,
+        protocol: Optional[Union[str, SASProtocol]] = None,
+    ) -> str:
         """
         Generates a shared access signature for the account.
         Use the returned signature with the sas_token parameter of the service
         or to create a new account object.
 
         :param str services:
             Specifies the services as a bitmap accessible with the account SAS. You can
@@ -244,16 +238,15 @@
             string_to_sign = string_to_sign[:-1]
 
         self._add_query(
             QueryStringConstants.SIGNED_SIGNATURE,
             _sign_string(account_key, string_to_sign),
         )
 
-    def add_account_signature(self, account_name, account_key):
-        # type: (str, str) -> None
+    def add_account_signature(self, account_name: str, account_key: str) -> None:
         def get_value_to_append(query):
             return_value = self.query_dict.get(query) or ""
             return return_value + "\n"
 
         string_to_sign = (
             account_name
             + "\n"
@@ -268,16 +261,15 @@
         )
 
         self._add_query(
             QueryStringConstants.SIGNED_SIGNATURE,
             _sign_string(account_key, string_to_sign),
         )
 
-    def get_token(self):
-        # type: () -> str
+    def get_token(self) -> str:
         return "&".join(
             [
                 "{0}={1}".format(n, url_quote(v))
                 for n, v in self.query_dict.items()
                 if v is not None
             ]
         )
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_table_batch.py` & `azure-data-tables-12.4.3/azure/data/tables/_table_batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from typing import (
-    TYPE_CHECKING,
     Union,
     Any,
     Dict,
     Mapping,
     Optional,
     List,
     Tuple
 )
 
 from azure.core import MatchConditions
+from azure.core.pipeline.transport import HttpRequest
 
 from ._common_conversion import _transform_patch_to_cosmos_post
 from ._models import UpdateMode, TransactionOperation
 from ._serialize import _get_match_headers, _add_entity_properties, _prepare_key
 from ._entity import TableEntity
-
-if TYPE_CHECKING:
-    from azure.core.pipeline.transport import HttpRequest
-    from ._generated import models, AzureTable
-    from ._generated._configuration import AzureTableConfiguration
-    from ._generated._serialization import Serializer
-    from ._generated._serialization import Deserializer
+from ._generated import models, AzureTable
+from ._generated._configuration import AzureTableConfiguration
+from ._generated._serialization import Serializer, Deserializer
 
 
 EntityType = Union[TableEntity, Mapping[str, Any]]
 OperationType = Union[TransactionOperation, str]
 TransactionOperationType = Union[Tuple[OperationType, EntityType], Tuple[OperationType, EntityType, Mapping[str, Any]]]
 
 
@@ -44,21 +40,21 @@
     supported within a single transaction. The batch can include at most 100
     entities, and its total payload may be no more than 4 MB in size.
 
     """
 
     def __init__(
         self,
-        client,  # type: AzureTable
-        serializer,  # type: Serializer
-        deserializer,  # type: Deserializer
-        config,  # type: AzureTableConfiguration
-        table_name,  # type: str
-        is_cosmos_endpoint=False,  # type: bool
-        **kwargs  # type: Dict[str, Any]
+        client: AzureTable,
+        serializer: Serializer,
+        deserializer: Deserializer,
+        config: AzureTableConfiguration,
+        table_name: str,
+        is_cosmos_endpoint: bool = False,
+        **kwargs
     ):
         """Create TableClient from a Credential.
 
         :param client: an AzureTable object
         :type client: AzureTable
         :param serializer: serializer object for request serialization
         :type serializer: ~azure.data.tables._generated._serialization.Serializer
@@ -82,41 +78,32 @@
 
         self._partition_key = kwargs.pop("partition_key", None)
         self.requests = []  # type: List[HttpRequest]
 
     def __len__(self):
         return len(self.requests)
 
-    def _verify_partition_key(
-        self, entity  # type: EntityType
-    ):
-        # (...) -> None
+    def _verify_partition_key(self, entity: EntityType) -> None:
         if self._partition_key is None:
             self._partition_key = entity["PartitionKey"]
         elif entity["PartitionKey"] != self._partition_key:
             raise ValueError("Partition Keys must all be the same")
 
-    def add_operation(self, operation):
-        # type: (TransactionOperationType) -> None
+    def add_operation(self, operation: TransactionOperationType) -> None:
         """Add a single operation to a batch."""
         try:
             operation_type, entity, kwargs = operation  # type: ignore
         except ValueError:
             operation_type, entity, kwargs = operation[0], operation[1], {}  # type: ignore
         try:
             getattr(self, operation_type.lower())(entity, **kwargs)
         except AttributeError:
             raise ValueError("Unrecognized operation: {}".format(operation))
 
-    def create(
-        self,
-        entity,  # type: EntityType
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def create(self, entity: EntityType, **kwargs) -> None:
         """Adds an insert operation to the current batch.
 
         :param entity: The properties for the table entity.
         :type entity: :class:`~azure.data.tables.TableEntity` or Dict[str,str]
         :return: None
         :rtype: None
         :raises ValueError:
@@ -137,37 +124,36 @@
             temp = _add_entity_properties(temp)
         else:
             raise ValueError("PartitionKey and/or RowKey were not provided in entity")
         self._batch_create_entity(table=self.table_name, entity=temp, **kwargs)
 
     def _batch_create_entity(
         self,
-        table,  # type: str
-        entity,  # type: EntityType
-        timeout=None,  # type: Optional[int]
-        request_id_parameter=None,  # type: Optional[str]
-        response_preference="return-no-content",  # type: Optional[Union[str, "models.ResponseFormat"]]
-        format=None,  # type: Optional[Union[str, "models.OdataMetadataFormat"]] # pylint: disable=redefined-builtin
-        **kwargs  # type: Any
-    ):
-        # (...) -> None
+        table: str,
+        entity: EntityType,
+        timeout: Optional[int] = None,
+        request_id_parameter: Optional[str] = None,
+        response_preference: Optional[Union[str, models.ResponseFormat]] = "return-no-content",
+        format: Optional[Union[str, models.OdataMetadataFormat]] = None, # pylint: disable=redefined-builtin
+        **kwargs
+    ) -> None:
         """
         Adds an insert operation to the batch. See
         :func:`azure.data.tables.TableClient.insert_entity` for more information
         on insert operations.
 
         The operation will not be executed until the batch is committed
 
         :param: table:
             The table to perform the operation on
         :type: table: str
         :param: entity:
             The entity to insert. Can be a dict or an entity object
             Must contain a PartitionKey and a RowKey.
-        :type: entity: dict or :class:`~azure.data.tables.models.Entity`
+        :type: entity: Dict or :class:`~azure.data.tables.models.Entity`
         :param timeout: The timeout parameter is expressed in seconds.
         :type timeout: int
         :param request_id_parameter: Provides a client-generated, opaque value with a 1 KB character
          limit that is recorded in the analytics logs when analytics logging is enabled.
         :type request_id_parameter: str
         :param response_preference: Specifies the return format. Default is return without content.
         :type response_preference: str or ~azure.data.tables.models.ResponseFormat
@@ -233,22 +219,15 @@
         request = self._client._client.post(  # pylint: disable=protected-access
             url, query_parameters, header_parameters, **body_content_kwargs
         )
         self.requests.append(request)
 
     _batch_create_entity.metadata = {"url": "/{table}"}  # type: ignore
 
-    def update(
-        self,
-        entity,  # type: EntityType
-        mode=UpdateMode.MERGE,  # type: Union[str, UpdateMode]
-        **kwargs  # type: Any
-    ):
-        # (...) -> None
-
+    def update(self, entity: EntityType, mode: Union[str, UpdateMode] = UpdateMode.MERGE, **kwargs) -> None:
         """Adds an update operation to the current batch.
 
         :param entity: The properties for the table entity.
         :type entity: :class:`~azure.data.tables.TableEntity` or Dict[str,str]
         :param mode: Merge or Replace entity
         :type mode: :class:`~azure.data.tables.UpdateMode`
         :keyword str etag: Etag of the entity
@@ -305,25 +284,24 @@
                 **kwargs
             )
         else:
             raise ValueError("Mode type '{}' is not supported.".format(mode))
 
     def _batch_update_entity(
         self,
-        table,  # type: str
-        partition_key,  # type: str
-        row_key,  # type: str
-        timeout=None,  # type: Optional[int]
-        request_id_parameter=None,  # type: Optional[str]
-        if_match=None,  # type: Optional[str]
-        table_entity_properties=None,  # type: Optional[EntityType]
-        format=None,  # type: Optional[Union[str, "models.OdataMetadataFormat"]] # pylint: disable=redefined-builtin
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        table: str,
+        partition_key: str,
+        row_key: str,
+        timeout: Optional[int] = None,
+        request_id_parameter: Optional[str] = None,
+        if_match: Optional[str] = None,
+        table_entity_properties: Optional[EntityType] = None,
+        format: Optional[Union[str, models.OdataMetadataFormat]] = None, # pylint: disable=redefined-builtin
+        **kwargs
+    ) -> None:
         """Update entity in a table.
 
         :param table: The name of the table.
         :type table: str
         :param partition_key: The partition key of the entity.
         :type partition_key: str
         :param row_key: The row key of the entity.
@@ -335,15 +313,15 @@
         :type request_id_parameter: str
         :param if_match: Match condition for an entity to be updated. If specified and a matching
          entity is not found, an error will be raised. To force an unconditional update, set to the
          wildcard character (*). If not specified, an insert will be performed when no existing entity
          is found to update and a replace will be performed if an existing entity is found.
         :type if_match: str
         :param table_entity_properties: The properties for the table entity.
-        :type table_entity_properties: dict[str, object]
+        :type table_entity_properties: Dict[str, object]
         :param format: Specifies the media type for the response. Known values are:
          "application/json;odata=nometadata", "application/json;odata=minimalmetadata", and
          "application/json;odata=fullmetadata".
         :type format: str or ~azure.data.tables.models.OdataMetadataFormat
         :return: None
         :rtype: None
         """
@@ -410,25 +388,24 @@
 
     _batch_update_entity.metadata = {  # type: ignore
         "url": "/{table}(PartitionKey='{partitionKey}',RowKey='{rowKey}')"
     }  # type: ignore
 
     def _batch_merge_entity(
         self,
-        table,  # type: str
-        partition_key,  # type: str
-        row_key,  # type: str
-        timeout=None,  # type: Optional[int]
-        request_id_parameter=None,  # type: Optional[str]
-        if_match=None,  # type: Optional[str]
-        table_entity_properties=None,  # type: Optional[EntityType]
-        format=None,  # type: Optional[Union[str, "models.OdataMetadataFormat"]] # pylint: disable=redefined-builtin
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        table: str,
+        partition_key: str,
+        row_key: str,
+        timeout: Optional[int] = None,
+        request_id_parameter: Optional[str] = None,
+        if_match: Optional[str] = None,
+        table_entity_properties: Optional[EntityType] = None,
+        format: Optional[Union[str, models.OdataMetadataFormat]] = None, # pylint: disable=redefined-builtin
+        **kwargs
+    ) -> None:
         """Merge entity in a table.
 
         :param table: The name of the table.
         :type table: str
         :param partition_key: The partition key of the entity.
         :type partition_key: str
         :param row_key: The row key of the entity.
@@ -440,15 +417,15 @@
         :type request_id_parameter: str
         :param if_match: Match condition for an entity to be updated. If specified and a matching
          entity is not found, an error will be raised. To force an unconditional update, set to the
          wildcard character (*). If not specified, an insert will be performed when no existing entity
          is found to update and a merge will be performed if an existing entity is found.
         :type if_match: str
         :param table_entity_properties: The properties for the table entity.
-        :type table_entity_properties: dict[str, object]
+        :type table_entity_properties: Dict[str, object]
         :param format: Specifies the media type for the response. Known values are:
          "application/json;odata=nometadata", "application/json;odata=minimalmetadata", and
          "application/json;odata=fullmetadata".
         :type format: str or ~azure.data.tables.models.OdataMetadataFormat
         :return: None
         :rtype: None
         """
@@ -514,20 +491,15 @@
             _transform_patch_to_cosmos_post(request)
         self.requests.append(request)
 
     _batch_merge_entity.metadata = {  # type: ignore
         "url": "/{table}(PartitionKey='{partitionKey}',RowKey='{rowKey}')"
     }
 
-    def delete(
-        self,
-        entity,  # type: EntityType
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def delete(self, entity: EntityType, **kwargs) -> None:
         """Adds a delete operation to the current branch.
 
         :param partition_key: The partition key of the entity.
         :type partition_key: str
         :param row_key: The row key of the entity.
         :type row_key: str
         :keyword str etag: Etag of the entity
@@ -567,23 +539,22 @@
             row_key=row_key,
             if_match=if_match,
             **kwargs
         )
 
     def _batch_delete_entity(
         self,
-        table,  # type: str
-        partition_key,  # type: str
-        row_key,  # type: str
-        if_match,  # type: str
-        timeout=None,  # type: Optional[int]
-        request_id_parameter=None,  # type: Optional[str]
-        format=None,  # type: Optional[Union[str, "models.OdataMetadataFormat"]] # pylint: disable=redefined-builtin
-    ):
-        # type: (...) -> None
+        table: str,
+        partition_key: str,
+        row_key: str,
+        if_match: str,
+        timeout: Optional[int] = None,
+        request_id_parameter: Optional[str] = None,
+        format: Optional[Union[str, models.OdataMetadataFormat]] = None, # pylint: disable=redefined-builtin
+    ) -> None:
         """Deletes the specified entity in a table.
 
         :param table: The name of the table.
         :type table: str
         :param partition_key: The partition key of the entity.
         :type partition_key: str
         :param row_key: The row key of the entity.
@@ -654,21 +625,15 @@
         )
         self.requests.append(request)
 
     _batch_delete_entity.metadata = {  # type: ignore
         "url": "/{table}(PartitionKey='{partitionKey}',RowKey='{rowKey}')"
     }
 
-    def upsert(
-        self,
-        entity,  # type: EntityType
-        mode=UpdateMode.MERGE,  # type: Union[str, UpdateMode]
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def upsert(self, entity: EntityType, mode: Union[str, UpdateMode] = UpdateMode.MERGE, **kwargs) -> None:
         """Adds an upsert (update/merge) operation to the batch.
 
         :param entity: The properties for the table entity.
         :type entity: :class:`~azure.data.tables.TableEntity` or Dict[str,str]
         :param mode: Merge or Replace entity
         :type mode: :class:`~azure.data.tables.UpdateMode`
         :raises ValueError:
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_authentication.py` & `azure-data-tables-12.4.3/azure/data/tables/_authentication.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-
-from typing import TYPE_CHECKING
-
 try:
     from urllib.parse import urlparse
 except ImportError:
     from urlparse import urlparse  # type: ignore
+from typing import Optional, Union, overload, cast
 
+from azure.core.credentials import TokenCredential, AzureSasCredential, AzureNamedKeyCredential
 from azure.core.exceptions import ClientAuthenticationError
-from azure.core.pipeline.policies import BearerTokenCredentialPolicy, SansIOHTTPPolicy
+from azure.core.pipeline import PipelineResponse, PipelineRequest
+from azure.core.pipeline.policies import BearerTokenCredentialPolicy, SansIOHTTPPolicy, AzureSasCredentialPolicy
 
 try:
     from azure.core.pipeline.transport import AsyncHttpTransport
 except ImportError:
     AsyncHttpTransport = None  # type: ignore
 
 try:
     from yarl import URL # cspell:disable-line
 except ImportError:
     pass
 
-from ._common_conversion import (
-    _sign_string,
-)
-
-from ._error import (
-    _wrap_exception,
-)
-
-if TYPE_CHECKING:
-    from typing import Any
-    from azure.core.credentials import TokenCredential
-    from azure.core.pipeline import PipelineResponse, PipelineRequest  # pylint: disable=ungrouped-imports
+from ._common_conversion import _sign_string
+from ._error import _wrap_exception
+from ._constants import STORAGE_OAUTH_SCOPE
 
 
 class AzureSigningError(ClientAuthenticationError):
     """
     Represents a fatal error when attempting to sign a request.
     In general, the cause of this exception is user error. For example, the given account key is not valid.
     Please visit https://docs.microsoft.com/en-us/azure/storage/common/storage-create-storage-account for more info.
@@ -146,19 +137,18 @@
             auth_string = "SharedKey " + self._credential.named_key.name + ":" + signature
             request.headers["Authorization"] = auth_string
         except Exception as ex:
             # Wrap any error that occurred as signing error
             # Doing so will clarify/locate the source of problem
             raise _wrap_exception(ex, AzureSigningError)
 
-    def on_request(self, request):
-    # type: (PipelineRequest) -> None
+    def on_request(self, request: PipelineRequest) -> None:
         self.sign_request(request)
 
-    def sign_request(self, request):
+    def sign_request(self, request: PipelineRequest) -> None:
         string_to_sign = (
             self._get_verb(request.http_request)
             + self._get_headers(
                 request.http_request,
                 ["content-md5", "content-type", "x-ms-date"],
             )
             + self._get_canonicalized_resource(request)
@@ -186,25 +176,25 @@
     :keyword bool discover_scopes: Determines if scopes from authentication challenges should be provided to token
         requests, instead of the scopes given to the policy's constructor, if any are present. Defaults to True.
     :raises: :class:`~azure.core.exceptions.ServiceRequestError`
     """
 
     def __init__(
         self,
-        credential: "TokenCredential",
+        credential: TokenCredential,
         *scopes: str,
         discover_tenant: bool = True,
         discover_scopes: bool = True,
-        **kwargs: "Any"
+        **kwargs
     ) -> None:
         self._discover_tenant = discover_tenant
         self._discover_scopes = discover_scopes
         super().__init__(credential, *scopes, **kwargs)
 
-    def on_challenge(self, request: "PipelineRequest", response: "PipelineResponse") -> bool:
+    def on_challenge(self, request: PipelineRequest, response: PipelineResponse) -> bool:
         """Authorize request according to an authentication challenge
 
         This method is called when the resource provider responds 401 with a WWW-Authenticate header.
 
         :param ~azure.core.pipeline.PipelineRequest request: the request which elicited an authentication challenge
         :param ~azure.core.pipeline.PipelineResponse response: the resource provider's response
         :returns: a bool indicating whether the policy should send the request
@@ -224,7 +214,59 @@
             return False
 
         if self._discover_tenant:
             self.authorize_request(request, scope, tenant_id=challenge.tenant_id)
         else:
             self.authorize_request(request, scope)
         return True
+
+
+@overload
+def _configure_credential(credential: AzureNamedKeyCredential) -> SharedKeyCredentialPolicy:
+    ...
+
+@overload
+def _configure_credential(credential: SharedKeyCredentialPolicy) -> SharedKeyCredentialPolicy:
+    ...
+
+@overload
+def _configure_credential(credential: AzureSasCredential) -> AzureSasCredentialPolicy:
+    ...
+
+@overload
+def _configure_credential(credential: TokenCredential) -> BearerTokenChallengePolicy:
+    ...
+
+@overload
+def _configure_credential(credential: None) -> None:
+    ...
+
+def _configure_credential(
+    credential: Optional[
+        Union[
+            AzureNamedKeyCredential,
+            AzureSasCredential,
+            TokenCredential,
+            SharedKeyCredentialPolicy
+        ]
+    ]
+) -> Optional[
+    Union[
+        BearerTokenChallengePolicy,
+        AzureSasCredentialPolicy,
+        SharedKeyCredentialPolicy
+    ]
+]:
+    if hasattr(credential, "get_token"):
+        credential = cast(TokenCredential, credential)
+        return BearerTokenChallengePolicy(
+            credential, STORAGE_OAUTH_SCOPE
+        )
+    if isinstance(credential, SharedKeyCredentialPolicy):
+        return credential
+    if isinstance(credential, AzureSasCredential):
+        return AzureSasCredentialPolicy(credential)
+    if isinstance(credential, AzureNamedKeyCredential):
+        return SharedKeyCredentialPolicy(credential)
+    if credential is not None:
+        raise TypeError("Unsupported credential: {}".format(credential))
+    return None
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_table_client.py` & `azure-data-tables-12.4.3/azure/data/tables/_table_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 import functools
-from typing import Optional, Any, TYPE_CHECKING, Union, List, Dict, Mapping, Iterable, overload, cast
+from typing import Optional, Any, Union, List, Dict, Mapping, Iterable, overload, cast
+
 try:
     from urllib.parse import urlparse, unquote
 except ImportError:
     from urlparse import urlparse  # type: ignore
     from urllib2 import unquote  # type: ignore
 
 from azure.core import MatchConditions
+from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential, TokenCredential
 from azure.core.exceptions import HttpResponseError
 from azure.core.paging import ItemPaged
 from azure.core.tracing.decorator import distributed_trace
 
-from ._deserialize import _convert_to_entity, _trim_service_metadata
+from ._base_client import parse_connection_str, TablesBaseClient
 from ._entity import TableEntity
-from ._error import (
-    _decode_error,
-    _process_table_error,
-    _reprocess_error,
-    _reraise_error,
-    _validate_tablename_error
-)
-from ._generated.models import (
-    SignedIdentifier,
-    TableProperties
+from ._error import _decode_error, _process_table_error, _reprocess_error, _reraise_error, _validate_tablename_error
+from ._generated.models import SignedIdentifier, TableProperties
+from ._serialize import(
+    serialize_iso, _parameter_filter_substitution, _get_match_headers, _add_entity_properties, _prepare_key
 )
-from ._serialize import _get_match_headers, _add_entity_properties, _prepare_key
-from ._base_client import parse_connection_str, TablesBaseClient
-from ._serialize import serialize_iso, _parameter_filter_substitution
-from ._deserialize import deserialize_iso, _return_headers_and_deserialized
+from ._deserialize import deserialize_iso, _return_headers_and_deserialized, _convert_to_entity, _trim_service_metadata
 from ._table_batch import TableBatchOperations, EntityType, TransactionOperationType
-from ._models import (
-    TableEntityPropertiesPaged,
-    UpdateMode,
-    TableAccessPolicy,
-    TableItem
-)
-
-if TYPE_CHECKING:
-    from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential
+from ._models import TableEntityPropertiesPaged, UpdateMode, TableAccessPolicy, TableItem
 
 
 class TableClient(TablesBaseClient):
     """A client to interact with a specific Table in an Azure Tables account.
 
     :ivar str account_name: The name of the Tables account.
     :ivar str table_name: The name of the table.
     :ivar str url: The full URL to the Tables account.
     """
 
-    def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
+    def __init__( # pylint: disable=missing-client-constructor-parameter-credential
         self,
-        endpoint,  # type: str
-        table_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        endpoint: str,
+        table_name: str,
+        *,
+        credential: Optional[Union[AzureSasCredential, AzureNamedKeyCredential, TokenCredential]] = None,
+        **kwargs
+    ) -> None:
         """Create TableClient from a Credential.
 
         :param str endpoint: A URL to an Azure Tables account.
         :param str table_name: The table name.
         :keyword credential:
             The credentials with which to authenticate. This is optional if the
             account URL already has a SAS token. The value can be one of AzureNamedKeyCredential (azure-core),
@@ -78,30 +64,24 @@
         :paramtype api_version: str
 
         :returns: None
         """
         if not table_name:
             raise ValueError("Please specify a table name.")
         self.table_name = table_name
-        super(TableClient, self).__init__(endpoint, **kwargs)
+        super(TableClient, self).__init__(endpoint, credential=credential, **kwargs)
 
     def _format_url(self, hostname):
         """Format the endpoint URL according to the current location
         mode hostname.
         """
         return "{}://{}{}".format(self.scheme, hostname, self._query_str)
 
     @classmethod
-    def from_connection_string(
-        cls,
-        conn_str,  # type: str
-        table_name,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> TableClient
+    def from_connection_string(cls, conn_str: str, table_name: str, **kwargs) -> "TableClient":
         """Create TableClient from a Connection String.
 
         :param str conn_str: A connection string to an Azure Tables account.
         :param str table_name: The table name.
         :returns: A table client.
         :rtype: :class:`~azure.data.tables.TableClient`
 
@@ -110,22 +90,25 @@
             .. literalinclude:: ../samples/sample_create_client.py
                 :start-after: [START create_table_client]
                 :end-before: [END create_table_client]
                 :language: python
                 :dedent: 8
                 :caption: Authenticating a TableServiceClient from a connection_string
         """
-        endpoint, credential = parse_connection_str(
-            conn_str=conn_str, credential=None, keyword_args=kwargs
-        )
+        endpoint, credential = parse_connection_str(conn_str=conn_str, credential=None, keyword_args=kwargs)
         return cls(endpoint, table_name=table_name, credential=credential, **kwargs)
 
     @classmethod
-    def from_table_url(cls, table_url, **kwargs):
-        # type: (str, Any) -> TableClient
+    def from_table_url(
+        cls,
+        table_url: str,
+        *,
+        credential: Optional[Union[AzureNamedKeyCredential, AzureSasCredential]] = None,
+        **kwargs
+    ) -> "TableClient":
         """A client to interact with a specific Table.
 
         :param str table_url: The full URI to the table, including SAS token if used.
         :keyword credential:
             The credentials with which to authenticate. This is optional if the
             account URL already has a SAS token. The value can be one of AzureNamedKeyCredential
             or AzureSasCredential from azure-core.
@@ -155,24 +138,19 @@
             account_path,
             parsed_url.query,
         )
         table_name = unquote(table_path[-1])
         if table_name.lower().startswith("tables('"):
             table_name = table_name[8:-2]
         if not table_name:
-            raise ValueError(
-                "Invalid URL. Please provide a URL with a valid table name"
-            )
-        return cls(endpoint, table_name=table_name, **kwargs)
+            raise ValueError("Invalid URL. Please provide a URL with a valid table name")
+        return cls(endpoint, table_name=table_name, credential=credential, **kwargs)
 
     @distributed_trace
-    def get_table_access_policy(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> Dict[str, Optional[TableAccessPolicy]]
+    def get_table_access_policy(self, **kwargs) -> Dict[str, Optional[TableAccessPolicy]]:
         """Retrieves details about any stored access policies specified on the table that may be
         used with Shared Access Signatures.
 
         :return: Dictionary of SignedIdentifiers
         :rtype: Dict[str, Optional[:class:`~azure.data.tables.TableAccessPolicy`]]
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
@@ -188,61 +166,53 @@
             _process_table_error(error, table_name=self.table_name)
         output = {}  # type: Dict[str, Optional[TableAccessPolicy]]
         for identifier in cast(List[SignedIdentifier], identifiers):
             if identifier.access_policy:
                 output[identifier.id] = TableAccessPolicy(
                     start=deserialize_iso(identifier.access_policy.start),
                     expiry=deserialize_iso(identifier.access_policy.expiry),
-                    permission=identifier.access_policy.permission
+                    permission=identifier.access_policy.permission,
                 )
             else:
                 output[identifier.id] = None
         return output
 
     @distributed_trace
     def set_table_access_policy(
-        self,
-        signed_identifiers,  # type: Dict[str, Optional[TableAccessPolicy]]
-        **kwargs
-    ):
-        # type: (...) -> None
+        self, signed_identifiers: Dict[str, Optional[TableAccessPolicy]], **kwargs
+    ) -> None:
         """Sets stored access policies for the table that may be used with Shared Access Signatures.
 
         :param signed_identifiers: Access policies to set for the table
         :type signed_identifiers: Dict[str, Optional[:class:`~azure.data.tables.TableAccessPolicy`]]
         :return: None
         :rtype: None
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         identifiers = []
         for key, value in signed_identifiers.items():
             payload = None
             if value:
                 payload = TableAccessPolicy(
-                    start=serialize_iso(value.start),
-                    expiry=serialize_iso(value.expiry),
-                    permission=value.permission
+                    start=serialize_iso(value.start), expiry=serialize_iso(value.expiry), permission=value.permission
                 )
             identifiers.append(SignedIdentifier(id=key, access_policy=payload))
         try:
             self._client.table.set_access_policy(
                 table=self.table_name, table_acl=identifiers or None, **kwargs  # type: ignore
             )
         except HttpResponseError as error:
             try:
                 _process_table_error(error, table_name=self.table_name)
             except HttpResponseError as table_error:
                 _reprocess_error(table_error, identifiers=identifiers)
                 raise
 
     @distributed_trace
-    def create_table(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> TableItem
+    def create_table(self, **kwargs) -> TableItem:
         """Creates a new table under the current account.
 
         :return: A TableItem representing the created table.
         :rtype: :class:`~azure.data.tables.TableItem`
         :raises: :class:`~azure.core.exceptions.ResourceExistsError` If the entity already exists
 
         .. admonition:: Example:
@@ -262,18 +232,15 @@
                 _process_table_error(error, table_name=self.table_name)
             except HttpResponseError as decoded_error:
                 _reprocess_error(decoded_error)
                 raise
         return TableItem(name=result.table_name)  # type: ignore
 
     @distributed_trace
-    def delete_table(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def delete_table(self, **kwargs) -> None:
         """Deletes the table under the current account. No error will be raised
         if the table does not exist
 
         :return: None
         :rtype: None
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
 
@@ -294,26 +261,23 @@
             try:
                 _process_table_error(error, table_name=self.table_name)
             except HttpResponseError as decoded_error:
                 _reprocess_error(decoded_error)
                 raise
 
     @overload
-    def delete_entity(self, partition_key, row_key, **kwargs):
-        # type: (str, str, Any) -> None
+    def delete_entity(self, partition_key: str, row_key: str, **kwargs) -> None:
         pass
 
     @overload
-    def delete_entity(self, entity, **kwargs):
-        # type: (Union[TableEntity, Mapping[str, Any]], Any) -> None
+    def delete_entity(self, entity: Union[TableEntity, Mapping[str, Any]], **kwargs) -> None:
         pass
 
     @distributed_trace
-    def delete_entity(self, *args, **kwargs):
-        # type: (Union[TableEntity, str], Any) -> None
+    def delete_entity(self, *args: Union[TableEntity, str], **kwargs) -> None:
         """Deletes the specified entity in a table. No error will be raised if
         the entity or PartitionKey-RowKey pairing is not found.
 
         :param str partition_key: The partition key of the entity.
         :param str row_key: The row key of the entity.
         :param entity: The entity to delete
         :type entity: Union[TableEntity, Mapping[str, str]]
@@ -332,19 +296,19 @@
                 :start-after: [START delete_entity]
                 :end-before: [END delete_entity]
                 :language: python
                 :dedent: 12
                 :caption: Deleting an entity of a Table
         """
         try:
-            entity = kwargs.pop('entity', None)
+            entity = kwargs.pop("entity", None)
             if not entity:
                 entity = args[0]
-            partition_key = entity['PartitionKey']
-            row_key = entity['RowKey']
+            partition_key = entity["PartitionKey"]
+            row_key = entity["RowKey"]
         except (TypeError, IndexError):
             partition_key = kwargs.pop('partition_key', None)
             if partition_key is None:
                 partition_key = args[0]
             row_key = kwargs.pop("row_key", None)
             if row_key is None:
                 row_key = args[1]
@@ -371,20 +335,15 @@
             )
         except HttpResponseError as error:
             if error.status_code == 404:
                 return
             _process_table_error(error, table_name=self.table_name)
 
     @distributed_trace
-    def create_entity(
-        self,
-        entity,  # type: EntityType
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Dict[str,str]
+    def create_entity(self, entity: EntityType, **kwargs) -> Dict[str, str]:
         """Insert entity in a table.
 
         :param entity: The properties for the table entity.
         :type entity: Union[TableEntity, Mapping[str, Any]]
         :return: Dictionary mapping operation metadata returned from the service
         :rtype: Dict[str,str]
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
@@ -414,21 +373,15 @@
                 if entity.get("RowKey") is None:
                     raise ValueError("RowKey must be present in an entity")
             _validate_tablename_error(decoded, self.table_name)
             _reraise_error(error)
         return _trim_service_metadata(metadata, content=content)  # type: ignore
 
     @distributed_trace
-    def update_entity(
-        self,
-        entity,  # type: EntityType
-        mode=UpdateMode.MERGE,  # type: UpdateMode
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Dict[str,str]
+    def update_entity(self, entity: EntityType, mode: UpdateMode = UpdateMode.MERGE, **kwargs) -> Dict[str, str]:
         """Update entity in a table.
 
         :param entity: The properties for the table entity.
         :type entity: :class:`~azure.data.tables.TableEntity` or Dict[str,str]
         :param mode: Merge or Replace entity
         :type mode: :class:`~azure.data.tables.UpdateMode`
         :keyword str etag: Etag of the entity
@@ -489,18 +442,15 @@
             else:
                 raise ValueError("Mode type '{}' is not supported.".format(mode))
         except HttpResponseError as error:
             _process_table_error(error, table_name=self.table_name)
         return _trim_service_metadata(metadata, content=content)  # type: ignore
 
     @distributed_trace
-    def list_entities(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> ItemPaged[TableEntity]
+    def list_entities(self, **kwargs) -> ItemPaged[TableEntity]:
         """Lists entities in a table.
 
         :keyword int results_per_page: Number of entities returned per service request.
         :keyword select: Specify desired properties of an entity to return.
         :paramtype select: str or List[str]
         :return: ItemPaged[:class:`~azure.data.tables.TableEntity`]
         :rtype: ~azure.core.paging.ItemPaged
@@ -526,20 +476,16 @@
             table=self.table_name,
             results_per_page=top,
             select=user_select,
             page_iterator_class=TableEntityPropertiesPaged,
         )
 
     @distributed_trace
-    def query_entities(  # pylint: disable=line-too-long
-        self,
-        query_filter,
-        **kwargs
-    ):
-        # type: (str, Dict[str, Any]) -> ItemPaged[TableEntity]
+    def query_entities(self, query_filter: str, **kwargs) -> ItemPaged[TableEntity]:
+        # pylint: disable=line-too-long
         """Lists entities in a table.
 
         :param str query_filter: Specify a filter to return certain entities. For more information
          on filter formatting, see the `samples documentation <https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/tables/azure-data-tables/samples#writing-filters>`_.
         :keyword int results_per_page: Number of entities returned per service request.
         :keyword select: Specify desired properties of an entity to return.
         :paramtype select: str or List[str]
@@ -555,17 +501,15 @@
                 :start-after: [START query_entities]
                 :end-before: [END query_entities]
                 :language: python
                 :dedent: 8
                 :caption: Query entities held within a table
         """
         parameters = kwargs.pop("parameters", None)
-        query_filter = _parameter_filter_substitution(
-            parameters, query_filter  # type: ignore
-        )
+        query_filter = _parameter_filter_substitution(parameters, query_filter)  # type: ignore
         top = kwargs.pop("results_per_page", None)
         user_select = kwargs.pop("select", None)
         if user_select and not isinstance(user_select, str):
             user_select = ",".join(user_select)  # type: ignore
 
         command = functools.partial(self._client.table.query_entities, **kwargs)
         return ItemPaged(
@@ -574,21 +518,15 @@
             results_per_page=top,
             filter=query_filter,
             select=user_select,
             page_iterator_class=TableEntityPropertiesPaged,
         )
 
     @distributed_trace
-    def get_entity(
-        self,
-        partition_key,  # type: str
-        row_key,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> TableEntity
+    def get_entity(self, partition_key: str, row_key: str, **kwargs) -> TableEntity:
         """Get a single entity in a table.
 
         :param partition_key: The partition key of the entity.
         :type partition_key: str
         :param row_key: The row key of the entity.
         :type row_key: str
         :keyword select: Specify desired properties of an entity to return.
@@ -618,21 +556,15 @@
                 **kwargs
             )
         except HttpResponseError as error:
             _process_table_error(error, table_name=self.table_name)
         return _convert_to_entity(entity)
 
     @distributed_trace
-    def upsert_entity(
-        self,
-        entity,  # type: EntityType
-        mode=UpdateMode.MERGE,  # type: UpdateMode
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Dict[str,str]
+    def upsert_entity(self, entity: EntityType, mode: UpdateMode = UpdateMode.MERGE, **kwargs) -> Dict[str, str]:
         """Update/Merge or Insert entity into table.
 
         :param entity: The properties for the table entity.
         :type entity: :class:`~azure.data.tables.TableEntity` or Dict[str,str]
         :param mode: Merge or Replace entity
         :type mode: :class:`~azure.data.tables.UpdateMode`
         :return: Dictionary mapping operation metadata returned from the service
@@ -680,19 +612,16 @@
                     )
                 )
         except HttpResponseError as error:
             _process_table_error(error, table_name=self.table_name)
         return _trim_service_metadata(metadata, content=content)  # type: ignore
 
     def submit_transaction(
-        self,
-        operations,  # type: Iterable[TransactionOperationType]
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> List[Mapping[str, Any]]
+        self, operations: Iterable[TransactionOperationType], **kwargs
+    ) -> List[Mapping[str, Any]]:
         """Commit a list of operations as a single transaction.
 
         If any one of these operations fails, the entire transaction will be rejected.
 
         :param operations: The list of operations to commit in a transaction. This should be an iterable of
          tuples containing an operation name, the entity on which to operate, and optionally, a dict of additional
          kwargs for that operation. For example::
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_deserialize.py` & `azure-data-tables-12.4.3/azure/data/tables/_deserialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,26 +42,23 @@
         return None
     try:
         return value.value
     except AttributeError:
         return value
 
 
-def _from_entity_binary(value):
-    # type: (str) -> EntityProperty
+def _from_entity_binary(value: str) -> bytes:
     return _decode_base64_to_bytes(value)
 
 
-def _from_entity_int32(value):
-    # type: (str) -> int
+def _from_entity_int32(value: str) -> int:
     return int(value)
 
 
-def _from_entity_int64(value):
-    # type: (str) -> EntityProperty
+def _from_entity_int64(value: str) -> EntityProperty:
     return EntityProperty(int(value), EdmType.INT64)
 
 
 def _from_entity_datetime(value):
     # Cosmos returns this with a decimal point that throws an error on deserialization
     cleaned_value = clean_up_dotnet_timestamps(value)
     try:
@@ -97,16 +94,15 @@
     return _from_entity_datetime(value)
 
 
 def _from_entity_guid(value):
     return UUID(value)
 
 
-def _from_entity_str(value):
-    # type: (Union[str, bytes]) -> str
+def _from_entity_str(value: Union[str, bytes]) -> str:
     if isinstance(value, six.binary_type):
         return value.decode('utf-8')
     return value
 
 
 _EDM_TYPES = [
     EdmType.BINARY,
@@ -225,15 +221,15 @@
 
     return None
 
 
 def _extract_continuation_token(continuation_token):
     """Extract list entity continuation headers from token.
 
-    :param dict(str,str) continuation_token: The listing continuation token.
+    :param Dict(str,str) continuation_token: The listing continuation token.
     :returns: The next partition key and next row key in a tuple
     :rtype: (str,str)
     """
     if not continuation_token:
         return None, None
     try:
         return continuation_token.get("PartitionKey"), continuation_token.get("RowKey")
@@ -258,16 +254,15 @@
 
 def _return_context_and_deserialized(
     response, deserialized, response_headers
 ):  # pylint: disable=unused-argument
     return response.context['location_mode'], deserialized, response_headers
 
 
-def _trim_service_metadata(metadata, content=None):
-    # type: (Dict[str, str], Optional[Dict[str, Any]]) -> Dict[str, Any]
+def _trim_service_metadata(metadata: Dict[str, str], content: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
     result = {
         "date": metadata.pop("date", None),
         "etag": metadata.pop("etag", None),
         "version": metadata.pop("version", None),
     }
     preference = metadata.pop('preference_applied', None)
     if preference:
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_constants.py` & `azure-data-tables-12.4.3/azure/data/tables/_constants.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/__init__.py` & `azure-data-tables-12.4.3/azure/data/tables/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_sdk_moniker.py` & `azure-data-tables-12.4.3/azure/data/tables/_sdk_moniker.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_common_conversion.py` & `azure-data-tables-12.4.3/azure/data/tables/_common_conversion.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_models.py` & `azure-data-tables-12.4.3/azure/data/tables/_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Dict, List
+from typing import Any, Dict, List
 
 from azure.core import CaseInsensitiveEnumMeta
 from azure.core.exceptions import HttpResponseError
 from azure.core.paging import PageIterator
-# from azure.core import CaseInsensitiveEnumMeta
-# from six import with_metaclass
-
+from ._generated.models import TableQueryResponse
 from ._generated.models import TableServiceStats as GenTableServiceStats
+from ._generated.models import TableServiceProperties as GenTableServiceProperties
 from ._generated.models import AccessPolicy as GenAccessPolicy
 from ._generated.models import Logging as GeneratedLogging
 from ._generated.models import Metrics as GeneratedMetrics
 from ._generated.models import RetentionPolicy as GeneratedRetentionPolicy
 from ._generated.models import CorsRule as GeneratedCorsRule
 from ._deserialize import (
     _convert_to_entity,
     _return_context_and_deserialized,
     _extract_continuation_token,
 )
 from ._error import _process_table_error
 from ._constants import NEXT_PARTITION_KEY, NEXT_ROW_KEY, NEXT_TABLE_NAME
 
-if TYPE_CHECKING:
-    from ._generated.models import TableQueryResponse
-    from ._generated.models import TableServiceProperties as GenTableServiceProperties
-
 
 class TableAccessPolicy(GenAccessPolicy):
     """Access Policy class used by the set and get access policy methods.
 
     A stored access policy can specify the start time, expiry time, and
     permissions for the Shared Access Signatures with which it's associated.
     Depending on how you want to control access to your resource, you can
@@ -74,16 +69,15 @@
     :paramtype start: ~datetime.datetime or str
     """
     def __init__(self, **kwargs):  # pylint: disable=super-init-not-called
         self.start = kwargs.get('start')
         self.expiry = kwargs.get('expiry')
         self.permission = kwargs.get('permission')
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return "TableAccessPolicy(start={}, expiry={}, permission={})".format(
             self.start, self.expiry, self.permission
         )[1024:]
 
 
 class TableAnalyticsLogging(GeneratedLogging):
     """Azure Analytics Logging settings.
@@ -94,16 +88,15 @@
     :keyword bool delete: Required. Indicates whether all delete requests should be logged.
     :keyword bool read: Required. Indicates whether all read requests should be logged.
     :keyword bool write: Required. Indicates whether all write requests should be logged.
     :keyword ~azure.data.tables.TableRetentionPolicy retention_policy: Required.
         The retention policy for the metrics.
     """
 
-    def __init__(self, **kwargs):  # pylint: disable=super-init-not-called
-        # type: (Any)-> None
+    def __init__(self, **kwargs) -> None:  # pylint: disable=super-init-not-called
         self.version = kwargs.get("version", u"1.0")
         self.delete = kwargs.get("delete", False)
         self.read = kwargs.get("read", False)
         self.write = kwargs.get("write", False)
         self.retention_policy = kwargs.get("retention_policy") or TableRetentionPolicy()
 
     @classmethod
@@ -116,16 +109,15 @@
             read=generated.read,
             write=generated.write,
             retention_policy=TableRetentionPolicy._from_generated(  # pylint: disable=protected-access
                 generated.retention_policy
             )
         )
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return "TableAnalyticsLogging(version={}, delete={}, read={}, write={}, retention_policy={})".format(
             self.version, self.delete, self.read, self.write, self.retention_policy
         )[1024:]
 
 
 class TableMetrics(GeneratedMetrics):
     """A summary of request statistics grouped by API in hour or minute aggregates.
@@ -136,24 +128,22 @@
     :keyword bool enabled: Required. Indicates whether metrics are enabled for the service.
     :keyword bool include_apis: Indicates whether metrics should generate summary
         statistics for called API operations.
     :keyword ~azure.data.tables.TableRetentionPolicy retention_policy: Required.
         The retention policy for the metrics.
     """
 
-    def __init__(self, **kwargs):  # pylint: disable=super-init-not-called
-        # type: (Any) -> None
+    def __init__(self, **kwargs) -> None:  # pylint: disable=super-init-not-called
         self.version = kwargs.get("version", u"1.0")
         self.enabled = kwargs.get("enabled", False)
         self.include_apis = kwargs.get("include_apis")
         self.retention_policy = kwargs.get("retention_policy") or TableRetentionPolicy()
 
     @classmethod
-    def _from_generated(cls, generated):
-        # type: (...) -> TableMetrics
+    def _from_generated(cls, generated) -> 'TableMetrics':
         """A summary of request statistics grouped by API in hour or minute aggregates.
 
         :param TableMetrics generated: generated Metrics
         """
         if not generated:
             return cls()
         return cls(
@@ -161,24 +151,22 @@
             enabled=generated.enabled,
             include_apis=generated.include_apis,
             retention_policy=TableRetentionPolicy._from_generated(  # pylint: disable=protected-access
                 generated.retention_policy
             )
         )
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return "TableMetrics(version={}, enabled={}, include_apis={}, retention_policy={})".format(
             self.version, self.enabled, self.include_apis, self.retention_policy
         )[1024:]
 
 
 class TableRetentionPolicy(GeneratedRetentionPolicy):
-    def __init__(self, **kwargs):  # pylint: disable=super-init-not-called
-        # type: (Any) -> None
+    def __init__(self, **kwargs) -> None:  # pylint: disable=super-init-not-called
         """The retention policy which determines how long the associated data should
         persist.
 
         All required parameters must be populated in order to send to Azure.
 
         :keyword bool enabled: Required. Indicates whether a retention policy is enabled
             for the storage service. Default value is False.
@@ -188,72 +176,64 @@
         """
         self.enabled = kwargs.get('enabled', False)
         self.days = kwargs.get('days')
         if self.enabled and (self.days is None):
             raise ValueError("If policy is enabled, 'days' must be specified.")
 
     @classmethod
-    def _from_generated(cls, generated, **kwargs):  # pylint: disable=unused-argument
-        # type: (GeneratedRetentionPolicy, Dict[str, Any]) -> TableRetentionPolicy
+    def _from_generated(cls, generated: GeneratedRetentionPolicy) -> 'TableRetentionPolicy':
         """The retention policy which determines how long the associated data should
         persist.
 
         All required parameters must be populated in order to send to Azure.
 
         :param TableRetentionPolicy generated: Generated Retention Policy
         """
 
         if not generated:
             return cls()
         return cls(
             enabled=generated.enabled,
             days=generated.days,
         )
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return "TableRetentionPolicy(enabled={}, days={})".format(self.enabled, self.days)[1024:]
 
 
 class TableCorsRule(object):
     """CORS is an HTTP feature that enables a web application running under one
     domain to access resources in another domain. Web browsers implement a
     security restriction known as same-origin policy that prevents a web page
     from calling APIs in a different domain; CORS provides a secure way to
     allow one domain (the origin domain) to call APIs in another domain.
 
     All required parameters must be populated in order to send to Azure.
 
-    :param list[str] allowed_origins:
+    :param List[str] allowed_origins:
         A list of origin domains that will be allowed via CORS, or "*" to allow
         all domains. The list of must contain at least one entry. Limited to 64
         origin domains. Each allowed origin can have up to 256 characters.
-    :param list[str] allowed_methods:
+    :param List[str] allowed_methods:
         A list of HTTP methods that are allowed to be executed by the origin.
         The list of must contain at least one entry. For Azure Storage,
         permitted methods are DELETE, GET, HEAD, MERGE, POST, OPTIONS or PUT.
     :keyword int max_age_in_seconds:
         The number of seconds that the client/browser should cache a
         pre-flight response.
-    :keyword list[str] exposed_headers:
+    :keyword List[str] exposed_headers:
         Defaults to an empty list. A list of response headers to expose to CORS
         clients. Limited to 64 defined headers and two prefixed headers. Each
         header can be up to 256 characters.
-    :keyword list[str] allowed_headers:
+    :keyword List[str] allowed_headers:
         Defaults to an empty list. A list of headers allowed to be part of
         the cross-origin request. Limited to 64 defined headers and 2 prefixed
         headers. Each header can be up to 256 characters.
     """
 
-    def __init__(
-        self,
-        allowed_origins,  # type: List[str]
-        allowed_methods,  # type: List[str]
-        **kwargs  # type: Any
-    ):
-        # type: (...)-> None
+    def __init__(self, allowed_origins: List[str], allowed_methods: List[str], **kwargs) -> None:
         self.allowed_origins = allowed_origins
         self.allowed_methods = allowed_methods
         self.allowed_headers = kwargs.get("allowed_headers", [])
         self.exposed_headers = kwargs.get("exposed_headers", [])
         self.max_age_in_seconds = kwargs.get("max_age_in_seconds", 0)
 
     def _to_generated(self):
@@ -273,16 +253,15 @@
             generated.allowed_origins.split(','),
             generated.allowed_methods.split(','),
             allowed_headers=allowedheaders,
             exposed_headers=exposedheaders,
             max_age_in_seconds=generated.max_age_in_seconds,
         )
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return "TableCorsRules(allowed_origins={}, allowed_methods={}, allowed_headers={}, exposed_headers={}, max_age_in_seconds={})".format(  # pylint: disable=line-too-long
             self.allowed_origins, self.allowed_methods, self.allowed_headers, self.exposed_headers, self.max_age_in_seconds  # pylint: disable=line-too-long
         )[1024:]
 
 
 class TablePropertiesPaged(PageIterator):
     """An iterable of Table properties.
@@ -379,107 +358,94 @@
                 "PartitionKey": self._headers[NEXT_PARTITION_KEY],
                 "RowKey": self._headers[NEXT_ROW_KEY],
             }
         return next_entity or None, props_list
 
 
 class TableSasPermissions(object):
-    def __init__(self, **kwargs):
-        # type: (Any) -> None
+    def __init__(self, **kwargs) -> None:
         """
         :keyword bool read:
             Get entities and query entities.
         :keyword bool add:
             Add entities. Add and Update permissions are required for upsert operations.
         :keyword bool update:
             Update entities. Add and Update permissions are required for upsert operations.
         :keyword bool delete:
             Delete entities.
         """
-        _str = kwargs.pop('_str', "") or ""
-        self.read = kwargs.pop("read", False) or ("r" in _str)
-        self.add = kwargs.pop("add", False) or ("a" in _str)
-        self.update = kwargs.pop("update", False) or ("u" in _str)
-        self.delete = kwargs.pop("delete", False) or ("d" in _str)
+        self._str = kwargs.pop('_str', "") or ""
+        self.read = kwargs.pop("read", False) or ("r" in self._str)
+        self.add = kwargs.pop("add", False) or ("a" in self._str)
+        self.update = kwargs.pop("update", False) or ("u" in self._str)
+        self.delete = kwargs.pop("delete", False) or ("d" in self._str)
 
-    def __or__(self, other):
-        # type: (TableSasPermissions) -> TableSasPermissions
+    def __or__(self, other: 'TableSasPermissions') -> 'TableSasPermissions':
         """
         :param other:
         :type other: :class:`~azure.data.tables.TableSasPermissions`
         """
         return TableSasPermissions(_str=str(self) + str(other))
 
-    def __add__(self, other):
-        # type: (TableSasPermissions) -> TableSasPermissions
+    def __add__(self, other: 'TableSasPermissions') -> 'TableSasPermissions':
         """
         :param other:
         :type other: :class:`~azure.data.tables.TableSasPermissions`
         """
         return TableSasPermissions(_str=str(self) + str(other))
 
-    def __str__(self):
-        # type: () -> str
+    def __str__(self) -> str:
         return (
             ("r" if self.read else "")
             + ("a" if self.add else "")
             + ("u" if self.update else "")
             + ("d" if self.delete else "")
         )
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return "TableSasPermissions(read={}, add={}, update={}, delete={})".format(
             self.read, self.add, self.update, self.delete
         )[1024:]
 
     @classmethod
-    def from_string(
-        cls,
-        permission,
-        **kwargs
-    ):
-        # Type: (str, Dict[str, Any]) -> AccountSasPermissions
-        """Create AccountSasPermissions from a string.
+    def from_string(cls, permission: str, **kwargs) -> 'TableSasPermissions':
+        """Create TableSasPermissions from a string.
 
         To specify read, write, delete, etc. permissions you need only to
         include the first letter of the word in the string. E.g. for read and write
         permissions you would provide a string "rw".
 
         :param str permission: Specify permissions in
             the string with the first letter of the word.
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An AccountSasPermissions object
-        :rtype: :class:`~azure.data.tables.AccountSasPermissions`
+        :return: An TableSasPermissions object
+        :rtype: :class:`~azure.data.tables.TableSasPermissions`
         """
         p_read = "r" in permission
         p_add = "a" in permission
         p_delete = "d" in permission
         p_update = "u" in permission
 
         parsed = cls(
             **dict(kwargs, read=p_read, add=p_add, delete=p_delete, update=p_update)
         )
         parsed._str = permission  # pylint: disable=protected-access,attribute-defined-outside-init
         return parsed
 
 
-def service_stats_deserialize(generated):
-    # type: (GenTableServiceStats) -> Dict[str, Any]
+def service_stats_deserialize(generated: GenTableServiceStats) -> Dict[str, Any]:
     """Deserialize a ServiceStats objects into a dict."""
     return {
         "geo_replication": {
             "status": generated.geo_replication.status,  # type: ignore
             "last_sync_time": generated.geo_replication.last_sync_time,  # type: ignore
         }
     }
 
 
-def service_properties_deserialize(generated):
-    # type: (GenTableServiceProperties) -> Dict[str, Any]
+def service_properties_deserialize(generated: GenTableServiceProperties) -> Dict[str, Any]:
     """Deserialize a ServiceProperties objects into a dict."""
     return {
         "analytics_logging": TableAnalyticsLogging._from_generated(generated.logging),  # pylint: disable=protected-access
         "hour_metrics": TableMetrics._from_generated(  # pylint: disable=protected-access
             generated.hour_metrics
         ),
         "minute_metrics": TableMetrics._from_generated(  # pylint: disable=protected-access
@@ -496,29 +462,26 @@
     """
     Represents an Azure TableItem.
     Returned by TableServiceClient.list_tables and TableServiceClient.query_tables.
 
     :ivar str name: The name of the table.
     """
 
-    def __init__(self, name):
-        # type: (str) -> None
+    def __init__(self, name: str) -> None:
         """
         :param str name: Name of the Table
         """
         self.name = name
 
     # TODO: TableQueryResponse is not the correct type
     @classmethod
-    def _from_generated(cls, generated, **kwargs):  # pylint: disable=unused-argument
-        # type: (TableQueryResponse, Any) -> TableItem
+    def _from_generated(cls, generated: TableQueryResponse, **kwargs) -> 'TableItem':  # pylint: disable=unused-argument
         return cls(generated.table_name)  # type: ignore
 
-    def __repr__(self):
-        # type: () -> str
+    def __repr__(self) -> str:
         return "TableItem(name={})".format(self.name)[1024:]
 
 
 class TablePayloadFormat(object):
     """
     Specifies the accepted content type of the response payload. More information
     can be found here: https://msdn.microsoft.com/en-us/library/azure/dn535600.aspx
@@ -571,26 +534,24 @@
     :keyword bool service:
         Access to service-level APIs (e.g., Get/Set Service Properties,
         Get Service Stats, List Tables)
     :keyword bool object:
         Access to object-level APIs for tables (e.g. Get/Create/Query Entity etc.)
     """
 
-    def __init__(self, **kwargs):
-        # type: (Any) -> None
+    def __init__(self, **kwargs) -> None:
         self.service = kwargs.get('service', False)
         self.object = kwargs.get('object', False)
         self._str = ("s" if self.service else "") + ("o" if self.object else "")
 
     def __str__(self):
         return self._str
 
     @classmethod
-    def from_string(cls, string):
-        # type: (str) -> ResourceTypes
+    def from_string(cls, string: str) -> 'ResourceTypes':
         """Create a ResourceTypes from a string.
 
         To specify service, container, or object you need only to
         include the first letter of the word in the string. E.g. service and container,
         you would provide a string "sc".
 
         :param str string: Specify service, container, or object in
@@ -652,16 +613,15 @@
             + ("p" if self.process else "")
         )
 
     def __str__(self):
         return self._str
 
     @classmethod
-    def from_string(cls, permission, **kwargs):
-        # type: (str, Dict[str, Any]) -> AccountSasPermissions
+    def from_string(cls, permission: str, **kwargs) -> 'AccountSasPermissions':
         """Create AccountSasPermissions from a string.
 
         To specify read, write, delete, etc. permissions you need only to
         include the first letter of the word in the string. E.g. for read and write
         permissions you would provide a string "rw".
 
         :param permission: Specify permissions in the string with the first letter of the word.
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_error.py` & `azure-data-tables-12.4.3/azure/data/tables/_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,39 +200,43 @@
         raise storage_error
     if table_name:
         _validate_tablename_error(decoded_error, table_name)
     _reraise_error(decoded_error)
 
 
 def _reprocess_error(decoded_error, identifiers=None):
-    error_code = decoded_error.error_code
-    message = decoded_error.message
-    authentication_failed = "Server failed to authenticate the request"
-    invalid_input = "The number of keys specified in the URI does not match number of key properties for the resource"
-    invalid_query_parameter_value = "Value for one of the query parameters specified in the request URI is invalid"
-    invalid_url = "Request url is invalid"
-    properties_need_value = "The values are not specified for all properties in the entity"
-    table_does_not_exist = "The table specified does not exist"
-    if (error_code == "AuthenticationFailed" and authentication_failed in message or # pylint: disable=too-many-boolean-expressions
-        error_code == "InvalidInput" and invalid_input in message or
-        error_code == "InvalidInput" and invalid_url in message or
-        error_code == "InvalidQueryParameterValue" and invalid_query_parameter_value in message or
-        error_code == "PropertiesNeedValue" and properties_need_value in message or
-        error_code =="TableNotFound" and table_does_not_exist in message
-        ):
-        args_list = list(decoded_error.args)
-        args_list[0] += "\nA possible cause of this error could be that the account URL used to"\
-            "create the Client includes an invalid path, for example the table name. Please check your account URL."
-        decoded_error.args = tuple(args_list)
-
-    if (identifiers is not None and error_code == "InvalidXmlDocument" and len(identifiers) > 5):
-        raise ValueError(
-            "Too many access policies provided. The server does not support setting more than 5 access policies"\
-                "on a single resource."
-            )
+    try:
+        error_code = decoded_error.error_code
+        message = decoded_error.message
+        authentication_failed = "Server failed to authenticate the request"
+        invalid_input = "The number of keys specified in the URI does not match number of key properties "\
+            "for the resource"
+        invalid_query_parameter_value = "Value for one of the query parameters specified in the request URI is invalid"
+        invalid_url = "Request url is invalid"
+        properties_need_value = "The values are not specified for all properties in the entity"
+        table_does_not_exist = "The table specified does not exist"
+        if (error_code == "AuthenticationFailed" and authentication_failed in message or # pylint: disable=too-many-boolean-expressions
+            error_code == "InvalidInput" and invalid_input in message or
+            error_code == "InvalidInput" and invalid_url in message or
+            error_code == "InvalidQueryParameterValue" and invalid_query_parameter_value in message or
+            error_code == "PropertiesNeedValue" and properties_need_value in message or
+            error_code =="TableNotFound" and table_does_not_exist in message
+            ):
+            args_list = list(decoded_error.args)
+            args_list[0] += "\nA possible cause of this error could be that the account URL used to"\
+                "create the Client includes an invalid path, for example the table name. Please check your account URL."
+            decoded_error.args = tuple(args_list)
+
+        if (identifiers is not None and error_code == "InvalidXmlDocument" and len(identifiers) > 5):
+            raise ValueError(
+                "Too many access policies provided. The server does not support setting more than 5 access policies"\
+                    "on a single resource."
+                )
+    except AttributeError:
+        raise decoded_error
 
 
 class TableTransactionError(HttpResponseError):
     """There is a failure in the transaction operations.
 
     :ivar int index: If available, the index of the operation in the transaction that caused the error.
      Defaults to 0 in the case where an index was not provided, or the error applies across operations.
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_table_service_client.py` & `azure-data-tables-12.4.3/azure/data/tables/_table_service_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 import functools
-from typing import Any, Dict, TYPE_CHECKING
+from typing import Dict
 from azure.core.exceptions import HttpResponseError, ResourceExistsError
 from azure.core.paging import ItemPaged
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.pipeline import Pipeline
 
 from ._generated.models import TableServiceProperties
 from ._models import (
@@ -20,17 +20,14 @@
 )
 from ._base_client import parse_connection_str, TablesBaseClient, TransportWrapper
 from ._models import LocationMode
 from ._error import _process_table_error, _reprocess_error
 from ._table_client import TableClient
 from ._serialize import _parameter_filter_substitution
 
-if TYPE_CHECKING:
-    from ._models import TableCorsRule, TableMetrics, TableAnalyticsLogging
-
 
 class TableServiceClient(TablesBaseClient):
     """A client to interact with the Table Service at the account level.
 
     This client provides operations to retrieve and configure the account properties
     as well as list, create and delete tables within the account.
     For operations relating to a specific table, a client for this entity
@@ -67,24 +64,22 @@
                 :start-after: [START auth_from_shared_key]
                 :end-before: [END auth_from_shared_key]
                 :language: python
                 :dedent: 8
                 :caption: Authenticating a TableServiceClient from a Shared Account Key
         """
 
-    def _format_url(self, hostname):
-        # type: (str) -> str
+    def _format_url(self, hostname: str) -> str:
         """Format the endpoint URL according to the current location
         mode hostname.
         """
         return "{}://{}{}".format(self.scheme, hostname, self._query_str)
 
     @classmethod
-    def from_connection_string(cls, conn_str, **kwargs):
-        # type: (str, Any) -> TableServiceClient
+    def from_connection_string(cls, conn_str: str, **kwargs) -> 'TableServiceClient':
         """Create TableServiceClient from a connection string.
 
         :param str conn_str: A connection string to an Azure Storage or Cosmos account.
         :returns: A Table service client.
         :rtype: :class:`~azure.data.tables.TableServiceClient`
 
         .. admonition:: Example:
@@ -98,16 +93,15 @@
         """
         endpoint, credential = parse_connection_str(
             conn_str=conn_str, credential=None, keyword_args=kwargs
         )
         return cls(endpoint, credential=credential, **kwargs)
 
     @distributed_trace
-    def get_service_stats(self, **kwargs):
-        # type: (Any) -> Dict[str, object]
+    def get_service_stats(self, **kwargs) -> Dict[str, object]:
         """Retrieves statistics related to replication for the Table service. It is only available on the secondary
         location endpoint when read-access geo-redundant replication is enabled for the account.
 
         :return: Dictionary of service stats
         :rtype: Dict[str, object]
         :raises: :class:`~azure.core.exceptions.HttpResponseError:`
         """
@@ -117,16 +111,15 @@
                 timeout=timeout, use_location=LocationMode.SECONDARY, **kwargs
             )
         except HttpResponseError as error:
             _process_table_error(error)
         return service_stats_deserialize(stats)
 
     @distributed_trace
-    def get_service_properties(self, **kwargs):
-        # type: (Any) -> Dict[str, object]
+    def get_service_properties(self, **kwargs) -> Dict[str, object]:
         """Gets the properties of an account's Table service,
         including properties for Analytics and CORS (Cross-Origin Resource Sharing) rules.
 
         :return: Dictionary of service properties
         :rtype: Dict[str, object]
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
@@ -138,16 +131,15 @@
                 _process_table_error(error)
             except HttpResponseError as decoded_error:
                 _reprocess_error(decoded_error)
                 raise
         return service_properties_deserialize(service_props)
 
     @distributed_trace
-    def set_service_properties(self, **kwargs):
-        # type: (Any) -> None
+    def set_service_properties(self, **kwargs) -> None:
         """Sets properties for an account's Table service endpoint,
          including properties for Analytics and CORS (Cross-Origin Resource Sharing) rules.
 
         :keyword analytics_logging: Properties for analytics
         :paramtype analytics_logging: ~azure.data.tables.TableAnalyticsLogging
         :keyword hour_metrics: Hour level metrics
         :paramtype hour_metrics: ~azure.data.tables.TableMetrics
@@ -174,16 +166,15 @@
             try:
                 _process_table_error(error)
             except HttpResponseError as decoded_error:
                 _reprocess_error(decoded_error)
                 raise
 
     @distributed_trace
-    def create_table(self, table_name, **kwargs):
-        # type: (str, Any) -> TableClient
+    def create_table(self, table_name: str, **kwargs) -> TableClient:
         """Creates a new table under the current account.
 
         :param table_name: The Table name.
         :type table_name: str
         :return: TableClient
         :rtype: :class:`~azure.data.tables.TableClient`
         :raises: :class:`~azure.core.exceptions.ResourceExistsError`
@@ -198,16 +189,15 @@
                 :caption: Creating a table from the TableServiceClient object
         """
         table = self.get_table_client(table_name=table_name)
         table.create_table(**kwargs)
         return table
 
     @distributed_trace
-    def create_table_if_not_exists(self, table_name, **kwargs):
-        # type: (str, Any) -> TableClient
+    def create_table_if_not_exists(self, table_name: str, **kwargs) -> TableClient:
         """Creates a new table if it does not currently exist.
         If the table currently exists, the current table is
         returned.
 
         :param table_name: The Table name.
         :type table_name: str
         :return: TableClient
@@ -227,16 +217,15 @@
         try:
             table.create_table(**kwargs)
         except ResourceExistsError:
             pass
         return table
 
     @distributed_trace
-    def delete_table(self, table_name, **kwargs):
-        # type: (str, Any) -> None
+    def delete_table(self, table_name: str, **kwargs) -> None:
         """Deletes the table under the current account. No error will be raised
         if the given table is not found.
 
         :param table_name: The Table name.
         :type table_name: str
         :return: None
         :rtype: None
@@ -251,16 +240,15 @@
                 :dedent: 8
                 :caption: Deleting a table from the TableServiceClient object
         """
         table = self.get_table_client(table_name=table_name)
         table.delete_table(**kwargs)
 
     @distributed_trace
-    def query_tables(self, query_filter, **kwargs):
-        # type: (str, Any) -> ItemPaged[TableItem]
+    def query_tables(self, query_filter: str, **kwargs) -> ItemPaged[TableItem]:
         """Queries tables under the given account.
 
         :param str query_filter: Specify a filter to return certain tables.
         :keyword int results_per_page: Number of tables per page in return ItemPaged
         :keyword parameters: Dictionary for formatting query with additional, user defined parameters
         :paramtype parameters:  Dict[str, Any]
         :return: ItemPaged[:class:`~azure.data.tables.TableItem`]
@@ -287,16 +275,15 @@
             command,
             results_per_page=top,
             filter=query_filter,
             page_iterator_class=TablePropertiesPaged,
         )
 
     @distributed_trace
-    def list_tables(self, **kwargs):
-        # type: (Any) -> ItemPaged[TableItem]
+    def list_tables(self, **kwargs) -> ItemPaged[TableItem]:
         """Queries tables under the given account.
 
         :keyword int results_per_page: Number of tables per page in returned ItemPaged
         :return: ItemPaged[:class:`~azure.data.tables.TableItem`]
         :rtype: ~azure.core.paging.ItemPaged
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
 
@@ -314,16 +301,15 @@
         command = functools.partial(self._client.table.query, **kwargs)
         return ItemPaged(
             command,
             results_per_page=top,
             page_iterator_class=TablePropertiesPaged,
         )
 
-    def get_table_client(self, table_name, **kwargs):
-        # type: (str, Any) -> TableClient
+    def get_table_client(self, table_name: str, **kwargs) -> TableClient:
         """Get a client to interact with the specified table.
 
         The table need not already exist.
 
         :param str table_name: The table name
         :returns: A :class:`~azure.data.tables.TableClient` object.
         :rtype: :class:`~azure.data.tables.TableClient`
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_entity.py` & `azure-data-tables-12.4.3/azure/data/tables/_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     """
     An Entity dictionary with additional metadata
 
     """
     _metadata = {}  # type: Dict[str, Any]
 
     @property
-    def metadata(self):
-        # type: () -> Dict[str, Any]
+    def metadata(self) -> Dict[str, Any]:
         """Resets metadata to be a part of the entity
         :return Dict of entity metadata
         :rtype: Dict[str, Any]
         """
         return self._metadata
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_serialize.py` & `azure-data-tables-12.4.3/azure/data/tables/_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     """Duplicate the single quote char to escape."""
     try:
         return keyvalue.replace("'", "''")
     except AttributeError:
         raise TypeError('PartitionKey or RowKey must be of type string.')
 
 
-def _parameter_filter_substitution(parameters, query_filter):
-    # type: (Dict[str, str], str) -> str
+def _parameter_filter_substitution(parameters: Dict[str, str], query_filter: str) -> str:
     """Replace user defined parameter in filter
     :param parameters: User defined parameters
     :param str query_filter: Filter for querying
     """
     if parameters:
         filter_strings = query_filter.split(' ')
         for index, word in enumerate(filter_strings):
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_base_client.py` & `azure-data-tables-12.4.3/azure/data/tables/_base_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,94 +1,87 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import os
-from typing import Dict, Optional, Any, List, Mapping, Union, TYPE_CHECKING
+
 from uuid import uuid4
+from typing import Any, Dict, List, Optional, Mapping, Union
 try:
     from urllib.parse import parse_qs, quote, urlparse
 except ImportError:
     from urlparse import parse_qs, urlparse  # type: ignore
     from urllib2 import quote  # type: ignore
 
-from azure.core.credentials import AzureSasCredential, AzureNamedKeyCredential
+from azure.core.credentials import AzureSasCredential, AzureNamedKeyCredential, TokenCredential
 from azure.core.utils import parse_connection_string
 from azure.core.pipeline.transport import (
     HttpTransport,
     HttpRequest,
 )
 from azure.core.pipeline.policies import (
     RedirectPolicy,
     ContentDecodePolicy,
     ProxyPolicy,
     DistributedTracingPolicy,
     HttpLoggingPolicy,
     UserAgentPolicy,
-    AzureSasCredentialPolicy,
     NetworkTraceLoggingPolicy,
     CustomHookPolicy,
     RequestIdPolicy,
 )
 
 from ._generated import AzureTable
 from ._common_conversion import _is_cosmos_endpoint
 from ._shared_access_signature import QueryStringConstants
 from ._constants import (
-    STORAGE_OAUTH_SCOPE,
     DEFAULT_COSMOS_ENDPOINT_SUFFIX,
     DEFAULT_STORAGE_ENDPOINT_SUFFIX,
 )
 from ._error import (
     RequestTooLargeError,
     TableTransactionError,
     _decode_error,
     _validate_tablename_error
 )
 from ._models import LocationMode
-from ._authentication import BearerTokenChallengePolicy, SharedKeyCredentialPolicy
+from ._authentication import _configure_credential
 from ._policies import (
     CosmosPatchTransformPolicy,
     StorageHeadersPolicy,
     StorageHosts,
     TablesRetryPolicy,
 )
 from ._sdk_moniker import SDK_MONIKER
 
-if TYPE_CHECKING:
-    from azure.core.credentials import TokenCredential
-    from typing import Literal
-
 _SUPPORTED_API_VERSIONS = ["2019-02-02", "2019-07-07", "2020-12-06"]
 # cspell:disable-next-line
 _DEV_CONN_STRING = "DefaultEndpointsProtocol=http;AccountName=devstoreaccount1;AccountKey=Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw==;TableEndpoint=http://127.0.0.1:10002/devstoreaccount1" # pylint: disable=line-too-long
 
 
-def get_api_version(kwargs, default):
-    # type: (Dict[str, Any], Literal["2019-02-02"]) -> Literal["2019-02-02"]
+def get_api_version(kwargs: Dict[str, Any], default: str) -> str:
     api_version = kwargs.pop("api_version", None)
     if api_version and api_version not in _SUPPORTED_API_VERSIONS:
         versions = "\n".join(_SUPPORTED_API_VERSIONS)
         raise ValueError(
             "Unsupported API version '{}'. Please select from:\n{}".format(
                 api_version, versions
             )
         )
     return api_version or default
 
 
 class AccountHostsMixin(object):  # pylint: disable=too-many-instance-attributes
     def __init__(
         self,
-        account_url,  # type: Any
-        credential=None,  # type: Optional[Union[AzureNamedKeyCredential, AzureSasCredential, "TokenCredential"]]
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+        account_url: str,
+        credential: Optional[Union[AzureNamedKeyCredential, AzureSasCredential, TokenCredential]] = None,
+        **kwargs
+    ) -> None:
         try:
             if not account_url.lower().startswith("http"):
                 account_url = "https://" + account_url
         except AttributeError:
             raise ValueError("Account URL must be a string.")
         parsed_url = urlparse(account_url.rstrip("/"))
         if not parsed_url.netloc:
@@ -140,16 +133,15 @@
             if kwargs.get("secondary_hostname"):
                 secondary_hostname = kwargs["secondary_hostname"]
             primary_hostname = (parsed_url.netloc + parsed_url.path).rstrip("/")
             self._hosts = {
                 LocationMode.PRIMARY: primary_hostname,
                 LocationMode.SECONDARY: secondary_hostname,
             }
-        self._credential_policy = None  # type: ignore
-        self._configure_credential(self.credential)  # type: ignore
+
         self._policies = self._configure_policies(hosts=self._hosts, **kwargs)  # type: ignore
         if self._cosmos_endpoint:
             self._policies.insert(0, CosmosPatchTransformPolicy())
 
     @property
     def url(self):
         """The full endpoint URL to this entity, including SAS token if used.
@@ -222,70 +214,55 @@
         :class:`~azure.core.credentials.AzureSasCredential` or
         :class:`~azure.core.credentials.TokenCredential`
     :keyword api_version: Specifies the version of the operation to use for this request. Default value
         is "2019-02-02". Note that overriding this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
+    def __init__( # pylint: disable=missing-client-constructor-parameter-credential
         self,
-        endpoint,  # type: str
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> None
-        credential = kwargs.pop('credential', None)
-        super(TablesBaseClient, self).__init__(endpoint, credential=credential, **kwargs)
+        endpoint: str,
+        *,
+        credential: Optional[Union[AzureSasCredential, AzureNamedKeyCredential, TokenCredential]] = None,
+        **kwargs
+    ) -> None:
+        super(TablesBaseClient, self).__init__(endpoint, credential=credential, **kwargs) # type: ignore
         self._client = AzureTable(
             self.url,
             policies=kwargs.pop('policies', self._policies),
             **kwargs
         )
-        self._client._config.version = get_api_version(kwargs, self._client._config.version)  # pylint: disable=protected-access
+        self._client._config.version = get_api_version(kwargs, self._client._config.version) # type: ignore # pylint: disable=protected-access
 
     def __enter__(self):
         self._client.__enter__()
         return self
 
     def __exit__(self, *args):
         self._client.__exit__(*args)
 
     def _configure_policies(self, **kwargs):
+        credential_policy = _configure_credential(self.credential)
         return [
             RequestIdPolicy(**kwargs),
             StorageHeadersPolicy(**kwargs),
             UserAgentPolicy(sdk_moniker=SDK_MONIKER, **kwargs),
             ProxyPolicy(**kwargs),
-            self._credential_policy,
+            credential_policy,
             ContentDecodePolicy(response_encoding="utf-8"),
             RedirectPolicy(**kwargs),
             StorageHosts(**kwargs),
             TablesRetryPolicy(**kwargs),
             CustomHookPolicy(**kwargs),
             NetworkTraceLoggingPolicy(**kwargs),
             DistributedTracingPolicy(**kwargs),
             HttpLoggingPolicy(**kwargs),
         ]
 
-    def _configure_credential(self, credential):
-        # type: (Any) -> None
-        if hasattr(credential, "get_token"):
-            self._credential_policy = BearerTokenChallengePolicy(  # type: ignore
-                credential, STORAGE_OAUTH_SCOPE
-            )
-        elif isinstance(credential, SharedKeyCredentialPolicy):
-            self._credential_policy = credential  # type: ignore
-        elif isinstance(credential, AzureSasCredential):
-            self._credential_policy = AzureSasCredentialPolicy(credential)  # type: ignore
-        elif isinstance(credential, AzureNamedKeyCredential):
-            self._credential_policy = SharedKeyCredentialPolicy(credential)  # type: ignore
-        elif credential is not None:
-            raise TypeError("Unsupported credential: {}".format(credential))
-
-    def _batch_send(self, table_name, *reqs, **kwargs):
-        # type: (str, List[HttpRequest], Any) -> List[Mapping[str, Any]]
+    def _batch_send(self, table_name: str, *reqs: HttpRequest, **kwargs) -> List[Mapping[str, Any]]:
         """Given a series of request, do a Storage batch call."""
         # Pop it here, so requests doesn't feel bad about additional kwarg
         policies = [StorageHeadersPolicy()]
 
         changeset = HttpRequest("POST", None)  # type: ignore
         changeset.set_multipart_mixed(
             *reqs, policies=policies, boundary="changeset_{}".format(uuid4())  # type: ignore
@@ -330,16 +307,15 @@
                 response=error_parts[0],
                 error_type=TableTransactionError
             )
             _validate_tablename_error(decoded, table_name)
             raise decoded
         return [extract_batch_part_metadata(p) for p in parts]
 
-    def close(self):
-        # type: () -> None
+    def close(self) -> None:
         """This method is to close the sockets opened by the client.
         It need not be used when using with a context manager.
         """
         self._client.close()
 
 
 class TransportWrapper(HttpTransport):
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_policies.py` & `azure-data-tables-12.4.3/azure/data/tables/_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 import time
-from typing import Any, TYPE_CHECKING, Dict
+from typing import Any, Dict
 from wsgiref.handlers import format_date_time
 try:
     from urllib.parse import urlparse
 except ImportError:
     from urlparse import urlparse  # type: ignore
 
 from azure.core.pipeline.policies import (
     HeadersPolicy,
     SansIOHTTPPolicy,
     RetryPolicy,
 )
+from azure.core.pipeline import PipelineRequest
 from azure.core.exceptions import AzureError, ServiceRequestError, ClientAuthenticationError
 
 from ._common_conversion import _transform_patch_to_cosmos_post
 from ._models import LocationMode
 
-if TYPE_CHECKING:
-    from azure.core.pipeline import PipelineRequest
 
-
-def set_next_host_location(settings, request):
-    # type: (Dict[str, Any], PipelineRequest) -> None
+def set_next_host_location(settings: Dict[str, Any], request: PipelineRequest) -> None:
     """
     A function which sets the next host location on the request, if applicable.
     """
     if request.http_request.method not in ['GET', 'HEAD']:
         return
     try:
         if settings["retry_secondary"] and settings["hosts"] and all(settings["hosts"].values()):
@@ -45,31 +42,29 @@
             request.http_request.url = updated.geturl()
     except KeyError:
         pass
 
 
 class StorageHeadersPolicy(HeadersPolicy):
 
-    def on_request(self, request):
-        # type: (PipelineRequest) -> None
+    def on_request(self, request: PipelineRequest) -> None:
         super(StorageHeadersPolicy, self).on_request(request)
 
         # Add required date headers
         current_time = format_date_time(time.time())
         request.http_request.headers["x-ms-date"] = current_time
         request.http_request.headers["Date"] = current_time
 
 
 class StorageHosts(SansIOHTTPPolicy):
     def __init__(self, hosts=None, **kwargs):  # pylint: disable=unused-argument
         self.hosts = hosts
         super(StorageHosts, self).__init__()
 
-    def on_request(self, request):
-        # type: (PipelineRequest) -> None
+    def on_request(self, request: PipelineRequest) -> None:
         request.context.options["hosts"] = self.hosts
         parsed_url = urlparse(request.http_request.url)
 
         # Detect what location mode we're currently requesting with
         location_mode = LocationMode.PRIMARY
         for key, value in self.hosts.items():
             if parsed_url.netloc == value:
@@ -147,38 +142,38 @@
         return should_retry
 
     def configure_retries(self, options):
         """Configures the retry settings.
 
         :param options: keyword arguments from context.
         :return: A dict containing settings and history for retries.
-        :rtype: dict
+        :rtype: Dict
         """
         config = super(TablesRetryPolicy, self).configure_retries(options)
         config["retry_secondary"] = options.pop("retry_to_secondary", self.retry_to_secondary)
         config["mode"] = options.pop("location_mode", LocationMode.PRIMARY)
         config["hosts"] = options.pop("hosts", None)
         return config
 
     def update_context(self, context, retry_settings):
         """Updates retry history in pipeline context.
 
         :param context: The pipeline context.
         :type context: ~azure.core.pipeline.PipelineContext
         :param retry_settings: The retry settings.
-        :type retry_settings: dict
+        :type retry_settings: Dict
         """
         super(TablesRetryPolicy, self).update_context(context, retry_settings)
         context['location_mode'] = retry_settings['mode']
 
     def update_request(self, request, retry_settings):  # pylint:disable=no-self-use
         """Updates the pipeline request before attempting to retry.
 
         :param PipelineRequest request: The outgoing request.
-        :param dict(str, Any) retry_settings: The current retry context settings.
+        :param Dict(str, Any) retry_settings: The current retry context settings.
         """
         set_next_host_location(retry_settings, request)
 
     def send(self, request):
         """Sends the PipelineRequest object to the next policy. Uses retry settings if necessary.
 
         :param request: The PipelineRequest object
@@ -231,11 +226,10 @@
         self.update_context(response.context, retry_settings)
         return response
 
 
 class CosmosPatchTransformPolicy(SansIOHTTPPolicy):
     """Policy to transform PATCH requests into POST requests with the "X-HTTP-Method":"MERGE" header set."""
 
-    def on_request(self, request):
-        # type: (PipelineRequest) -> None
+    def on_request(self, request: PipelineRequest) -> None:
         if request.http_request.method == "PATCH":
             _transform_patch_to_cosmos_post(request.http_request)
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_table_shared_access_signature.py` & `azure-data-tables-12.4.3/azure/data/tables/_table_shared_access_signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-from typing import Union, Any, TYPE_CHECKING
+from datetime import datetime
+from typing import Union
+from azure.core.credentials import AzureNamedKeyCredential
 
-from ._models import AccountSasPermissions
+from ._models import AccountSasPermissions, ResourceTypes
 from ._common_conversion import _sign_string
 from ._error import _validate_not_none
 from ._constants import X_MS_VERSION
 from ._shared_access_signature import (
     _SharedAccessHelper,
     SharedAccessSignature,
     QueryStringConstants,
 )
 
-if TYPE_CHECKING:
-    from datetime import datetime
-    from azure.core.credentials import AzureNamedKeyCredential
-    from ._models import ResourceTypes
-
 
 def generate_account_sas(
-    credential,  # type: AzureNamedKeyCredential
-    resource_types,  # type: ResourceTypes
-    permission,  # type: Union[str, AccountSasPermissions]
-    expiry,  # type: Union[datetime, str]
-    **kwargs  # type: Any
-):
-    # type: (...) -> str
+    credential: AzureNamedKeyCredential,
+    resource_types: ResourceTypes,
+    permission: Union[str, AccountSasPermissions],
+    expiry: Union[datetime, str],
+    **kwargs
+) -> str:
     """
     Generates a shared access signature for the table service.
     Use the returned signature with the sas_token parameter of TableService.
 
     :param credential: Credential for the Azure account
     :type credential: :class:`~azure.core.credentials.AzureNamedKeyCredential`
     :param resource_types:
@@ -84,16 +80,15 @@
         expiry,
         start=kwargs.pop("start", None),
         ip_address_or_range=kwargs.pop("ip_address_or_range", None),
         protocol=kwargs.pop("protocol", None),
     )
 
 
-def generate_table_sas(credential, table_name, **kwargs):
-    # type: (AzureNamedKeyCredential, str, **Any) -> str
+def generate_table_sas(credential: AzureNamedKeyCredential, table_name: str, **kwargs) -> str:
     """
     Generates a shared access signature for the table service.
     Use the returned signature with the sas_token parameter of TableService.
 
 
     :param credential: Credential used for creating Shared Access Signature
     :type credential: :class:`~azure.core.credentials.AzureNamedKeyCredential`
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/aio/_table_batch_async.py` & `azure-data-tables-12.4.3/azure/data/tables/aio/_table_batch_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-from typing import Dict, Any, Optional, Union, TYPE_CHECKING
+from typing import Dict, Any, Optional, Union
 
 from azure.core import MatchConditions
 
 from .._common_conversion import _transform_patch_to_cosmos_post
 from .._models import UpdateMode
 from .._table_batch import EntityType, TransactionOperationType
 from .._serialize import (
     _prepare_key,
     _get_match_headers,
     _add_entity_properties,
 )
+from .._generated import models
 from .._generated.aio import AzureTable
 from .._generated.aio._configuration import AzureTableConfiguration
 from .._generated._serialization import Serializer, Deserializer
 
-if TYPE_CHECKING:
-    from .._generated import models
-
 
 class TableBatchOperations(object):
     """
     This is the class that is used for batch operations for the data tables
     service.
 
     The Tables service supports batch transactions on entities that are in the
@@ -39,15 +37,15 @@
         self,
         client: AzureTable,
         serializer: Serializer,
         deserializer: Deserializer,
         config: AzureTableConfiguration,
         table_name: str,
         is_cosmos_endpoint: bool = False,
-        **kwargs: Dict[str, Any]
+        **kwargs
     ) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
         self._is_cosmos_endpoint = is_cosmos_endpoint
         self.table_name = table_name
@@ -110,32 +108,32 @@
 
     def _batch_create_entity(
         self,
         table: str,
         entity: EntityType,
         timeout: Optional[int] = None,
         request_id_parameter: Optional[str] = None,
-        response_preference: Optional[Union[str, "models.ResponseFormat"]] = "return-no-content",
-        format: Optional[Union[str, "models.OdataMetadataFormat"]] = None,  # pylint: disable=redefined-builtin
-        **kwargs: Any
+        response_preference: Optional[Union[str, models.ResponseFormat]] = "return-no-content",
+        format: Optional[Union[str, models.OdataMetadataFormat]] = None,  # pylint: disable=redefined-builtin
+        **kwargs
     ) -> None:
         """
         Adds an insert operation to the batch. See
         :func:`azure.data.tables.TableClient.insert_entity` for more information
         on insert operations.
 
         The operation will not be executed until the batch is committed
 
         :param: table:
             The table to perform the operation on
         :type: table: str
         :param: entity:
             The entity to insert. Can be a dict or an entity object
             Must contain a PartitionKey and a RowKey.
-        :type: entity: dict or :class:`~azure.data.tables.models.Entity`
+        :type: entity: Dict or :class:`~azure.data.tables.models.Entity`
         :param timeout: The timeout parameter is expressed in seconds.
         :type timeout: int
         :param request_id_parameter: Provides a client-generated, opaque value with a 1 KB character
          limit that is recorded in the analytics logs when analytics logging is enabled.
         :type request_id_parameter: str
         :param response_preference: Specifies the return format. Default is return without content.
         :type response_preference: str or ~azure.data.tables.models.ResponseFormat
@@ -205,15 +203,15 @@
 
     _batch_create_entity.metadata = {"url": "/{table}"}  # type: ignore
 
     def update(
         self,
         entity: EntityType,
         mode: Union[str, UpdateMode] = UpdateMode.MERGE,
-        **kwargs: Any
+        **kwargs
     ) -> None:
         """Adds an update operation to the current batch.
 
         :param entity: The properties for the table entity.
         :type entity: :class:`~azure.data.tables.TableEntity` or Dict[str,str]
         :param mode: Merge or Replace entity
         :type mode: :class:`~azure.data.tables.UpdateMode`
@@ -277,16 +275,16 @@
         table: str,
         partition_key: str,
         row_key: str,
         timeout: Optional[int] = None,
         request_id_parameter: Optional[str] = None,
         if_match: Optional[str] = None,
         table_entity_properties: Optional[EntityType] = None,
-        format: Optional[Union[str, "models.OdataMetadataFormat"]] = None, # pylint: disable=redefined-builtin
-        **kwargs: Any
+        format: Optional[Union[str, models.OdataMetadataFormat]] = None, # pylint: disable=redefined-builtin
+        **kwargs
     ) -> None:
         """Update entity in a table.
 
         :param table: The name of the table.
         :type table: str
         :param partition_key: The partition key of the entity.
         :type partition_key: str
@@ -299,15 +297,15 @@
         :type request_id_parameter: str
         :param if_match: Match condition for an entity to be updated. If specified and a matching
          entity is not found, an error will be raised. To force an unconditional update, set to the
          wildcard character (*). If not specified, an insert will be performed when no existing entity
          is found to update and a replace will be performed if an existing entity is found.
         :type if_match: str
         :param table_entity_properties: The properties for the table entity.
-        :type table_entity_properties: dict[str, object]
+        :type table_entity_properties: Dict[str, object]
         :param format: Specifies the media type for the response. Known values are:
          "application/json;odata=nometadata", "application/json;odata=minimalmetadata", and
          "application/json;odata=fullmetadata".
         :type format: str or ~azure.data.tables.models.OdataMetadataFormat
         """
         data_service_version = "3.0"
         content_type = kwargs.pop("content_type", "application/json")
@@ -379,15 +377,15 @@
         table: str,
         partition_key: str,
         row_key: str,
         timeout: Optional[int] = None,
         request_id_parameter: Optional[str] = None,
         if_match: Optional[str] = None,
         table_entity_properties: Optional[EntityType] = None,
-        format: Optional[Union[str, "models.OdataMetadataFormat"]] = None, # pylint: disable=redefined-builtin
+        format: Optional[Union[str, models.OdataMetadataFormat]] = None, # pylint: disable=redefined-builtin
         **kwargs
     ) -> None:
         """Merge entity in a table.
 
         :param table: The name of the table.
         :type table: str
         :param partition_key: The partition key of the entity.
@@ -401,15 +399,15 @@
         :type request_id_parameter: str
         :param if_match: Match condition for an entity to be updated. If specified and a matching
          entity is not found, an error will be raised. To force an unconditional update, set to the
          wildcard character (*). If not specified, an insert will be performed when no existing entity
          is found to update and a merge will be performed if an existing entity is found.
         :type if_match: str
         :param table_entity_properties: The properties for the table entity.
-        :type table_entity_properties: dict[str, object]
+        :type table_entity_properties: Dict[str, object]
         :param format: Specifies the media type for the response. Known values are:
          "application/json;odata=nometadata", "application/json;odata=minimalmetadata", and
          "application/json;odata=fullmetadata".
         :type format: str or ~azure.data.tables.models.OdataMetadataFormat
         """
         data_service_version = "3.0"
         content_type = kwargs.pop("content_type", "application/json")
@@ -531,15 +529,15 @@
         self,
         table: str,
         partition_key: str,
         row_key: str,
         if_match: str,
         timeout: Optional[int] = None,
         request_id_parameter: Optional[str] = None,
-        format: Optional[Union[str, "models.OdataMetadataFormat"]] = None, # pylint: disable=redefined-builtin
+        format: Optional[Union[str, models.OdataMetadataFormat]] = None, # pylint: disable=redefined-builtin
     ) -> None:
         """Deletes the specified entity in a table.
 
         :param table: The name of the table.
         :type table: str
         :param partition_key: The partition key of the entity.
         :type partition_key: str
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/aio/_base_client_async.py` & `azure-data-tables-12.4.3/azure/data/tables/aio/_base_client_async.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,132 +1,111 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-
-from typing import Any, List, Mapping, Optional, Union, TYPE_CHECKING
+from typing import Any, List, Mapping, Optional, Union
 from uuid import uuid4
 
 from azure.core.credentials import AzureSasCredential, AzureNamedKeyCredential
+from azure.core.credentials_async import AsyncTokenCredential
 from azure.core.pipeline.policies import (
     ContentDecodePolicy,
     AsyncRedirectPolicy,
     DistributedTracingPolicy,
     HttpLoggingPolicy,
     UserAgentPolicy,
     ProxyPolicy,
-    AzureSasCredentialPolicy,
     RequestIdPolicy,
     CustomHookPolicy,
     NetworkTraceLoggingPolicy,
 )
 from azure.core.pipeline.transport import (
     AsyncHttpTransport,
     HttpRequest,
 )
 
-from ._authentication_async import AsyncBearerTokenChallengePolicy
+from ._authentication_async import _configure_credential
 from .._generated.aio import AzureTable
 from .._base_client import AccountHostsMixin, get_api_version, extract_batch_part_metadata
-from .._authentication import SharedKeyCredentialPolicy
-from .._constants import STORAGE_OAUTH_SCOPE
 from .._error import (
     RequestTooLargeError,
     TableTransactionError,
     _decode_error,
-    _validate_tablename_error
+    _validate_tablename_error,
 )
 from .._policies import StorageHosts, StorageHeadersPolicy
 from .._sdk_moniker import SDK_MONIKER
 from ._policies_async import AsyncTablesRetryPolicy
 
-if TYPE_CHECKING:
-    from azure.core.credentials_async import AsyncTokenCredential
-
 
 class AsyncTablesBaseClient(AccountHostsMixin):
     """Base class for TableClient
 
     :param str endpoint: A URL to an Azure Tables account.
     :keyword credential:
         The credentials with which to authenticate. This is optional if the
         account URL already has a SAS token. The value can be one of AzureNamedKeyCredential (azure-core),
-        AzureSasCredential (azure-core), or TokenCredentials from azure-identity.
+        AzureSasCredential (azure-core), or AsyncTokenCredential from azure-identity.
     :paramtype credential:
         :class:`~azure.core.credentials.AzureNamedKeyCredential` or
         :class:`~azure.core.credentials.AzureSasCredential` or
-        :class:`~azure.core.credentials.TokenCredential`
+        :class:`~azure.core.credentials.AsyncTokenCredential`
     :keyword api_version: Specifies the version of the operation to use for this request. Default value
         is "2019-02-02". Note that overriding this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
-    def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
+    def __init__( # pylint: disable=missing-client-constructor-parameter-credential
         self,
         endpoint: str,
         *,
-        credential: Optional[Union[AzureSasCredential, AzureNamedKeyCredential, "AsyncTokenCredential"]] = None,
-        **kwargs: Any
+        credential: Optional[Union[AzureSasCredential, AzureNamedKeyCredential, AsyncTokenCredential]] = None,
+        **kwargs
     ) -> None:
         super(AsyncTablesBaseClient, self).__init__(endpoint, credential=credential, **kwargs)  # type: ignore
         self._client = AzureTable(
             self.url,
             policies=kwargs.pop('policies', self._policies),
             **kwargs
         )
-        self._client._config.version = get_api_version(kwargs, self._client._config.version)  # pylint: disable=protected-access
-
+        self._client._config.version = get_api_version(kwargs, self._client._config.version) # type: ignore # pylint: disable=protected-access
 
     async def __aenter__(self):
         await self._client.__aenter__()
         return self
 
     async def __aexit__(self, *args):
         await self._client.__aexit__(*args)
 
     async def close(self) -> None:
         """This method is to close the sockets opened by the client.
         It need not be used when using with a context manager.
         """
         await self._client.close()
 
-    def _configure_credential(self, credential):
-        # type: (Any) -> None
-        if hasattr(credential, "get_token"):
-            self._credential_policy = AsyncBearerTokenChallengePolicy(  # type: ignore
-                credential, STORAGE_OAUTH_SCOPE
-            )
-        elif isinstance(credential, SharedKeyCredentialPolicy):
-            self._credential_policy = credential  # type: ignore
-        elif isinstance(credential, AzureSasCredential):
-            self._credential_policy = AzureSasCredentialPolicy(credential)  # type: ignore
-        elif isinstance(credential, AzureNamedKeyCredential):
-            self._credential_policy = SharedKeyCredentialPolicy(credential)  # type: ignore
-        elif credential is not None:
-            raise TypeError("Unsupported credential: {}".format(credential))
-
     def _configure_policies(self, **kwargs):
+        credential_policy = _configure_credential(self.credential)
         return [
             RequestIdPolicy(**kwargs),
             StorageHeadersPolicy(**kwargs),
             UserAgentPolicy(sdk_moniker=SDK_MONIKER, **kwargs),
             ProxyPolicy(**kwargs),
-            self._credential_policy,
+            credential_policy,
             ContentDecodePolicy(response_encoding="utf-8"),
             AsyncRedirectPolicy(**kwargs),
             StorageHosts(**kwargs),
             AsyncTablesRetryPolicy(**kwargs),
             CustomHookPolicy(**kwargs),
             NetworkTraceLoggingPolicy(**kwargs),
             DistributedTracingPolicy(**kwargs),
             HttpLoggingPolicy(**kwargs),
         ]
 
-    async def _batch_send(self, table_name: str, *reqs: "HttpRequest", **kwargs) -> List[Mapping[str, Any]]:
+    async def _batch_send(self, table_name: str, *reqs: HttpRequest, **kwargs) -> List[Mapping[str, Any]]:
         """Given a series of request, do a Storage batch call."""
         # Pop it here, so requests doesn't feel bad about additional kwarg
         policies = [StorageHeadersPolicy()]
 
         changeset = HttpRequest("POST", None)  # type: ignore
         changeset.set_multipart_mixed(
             *reqs, policies=policies, boundary="changeset_{}".format(uuid4())
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/aio/__init__.py` & `azure-data-tables-12.4.3/azure/data/tables/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/aio/_policies_async.py` & `azure-data-tables-12.4.3/azure/data/tables/aio/_policies_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,38 +70,38 @@
         return should_retry
 
     def configure_retries(self, options):
         """Configures the retry settings.
 
         :param options: keyword arguments from context.
         :return: A dict containing settings and history for retries.
-        :rtype: dict
+        :rtype: Dict
         """
         config = super(AsyncTablesRetryPolicy, self).configure_retries(options)
         config["retry_secondary"] = options.pop("retry_to_secondary", self.retry_to_secondary)
         config["mode"] = options.pop("location_mode", LocationMode.PRIMARY)
         config["hosts"] = options.pop("hosts", None)
         return config
 
     def update_context(self, context, retry_settings):
         """Updates retry history in pipeline context.
 
         :param context: The pipeline context.
         :type context: ~azure.core.pipeline.PipelineContext
         :param retry_settings: The retry settings.
-        :type retry_settings: dict
+        :type retry_settings: Dict
         """
         super(AsyncTablesRetryPolicy, self).update_context(context, retry_settings)
         context['location_mode'] = retry_settings['mode']
 
     def update_request(self, request, retry_settings):  # pylint: disable=no-self-use
         """Updates the pipeline request before attempting to retry.
 
         :param PipelineRequest request: The outgoing request.
-        :param dict(str, Any) retry_settings: The current retry context settings.
+        :param Dict(str, Any) retry_settings: The current retry context settings.
         """
         set_next_host_location(retry_settings, request)
 
     async def send(self, request):
         """Uses the configured retry policy to send the request to the next policy in the pipeline.
 
         :param request: The PipelineRequest object
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/aio/_models.py` & `azure-data-tables-12.4.3/azure/data/tables/aio/_models.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/aio/_table_client_async.py` & `azure-data-tables-12.4.3/azure/data/tables/aio/_table_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,80 +1,79 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import functools
-from typing import AsyncIterable, List, Union, Any, Optional, Mapping, Iterable, Dict, overload, cast, TYPE_CHECKING
+from typing import AsyncIterable, List, Union, Any, Optional, Mapping, Iterable, Dict, overload, cast
 try:
     from urllib.parse import urlparse, unquote
 except ImportError:
     from urlparse import urlparse  # type: ignore
     from urllib2 import unquote  # type: ignore
 
 from azure.core import MatchConditions
 from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential
+from azure.core.credentials_async import AsyncTokenCredential
 from azure.core.async_paging import AsyncItemPaged
 from azure.core.exceptions import HttpResponseError
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
 
 from .._base_client import parse_connection_str
 from .._entity import TableEntity
 from .._generated.models import SignedIdentifier, TableProperties
-from .._models import TableAccessPolicy, TableItem
-from .._serialize import serialize_iso, _parameter_filter_substitution, _prepare_key
-from .._deserialize import deserialize_iso, _return_headers_and_deserialized
+from .._models import TableAccessPolicy, TableItem, UpdateMode
+from .._serialize import(
+    serialize_iso, _parameter_filter_substitution, _prepare_key, _add_entity_properties, _get_match_headers
+)
+from .._deserialize import(
+    deserialize_iso, _return_headers_and_deserialized, _convert_to_entity, _trim_service_metadata
+)
 from .._error import (
     _decode_error,
     _process_table_error,
     _reprocess_error,
     _reraise_error,
     _validate_tablename_error
 )
-from .._models import UpdateMode
-from .._deserialize import _convert_to_entity, _trim_service_metadata
-from .._serialize import _add_entity_properties, _get_match_headers
 from .._table_client import EntityType, TransactionOperationType
 from ._base_client_async import AsyncTablesBaseClient
 from ._models import TableEntityPropertiesPaged
 from ._table_batch_async import TableBatchOperations
 
-if TYPE_CHECKING:
-    from azure.core.credentials_async import AsyncTokenCredential
-
 
 class TableClient(AsyncTablesBaseClient):
     """A client to interact with a specific Table in an Azure Tables account.
 
     :ivar str account_name: The name of the Tables account.
     :ivar str table_name: The name of the table.
     :ivar str url: The full URL to the Tables account.
     """
 
-    def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
+    def __init__( # pylint: disable=missing-client-constructor-parameter-credential
         self,
         endpoint: str,
         table_name: str,
         *,
-        credential: Optional[Union[AzureSasCredential, AzureNamedKeyCredential, "AsyncTokenCredential"]] = None,
+        credential: Optional[Union[AzureSasCredential, AzureNamedKeyCredential, AsyncTokenCredential]] = None,
         **kwargs
     ) -> None:
         """Create TableClient from a Credential.
 
         :param str endpoint: A URL to an Azure Tables account.
         :param str table_name: The table name.
         :keyword credential:
             The credentials with which to authenticate. This is optional if the
             account URL already has a SAS token. The value can be one of AzureNamedKeyCredential (azure-core),
-            AzureSasCredential (azure-core), or TokenCredentials from azure-identity.
+            AzureSasCredential (azure-core), or AsyncTokenCredential from azure-identity.
         :paramtype credential:
             :class:`~azure.core.credentials.AzureNamedKeyCredential` or
             :class:`~azure.core.credentials.AzureSasCredential` or
-            :class:`~azure.core.credentials.TokenCredential`
+            :class:`~azure.core.credentials.AsyncTokenCredential`
         :keyword api_version: Specifies the version of the operation to use for this request. Default value
             is "2019-02-02". Note that overriding this default value may result in unsupported behavior.
         :paramtype api_version: str
 
         :returns: None
         """
         if not table_name:
@@ -107,25 +106,25 @@
             .. literalinclude:: ../samples/async_samples/sample_create_client_async.py
                 :start-after: [START create_table_client]
                 :end-before: [END create_table_client]
                 :language: python
                 :dedent: 8
                 :caption: Creating the TableClient from a connection string.
         """
-        endpoint, credential = parse_connection_str(
-            conn_str=conn_str, credential=None, keyword_args=kwargs
-        )
+        endpoint, credential = parse_connection_str(conn_str=conn_str, credential=None, keyword_args=kwargs)
         return cls(endpoint, table_name=table_name, credential=credential, **kwargs)
 
     @classmethod
     def from_table_url(
         cls,
         table_url: str,
+        *,
+        credential: Optional[Union[AzureNamedKeyCredential, AzureSasCredential]] = None,
         **kwargs
-    ) -> 'TableClient':
+    ) -> "TableClient":
         """A client to interact with a specific Table.
 
         :param str table_url: The full URI to the table, including SAS token if used.
         :keyword credential:
             The credentials with which to authenticate. This is optional if the
             table URL already has a SAS token. The value can be one of AzureNamedKeyCredential
             or AzureSasCredential from azure-core.
@@ -158,15 +157,15 @@
         table_name = unquote(table_path[-1])
         if table_name.lower().startswith("tables('"):
             table_name = table_name[8:-2]
         if not table_name:
             raise ValueError(
                 "Invalid URL. Please provide a URL with a valid table name"
             )
-        return cls(endpoint, table_name=table_name, **kwargs)
+        return cls(endpoint, table_name=table_name, credential=credential, **kwargs)
 
     @distributed_trace_async
     async def get_table_access_policy(self, **kwargs) -> Mapping[str, Optional[TableAccessPolicy]]:
         """
         Retrieves details about any stored access policies specified on the table that may be
         used with Shared Access Signatures.
 
@@ -285,23 +284,23 @@
             try:
                 _process_table_error(error, table_name=self.table_name)
             except HttpResponseError as decoded_error:
                 _reprocess_error(decoded_error)
                 raise
 
     @overload
-    async def delete_entity(self, partition_key: str, row_key: str, **kwargs: Any) -> None:
+    async def delete_entity(self, partition_key: str, row_key: str, **kwargs) -> None:
         ...
 
     @overload
-    async def delete_entity(self, entity: Union[TableEntity, Mapping[str, Any]], **kwargs: Any) -> None:
+    async def delete_entity(self, entity: Union[TableEntity, Mapping[str, Any]], **kwargs) -> None:
         ...
 
     @distributed_trace_async
-    async def delete_entity(self, *args: Union[TableEntity, str], **kwargs: Any) -> None:
+    async def delete_entity(self, *args: Union[TableEntity, str], **kwargs) -> None:
         """Deletes the specified entity in a table. No error will be raised if
         the entity or PartitionKey-RowKey pairing is not found.
 
         :param str partition_key: The partition key of the entity.
         :param str row_key: The row key of the entity.
         :param entity: The entity to delete
         :type entity: Union[TableEntity, Mapping[str, str]]
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/aio/_table_service_client_async.py` & `azure-data-tables-12.4.3/azure/data/tables/aio/_table_service_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 import functools
-from typing import (
-    Optional,
-    Dict,
-    List,
-    TYPE_CHECKING
-)
+from typing import Optional, Dict, List
 
 from azure.core.async_paging import AsyncItemPaged
 from azure.core.exceptions import HttpResponseError, ResourceExistsError
 from azure.core.pipeline import AsyncPipeline
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
 
 from .._base_client import parse_connection_str
 from .._generated.models import TableServiceProperties
 from .._models import service_stats_deserialize, service_properties_deserialize
 from .._error import _process_table_error, _reprocess_error
-from .._models import TableItem, LocationMode
+from .._models import TableItem, LocationMode, TableCorsRule, TableMetrics, TableAnalyticsLogging
 from .._serialize import _parameter_filter_substitution
 from ._table_client_async import TableClient
 from ._base_client_async import AsyncTablesBaseClient, AsyncTransportWrapper
 from ._models import TablePropertiesPaged
 
-if TYPE_CHECKING:
-    from .._models import TableCorsRule, TableMetrics, TableAnalyticsLogging
-
 
 class TableServiceClient(AsyncTablesBaseClient):
     """A client to interact with the Table Service at the account level.
 
     This client provides operations to retrieve and configure the account properties
     as well as list, create and delete tables within the account.
     For operations relating to a specific table, a client for this entity
@@ -44,19 +36,19 @@
     :param str endpoint:
         The URL to the table service endpoint. Any other entities included
         in the URL path (e.g. table) will be discarded. This URL can be optionally
         authenticated with a SAS token.
     :keyword credential:
         The credentials with which to authenticate. This is optional if the
         account URL already has a SAS token. The value can be one of AzureNamedKeyCredential (azure-core),
-        AzureSasCredential (azure-core), or TokenCredentials from azure-identity.
+        AzureSasCredential (azure-core), or AsyncTokenCredential from azure-identity.
     :paramtype credential:
         :class:`~azure.core.credentials.AzureNamedKeyCredential` or
         :class:`~azure.core.credentials.AzureSasCredential` or
-        :class:`~azure.core.credentials.TokenCredential`
+        :class:`~azure.core.credentials.AsyncTokenCredential`
     :keyword str api_version:
         The Storage API version to use for requests. Default value is '2019-02-02'.
         Setting to an older version may result in reduced feature compatibility.
 
     .. admonition:: Example:
 
         .. literalinclude:: ../samples/async_samples/sample_authentication_async.py
@@ -142,18 +134,18 @@
                 raise
         return service_properties_deserialize(service_props)
 
     @distributed_trace_async
     async def set_service_properties(
         self,
         *,
-        analytics_logging: Optional['TableAnalyticsLogging'] = None,
-        hour_metrics: Optional['TableMetrics'] = None,
-        minute_metrics: Optional['TableMetrics'] = None,
-        cors: Optional[List['TableCorsRule']] = None,
+        analytics_logging: Optional[TableAnalyticsLogging] = None,
+        hour_metrics: Optional[TableMetrics] = None,
+        minute_metrics: Optional[TableMetrics] = None,
+        cors: Optional[List[TableCorsRule]] = None,
         **kwargs
     ) -> None:
         """Sets properties for an account's Table service endpoint,
          including properties for Analytics and CORS (Cross-Origin Resource Sharing) rules.
 
         :keyword analytics_logging: Properties for analytics
         :paramtype analytics_logging: ~azure.data.tables.TableAnalyticsLogging
```

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/_client.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/_client.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/_vendor.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/_configuration.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/__init__.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/_serialization.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/_patch.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_client.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_client.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_configuration.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/aio/__init__.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/aio/_patch.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/__init__.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/_operations.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/aio/operations/_patch.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/models/__init__.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/models/_enums.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/models/_enums.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/models/_models.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/models/_patch.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/operations/__init__.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/operations/_operations.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/azure/data/tables/_generated/operations/_patch.py` & `azure-data-tables-12.4.3/azure/data/tables/_generated/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_create_delete_table.py` & `azure-data-tables-12.4.3/samples/sample_create_delete_table.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_query_table.py` & `azure-data-tables-12.4.3/samples/sample_query_table.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_copy_table.py` & `azure-data-tables-12.4.3/samples/sample_copy_table.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_query_tables.py` & `azure-data-tables-12.4.3/samples/sample_query_tables.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_insert_delete_entities.py` & `azure-data-tables-12.4.3/samples/sample_insert_delete_entities.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_conditional_update.py` & `azure-data-tables-12.4.3/samples/sample_conditional_update.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_authentication.py` & `azure-data-tables-12.4.3/samples/sample_authentication.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_batching.py` & `azure-data-tables-12.4.3/samples/sample_batching.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_update_upsert_merge_entities.py` & `azure-data-tables-12.4.3/samples/sample_update_upsert_merge_entities.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/README.md` & `azure-data-tables-12.4.3/samples/README.md`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/sample_create_client.py` & `azure-data-tables-12.4.3/samples/sample_create_client.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_create_client_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_create_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_query_table_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_query_table_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_batching_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_batching_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_conditional_update_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_conditional_update_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             entity2 = await table_client.get_entity(partition_key=self.entity1["PartitionKey"], row_key=self.entity1["RowKey"])
             print("Entity after merge:")
             print(entity2)
 
             # Update an existing entity by replacing all of its properties with those specified.
             # This operation will only succeed if the entity has not been modified since we last retrieved the Etag.
             try:
-                table_client.update_entity(entity=self.entity2, mode=UpdateMode.REPLACE, match_condition=MatchConditions.IfNotModified, etag=metadata2["etag"])
+                await table_client.update_entity(entity=self.entity2, mode=UpdateMode.REPLACE, match_condition=MatchConditions.IfNotModified, etag=metadata2["etag"])
             except ResourceModifiedError:
                 print("This entity has been altered and may no longer be in the expected state.")
             entity3 = await table_client.get_entity(partition_key=self.entity1["PartitionKey"], row_key=self.entity1["RowKey"])
             print("Entity after replace:")
             print(entity3)
 
             await table_client.delete_table()
```

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_create_delete_table_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_create_delete_table_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_update_upsert_merge_entities_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_update_upsert_merge_entities_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_authentication_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_authentication_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_copy_table_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_copy_table_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_insert_delete_entities_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_insert_delete_entities_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/samples/async_samples/sample_query_tables_async.py` & `azure-data-tables-12.4.3/samples/async_samples/sample_query_tables_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/preparers.py` & `azure-data-tables-12.4.3/tests/preparers.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_service_stats_cosmos.py` & `azure-data-tables-12.4.3/tests/test_table_service_stats_cosmos.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_retry.py` & `azure-data-tables-12.4.3/tests/test_retry.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_service_properties_cosmos_async.py` & `azure-data-tables-12.4.3/tests/test_table_service_properties_cosmos_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_batch.py` & `azure-data-tables-12.4.3/tests/test_table_batch.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_cosmos_async.py` & `azure-data-tables-12.4.3/tests/test_table_cosmos_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_retry_async.py` & `azure-data-tables-12.4.3/tests/test_retry_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_entity_cosmos_async.py` & `azure-data-tables-12.4.3/tests/test_table_entity_cosmos_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_challenge_auth_async.py` & `azure-data-tables-12.4.3/tests/test_challenge_auth_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_service_stats_async.py` & `azure-data-tables-12.4.3/tests/test_table_service_stats_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_service_properties_cosmos.py` & `azure-data-tables-12.4.3/tests/test_table_service_properties_cosmos.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_service_stats.py` & `azure-data-tables-12.4.3/tests/test_table_service_stats.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_aad_async.py` & `azure-data-tables-12.4.3/tests/test_table_aad_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_client.py` & `azure-data-tables-12.4.3/tests/test_table_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from devtools_testutils import AzureRecordedTestCase, recorded_by_proxy
 
 from azure.data.tables._error import _validate_storage_tablename
 from azure.data.tables import TableServiceClient, TableClient
 from azure.data.tables import __version__ as VERSION
 from azure.data.tables._constants import DEFAULT_STORAGE_ENDPOINT_SUFFIX
 from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential
-from azure.core.exceptions import ResourceNotFoundError, HttpResponseError
+from azure.core.exceptions import ResourceNotFoundError, HttpResponseError, ClientAuthenticationError
+from azure.identity import DefaultAzureCredential
 
 from _shared.testcase import (
     TableTestCase
 )
 
 from preparers import tables_decorator
 
@@ -168,14 +169,29 @@
         assert ("Please check your account URL.") in str(exc.value)
         # test deleting a table when it already exists
         with pytest.raises(HttpResponseError) as exc:
             tc.delete_table()
         assert ("URI does not match number of key properties for the resource") in str(exc.value)
         assert ("Please check your account URL.") in str(exc.value)
         valid_tc.delete_table()
+    
+    @tables_decorator
+    @recorded_by_proxy
+    def test_error_handling(self, tables_storage_account_name, tables_primary_storage_account_key):
+        with TableServiceClient(
+            self.account_url(tables_storage_account_name, "table"),
+            credential=DefaultAzureCredential(
+                exclude_shared_token_cache_credential=True,
+                exclude_powershell_credential=True,
+                exclude_cli_credential=True,
+                exclude_environment_credential=True,
+            )
+        ) as service_client:
+            with pytest.raises(ClientAuthenticationError):
+                service_client.create_table_if_not_exists(table_name="TestInsert")
 
 
 # --Helpers-----------------------------------------------------------------
 def validate_standard_account_endpoints(service, account_name, account_key):
     endpoint_suffix = os.getenv("TABLES_STORAGE_ENDPOINT_SUFFIX", DEFAULT_STORAGE_ENDPOINT_SUFFIX)
     assert service is not None
     assert service.account_name == account_name
```

## Comparing `azure-data-tables-12.4.2/tests/test_table_client_async.py` & `azure-data-tables-12.4.3/tests/test_table_client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import platform
 import os
 
 from devtools_testutils import AzureRecordedTestCase
 from devtools_testutils.aio import recorded_by_proxy_async
 
 from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential
-from azure.core.exceptions import ResourceNotFoundError, HttpResponseError
+from azure.core.exceptions import ResourceNotFoundError, HttpResponseError, ClientAuthenticationError
+from azure.identity.aio import DefaultAzureCredential
 from azure.data.tables.aio import TableServiceClient, TableClient
 from azure.data.tables._version import VERSION
 from azure.data.tables._constants import DEFAULT_STORAGE_ENDPOINT_SUFFIX
 
 from _shared.asynctestcase import AsyncTableTestCase
 from async_preparers import tables_decorator_async
 from test_table_client import validate_standard_account_endpoints
@@ -169,14 +170,29 @@
         assert ("Please check your account URL.") in str(exc.value)
         # test deleting a table when it already exists
         with pytest.raises(HttpResponseError) as exc:
             await tc.delete_table()
         assert ("URI does not match number of key properties for the resource") in str(exc.value)
         assert ("Please check your account URL.") in str(exc.value)
         await valid_tc.delete_table()
+    
+    @tables_decorator_async
+    @recorded_by_proxy_async
+    async def test_error_handling(self, tables_storage_account_name, tables_primary_storage_account_key):
+        async with TableServiceClient(
+            self.account_url(tables_storage_account_name, "table"),
+            credential=DefaultAzureCredential(
+                exclude_shared_token_cache_credential=True,
+                exclude_powershell_credential=True,
+                exclude_cli_credential=True,
+                exclude_environment_credential=True,
+            )
+        ) as service_client:
+            with pytest.raises(ClientAuthenticationError):
+                await service_client.create_table_if_not_exists(table_name="TestInsert")
 
 
 class TestTableClientAsyncUnitTests(AsyncTableTestCase):
     tables_storage_account_name = "fake_storage_account"
     tables_primary_storage_account_key = "fakeXMZjnGsZGvd4bVr3Il5SeHA"
     credential = AzureNamedKeyCredential(name=tables_storage_account_name, key=tables_primary_storage_account_key)
```

## Comparing `azure-data-tables-12.4.2/tests/test_table_service_properties.py` & `azure-data-tables-12.4.3/tests/test_table_service_properties.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table.py` & `azure-data-tables-12.4.3/tests/test_table.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_entity_cosmos.py` & `azure-data-tables-12.4.3/tests/test_table_entity_cosmos.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_encoder.py` & `azure-data-tables-12.4.3/tests/test_encoder.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_batch_cosmos.py` & `azure-data-tables-12.4.3/tests/test_table_batch_cosmos.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_async.py` & `azure-data-tables-12.4.3/tests/test_table_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_service_properties_async.py` & `azure-data-tables-12.4.3/tests/test_table_service_properties_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/conftest.py` & `azure-data-tables-12.4.3/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/async_preparers.py` & `azure-data-tables-12.4.3/tests/async_preparers.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_entity_async.py` & `azure-data-tables-12.4.3/tests/test_table_entity_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_service_stats_cosmos_async.py` & `azure-data-tables-12.4.3/tests/test_table_service_stats_cosmos_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_aad.py` & `azure-data-tables-12.4.3/tests/test_table_aad.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_batch_cosmos_async.py` & `azure-data-tables-12.4.3/tests/test_table_batch_cosmos_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_batch_async.py` & `azure-data-tables-12.4.3/tests/test_table_batch_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_cosmos.py` & `azure-data-tables-12.4.3/tests/test_table_cosmos.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_challenge_auth.py` & `azure-data-tables-12.4.3/tests/test_challenge_auth.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_entity.py` & `azure-data-tables-12.4.3/tests/test_table_entity.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_client_cosmos_async.py` & `azure-data-tables-12.4.3/tests/test_table_client_cosmos_async.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/test_table_client_cosmos.py` & `azure-data-tables-12.4.3/tests/test_table_client_cosmos.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/_shared/asynctestcase.py` & `azure-data-tables-12.4.3/tests/_shared/asynctestcase.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/_shared/cosmos_testcase.py` & `azure-data-tables-12.4.3/tests/_shared/cosmos_testcase.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/_shared/testcase.py` & `azure-data-tables-12.4.3/tests/_shared/testcase.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/perfstress_tests/create_entity.py` & `azure-data-tables-12.4.3/tests/perfstress_tests/create_entity.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/perfstress_tests/create_entity_batch.py` & `azure-data-tables-12.4.3/tests/perfstress_tests/create_entity_batch.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/perfstress_tests/_base.py` & `azure-data-tables-12.4.3/tests/perfstress_tests/_base.py`

 * *Files identical despite different names*

## Comparing `azure-data-tables-12.4.2/tests/perfstress_tests/list_entities.py` & `azure-data-tables-12.4.3/tests/perfstress_tests/list_entities.py`

 * *Files identical despite different names*

