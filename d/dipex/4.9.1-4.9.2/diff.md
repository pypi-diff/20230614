# Comparing `tmp/dipex-4.9.1.tar.gz` & `tmp/dipex-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipex-4.9.1.tar", max compression
+gzip compressed data, was "dipex-4.9.2.tar", max compression
```

## Comparing `dipex-4.9.1.tar` & `dipex-4.9.2.tar`

### file list

```diff
@@ -1,181 +1,181 @@
--rw-r--r--   0        0        0     1392 2023-03-31 06:49:01.872391 dipex-4.9.1/README.rst
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.112424 dipex-4.9.1/exporters/sql_export/__init__.py
--rw-r--r--   0        0        0     2129 2023-03-31 06:49:01.898395 dipex-4.9.1/exporters/sql_export/lc_for_jobs_db.py
--rw-r--r--   0        0        0    56625 2023-03-31 06:49:01.898395 dipex-4.9.1/exporters/sql_export/lora_cache.py
--rw-r--r--   0        0        0     2529 2023-03-31 06:49:01.899395 dipex-4.9.1/exporters/sql_export/main.py
--rw-r--r--   0        0        0    26967 2023-03-31 06:49:01.901395 dipex-4.9.1/exporters/sql_export/sql_export.py
--rw-r--r--   0        0        0     9581 2023-03-31 06:49:01.901395 dipex-4.9.1/exporters/sql_export/sql_table_defs.py
--rw-r--r--   0        0        0     5385 2023-03-31 06:49:01.901395 dipex-4.9.1/exporters/sql_export/sql_url.py
--rw-r--r--   0        0        0     4543 2023-03-31 06:49:01.902395 dipex-4.9.1/exporters/sql_export/trigger.py
--rw-r--r--   0        0        0     5075 2023-03-31 06:49:01.905396 dipex-4.9.1/exporters/utils/priority_by_class.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.115424 dipex-4.9.1/integrations/SD_Lon/sdlon/__init__.py
--rw-r--r--   0        0        0     5430 2023-03-31 06:49:01.910396 dipex-4.9.1/integrations/SD_Lon/sdlon/config.py
--rw-r--r--   0        0        0     5327 2023-03-31 06:49:01.910396 dipex-4.9.1/integrations/SD_Lon/sdlon/date_utils.py
--rw-r--r--   0        0        0     3797 2023-03-31 06:49:01.910396 dipex-4.9.1/integrations/SD_Lon/sdlon/engagement.py
--rw-r--r--   0        0        0       53 2023-03-31 06:49:01.910396 dipex-4.9.1/integrations/SD_Lon/sdlon/exceptions.py
--rw-r--r--   0        0        0    23227 2023-03-31 06:49:01.911396 dipex-4.9.1/integrations/SD_Lon/sdlon/fix_departments.py
--rw-r--r--   0        0        0     1864 2023-03-31 06:49:01.911396 dipex-4.9.1/integrations/SD_Lon/sdlon/main.py
--rw-r--r--   0        0        0      310 2023-03-31 06:49:01.911396 dipex-4.9.1/integrations/SD_Lon/sdlon/models.py
--rw-r--r--   0        0        0    60272 2023-03-31 06:49:01.911396 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_changed_at.py
--rw-r--r--   0        0        0     2147 2023-03-31 06:49:01.912397 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_changed_at_redo.py
--rw-r--r--   0        0        0      807 2023-03-31 06:49:01.912397 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_cli.py
--rw-r--r--   0        0        0     8897 2023-03-31 06:49:01.912397 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_common.py
--rw-r--r--   0        0        0    15184 2023-03-31 06:49:01.912397 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_fixup.py
--rw-r--r--   0        0        0    30844 2023-03-31 06:49:01.912397 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_importer.py
--rw-r--r--   0        0        0     6864 2023-03-31 06:49:01.913397 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_log_analyzer.py
--rw-r--r--   0        0        0      914 2023-03-31 06:49:01.913397 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_logging.py
--rw-r--r--   0        0        0     4533 2023-03-31 06:49:01.913397 dipex-4.9.1/integrations/SD_Lon/sdlon/sd_payloads.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.116425 dipex-4.9.1/integrations/SD_Lon/sdlon/sdclient/__init__.py
--rw-r--r--   0        0        0     3371 2023-03-31 06:49:01.913397 dipex-4.9.1/integrations/SD_Lon/sdlon/sdclient/client.py
--rw-r--r--   0        0        0     3309 2023-03-31 06:49:01.913397 dipex-4.9.1/integrations/SD_Lon/sdlon/sdclient/requests.py
--rw-r--r--   0        0        0     1327 2023-03-31 06:49:01.914397 dipex-4.9.1/integrations/SD_Lon/sdlon/sdclient/responses.py
--rw-r--r--   0        0        0      924 2023-03-31 06:49:01.914397 dipex-4.9.1/integrations/SD_Lon/sdlon/skip.py
--rw-r--r--   0        0        0     9414 2023-03-31 06:49:01.914397 dipex-4.9.1/integrations/SD_Lon/sdlon/sync_job_id.py
--rw-r--r--   0        0        0    12791 2023-03-31 06:49:01.915397 dipex-4.9.1/integrations/SD_Lon/sdlon/test_mo_against_sd.py
--rw-r--r--   0        0        0     2127 2023-03-31 06:49:01.915397 dipex-4.9.1/integrations/SD_Lon/sdlon/test_sd_connectivity.py
--rw-r--r--   0        0        0      361 2023-03-31 06:49:01.915397 dipex-4.9.1/integrations/SD_Lon/tests/__init__.py
--rw-r--r--   0        0        0    33857 2023-03-31 06:49:01.915397 dipex-4.9.1/integrations/SD_Lon/tests/fixtures.py
--rw-r--r--   0        0        0    10729 2023-03-31 06:49:01.916397 dipex-4.9.1/integrations/SD_Lon/tests/org_manipulations.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.119425 dipex-4.9.1/integrations/SD_Lon/tests/sdclient/__init__.py
--rw-r--r--   0        0        0     1643 2023-03-31 06:49:01.917397 dipex-4.9.1/integrations/SD_Lon/tests/sdclient/manual.py
--rw-r--r--   0        0        0      893 2023-03-31 06:49:01.917397 dipex-4.9.1/integrations/SD_Lon/tests/sdclient/test_requests.py
--rw-r--r--   0        0        0      568 2023-03-31 06:49:01.917397 dipex-4.9.1/integrations/SD_Lon/tests/sdclient/test_sdclient.py
--rw-r--r--   0        0        0     8901 2023-03-31 06:49:01.917397 dipex-4.9.1/integrations/SD_Lon/tests/test_config.py
--rw-r--r--   0        0        0    10906 2023-03-31 06:49:01.917397 dipex-4.9.1/integrations/SD_Lon/tests/test_date_utils.py
--rw-r--r--   0        0        0     2542 2023-03-31 06:49:01.917397 dipex-4.9.1/integrations/SD_Lon/tests/test_engagement.py
--rw-r--r--   0        0        0    16435 2023-03-31 06:49:01.918397 dipex-4.9.1/integrations/SD_Lon/tests/test_fix_departments.py
--rw-r--r--   0        0        0    38191 2023-03-31 06:49:01.918397 dipex-4.9.1/integrations/SD_Lon/tests/test_sd_changed_at.py
--rw-r--r--   0        0        0      743 2023-03-31 06:49:01.918397 dipex-4.9.1/integrations/SD_Lon/tests/test_sd_common.py
--rw-r--r--   0        0        0    23810 2023-03-31 06:49:01.919397 dipex-4.9.1/integrations/SD_Lon/tests/test_sd_importer.py
--rw-r--r--   0        0        0     8259 2023-03-31 06:49:01.919397 dipex-4.9.1/integrations/SD_Lon/tests/test_sd_log_analyzer.py
--rw-r--r--   0        0        0      970 2023-03-31 06:49:01.919397 dipex-4.9.1/integrations/SD_Lon/tests/test_skip.py
--rw-r--r--   0        0        0      916 2023-03-31 06:49:01.919397 dipex-4.9.1/integrations/SD_Lon/tests/test_sync_job_id.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.120425 dipex-4.9.1/integrations/__init__.py
--rw-r--r--   0        0        0     2897 2023-03-31 06:49:01.920398 dipex-4.9.1/integrations/aarhus/config.py
--rw-r--r--   0        0        0     3164 2023-03-31 06:49:01.920398 dipex-4.9.1/integrations/aarhus/initial.py
--rw-r--r--   0        0        0     3407 2023-03-31 06:49:01.920398 dipex-4.9.1/integrations/aarhus/initial_classes.py
--rw-r--r--   0        0        0     9582 2023-03-31 06:49:01.920398 dipex-4.9.1/integrations/aarhus/los_files.py
--rw-r--r--   0        0        0     3610 2023-03-31 06:49:01.920398 dipex-4.9.1/integrations/aarhus/los_import.py
--rw-r--r--   0        0        0     5086 2023-03-31 06:49:01.920398 dipex-4.9.1/integrations/aarhus/los_leder.py
--rw-r--r--   0        0        0    18423 2023-03-31 06:49:01.921398 dipex-4.9.1/integrations/aarhus/los_org.py
--rw-r--r--   0        0        0     9228 2023-03-31 06:49:01.921398 dipex-4.9.1/integrations/aarhus/los_pers.py
--rw-r--r--   0        0        0    16140 2023-03-31 06:49:01.921398 dipex-4.9.1/integrations/aarhus/los_stam.py
--rw-r--r--   0        0        0     4085 2023-03-31 06:49:01.921398 dipex-4.9.1/integrations/aarhus/payloads.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.120425 dipex-4.9.1/integrations/aarhus/tests/__init__.py
--rw-r--r--   0        0        0     1262 2023-03-31 06:49:01.922398 dipex-4.9.1/integrations/aarhus/tests/conftest.py
--rw-r--r--   0        0        0     3117 2023-03-31 06:49:01.922398 dipex-4.9.1/integrations/aarhus/tests/helpers.py
--rw-r--r--   0        0        0     2101 2023-03-31 06:49:01.922398 dipex-4.9.1/integrations/aarhus/tests/strategies.py
--rw-r--r--   0        0        0     1447 2023-03-31 06:49:01.922398 dipex-4.9.1/integrations/aarhus/tests/test_config.py
--rw-r--r--   0        0        0     1009 2023-03-31 06:49:01.922398 dipex-4.9.1/integrations/aarhus/tests/test_initial.py
--rw-r--r--   0        0        0     3178 2023-03-31 06:49:01.922398 dipex-4.9.1/integrations/aarhus/tests/test_los_files.py
--rw-r--r--   0        0        0     1200 2023-03-31 06:49:01.922398 dipex-4.9.1/integrations/aarhus/tests/test_los_import.py
--rw-r--r--   0        0        0    10703 2023-03-31 06:49:01.922398 dipex-4.9.1/integrations/aarhus/tests/test_los_leder.py
--rw-r--r--   0        0        0    11047 2023-03-31 06:49:01.923398 dipex-4.9.1/integrations/aarhus/tests/test_los_org.py
--rw-r--r--   0        0        0     6712 2023-03-31 06:49:01.923398 dipex-4.9.1/integrations/aarhus/tests/test_los_pers.py
--rw-r--r--   0        0        0    10378 2023-03-31 06:49:01.923398 dipex-4.9.1/integrations/aarhus/tests/test_los_stam.py
--rw-r--r--   0        0        0     1045 2023-03-31 06:49:01.923398 dipex-4.9.1/integrations/aarhus/tests/test_payloads.py
--rw-r--r--   0        0        0     7336 2023-03-31 06:49:01.923398 dipex-4.9.1/integrations/aarhus/tests/test_util.py
--rw-r--r--   0        0        0     6857 2023-03-31 06:49:01.924398 dipex-4.9.1/integrations/aarhus/util.py
--rw-r--r--   0        0        0     1073 2023-03-31 06:49:01.924398 dipex-4.9.1/integrations/aarhus/uuids.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.120425 dipex-4.9.1/integrations/ad_integration/__init__.py
--rw-r--r--   0        0        0    15777 2023-03-31 06:49:01.925398 dipex-4.9.1/integrations/ad_integration/ad_common.py
--rw-r--r--   0        0        0      852 2023-03-31 06:49:01.925398 dipex-4.9.1/integrations/ad_integration/ad_exceptions.py
--rw-r--r--   0        0        0     8746 2023-03-31 06:49:01.925398 dipex-4.9.1/integrations/ad_integration/ad_fix_enddate.py
--rw-r--r--   0        0        0     1272 2023-03-31 06:49:01.925398 dipex-4.9.1/integrations/ad_integration/ad_helpers.py
--rw-r--r--   0        0        0     3960 2023-03-31 06:49:01.925398 dipex-4.9.1/integrations/ad_integration/ad_jinja_filters.py
--rwxr-xr-x   0        0        0    19790 2023-03-31 06:49:01.925398 dipex-4.9.1/integrations/ad_integration/ad_life_cycle.py
--rw-r--r--   0        0        0     2446 2023-03-31 06:49:01.926398 dipex-4.9.1/integrations/ad_integration/ad_logger.py
--rw-r--r--   0        0        0     7800 2023-03-31 06:49:01.926398 dipex-4.9.1/integrations/ad_integration/ad_reader.py
--rw-r--r--   0        0        0    34383 2023-03-31 06:49:01.926398 dipex-4.9.1/integrations/ad_integration/ad_sync.py
--rw-r--r--   0        0        0    13395 2023-03-31 06:49:01.926398 dipex-4.9.1/integrations/ad_integration/ad_template_engine.py
--rw-r--r--   0        0        0      384 2023-03-31 06:49:01.927399 dipex-4.9.1/integrations/ad_integration/ad_templates.py
--rw-r--r--   0        0        0    48873 2023-03-31 06:49:01.927399 dipex-4.9.1/integrations/ad_integration/ad_writer.py
--rw-r--r--   0        0        0     6662 2023-03-31 06:49:01.927399 dipex-4.9.1/integrations/ad_integration/execute_ad_script.py
--rw-r--r--   0        0        0    11136 2023-03-31 06:49:01.927399 dipex-4.9.1/integrations/ad_integration/import_ad_group_into_mo.py
--rw-r--r--   0        0        0     8329 2023-03-31 06:49:01.928399 dipex-4.9.1/integrations/ad_integration/mo_to_ad_sync.py
--rw-r--r--   0        0        0     2522 2023-03-31 06:49:01.928399 dipex-4.9.1/integrations/ad_integration/payloads.py
--rw-r--r--   0        0        0     9037 2023-03-31 06:49:01.928399 dipex-4.9.1/integrations/ad_integration/read_ad_conf_settings.py
--rw-r--r--   0        0        0     7723 2023-03-31 06:49:01.928399 dipex-4.9.1/integrations/ad_integration/sync_mo_uuid_to_ad.py
--rw-r--r--   0        0        0     7502 2023-03-31 06:49:01.928399 dipex-4.9.1/integrations/ad_integration/test_connectivity.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.120425 dipex-4.9.1/integrations/ad_integration/tests/__init__.py
--rw-r--r--   0        0        0    14298 2023-03-31 06:49:01.929399 dipex-4.9.1/integrations/ad_integration/tests/mocks.py
--rw-r--r--   0        0        0      578 2023-03-31 06:49:01.929399 dipex-4.9.1/integrations/ad_integration/tests/name_simulator.py
--rw-r--r--   0        0        0     3238 2023-03-31 06:49:01.929399 dipex-4.9.1/integrations/ad_integration/tests/test_ad_common.py
--rw-r--r--   0        0        0     3374 2023-03-31 06:49:01.929399 dipex-4.9.1/integrations/ad_integration/tests/test_ad_fix_enddate.py
--rw-r--r--   0        0        0     4989 2023-03-31 06:49:01.929399 dipex-4.9.1/integrations/ad_integration/tests/test_ad_jinja_filters.py
--rw-r--r--   0        0        0    21234 2023-03-31 06:49:01.930399 dipex-4.9.1/integrations/ad_integration/tests/test_ad_life_cycle.py
--rw-r--r--   0        0        0      580 2023-03-31 06:49:01.930399 dipex-4.9.1/integrations/ad_integration/tests/test_ad_logger.py
--rw-r--r--   0        0        0     3989 2023-03-31 06:49:01.930399 dipex-4.9.1/integrations/ad_integration/tests/test_ad_reader.py
--rw-r--r--   0        0        0    43879 2023-03-31 06:49:01.930399 dipex-4.9.1/integrations/ad_integration/tests/test_ad_sync.py
--rw-r--r--   0        0        0    62395 2023-03-31 06:49:01.931399 dipex-4.9.1/integrations/ad_integration/tests/test_ad_writer.py
--rw-r--r--   0        0        0     2259 2023-03-31 06:49:01.931399 dipex-4.9.1/integrations/ad_integration/tests/test_dot_mapping.py
--rw-r--r--   0        0        0     1205 2023-03-31 06:49:01.931399 dipex-4.9.1/integrations/ad_integration/tests/test_first_included.py
--rw-r--r--   0        0        0     5180 2023-03-31 06:49:01.931399 dipex-4.9.1/integrations/ad_integration/tests/test_import_ad_group_into_mo.py
--rw-r--r--   0        0        0     4116 2023-03-31 06:49:01.931399 dipex-4.9.1/integrations/ad_integration/tests/test_location_element.py
--rw-r--r--   0        0        0     4983 2023-03-31 06:49:01.932399 dipex-4.9.1/integrations/ad_integration/tests/test_mo_data_source.py
--rw-r--r--   0        0        0     5527 2023-03-31 06:49:01.932399 dipex-4.9.1/integrations/ad_integration/tests/test_mo_to_ad_sync.py
--rw-r--r--   0        0        0     1434 2023-03-31 06:49:01.932399 dipex-4.9.1/integrations/ad_integration/tests/test_morestsource.py
--rw-r--r--   0        0        0     5408 2023-03-31 06:49:01.932399 dipex-4.9.1/integrations/ad_integration/tests/test_read_ad_conf_settings.py
--rw-r--r--   0        0        0     1896 2023-03-31 06:49:01.932399 dipex-4.9.1/integrations/ad_integration/tests/test_recursive_dict_update.py
--rw-r--r--   0        0        0     4753 2023-03-31 06:49:01.932399 dipex-4.9.1/integrations/ad_integration/tests/test_sync_mo_uuid_to_ad.py
--rw-r--r--   0        0        0    24432 2023-03-31 06:49:01.933400 dipex-4.9.1/integrations/ad_integration/tests/test_usernames.py
--rw-r--r--   0        0        0    20179 2023-03-31 06:49:01.933400 dipex-4.9.1/integrations/ad_integration/tests/test_utils.py
--rw-r--r--   0        0        0    16376 2023-03-31 06:49:01.933400 dipex-4.9.1/integrations/ad_integration/user_names.py
--rw-r--r--   0        0        0     4306 2023-03-31 06:49:01.933400 dipex-4.9.1/integrations/ad_integration/username_rules/method_2.py
--rw-r--r--   0        0        0     5291 2023-03-31 06:49:01.933400 dipex-4.9.1/integrations/ad_integration/utils.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.120425 dipex-4.9.1/integrations/adtreesync/__init__.py
--rw-r--r--   0        0        0      627 2023-03-31 06:49:01.934399 dipex-4.9.1/integrations/adtreesync/config.py
--rw-r--r--   0        0        0     1777 2023-03-31 06:49:01.934399 dipex-4.9.1/integrations/adtreesync/ldap.py
--rw-r--r--   0        0        0     9319 2023-03-31 06:49:01.934399 dipex-4.9.1/integrations/adtreesync/main.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.121425 dipex-4.9.1/integrations/adtreesync/tests/__init__.py
--rw-r--r--   0        0        0     2641 2023-03-31 06:49:01.934399 dipex-4.9.1/integrations/adtreesync/tests/test_main.py
--rw-r--r--   0        0        0    33116 2023-03-31 06:49:01.934399 dipex-4.9.1/integrations/apos_importer.py
--rw-r--r--   0        0        0      539 2023-03-31 06:49:01.935400 dipex-4.9.1/integrations/ballerup/ballerup-amqp.py
--rw-r--r--   0        0        0     2059 2023-03-31 06:49:01.935400 dipex-4.9.1/integrations/ballerup/ballerup.py
--rw-r--r--   0        0        0     9954 2023-03-31 06:49:01.935400 dipex-4.9.1/integrations/ballerup/udvalg_import.py
--rw-r--r--   0        0        0      964 2023-03-31 06:49:01.935400 dipex-4.9.1/integrations/brøndby/brøndby.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.122426 dipex-4.9.1/integrations/calculate_primary/__init__.py
--rw-r--r--   0        0        0     3149 2023-03-31 06:49:01.936400 dipex-4.9.1/integrations/calculate_primary/calculate_primary.py
--rw-r--r--   0        0        0    19033 2023-03-31 06:49:01.936400 dipex-4.9.1/integrations/calculate_primary/common.py
--rw-r--r--   0        0        0     2597 2023-03-31 06:49:01.936400 dipex-4.9.1/integrations/calculate_primary/default.py
--rw-r--r--   0        0        0     4045 2023-03-31 06:49:01.936400 dipex-4.9.1/integrations/calculate_primary/opus.py
--rw-r--r--   0        0        0     3651 2023-03-31 06:49:01.937400 dipex-4.9.1/integrations/calculate_primary/sd.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.122426 dipex-4.9.1/integrations/calculate_primary/tests/__init__.py
--rw-r--r--   0        0        0    19238 2023-03-31 06:49:01.937400 dipex-4.9.1/integrations/calculate_primary/tests/test_primary.py
--rw-r--r--   0        0        0      896 2023-03-31 06:49:01.937400 dipex-4.9.1/integrations/cpr_mapper.py
--rw-r--r--   0        0        0        0 2023-03-31 06:49:02.122426 dipex-4.9.1/integrations/dar_helper/__init__.py
--rw-r--r--   0        0        0     5035 2023-03-31 06:49:01.937400 dipex-4.9.1/integrations/dar_helper/dar_helper.py
--rw-r--r--   0        0        0     1010 2023-03-31 06:49:01.938400 dipex-4.9.1/integrations/dawa_helper.py
--rw-r--r--   0        0        0     1765 2023-03-31 06:49:01.938400 dipex-4.9.1/integrations/egedal/egedal.py
--rw-r--r--   0        0        0     3565 2023-03-31 06:49:01.938400 dipex-4.9.1/integrations/fkorg_it_systems/import_fkorg_orgunits.py
--rw-r--r--   0        0        0     1569 2023-03-31 06:49:01.938400 dipex-4.9.1/integrations/fkorg_it_systems/test_import_fk_org.py
--rw-r--r--   0        0        0    20309 2023-03-31 06:49:01.939400 dipex-4.9.1/integrations/gir/initial_read/emd_csv.py
--rw-r--r--   0        0        0     8600 2023-03-31 06:49:01.939400 dipex-4.9.1/integrations/gir/initial_read/main.py
--rw-r--r--   0        0        0     1416 2023-03-31 06:49:01.939400 dipex-4.9.1/integrations/gir/initial_read/mo_lora_client.py
--rw-r--r--   0        0        0     4304 2023-03-31 06:49:01.939400 dipex-4.9.1/integrations/gir/initial_read/org_unit_csv.py
--rw-r--r--   0        0        0      954 2023-03-31 06:49:01.940400 dipex-4.9.1/integrations/hjørring/hjørring.py
--rw-r--r--   0        0        0     1395 2023-03-31 06:49:01.940400 dipex-4.9.1/integrations/holstebro/holstebro.py
--rw-r--r--   0        0        0    16956 2023-03-31 06:49:01.941401 dipex-4.9.1/integrations/kle/kle_import_export.py
--rw-r--r--   0        0        0     8663 2023-03-31 06:49:01.941401 dipex-4.9.1/integrations/kle/kle_xlsx.py
--rw-r--r--   0        0        0      745 2023-03-31 06:49:01.941401 dipex-4.9.1/integrations/næstved/næstved.py
--rw-r--r--   0        0        0     4550 2023-03-31 06:49:01.942401 dipex-4.9.1/integrations/opus/clear_and_import_opus.py
--rw-r--r--   0        0        0    40259 2023-03-31 06:49:01.942401 dipex-4.9.1/integrations/opus/opus_diff_import.py
--rw-r--r--   0        0        0      353 2023-03-31 06:49:01.942401 dipex-4.9.1/integrations/opus/opus_exceptions.py
--rw-r--r--   0        0        0     4348 2023-03-31 06:49:01.942401 dipex-4.9.1/integrations/opus/opus_file_reader.py
--rw-r--r--   0        0        0    14217 2023-03-31 06:49:01.943401 dipex-4.9.1/integrations/opus/opus_helpers.py
--rw-r--r--   0        0        0     2958 2023-03-31 06:49:01.943401 dipex-4.9.1/integrations/opus/opus_reimport_one.py
--rw-r--r--   0        0        0     4515 2023-03-31 06:49:01.943401 dipex-4.9.1/integrations/opus/org_tree_print/main.py
--rw-r--r--   0        0        0     5449 2023-03-31 06:49:01.943401 dipex-4.9.1/integrations/opus/payloads.py
--rw-r--r--   0        0        0    18762 2023-03-31 06:49:01.944401 dipex-4.9.1/integrations/opus/tests/test_opus_diff_import.py
--rw-r--r--   0        0        0     1406 2023-03-31 06:49:01.944401 dipex-4.9.1/integrations/opus/tests/test_opus_file_reader.py
--rw-r--r--   0        0        0     4016 2023-03-31 06:49:01.944401 dipex-4.9.1/integrations/opus/tests/test_opus_helpers.py
--rw-r--r--   0        0        0     1789 2023-03-31 06:49:01.945401 dipex-4.9.1/integrations/related_units/from_adtreesync.py
--rw-r--r--   0        0        0     1368 2023-03-31 06:49:01.945401 dipex-4.9.1/integrations/related_units/import_related_units.py
--rw-r--r--   0        0        0     4562 2023-03-31 06:49:01.946401 dipex-4.9.1/integrations/rundb/db_overview.py
--rw-r--r--   0        0        0     1228 2023-03-31 06:49:01.946401 dipex-4.9.1/integrations/rundb/tests/test_db_overview.py
--rw-r--r--   0        0        0     9290 2023-03-31 06:49:01.947401 dipex-4.9.1/integrations/viborg/udvalg_import.py
--rw-r--r--   0        0        0     2919 2023-03-31 06:49:01.947401 dipex-4.9.1/integrations/viborg/viborg.py
--rw-r--r--   0        0        0      922 2023-03-31 06:49:01.947401 dipex-4.9.1/integrations/viborg/viborg_uuids.py
--rw-r--r--   0        0        0     3147 2023-03-31 06:49:01.948402 dipex-4.9.1/integrations/viborg/viborg_without_ad.py
--rw-r--r--   0        0        0     2525 2023-03-31 06:49:05.850941 dipex-4.9.1/pyproject.toml
--rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 dipex-4.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1392 2023-03-31 09:19:41.414775 dipex-4.9.2/README.rst
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.605801 dipex-4.9.2/exporters/sql_export/__init__.py
+-rw-r--r--   0        0        0     2129 2023-03-31 09:19:41.437778 dipex-4.9.2/exporters/sql_export/lc_for_jobs_db.py
+-rw-r--r--   0        0        0    56625 2023-03-31 09:19:41.438778 dipex-4.9.2/exporters/sql_export/lora_cache.py
+-rw-r--r--   0        0        0     2529 2023-03-31 09:19:41.438778 dipex-4.9.2/exporters/sql_export/main.py
+-rw-r--r--   0        0        0    26967 2023-03-31 09:19:41.440779 dipex-4.9.2/exporters/sql_export/sql_export.py
+-rw-r--r--   0        0        0     9581 2023-03-31 09:19:41.440779 dipex-4.9.2/exporters/sql_export/sql_table_defs.py
+-rw-r--r--   0        0        0     5385 2023-03-31 09:19:41.440779 dipex-4.9.2/exporters/sql_export/sql_url.py
+-rw-r--r--   0        0        0     4543 2023-03-31 09:19:41.441779 dipex-4.9.2/exporters/sql_export/trigger.py
+-rw-r--r--   0        0        0     5075 2023-03-31 09:19:41.444779 dipex-4.9.2/exporters/utils/priority_by_class.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.610802 dipex-4.9.2/integrations/SD_Lon/sdlon/__init__.py
+-rw-r--r--   0        0        0     5430 2023-03-31 09:19:41.449780 dipex-4.9.2/integrations/SD_Lon/sdlon/config.py
+-rw-r--r--   0        0        0     5327 2023-03-31 09:19:41.449780 dipex-4.9.2/integrations/SD_Lon/sdlon/date_utils.py
+-rw-r--r--   0        0        0     3797 2023-03-31 09:19:41.449780 dipex-4.9.2/integrations/SD_Lon/sdlon/engagement.py
+-rw-r--r--   0        0        0       53 2023-03-31 09:19:41.449780 dipex-4.9.2/integrations/SD_Lon/sdlon/exceptions.py
+-rw-r--r--   0        0        0    23227 2023-03-31 09:19:41.450780 dipex-4.9.2/integrations/SD_Lon/sdlon/fix_departments.py
+-rw-r--r--   0        0        0     1864 2023-03-31 09:19:41.450780 dipex-4.9.2/integrations/SD_Lon/sdlon/main.py
+-rw-r--r--   0        0        0      310 2023-03-31 09:19:41.450780 dipex-4.9.2/integrations/SD_Lon/sdlon/models.py
+-rw-r--r--   0        0        0    60272 2023-03-31 09:19:41.451780 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_changed_at.py
+-rw-r--r--   0        0        0     2147 2023-03-31 09:19:41.451780 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_changed_at_redo.py
+-rw-r--r--   0        0        0      807 2023-03-31 09:19:41.451780 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_cli.py
+-rw-r--r--   0        0        0     8897 2023-03-31 09:19:41.451780 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_common.py
+-rw-r--r--   0        0        0    15184 2023-03-31 09:19:41.452780 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_fixup.py
+-rw-r--r--   0        0        0    30844 2023-03-31 09:19:41.452780 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_importer.py
+-rw-r--r--   0        0        0     6864 2023-03-31 09:19:41.452780 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_log_analyzer.py
+-rw-r--r--   0        0        0      914 2023-03-31 09:19:41.453781 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_logging.py
+-rw-r--r--   0        0        0     4533 2023-03-31 09:19:41.453781 dipex-4.9.2/integrations/SD_Lon/sdlon/sd_payloads.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.652808 dipex-4.9.2/integrations/SD_Lon/sdlon/sdclient/__init__.py
+-rw-r--r--   0        0        0     3371 2023-03-31 09:19:41.453781 dipex-4.9.2/integrations/SD_Lon/sdlon/sdclient/client.py
+-rw-r--r--   0        0        0     3309 2023-03-31 09:19:41.453781 dipex-4.9.2/integrations/SD_Lon/sdlon/sdclient/requests.py
+-rw-r--r--   0        0        0     1327 2023-03-31 09:19:41.453781 dipex-4.9.2/integrations/SD_Lon/sdlon/sdclient/responses.py
+-rw-r--r--   0        0        0      924 2023-03-31 09:19:41.453781 dipex-4.9.2/integrations/SD_Lon/sdlon/skip.py
+-rw-r--r--   0        0        0     9414 2023-03-31 09:19:41.453781 dipex-4.9.2/integrations/SD_Lon/sdlon/sync_job_id.py
+-rw-r--r--   0        0        0    12791 2023-03-31 09:19:41.454781 dipex-4.9.2/integrations/SD_Lon/sdlon/test_mo_against_sd.py
+-rw-r--r--   0        0        0     2127 2023-03-31 09:19:41.454781 dipex-4.9.2/integrations/SD_Lon/sdlon/test_sd_connectivity.py
+-rw-r--r--   0        0        0      361 2023-03-31 09:19:41.454781 dipex-4.9.2/integrations/SD_Lon/tests/__init__.py
+-rw-r--r--   0        0        0    33857 2023-03-31 09:19:41.454781 dipex-4.9.2/integrations/SD_Lon/tests/fixtures.py
+-rw-r--r--   0        0        0    10729 2023-03-31 09:19:41.455781 dipex-4.9.2/integrations/SD_Lon/tests/org_manipulations.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.652808 dipex-4.9.2/integrations/SD_Lon/tests/sdclient/__init__.py
+-rw-r--r--   0        0        0     1643 2023-03-31 09:19:41.455781 dipex-4.9.2/integrations/SD_Lon/tests/sdclient/manual.py
+-rw-r--r--   0        0        0      893 2023-03-31 09:19:41.456781 dipex-4.9.2/integrations/SD_Lon/tests/sdclient/test_requests.py
+-rw-r--r--   0        0        0      568 2023-03-31 09:19:41.456781 dipex-4.9.2/integrations/SD_Lon/tests/sdclient/test_sdclient.py
+-rw-r--r--   0        0        0     8901 2023-03-31 09:19:41.456781 dipex-4.9.2/integrations/SD_Lon/tests/test_config.py
+-rw-r--r--   0        0        0    10906 2023-03-31 09:19:41.456781 dipex-4.9.2/integrations/SD_Lon/tests/test_date_utils.py
+-rw-r--r--   0        0        0     2542 2023-03-31 09:19:41.456781 dipex-4.9.2/integrations/SD_Lon/tests/test_engagement.py
+-rw-r--r--   0        0        0    16435 2023-03-31 09:19:41.456781 dipex-4.9.2/integrations/SD_Lon/tests/test_fix_departments.py
+-rw-r--r--   0        0        0    38191 2023-03-31 09:19:41.457781 dipex-4.9.2/integrations/SD_Lon/tests/test_sd_changed_at.py
+-rw-r--r--   0        0        0      743 2023-03-31 09:19:41.457781 dipex-4.9.2/integrations/SD_Lon/tests/test_sd_common.py
+-rw-r--r--   0        0        0    23810 2023-03-31 09:19:41.457781 dipex-4.9.2/integrations/SD_Lon/tests/test_sd_importer.py
+-rw-r--r--   0        0        0     8259 2023-03-31 09:19:41.457781 dipex-4.9.2/integrations/SD_Lon/tests/test_sd_log_analyzer.py
+-rw-r--r--   0        0        0      970 2023-03-31 09:19:41.457781 dipex-4.9.2/integrations/SD_Lon/tests/test_skip.py
+-rw-r--r--   0        0        0      916 2023-03-31 09:19:41.457781 dipex-4.9.2/integrations/SD_Lon/tests/test_sync_job_id.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.652808 dipex-4.9.2/integrations/__init__.py
+-rw-r--r--   0        0        0     2897 2023-03-31 09:19:41.458781 dipex-4.9.2/integrations/aarhus/config.py
+-rw-r--r--   0        0        0     3164 2023-03-31 09:19:41.458781 dipex-4.9.2/integrations/aarhus/initial.py
+-rw-r--r--   0        0        0     3407 2023-03-31 09:19:41.458781 dipex-4.9.2/integrations/aarhus/initial_classes.py
+-rw-r--r--   0        0        0     9582 2023-03-31 09:19:41.459781 dipex-4.9.2/integrations/aarhus/los_files.py
+-rw-r--r--   0        0        0     3610 2023-03-31 09:19:41.459781 dipex-4.9.2/integrations/aarhus/los_import.py
+-rw-r--r--   0        0        0     5086 2023-03-31 09:19:41.459781 dipex-4.9.2/integrations/aarhus/los_leder.py
+-rw-r--r--   0        0        0    18423 2023-03-31 09:19:41.459781 dipex-4.9.2/integrations/aarhus/los_org.py
+-rw-r--r--   0        0        0     9228 2023-03-31 09:19:41.460781 dipex-4.9.2/integrations/aarhus/los_pers.py
+-rw-r--r--   0        0        0    16140 2023-03-31 09:19:41.460781 dipex-4.9.2/integrations/aarhus/los_stam.py
+-rw-r--r--   0        0        0     4085 2023-03-31 09:19:41.460781 dipex-4.9.2/integrations/aarhus/payloads.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.652808 dipex-4.9.2/integrations/aarhus/tests/__init__.py
+-rw-r--r--   0        0        0     1262 2023-03-31 09:19:41.460781 dipex-4.9.2/integrations/aarhus/tests/conftest.py
+-rw-r--r--   0        0        0     3117 2023-03-31 09:19:41.460781 dipex-4.9.2/integrations/aarhus/tests/helpers.py
+-rw-r--r--   0        0        0     2101 2023-03-31 09:19:41.460781 dipex-4.9.2/integrations/aarhus/tests/strategies.py
+-rw-r--r--   0        0        0     1447 2023-03-31 09:19:41.461782 dipex-4.9.2/integrations/aarhus/tests/test_config.py
+-rw-r--r--   0        0        0     1009 2023-03-31 09:19:41.461782 dipex-4.9.2/integrations/aarhus/tests/test_initial.py
+-rw-r--r--   0        0        0     3178 2023-03-31 09:19:41.461782 dipex-4.9.2/integrations/aarhus/tests/test_los_files.py
+-rw-r--r--   0        0        0     1200 2023-03-31 09:19:41.461782 dipex-4.9.2/integrations/aarhus/tests/test_los_import.py
+-rw-r--r--   0        0        0    10703 2023-03-31 09:19:41.461782 dipex-4.9.2/integrations/aarhus/tests/test_los_leder.py
+-rw-r--r--   0        0        0    11047 2023-03-31 09:19:41.461782 dipex-4.9.2/integrations/aarhus/tests/test_los_org.py
+-rw-r--r--   0        0        0     6712 2023-03-31 09:19:41.461782 dipex-4.9.2/integrations/aarhus/tests/test_los_pers.py
+-rw-r--r--   0        0        0    10378 2023-03-31 09:19:41.462782 dipex-4.9.2/integrations/aarhus/tests/test_los_stam.py
+-rw-r--r--   0        0        0     1045 2023-03-31 09:19:41.462782 dipex-4.9.2/integrations/aarhus/tests/test_payloads.py
+-rw-r--r--   0        0        0     7336 2023-03-31 09:19:41.462782 dipex-4.9.2/integrations/aarhus/tests/test_util.py
+-rw-r--r--   0        0        0     6857 2023-03-31 09:19:41.462782 dipex-4.9.2/integrations/aarhus/util.py
+-rw-r--r--   0        0        0     1073 2023-03-31 09:19:41.462782 dipex-4.9.2/integrations/aarhus/uuids.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.652808 dipex-4.9.2/integrations/ad_integration/__init__.py
+-rw-r--r--   0        0        0    15777 2023-03-31 09:19:41.463782 dipex-4.9.2/integrations/ad_integration/ad_common.py
+-rw-r--r--   0        0        0      852 2023-03-31 09:19:41.463782 dipex-4.9.2/integrations/ad_integration/ad_exceptions.py
+-rw-r--r--   0        0        0     8746 2023-03-31 09:19:41.463782 dipex-4.9.2/integrations/ad_integration/ad_fix_enddate.py
+-rw-r--r--   0        0        0     1272 2023-03-31 09:19:41.463782 dipex-4.9.2/integrations/ad_integration/ad_helpers.py
+-rw-r--r--   0        0        0     3960 2023-03-31 09:19:41.463782 dipex-4.9.2/integrations/ad_integration/ad_jinja_filters.py
+-rwxr-xr-x   0        0        0    19790 2023-03-31 09:19:41.464782 dipex-4.9.2/integrations/ad_integration/ad_life_cycle.py
+-rw-r--r--   0        0        0     2446 2023-03-31 09:19:41.464782 dipex-4.9.2/integrations/ad_integration/ad_logger.py
+-rw-r--r--   0        0        0     7800 2023-03-31 09:19:41.464782 dipex-4.9.2/integrations/ad_integration/ad_reader.py
+-rw-r--r--   0        0        0    34383 2023-03-31 09:19:41.464782 dipex-4.9.2/integrations/ad_integration/ad_sync.py
+-rw-r--r--   0        0        0    13395 2023-03-31 09:19:41.465782 dipex-4.9.2/integrations/ad_integration/ad_template_engine.py
+-rw-r--r--   0        0        0      384 2023-03-31 09:19:41.465782 dipex-4.9.2/integrations/ad_integration/ad_templates.py
+-rw-r--r--   0        0        0    48873 2023-03-31 09:19:41.465782 dipex-4.9.2/integrations/ad_integration/ad_writer.py
+-rw-r--r--   0        0        0     6662 2023-03-31 09:19:41.465782 dipex-4.9.2/integrations/ad_integration/execute_ad_script.py
+-rw-r--r--   0        0        0    11136 2023-03-31 09:19:41.466782 dipex-4.9.2/integrations/ad_integration/import_ad_group_into_mo.py
+-rw-r--r--   0        0        0     8329 2023-03-31 09:19:41.466782 dipex-4.9.2/integrations/ad_integration/mo_to_ad_sync.py
+-rw-r--r--   0        0        0     2522 2023-03-31 09:19:41.466782 dipex-4.9.2/integrations/ad_integration/payloads.py
+-rw-r--r--   0        0        0     9037 2023-03-31 09:19:41.466782 dipex-4.9.2/integrations/ad_integration/read_ad_conf_settings.py
+-rw-r--r--   0        0        0     7902 2023-03-31 09:19:41.466782 dipex-4.9.2/integrations/ad_integration/sync_mo_uuid_to_ad.py
+-rw-r--r--   0        0        0     7502 2023-03-31 09:19:41.466782 dipex-4.9.2/integrations/ad_integration/test_connectivity.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.653808 dipex-4.9.2/integrations/ad_integration/tests/__init__.py
+-rw-r--r--   0        0        0    14298 2023-03-31 09:19:41.467782 dipex-4.9.2/integrations/ad_integration/tests/mocks.py
+-rw-r--r--   0        0        0      578 2023-03-31 09:19:41.467782 dipex-4.9.2/integrations/ad_integration/tests/name_simulator.py
+-rw-r--r--   0        0        0     3238 2023-03-31 09:19:41.467782 dipex-4.9.2/integrations/ad_integration/tests/test_ad_common.py
+-rw-r--r--   0        0        0     3374 2023-03-31 09:19:41.467782 dipex-4.9.2/integrations/ad_integration/tests/test_ad_fix_enddate.py
+-rw-r--r--   0        0        0     4989 2023-03-31 09:19:41.467782 dipex-4.9.2/integrations/ad_integration/tests/test_ad_jinja_filters.py
+-rw-r--r--   0        0        0    21234 2023-03-31 09:19:41.468783 dipex-4.9.2/integrations/ad_integration/tests/test_ad_life_cycle.py
+-rw-r--r--   0        0        0      580 2023-03-31 09:19:41.468783 dipex-4.9.2/integrations/ad_integration/tests/test_ad_logger.py
+-rw-r--r--   0        0        0     3989 2023-03-31 09:19:41.468783 dipex-4.9.2/integrations/ad_integration/tests/test_ad_reader.py
+-rw-r--r--   0        0        0    43879 2023-03-31 09:19:41.468783 dipex-4.9.2/integrations/ad_integration/tests/test_ad_sync.py
+-rw-r--r--   0        0        0    62395 2023-03-31 09:19:41.469783 dipex-4.9.2/integrations/ad_integration/tests/test_ad_writer.py
+-rw-r--r--   0        0        0     2259 2023-03-31 09:19:41.469783 dipex-4.9.2/integrations/ad_integration/tests/test_dot_mapping.py
+-rw-r--r--   0        0        0     1205 2023-03-31 09:19:41.469783 dipex-4.9.2/integrations/ad_integration/tests/test_first_included.py
+-rw-r--r--   0        0        0     5180 2023-03-31 09:19:41.469783 dipex-4.9.2/integrations/ad_integration/tests/test_import_ad_group_into_mo.py
+-rw-r--r--   0        0        0     4116 2023-03-31 09:19:41.469783 dipex-4.9.2/integrations/ad_integration/tests/test_location_element.py
+-rw-r--r--   0        0        0     4983 2023-03-31 09:19:41.470783 dipex-4.9.2/integrations/ad_integration/tests/test_mo_data_source.py
+-rw-r--r--   0        0        0     5527 2023-03-31 09:19:41.470783 dipex-4.9.2/integrations/ad_integration/tests/test_mo_to_ad_sync.py
+-rw-r--r--   0        0        0     1434 2023-03-31 09:19:41.470783 dipex-4.9.2/integrations/ad_integration/tests/test_morestsource.py
+-rw-r--r--   0        0        0     5408 2023-03-31 09:19:41.470783 dipex-4.9.2/integrations/ad_integration/tests/test_read_ad_conf_settings.py
+-rw-r--r--   0        0        0     1896 2023-03-31 09:19:41.470783 dipex-4.9.2/integrations/ad_integration/tests/test_recursive_dict_update.py
+-rw-r--r--   0        0        0     5579 2023-03-31 09:19:41.470783 dipex-4.9.2/integrations/ad_integration/tests/test_sync_mo_uuid_to_ad.py
+-rw-r--r--   0        0        0    24432 2023-03-31 09:19:41.471783 dipex-4.9.2/integrations/ad_integration/tests/test_usernames.py
+-rw-r--r--   0        0        0    20179 2023-03-31 09:19:41.471783 dipex-4.9.2/integrations/ad_integration/tests/test_utils.py
+-rw-r--r--   0        0        0    16376 2023-03-31 09:19:41.471783 dipex-4.9.2/integrations/ad_integration/user_names.py
+-rw-r--r--   0        0        0     4306 2023-03-31 09:19:41.471783 dipex-4.9.2/integrations/ad_integration/username_rules/method_2.py
+-rw-r--r--   0        0        0     5291 2023-03-31 09:19:41.471783 dipex-4.9.2/integrations/ad_integration/utils.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.653808 dipex-4.9.2/integrations/adtreesync/__init__.py
+-rw-r--r--   0        0        0      627 2023-03-31 09:19:41.472783 dipex-4.9.2/integrations/adtreesync/config.py
+-rw-r--r--   0        0        0     1777 2023-03-31 09:19:41.472783 dipex-4.9.2/integrations/adtreesync/ldap.py
+-rw-r--r--   0        0        0     9319 2023-03-31 09:19:41.472783 dipex-4.9.2/integrations/adtreesync/main.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.653808 dipex-4.9.2/integrations/adtreesync/tests/__init__.py
+-rw-r--r--   0        0        0     2641 2023-03-31 09:19:41.472783 dipex-4.9.2/integrations/adtreesync/tests/test_main.py
+-rw-r--r--   0        0        0    33116 2023-03-31 09:19:41.473783 dipex-4.9.2/integrations/apos_importer.py
+-rw-r--r--   0        0        0      539 2023-03-31 09:19:41.473783 dipex-4.9.2/integrations/ballerup/ballerup-amqp.py
+-rw-r--r--   0        0        0     2059 2023-03-31 09:19:41.473783 dipex-4.9.2/integrations/ballerup/ballerup.py
+-rw-r--r--   0        0        0     9954 2023-03-31 09:19:41.473783 dipex-4.9.2/integrations/ballerup/udvalg_import.py
+-rw-r--r--   0        0        0      964 2023-03-31 09:19:41.473783 dipex-4.9.2/integrations/brøndby/brøndby.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.653808 dipex-4.9.2/integrations/calculate_primary/__init__.py
+-rw-r--r--   0        0        0     3149 2023-03-31 09:19:41.474783 dipex-4.9.2/integrations/calculate_primary/calculate_primary.py
+-rw-r--r--   0        0        0    19033 2023-03-31 09:19:41.474783 dipex-4.9.2/integrations/calculate_primary/common.py
+-rw-r--r--   0        0        0     2597 2023-03-31 09:19:41.474783 dipex-4.9.2/integrations/calculate_primary/default.py
+-rw-r--r--   0        0        0     4045 2023-03-31 09:19:41.475783 dipex-4.9.2/integrations/calculate_primary/opus.py
+-rw-r--r--   0        0        0     3651 2023-03-31 09:19:41.475783 dipex-4.9.2/integrations/calculate_primary/sd.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.656808 dipex-4.9.2/integrations/calculate_primary/tests/__init__.py
+-rw-r--r--   0        0        0    19238 2023-03-31 09:19:41.476784 dipex-4.9.2/integrations/calculate_primary/tests/test_primary.py
+-rw-r--r--   0        0        0      896 2023-03-31 09:19:41.476784 dipex-4.9.2/integrations/cpr_mapper.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:19:41.656808 dipex-4.9.2/integrations/dar_helper/__init__.py
+-rw-r--r--   0        0        0     5035 2023-03-31 09:19:41.476784 dipex-4.9.2/integrations/dar_helper/dar_helper.py
+-rw-r--r--   0        0        0     1010 2023-03-31 09:19:41.476784 dipex-4.9.2/integrations/dawa_helper.py
+-rw-r--r--   0        0        0     1765 2023-03-31 09:19:41.476784 dipex-4.9.2/integrations/egedal/egedal.py
+-rw-r--r--   0        0        0     3565 2023-03-31 09:19:41.477784 dipex-4.9.2/integrations/fkorg_it_systems/import_fkorg_orgunits.py
+-rw-r--r--   0        0        0     1569 2023-03-31 09:19:41.477784 dipex-4.9.2/integrations/fkorg_it_systems/test_import_fk_org.py
+-rw-r--r--   0        0        0    20309 2023-03-31 09:19:41.477784 dipex-4.9.2/integrations/gir/initial_read/emd_csv.py
+-rw-r--r--   0        0        0     8600 2023-03-31 09:19:41.478784 dipex-4.9.2/integrations/gir/initial_read/main.py
+-rw-r--r--   0        0        0     1416 2023-03-31 09:19:41.478784 dipex-4.9.2/integrations/gir/initial_read/mo_lora_client.py
+-rw-r--r--   0        0        0     4304 2023-03-31 09:19:41.478784 dipex-4.9.2/integrations/gir/initial_read/org_unit_csv.py
+-rw-r--r--   0        0        0      954 2023-03-31 09:19:41.478784 dipex-4.9.2/integrations/hjørring/hjørring.py
+-rw-r--r--   0        0        0     1395 2023-03-31 09:19:41.478784 dipex-4.9.2/integrations/holstebro/holstebro.py
+-rw-r--r--   0        0        0    16956 2023-03-31 09:19:41.479784 dipex-4.9.2/integrations/kle/kle_import_export.py
+-rw-r--r--   0        0        0     8663 2023-03-31 09:19:41.479784 dipex-4.9.2/integrations/kle/kle_xlsx.py
+-rw-r--r--   0        0        0      745 2023-03-31 09:19:41.479784 dipex-4.9.2/integrations/næstved/næstved.py
+-rw-r--r--   0        0        0     4550 2023-03-31 09:19:41.480784 dipex-4.9.2/integrations/opus/clear_and_import_opus.py
+-rw-r--r--   0        0        0    40259 2023-03-31 09:19:41.480784 dipex-4.9.2/integrations/opus/opus_diff_import.py
+-rw-r--r--   0        0        0      353 2023-03-31 09:19:41.480784 dipex-4.9.2/integrations/opus/opus_exceptions.py
+-rw-r--r--   0        0        0     4348 2023-03-31 09:19:41.480784 dipex-4.9.2/integrations/opus/opus_file_reader.py
+-rw-r--r--   0        0        0    14217 2023-03-31 09:19:41.481784 dipex-4.9.2/integrations/opus/opus_helpers.py
+-rw-r--r--   0        0        0     2958 2023-03-31 09:19:41.481784 dipex-4.9.2/integrations/opus/opus_reimport_one.py
+-rw-r--r--   0        0        0     4515 2023-03-31 09:19:41.481784 dipex-4.9.2/integrations/opus/org_tree_print/main.py
+-rw-r--r--   0        0        0     5449 2023-03-31 09:19:41.481784 dipex-4.9.2/integrations/opus/payloads.py
+-rw-r--r--   0        0        0    18762 2023-03-31 09:19:41.482784 dipex-4.9.2/integrations/opus/tests/test_opus_diff_import.py
+-rw-r--r--   0        0        0     1406 2023-03-31 09:19:41.482784 dipex-4.9.2/integrations/opus/tests/test_opus_file_reader.py
+-rw-r--r--   0        0        0     4016 2023-03-31 09:19:41.482784 dipex-4.9.2/integrations/opus/tests/test_opus_helpers.py
+-rw-r--r--   0        0        0     1789 2023-03-31 09:19:41.483785 dipex-4.9.2/integrations/related_units/from_adtreesync.py
+-rw-r--r--   0        0        0     1368 2023-03-31 09:19:41.483785 dipex-4.9.2/integrations/related_units/import_related_units.py
+-rw-r--r--   0        0        0     4562 2023-03-31 09:19:41.484785 dipex-4.9.2/integrations/rundb/db_overview.py
+-rw-r--r--   0        0        0     1228 2023-03-31 09:19:41.484785 dipex-4.9.2/integrations/rundb/tests/test_db_overview.py
+-rw-r--r--   0        0        0     9290 2023-03-31 09:19:41.485785 dipex-4.9.2/integrations/viborg/udvalg_import.py
+-rw-r--r--   0        0        0     2919 2023-03-31 09:19:41.485785 dipex-4.9.2/integrations/viborg/viborg.py
+-rw-r--r--   0        0        0      922 2023-03-31 09:19:41.485785 dipex-4.9.2/integrations/viborg/viborg_uuids.py
+-rw-r--r--   0        0        0     3147 2023-03-31 09:19:41.485785 dipex-4.9.2/integrations/viborg/viborg_without_ad.py
+-rw-r--r--   0        0        0     2525 2023-03-31 09:19:43.488062 dipex-4.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 dipex-4.9.2/PKG-INFO
```

### Comparing `dipex-4.9.1/README.rst` & `dipex-4.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/exporters/sql_export/lc_for_jobs_db.py` & `dipex-4.9.2/exporters/sql_export/lc_for_jobs_db.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/exporters/sql_export/lora_cache.py` & `dipex-4.9.2/exporters/sql_export/lora_cache.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/exporters/sql_export/main.py` & `dipex-4.9.2/exporters/sql_export/main.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/exporters/sql_export/sql_export.py` & `dipex-4.9.2/exporters/sql_export/sql_export.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/exporters/sql_export/sql_table_defs.py` & `dipex-4.9.2/exporters/sql_export/sql_table_defs.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/exporters/sql_export/sql_url.py` & `dipex-4.9.2/exporters/sql_export/sql_url.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/exporters/sql_export/trigger.py` & `dipex-4.9.2/exporters/sql_export/trigger.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/exporters/utils/priority_by_class.py` & `dipex-4.9.2/exporters/utils/priority_by_class.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/config.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/config.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/date_utils.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/date_utils.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/engagement.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/engagement.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/fix_departments.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/fix_departments.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/main.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/main.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_changed_at.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_changed_at.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_changed_at_redo.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_changed_at_redo.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_cli.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_cli.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_common.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_common.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_fixup.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_fixup.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_importer.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_importer.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_log_analyzer.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_log_analyzer.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_logging.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_logging.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sd_payloads.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sd_payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sdclient/client.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sdclient/client.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sdclient/requests.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sdclient/requests.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sdclient/responses.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sdclient/responses.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/skip.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/skip.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/sync_job_id.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/sync_job_id.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/test_mo_against_sd.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/test_mo_against_sd.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/sdlon/test_sd_connectivity.py` & `dipex-4.9.2/integrations/SD_Lon/sdlon/test_sd_connectivity.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/fixtures.py` & `dipex-4.9.2/integrations/SD_Lon/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/org_manipulations.py` & `dipex-4.9.2/integrations/SD_Lon/tests/org_manipulations.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/sdclient/manual.py` & `dipex-4.9.2/integrations/SD_Lon/tests/sdclient/manual.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/sdclient/test_requests.py` & `dipex-4.9.2/integrations/SD_Lon/tests/sdclient/test_requests.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/sdclient/test_sdclient.py` & `dipex-4.9.2/integrations/SD_Lon/tests/sdclient/test_sdclient.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_config.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_date_utils.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_date_utils.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_engagement.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_engagement.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_fix_departments.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_fix_departments.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_sd_changed_at.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_sd_changed_at.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_sd_common.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_sd_common.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_sd_importer.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_sd_importer.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_sd_log_analyzer.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_sd_log_analyzer.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_skip.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_skip.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/SD_Lon/tests/test_sync_job_id.py` & `dipex-4.9.2/integrations/SD_Lon/tests/test_sync_job_id.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/config.py` & `dipex-4.9.2/integrations/aarhus/config.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/initial.py` & `dipex-4.9.2/integrations/aarhus/initial.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/initial_classes.py` & `dipex-4.9.2/integrations/aarhus/initial_classes.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/los_files.py` & `dipex-4.9.2/integrations/aarhus/los_files.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/los_import.py` & `dipex-4.9.2/integrations/aarhus/los_import.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/los_leder.py` & `dipex-4.9.2/integrations/aarhus/los_leder.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/los_org.py` & `dipex-4.9.2/integrations/aarhus/los_org.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/los_pers.py` & `dipex-4.9.2/integrations/aarhus/los_pers.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/los_stam.py` & `dipex-4.9.2/integrations/aarhus/los_stam.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/payloads.py` & `dipex-4.9.2/integrations/aarhus/payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/conftest.py` & `dipex-4.9.2/integrations/aarhus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/helpers.py` & `dipex-4.9.2/integrations/aarhus/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/strategies.py` & `dipex-4.9.2/integrations/aarhus/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_config.py` & `dipex-4.9.2/integrations/aarhus/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_initial.py` & `dipex-4.9.2/integrations/aarhus/tests/test_initial.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_los_files.py` & `dipex-4.9.2/integrations/aarhus/tests/test_los_files.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_los_import.py` & `dipex-4.9.2/integrations/aarhus/tests/test_los_import.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_los_leder.py` & `dipex-4.9.2/integrations/aarhus/tests/test_los_leder.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_los_org.py` & `dipex-4.9.2/integrations/aarhus/tests/test_los_org.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_los_pers.py` & `dipex-4.9.2/integrations/aarhus/tests/test_los_pers.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_los_stam.py` & `dipex-4.9.2/integrations/aarhus/tests/test_los_stam.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_payloads.py` & `dipex-4.9.2/integrations/aarhus/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/tests/test_util.py` & `dipex-4.9.2/integrations/aarhus/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/util.py` & `dipex-4.9.2/integrations/aarhus/util.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/aarhus/uuids.py` & `dipex-4.9.2/integrations/aarhus/uuids.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_common.py` & `dipex-4.9.2/integrations/ad_integration/ad_common.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_exceptions.py` & `dipex-4.9.2/integrations/ad_integration/ad_exceptions.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_fix_enddate.py` & `dipex-4.9.2/integrations/ad_integration/ad_fix_enddate.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_helpers.py` & `dipex-4.9.2/integrations/ad_integration/ad_helpers.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_jinja_filters.py` & `dipex-4.9.2/integrations/ad_integration/ad_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_life_cycle.py` & `dipex-4.9.2/integrations/ad_integration/ad_life_cycle.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_logger.py` & `dipex-4.9.2/integrations/ad_integration/ad_logger.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_reader.py` & `dipex-4.9.2/integrations/ad_integration/ad_reader.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_sync.py` & `dipex-4.9.2/integrations/ad_integration/ad_sync.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_template_engine.py` & `dipex-4.9.2/integrations/ad_integration/ad_template_engine.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/ad_writer.py` & `dipex-4.9.2/integrations/ad_integration/ad_writer.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/execute_ad_script.py` & `dipex-4.9.2/integrations/ad_integration/execute_ad_script.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/import_ad_group_into_mo.py` & `dipex-4.9.2/integrations/ad_integration/import_ad_group_into_mo.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/mo_to_ad_sync.py` & `dipex-4.9.2/integrations/ad_integration/mo_to_ad_sync.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/payloads.py` & `dipex-4.9.2/integrations/ad_integration/payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/read_ad_conf_settings.py` & `dipex-4.9.2/integrations/ad_integration/read_ad_conf_settings.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/sync_mo_uuid_to_ad.py` & `dipex-4.9.2/integrations/ad_integration/sync_mo_uuid_to_ad.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,21 +128,25 @@
 
         logger.info("Will now attempt to sync {} users".format(len(users)))
         users = tqdm(users)
         users = map(construct_powershell_script, users)
 
         # Actually fire the powershell scripts, and trigger side-effects
         for ps_script in users:
-            response = self._run_ps_script(ps_script)
-            logger.debug("Response: {}".format(response))
-            if response:
-                msg = "Unexpected response: {}".format(response)
-                logger.exception(msg)
-                raise Exception(msg)
-            self.stats["updated"] += 1
+            try:
+                response = self._run_ps_script(ps_script)
+            except Exception:
+                logger.exception("failed to write MO UUID (ps_script=%r)", ps_script)
+            else:
+                logger.debug("Response: {}".format(response))
+                if response:
+                    msg = "Unexpected response: {}".format(response)
+                    logger.exception(msg)
+                    raise Exception(msg)
+                self.stats["updated"] += 1
         print(self.stats)
         logger.info(self.stats)
 
     def sync_one(self, cprno):
         print("Fetch AD User")
         ad_user = self.reader.read_user(cpr=cprno)
         if not ad_user:
```

### Comparing `dipex-4.9.1/integrations/ad_integration/test_connectivity.py` & `dipex-4.9.2/integrations/ad_integration/test_connectivity.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/mocks.py` & `dipex-4.9.2/integrations/ad_integration/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/name_simulator.py` & `dipex-4.9.2/integrations/ad_integration/tests/name_simulator.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_ad_common.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_ad_common.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_ad_fix_enddate.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_ad_fix_enddate.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_ad_jinja_filters.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_ad_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_ad_life_cycle.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_ad_life_cycle.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_ad_logger.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_ad_logger.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_ad_reader.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_ad_reader.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_ad_sync.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_ad_sync.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_ad_writer.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_ad_writer.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_dot_mapping.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_dot_mapping.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_first_included.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_first_included.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_import_ad_group_into_mo.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_import_ad_group_into_mo.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_location_element.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_location_element.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_mo_data_source.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_mo_data_source.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_mo_to_ad_sync.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_mo_to_ad_sync.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_morestsource.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_morestsource.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_read_ad_conf_settings.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_read_ad_conf_settings.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_recursive_dict_update.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_recursive_dict_update.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_sync_mo_uuid_to_ad.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_sync_mo_uuid_to_ad.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from contextlib import contextmanager
+from logging import ERROR
 from unittest import mock
 from unittest import TestCase
 
 import pytest
 from parameterized import parameterized
 
 from .. import ad_common
@@ -33,14 +34,20 @@
     def _build_user_credential(self):
         return ""
 
     def _run_ps_script(self, ps_script):
         self._scripts.append(ps_script)
 
 
+class _SyncMoUuidToAdRunPSScriptFails(_SyncMoUuidToAd):
+    def _run_ps_script(self, ps_script):
+        super()._run_ps_script(ps_script)
+        raise Exception("an exception!")
+
+
 # Based on this example:
 # https://docs.pytest.org/en/stable/example/parametrize.html#parametrizing-conditional-raising
 
 
 @contextmanager
 def does_not_raise():
     yield
@@ -70,14 +77,17 @@
             }
         )
 
 
 class TestSyncMoUuidToAd(TestCase):
     """Test `sync_mo_uuid_to_ad`"""
 
+    _ad_cpr_field_name = "extensionAttribute1"
+    _mo_cpr_no = "0123456789"
+
     def test_sync_one(self):
         instance = self._get_instance()
         instance.sync_one(instance._ad_cpr_no)
         self._assert_script_contents_ok(instance)
 
     @parameterized.expand(
         [
@@ -89,31 +99,43 @@
     )
     def test_sync_one_unknown_cpr_raises_exception(self, reader, expected_message):
         instance = self._get_instance(reader=reader)
         with self.assertRaisesRegex(Exception, expected_message):
             instance.sync_one(UNKNOWN_CPR_NO)
 
     def test_sync_one_uses_morahelper(self):
-        cpr_no = "mo-cpr-no"
         instance = self._get_instance()
-        instance.sync_one(cpr_no)
+        instance.sync_one(self._mo_cpr_no)
         # Assert that our mocked `MoraHelper` recorded one call to `read_user`
         # with the expected CPR as its only argument.
-        self.assertListEqual(instance.helper._read_user_calls, [cpr_no])
+        self.assertListEqual(instance.helper._read_user_calls, [self._mo_cpr_no])
 
     def test_sync_all(self):
         instance = self._get_instance()
         instance.sync_all()
         self._assert_script_contents_ok(instance)
 
-    def _get_instance(self, settings=None, reader=None):
+    def test_perform_sync_handles_run_ps_script_exception(self):
+        ad_users = [
+            {
+                self._ad_cpr_field_name: self._mo_cpr_no,
+                "SamAccountName": "example",
+            }
+        ]
+        mo_users = {self._mo_cpr_no: MO_UUID}
+        instance = self._get_instance(cls=_SyncMoUuidToAdRunPSScriptFails)
+        with self.assertLogs("MoUuidAdSync", ERROR) as cm:
+            instance.perform_sync(ad_users, mo_users)
+            self.assertIn("failed to write MO UUID", cm.records[0].message)
+
+    def _get_instance(self, settings=None, reader=None, cls=_SyncMoUuidToAd):
         _settings = {
             "integrations.ad.write.uuid_field": AD_UUID_FIELD,
             "integrations.ad": [{"properties": [AD_UUID_FIELD]}],
-            "primary": {"cpr_field": "extensionAttribute1", "cpr_separator": "-"},
+            "primary": {"cpr_field": self._ad_cpr_field_name, "cpr_separator": "-"},
             "global": {},
         }
 
         if settings:
             _settings.update(settings)
 
         read_settings_mock = mock.patch.object(
@@ -132,20 +154,20 @@
 
         reader_mock = mock.patch.object(
             sync_mo_uuid_to_ad,
             "ADParameterReader",
             new=lambda: reader,
         )
 
-        ad_cpr_no = reader.read_user()["extensionAttribute1"]
+        ad_cpr_no = reader.read_user()[self._ad_cpr_field_name]
 
         with read_settings_mock:
             with load_settings_mock:
                 with reader_mock:
-                    instance = _SyncMoUuidToAd(ad_cpr_no)
+                    instance = cls(ad_cpr_no)
                     return instance
 
     def _assert_script_contents_ok(self, instance):
         # Assert we tried to execute exactly one script, with the proper
         # contents.
         self.assertEqual(len(instance._scripts), 1)
         self.assertIn(
```

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_usernames.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_usernames.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/tests/test_utils.py` & `dipex-4.9.2/integrations/ad_integration/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/user_names.py` & `dipex-4.9.2/integrations/ad_integration/user_names.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/username_rules/method_2.py` & `dipex-4.9.2/integrations/ad_integration/username_rules/method_2.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ad_integration/utils.py` & `dipex-4.9.2/integrations/ad_integration/utils.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/adtreesync/config.py` & `dipex-4.9.2/integrations/adtreesync/config.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/adtreesync/ldap.py` & `dipex-4.9.2/integrations/adtreesync/ldap.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/adtreesync/main.py` & `dipex-4.9.2/integrations/adtreesync/main.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/adtreesync/tests/test_main.py` & `dipex-4.9.2/integrations/adtreesync/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/apos_importer.py` & `dipex-4.9.2/integrations/apos_importer.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ballerup/ballerup-amqp.py` & `dipex-4.9.2/integrations/ballerup/ballerup-amqp.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ballerup/ballerup.py` & `dipex-4.9.2/integrations/ballerup/ballerup.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/ballerup/udvalg_import.py` & `dipex-4.9.2/integrations/ballerup/udvalg_import.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/brøndby/brøndby.py` & `dipex-4.9.2/integrations/brøndby/brøndby.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/calculate_primary/calculate_primary.py` & `dipex-4.9.2/integrations/calculate_primary/calculate_primary.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/calculate_primary/common.py` & `dipex-4.9.2/integrations/calculate_primary/common.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/calculate_primary/default.py` & `dipex-4.9.2/integrations/calculate_primary/default.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/calculate_primary/opus.py` & `dipex-4.9.2/integrations/calculate_primary/opus.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/calculate_primary/sd.py` & `dipex-4.9.2/integrations/calculate_primary/sd.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/calculate_primary/tests/test_primary.py` & `dipex-4.9.2/integrations/calculate_primary/tests/test_primary.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/cpr_mapper.py` & `dipex-4.9.2/integrations/cpr_mapper.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/dar_helper/dar_helper.py` & `dipex-4.9.2/integrations/dar_helper/dar_helper.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/dawa_helper.py` & `dipex-4.9.2/integrations/dawa_helper.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/egedal/egedal.py` & `dipex-4.9.2/integrations/egedal/egedal.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/fkorg_it_systems/import_fkorg_orgunits.py` & `dipex-4.9.2/integrations/fkorg_it_systems/import_fkorg_orgunits.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/fkorg_it_systems/test_import_fk_org.py` & `dipex-4.9.2/integrations/fkorg_it_systems/test_import_fk_org.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/gir/initial_read/emd_csv.py` & `dipex-4.9.2/integrations/gir/initial_read/emd_csv.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/gir/initial_read/main.py` & `dipex-4.9.2/integrations/gir/initial_read/main.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/gir/initial_read/mo_lora_client.py` & `dipex-4.9.2/integrations/gir/initial_read/mo_lora_client.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/gir/initial_read/org_unit_csv.py` & `dipex-4.9.2/integrations/gir/initial_read/org_unit_csv.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/hjørring/hjørring.py` & `dipex-4.9.2/integrations/hjørring/hjørring.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/holstebro/holstebro.py` & `dipex-4.9.2/integrations/holstebro/holstebro.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/kle/kle_import_export.py` & `dipex-4.9.2/integrations/kle/kle_import_export.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/kle/kle_xlsx.py` & `dipex-4.9.2/integrations/kle/kle_xlsx.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/næstved/næstved.py` & `dipex-4.9.2/integrations/næstved/næstved.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/clear_and_import_opus.py` & `dipex-4.9.2/integrations/opus/clear_and_import_opus.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/opus_diff_import.py` & `dipex-4.9.2/integrations/opus/opus_diff_import.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/opus_file_reader.py` & `dipex-4.9.2/integrations/opus/opus_file_reader.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/opus_helpers.py` & `dipex-4.9.2/integrations/opus/opus_helpers.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/opus_reimport_one.py` & `dipex-4.9.2/integrations/opus/opus_reimport_one.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/org_tree_print/main.py` & `dipex-4.9.2/integrations/opus/org_tree_print/main.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/payloads.py` & `dipex-4.9.2/integrations/opus/payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/tests/test_opus_diff_import.py` & `dipex-4.9.2/integrations/opus/tests/test_opus_diff_import.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/tests/test_opus_file_reader.py` & `dipex-4.9.2/integrations/opus/tests/test_opus_file_reader.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/opus/tests/test_opus_helpers.py` & `dipex-4.9.2/integrations/opus/tests/test_opus_helpers.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/related_units/from_adtreesync.py` & `dipex-4.9.2/integrations/related_units/from_adtreesync.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/related_units/import_related_units.py` & `dipex-4.9.2/integrations/related_units/import_related_units.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/rundb/db_overview.py` & `dipex-4.9.2/integrations/rundb/db_overview.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/rundb/tests/test_db_overview.py` & `dipex-4.9.2/integrations/rundb/tests/test_db_overview.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/viborg/udvalg_import.py` & `dipex-4.9.2/integrations/viborg/udvalg_import.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/viborg/viborg.py` & `dipex-4.9.2/integrations/viborg/viborg.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/viborg/viborg_uuids.py` & `dipex-4.9.2/integrations/viborg/viborg_uuids.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/integrations/viborg/viborg_without_ad.py` & `dipex-4.9.2/integrations/viborg/viborg_without_ad.py`

 * *Files identical despite different names*

### Comparing `dipex-4.9.1/pyproject.toml` & `dipex-4.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DIPEX"
-version = "4.9.1"
+version = "4.9.2"
 authors = ["Magenta ApS <info@magenta.dk>"]
 description = "OS2mo-data-import-and-export"
 license = "MPL-2.0"
 readme = "README.rst"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/os2mo-data-import-and-export"
 keywords = ["DIPEX", "OS2mo-data-import-and-export"]
```

### Comparing `dipex-4.9.1/PKG-INFO` & `dipex-4.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dipex
-Version: 4.9.1
+Version: 4.9.2
 Summary: OS2mo-data-import-and-export
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: DIPEX,OS2mo-data-import-and-export
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11.0,<3.12.0
```

