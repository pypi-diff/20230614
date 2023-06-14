# Comparing `tmp/validio_sdk-0.1.0.tar.gz` & `tmp/validio_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_sdk-0.1.0.tar", max compression
+gzip compressed data, was "validio_sdk-0.2.0.tar", max compression
```

## Comparing `validio_sdk-0.1.0.tar` & `validio_sdk-0.2.0.tar`

### file list

```diff
@@ -1,198 +1,202 @@
--rw-r--r--   0        0        0    11340 2023-06-12 09:21:57.913576 validio_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0     4718 2023-06-12 09:22:09.649622 validio_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      492 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/__init__.py
--rw-r--r--   0        0        0      551 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/apply.py
--rw-r--r--   0        0        0     4155 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/plan.py
--rw-r--r--   0        0        0     1565 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/scaffold.py
--rw-r--r--   0        0        0      305 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/code/settings.py
--rw-r--r--   0        0        0     5644 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/config.py
--rw-r--r--   0        0        0   244487 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/__init__.py
--rw-r--r--   0        0        0      573 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/apply_validator_recommendation.py
--rw-r--r--   0        0        0     7251 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      526 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/aws_credential_secret_changed.py
--rw-r--r--   0        0        0      613 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
--rw-r--r--   0        0        0      614 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/backfill_source.py
--rw-r--r--   0        0        0     1899 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/base_model.py
--rw-r--r--   0        0        0   578403 2023-06-12 09:21:57.917576 validio_sdk-0.1.0/validio_sdk/graphql_client/client.py
--rw-r--r--   0        0        0      445 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_credential.py
--rw-r--r--   0        0        0      528 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py
--rw-r--r--   0        0        0      468 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_kinesis_source.py
--rw-r--r--   0        0        0      526 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_redshift_credential.py
--rw-r--r--   0        0        0      480 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_redshift_source.py
--rw-r--r--   0        0        0      418 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_s3_source.py
--rw-r--r--   0        0        0      843 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      823 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      455 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_demo_credential.py
--rw-r--r--   0        0        0      407 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_demo_source.py
--rw-r--r--   0        0        0      407 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_file_window.py
--rw-r--r--   0        0        0      468 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_fixed_batch_window.py
--rw-r--r--   0        0        0      702 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      682 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      539 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py
--rw-r--r--   0        0        0      481 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_big_query_source.py
--rw-r--r--   0        0        0      445 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_credential.py
--rw-r--r--   0        0        0      500 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      459 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      468 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_storage_source.py
--rw-r--r--   0        0        0      514 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_notification_rule_v2.py
--rw-r--r--   0        0        0      753 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      803 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      783 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      823 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      682 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      662 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      702 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      516 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_postgre_sql_credential.py
--rw-r--r--   0        0        0      468 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_postgre_sql_source.py
--rw-r--r--   0        0        0      733 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      713 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      753 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      753 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      528 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_saml_identity_provider.py
--rw-r--r--   0        0        0      438 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_segmentation.py
--rw-r--r--   0        0        0      477 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_sessionized_window.py
--rw-r--r--   0        0        0      429 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_slack_channel.py
--rw-r--r--   0        0        0      505 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_snowflake_credential.py
--rw-r--r--   0        0        0      517 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_snowflake_destination.py
--rw-r--r--   0        0        0      457 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_snowflake_source.py
--rw-r--r--   0        0        0      447 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_tumbling_window.py
--rw-r--r--   0        0        0      328 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_user.py
--rw-r--r--   0        0        0      672 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      652 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      449 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/create_webhook_channel.py
--rw-r--r--   0        0        0      364 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_channel.py
--rw-r--r--   0        0        0      614 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_credential.py
--rw-r--r--   0        0        0      622 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_credentials.py
--rw-r--r--   0        0        0      630 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_destination.py
--rw-r--r--   0        0        0      638 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_destinations.py
--rw-r--r--   0        0        0      376 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_identity.py
--rw-r--r--   0        0        0      487 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_identity_provider.py
--rw-r--r--   0        0        0      514 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_notification_rule_v2.py
--rw-r--r--   0        0        0      646 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_segmentation.py
--rw-r--r--   0        0        0      536 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_source.py
--rw-r--r--   0        0        0      544 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_sources.py
--rw-r--r--   0        0        0      328 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_user.py
--rw-r--r--   0        0        0      606 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_validators.py
--rw-r--r--   0        0        0      536 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_window.py
--rw-r--r--   0        0        0      544 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/delete_windows.py
--rw-r--r--   0        0        0      589 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py
--rw-r--r--   0        0        0     3065 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/enums.py
--rw-r--r--   0        0        0     2314 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/exceptions.py
--rw-r--r--   0        0        0   172648 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/fragments.py
--rw-r--r--   0        0        0      526 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py
--rw-r--r--   0        0        0     2896 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_channel_by_resource_name.py
--rw-r--r--   0        0        0     2427 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_channels.py
--rw-r--r--   0        0        0     4965 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_credential_by_resource_name.py
--rw-r--r--   0        0        0     5997 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_destination_by_resource_name.py
--rw-r--r--   0        0        0     2218 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
--rw-r--r--   0        0        0     2033 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_identity_providers.py
--rw-r--r--   0        0        0      652 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_notification_rule_v2_by_resource_name.py
--rw-r--r--   0        0        0      505 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_notification_rules_v2.py
--rw-r--r--   0        0        0     3324 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_segment_incidents.py
--rw-r--r--   0        0        0      357 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_segmentation.py
--rw-r--r--   0        0        0      572 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
--rw-r--r--   0        0        0    20258 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_source.py
--rw-r--r--   0        0        0    24833 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_source_by_resource_name.py
--rw-r--r--   0        0        0    21532 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_source_recommended_validators.py
--rw-r--r--   0        0        0      476 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_user_by_resource_name.py
--rw-r--r--   0        0        0      300 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_users.py
--rw-r--r--   0        0        0    40168 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator.py
--rw-r--r--   0        0        0    48254 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_by_resource_name.py
--rw-r--r--   0        0        0     3404 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_incidents.py
--rw-r--r--   0        0        0     3691 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_segment_incidents.py
--rw-r--r--   0        0        0     3986 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_segment_metrics.py
--rw-r--r--   0        0        0     5711 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/get_window_by_resource_name.py
--rw-r--r--   0        0        0      290 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
--rw-r--r--   0        0        0      308 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_aws_redshift_schema.py
--rw-r--r--   0        0        0      270 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_aws_s3_schema.py
--rw-r--r--   0        0        0      265 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_demo_schema.py
--rw-r--r--   0        0        0      309 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
--rw-r--r--   0        0        0      318 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
--rw-r--r--   0        0        0      287 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
--rw-r--r--   0        0        0      290 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_gcp_storage_schema.py
--rw-r--r--   0        0        0      290 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_postgre_sql_schema.py
--rw-r--r--   0        0        0      285 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/infer_snowflake_schema.py
--rw-r--r--   0        0        0    34024 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/input_types.py
--rw-r--r--   0        0        0     4316 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_credentials.py
--rw-r--r--   0        0        0     5202 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_destinations.py
--rw-r--r--   0        0        0      457 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_segmentations.py
--rw-r--r--   0        0        0    21364 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_sources.py
--rw-r--r--   0        0        0    42237 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_validators.py
--rw-r--r--   0        0        0     4976 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/list_windows.py
--rw-r--r--   0        0        0      603 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
--rw-r--r--   0        0        0      522 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/scalars.py
--rw-r--r--   0        0        0      592 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
--rw-r--r--   0        0        0      566 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/start_source.py
--rw-r--r--   0        0        0      550 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/stop_source.py
--rw-r--r--   0        0        0      441 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_credential.py
--rw-r--r--   0        0        0      524 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py
--rw-r--r--   0        0        0      464 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_kinesis_source.py
--rw-r--r--   0        0        0      522 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_redshift_credential.py
--rw-r--r--   0        0        0      476 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_redshift_source.py
--rw-r--r--   0        0        0      414 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_s3_source.py
--rw-r--r--   0        0        0      636 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py
--rw-r--r--   0        0        0      464 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_fixed_batch_window.py
--rw-r--r--   0        0        0      491 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_freshness_validator.py
--rw-r--r--   0        0        0      535 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py
--rw-r--r--   0        0        0      477 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_big_query_source.py
--rw-r--r--   0        0        0      441 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_credential.py
--rw-r--r--   0        0        0      496 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      455 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      464 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_storage_source.py
--rw-r--r--   0        0        0      534 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_local_identity_provider.py
--rw-r--r--   0        0        0      510 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_notification_rule_v2.py
--rw-r--r--   0        0        0      540 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
--rw-r--r--   0        0        0      596 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_numeric_validator.py
--rw-r--r--   0        0        0      512 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_postgre_sql_credential.py
--rw-r--r--   0        0        0      464 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_postgre_sql_source.py
--rw-r--r--   0        0        0      520 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_relative_time_validator.py
--rw-r--r--   0        0        0      540 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_relative_volume_validator.py
--rw-r--r--   0        0        0      524 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_saml_identity_provider.py
--rw-r--r--   0        0        0      473 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_sessionized_window.py
--rw-r--r--   0        0        0      425 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_slack_channel.py
--rw-r--r--   0        0        0      501 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_snowflake_credential.py
--rw-r--r--   0        0        0      513 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_snowflake_destination.py
--rw-r--r--   0        0        0      453 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_snowflake_source.py
--rw-r--r--   0        0        0      443 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_tumbling_window.py
--rw-r--r--   0        0        0      324 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_user.py
--rw-r--r--   0        0        0    57176 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0    56052 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0    58306 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      459 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_volume_validator.py
--rw-r--r--   0        0        0      445 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/graphql_client/update_webhook_channel.py
--rw-r--r--   0        0        0      265 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/metadata.py
--rw-r--r--   0        0        0        0 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/py.typed
--rw-r--r--   0        0        0      135 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/__init__.py
--rw-r--r--   0        0        0    20662 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_diff.py
--rw-r--r--   0        0        0     1208 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_diff_util.py
--rw-r--r--   0        0        0     1229 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_diffable.py
--rw-r--r--   0        0        0     1579 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_errors.py
--rw-r--r--   0        0        0     4262 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_field_selector.py
--rw-r--r--   0        0        0    17664 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_resource.py
--rw-r--r--   0        0        0      914 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_resource_graph.py
--rw-r--r--   0        0        0     5350 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_serde.py
--rw-r--r--   0        0        0    17500 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_server_resources.py
--rw-r--r--   0        0        0      844 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/_util.py
--rw-r--r--   0        0        0     5043 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/channels.py
--rw-r--r--   0        0        0     7709 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/credentials.py
--rw-r--r--   0        0        0     5398 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/destinations.py
--rw-r--r--   0        0        0     5523 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/filters.py
--rw-r--r--   0        0        0     4628 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/notification_rules_v2.py
--rw-r--r--   0        0        0     2040 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/segmentations.py
--rw-r--r--   0        0        0    23033 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/sources.py
--rw-r--r--   0        0        0        0 2023-06-12 09:21:57.921576 validio_sdk-0.1.0/validio_sdk/resource/tests/__init__.py
--rw-r--r--   0        0        0    15565 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/tests/test__diff.py
--rw-r--r--   0        0        0     1905 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/tests/test__field_selector.py
--rw-r--r--   0        0        0    16378 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/tests/test__resource.py
--rw-r--r--   0        0        0      868 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/tests/test_sources.py
--rw-r--r--   0        0        0     5638 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/thresholds.py
--rw-r--r--   0        0        0    32119 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/validators.py
--rw-r--r--   0        0        0     5995 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/resource/windows.py
--rw-r--r--   0        0        0     1316 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/scalars.py
--rw-r--r--   0        0        0     1813 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/util.py
--rw-r--r--   0        0        0     2453 2023-06-12 09:21:57.925576 validio_sdk-0.1.0/validio_sdk/validio_client.py
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 validio_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-06-14 09:21:20.180361 validio_sdk-0.2.0/LICENSE
+-rw-r--r--   0        0        0      302 2023-06-14 09:21:20.180361 validio_sdk-0.2.0/README_PUBLIC.md
+-rw-r--r--   0        0        0     4665 2023-06-14 09:21:30.948224 validio_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/code/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/code/apply.py
+-rw-r--r--   0        0        0     4767 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/code/plan.py
+-rw-r--r--   0        0        0     1565 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/code/scaffold.py
+-rw-r--r--   0        0        0      305 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/code/settings.py
+-rw-r--r--   0        0        0     5891 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/config.py
+-rw-r--r--   0        0        0   245071 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/graphql_client/__init__.py
+-rw-r--r--   0        0        0      573 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/graphql_client/apply_validator_recommendation.py
+-rw-r--r--   0        0        0     7319 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      526 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/graphql_client/aws_credential_secret_changed.py
+-rw-r--r--   0        0        0      613 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
+-rw-r--r--   0        0        0      614 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/graphql_client/backfill_source.py
+-rw-r--r--   0        0        0     1899 2023-06-14 09:21:20.184361 validio_sdk-0.2.0/validio_sdk/graphql_client/base_model.py
+-rw-r--r--   0        0        0   584680 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/client.py
+-rw-r--r--   0        0        0      445 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_aws_credential.py
+-rw-r--r--   0        0        0      528 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      468 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_aws_kinesis_source.py
+-rw-r--r--   0        0        0      526 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_aws_redshift_credential.py
+-rw-r--r--   0        0        0      480 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_aws_redshift_source.py
+-rw-r--r--   0        0        0      418 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_aws_s3_source.py
+-rw-r--r--   0        0        0      843 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      823 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      455 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_demo_credential.py
+-rw-r--r--   0        0        0      407 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_demo_source.py
+-rw-r--r--   0        0        0      407 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_file_window.py
+-rw-r--r--   0        0        0      468 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_fixed_batch_window.py
+-rw-r--r--   0        0        0      702 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      682 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      539 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      481 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_gcp_big_query_source.py
+-rw-r--r--   0        0        0      445 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_gcp_credential.py
+-rw-r--r--   0        0        0      500 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      459 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      468 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_gcp_storage_source.py
+-rw-r--r--   0        0        0      487 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_notification_rule.py
+-rw-r--r--   0        0        0      753 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      803 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      783 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      823 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      682 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      662 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      702 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      516 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_postgre_sql_credential.py
+-rw-r--r--   0        0        0      468 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_postgre_sql_source.py
+-rw-r--r--   0        0        0      733 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      713 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      753 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      753 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      528 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_saml_identity_provider.py
+-rw-r--r--   0        0        0      438 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_segmentation.py
+-rw-r--r--   0        0        0      477 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_sessionized_window.py
+-rw-r--r--   0        0        0      429 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_slack_channel.py
+-rw-r--r--   0        0        0      505 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_snowflake_credential.py
+-rw-r--r--   0        0        0      517 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_snowflake_destination.py
+-rw-r--r--   0        0        0      457 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_snowflake_source.py
+-rw-r--r--   0        0        0      447 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_tumbling_window.py
+-rw-r--r--   0        0        0      328 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_user.py
+-rw-r--r--   0        0        0      672 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      652 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      449 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/create_webhook_channel.py
+-rw-r--r--   0        0        0      364 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_channel.py
+-rw-r--r--   0        0        0      614 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_credential.py
+-rw-r--r--   0        0        0      622 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_credentials.py
+-rw-r--r--   0        0        0      630 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_destination.py
+-rw-r--r--   0        0        0      638 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_destinations.py
+-rw-r--r--   0        0        0      376 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_identity.py
+-rw-r--r--   0        0        0      487 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_identity_provider.py
+-rw-r--r--   0        0        0      487 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_notification_rule.py
+-rw-r--r--   0        0        0      646 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_segmentation.py
+-rw-r--r--   0        0        0      536 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_source.py
+-rw-r--r--   0        0        0      544 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_sources.py
+-rw-r--r--   0        0        0      328 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_user.py
+-rw-r--r--   0        0        0      606 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_validators.py
+-rw-r--r--   0        0        0      536 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_window.py
+-rw-r--r--   0        0        0      544 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/delete_windows.py
+-rw-r--r--   0        0        0      589 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py
+-rw-r--r--   0        0        0     3065 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/enums.py
+-rw-r--r--   0        0        0     2314 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/exceptions.py
+-rw-r--r--   0        0        0   175196 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/fragments.py
+-rw-r--r--   0        0        0      526 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py
+-rw-r--r--   0        0        0     2896 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_channel_by_resource_name.py
+-rw-r--r--   0        0        0     2427 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_channels.py
+-rw-r--r--   0        0        0     4965 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_credential_by_resource_name.py
+-rw-r--r--   0        0        0     5997 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_destination_by_resource_name.py
+-rw-r--r--   0        0        0     2218 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
+-rw-r--r--   0        0        0     2033 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_identity_providers.py
+-rw-r--r--   0        0        0     5368 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_incidents.py
+-rw-r--r--   0        0        0      627 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_notification_rules.py
+-rw-r--r--   0        0        0      460 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_segment_incidents.py
+-rw-r--r--   0        0        0      357 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_segmentation.py
+-rw-r--r--   0        0        0      572 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
+-rw-r--r--   0        0        0    20258 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_source.py
+-rw-r--r--   0        0        0    24833 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_source_by_resource_name.py
+-rw-r--r--   0        0        0     1727 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_source_incidents.py
+-rw-r--r--   0        0        0    21532 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_source_recommended_validators.py
+-rw-r--r--   0        0        0      476 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_user_by_resource_name.py
+-rw-r--r--   0        0        0      300 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_users.py
+-rw-r--r--   0        0        0    40168 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_validator.py
+-rw-r--r--   0        0        0    48254 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_validator_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_validator_incidents.py
+-rw-r--r--   0        0        0      551 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_validator_segment_incidents.py
+-rw-r--r--   0        0        0     3986 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_validator_segment_metrics.py
+-rw-r--r--   0        0        0     5711 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/get_window_by_resource_name.py
+-rw-r--r--   0        0        0      290 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
+-rw-r--r--   0        0        0      308 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_aws_redshift_schema.py
+-rw-r--r--   0        0        0      270 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_aws_s3_schema.py
+-rw-r--r--   0        0        0      265 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_demo_schema.py
+-rw-r--r--   0        0        0      309 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
+-rw-r--r--   0        0        0      318 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
+-rw-r--r--   0        0        0      287 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
+-rw-r--r--   0        0        0      290 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_gcp_storage_schema.py
+-rw-r--r--   0        0        0      290 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_postgre_sql_schema.py
+-rw-r--r--   0        0        0      285 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/infer_snowflake_schema.py
+-rw-r--r--   0        0        0    34411 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/input_types.py
+-rw-r--r--   0        0        0     4316 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/list_credentials.py
+-rw-r--r--   0        0        0     5202 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/list_destinations.py
+-rw-r--r--   0        0        0      457 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/list_segmentations.py
+-rw-r--r--   0        0        0    21364 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/list_sources.py
+-rw-r--r--   0        0        0    42237 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/list_validators.py
+-rw-r--r--   0        0        0     4976 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/list_windows.py
+-rw-r--r--   0        0        0      603 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
+-rw-r--r--   0        0        0      594 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/scalars.py
+-rw-r--r--   0        0        0      288 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/segments.py
+-rw-r--r--   0        0        0      499 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/segments_by_resource_name.py
+-rw-r--r--   0        0        0      592 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
+-rw-r--r--   0        0        0      566 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/start_source.py
+-rw-r--r--   0        0        0      550 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/stop_source.py
+-rw-r--r--   0        0        0      441 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_aws_credential.py
+-rw-r--r--   0        0        0      524 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      464 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_aws_kinesis_source.py
+-rw-r--r--   0        0        0      522 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_aws_redshift_credential.py
+-rw-r--r--   0        0        0      476 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_aws_redshift_source.py
+-rw-r--r--   0        0        0      414 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_aws_s3_source.py
+-rw-r--r--   0        0        0      636 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py
+-rw-r--r--   0        0        0      464 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_fixed_batch_window.py
+-rw-r--r--   0        0        0      491 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_freshness_validator.py
+-rw-r--r--   0        0        0      535 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      477 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_gcp_big_query_source.py
+-rw-r--r--   0        0        0      441 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_gcp_credential.py
+-rw-r--r--   0        0        0      496 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      455 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      464 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_gcp_storage_source.py
+-rw-r--r--   0        0        0      534 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_local_identity_provider.py
+-rw-r--r--   0        0        0      483 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_notification_rule.py
+-rw-r--r--   0        0        0      540 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
+-rw-r--r--   0        0        0      596 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_numeric_validator.py
+-rw-r--r--   0        0        0      512 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_postgre_sql_credential.py
+-rw-r--r--   0        0        0      464 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_postgre_sql_source.py
+-rw-r--r--   0        0        0      520 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_relative_time_validator.py
+-rw-r--r--   0        0        0      540 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_relative_volume_validator.py
+-rw-r--r--   0        0        0      524 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_saml_identity_provider.py
+-rw-r--r--   0        0        0      473 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_sessionized_window.py
+-rw-r--r--   0        0        0      425 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_slack_channel.py
+-rw-r--r--   0        0        0      501 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_snowflake_credential.py
+-rw-r--r--   0        0        0      513 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_snowflake_destination.py
+-rw-r--r--   0        0        0      453 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_snowflake_source.py
+-rw-r--r--   0        0        0      443 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_tumbling_window.py
+-rw-r--r--   0        0        0      324 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_user.py
+-rw-r--r--   0        0        0    57176 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0    56052 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0    58306 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      459 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_volume_validator.py
+-rw-r--r--   0        0        0      445 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/graphql_client/update_webhook_channel.py
+-rw-r--r--   0        0        0      265 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/metadata.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/py.typed
+-rw-r--r--   0        0        0      135 2023-06-14 09:21:20.188361 validio_sdk-0.2.0/validio_sdk/resource/__init__.py
+-rw-r--r--   0        0        0    21078 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_diff.py
+-rw-r--r--   0        0        0     1208 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_diff_util.py
+-rw-r--r--   0        0        0     1657 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_diffable.py
+-rw-r--r--   0        0        0     1579 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_errors.py
+-rw-r--r--   0        0        0     4002 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_field_selector.py
+-rw-r--r--   0        0        0    17790 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_resource.py
+-rw-r--r--   0        0        0     1355 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_resource_graph.py
+-rw-r--r--   0        0        0     5366 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_serde.py
+-rw-r--r--   0        0        0    21047 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_server_resources.py
+-rw-r--r--   0        0        0      844 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/_util.py
+-rw-r--r--   0        0        0     5027 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/channels.py
+-rw-r--r--   0        0        0     7692 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/credentials.py
+-rw-r--r--   0        0        0     5398 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/destinations.py
+-rw-r--r--   0        0        0     6255 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/filters.py
+-rw-r--r--   0        0        0     4846 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/notification_rules.py
+-rw-r--r--   0        0        0     2040 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/segmentations.py
+-rw-r--r--   0        0        0    25856 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/sources.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/tests/__init__.py
+-rw-r--r--   0        0        0    15408 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/tests/test__diff.py
+-rw-r--r--   0        0        0     1905 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/tests/test__field_selector.py
+-rw-r--r--   0        0        0    16357 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/tests/test__resource.py
+-rw-r--r--   0        0        0     5638 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/thresholds.py
+-rw-r--r--   0        0        0    32563 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/validators.py
+-rw-r--r--   0        0        0     5995 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/resource/windows.py
+-rw-r--r--   0        0        0     1377 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/scalars.py
+-rw-r--r--   0        0        0     1813 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/util.py
+-rw-r--r--   0        0        0     2382 2023-06-14 09:21:20.192361 validio_sdk-0.2.0/validio_sdk/validio_client.py
+-rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 validio_sdk-0.2.0/PKG-INFO
```

### Comparing `validio_sdk-0.1.0/LICENSE` & `validio_sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/pyproject.toml` & `validio_sdk-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "validio-sdk"
-version = "0.1.0"
+version = "0.2.0"
 description = "SDK to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
-packages = [{include = "validio_sdk"}]
+packages = [{ include = "validio_sdk" }]
 exclude = ["./validio_sdk/bin/pull_graphql.py", "./schema/**", "./plugins/**", "./examples/**"]
+readme = "README_PUBLIC.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 camel-converter = "^3.0.0"
 httpx = "^0.24.0"
-python-dotenv = "^1.0.0"
-tqdm = "^4.65.0"
-types-tqdm = "^4.65.0.1"
 platformdirs = "^3.5.0"
 pydantic = "^1.10.7"
-pytest = "^7.3.1"
-pytest-asyncio = "^0.21.0"
 
 [tool.poetry.group.dev.dependencies]
-ariadne-codegen = { git = "https://github.com/mirumee/ariadne-codegen.git", branch = "main" }
 black = "^23.3.0"
 licensecheck = "^2023.1.1"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
+pytest-asyncio = "^0.21.0"
 ruff = "^0.0.263"
 sphinx = "^6.2.1" # We use <7 because most themes only work with that.
 sphinx-rtd-theme = "^1.2.1"
+ariadne-codegen = "^0.7.1"
+tqdm = "^4.65.0"
+types-tqdm = "^4.65.0.1"
+python-dotenv = "^1.0.0"
 
 [tool.ariadne-codegen]
 queries_path = "./schema/operations/"
 schema_path = "./schema/schema.graphql"
 target_package_path = "./validio_sdk/"
 include_comments = false
 plugins = [
@@ -109,29 +109,29 @@
     "validio_sdk/graphql_client/*",
     # Docs (mostly generated)
     "docs/*",
 ]
 
 select = [
     "ARG", # flake8-unused-argument
-    "C4",  # flake8-comprehension
-    "D",   # pydocstyle
-    "E",   # pycodestyle error
-    "F",   # pyflakes
-    "I",   # isort
-    "N",   # pep8-naming
+    "C4", # flake8-comprehension
+    "D", # pydocstyle
+    "E", # pycodestyle error
+    "F", # pyflakes
+    "I", # isort
+    "N", # pep8-naming
     "PIE", # flake8-pie
-    "PL",  # pylint
-    "PT",  # flake8-pytest-style
+    "PL", # pylint
+    "PT", # flake8-pytest-style
     "PTH", # flake8-use-pathlib
     "RET", # flake8-ret
     "RUF", # ruff specific rules
     "SIM", # flake8-simplify
-    "UP",  # pyupgrade
-    "W",   # pycodestyle warning
+    "UP", # pyupgrade
+    "W", # pycodestyle warning
 ]
 
 ignore = [
     "D203", # `one-blank-line-before-class` Incompatible with D211
     "D212", # `multi-line-summary-first-line` Incompatible with D213
     "D205", #  blank line required between summary line and description
     "PLR0913", # Too many arguments to function call (named arguments take care of this)
@@ -141,18 +141,18 @@
 "__init__.py" = [
     # We don't need docstrings in __init__
     "D104",
 ]
 
 # Raw error handling for testing purposes
 # No need for documentation in binaries, examples or generated code
-"*/bin/*.py" = [ "D" ]
-"examples/*.py" = [ "D", "E" ]
-"*/graphql_client/*.py" = [ "D" ]
-"*/tests/*.py" = [ "D" ]
+"*/bin/*.py" = ["D"]
+"examples/*.py" = ["D", "E"]
+"*/graphql_client/*.py" = ["D"]
+"*/tests/*.py" = ["D"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.black]
 preview = true
 
@@ -162,7 +162,8 @@
         # Generated code
         validio_sdk/graphql_client/*
     )
 """
 
 [tool.mypy]
 ignore_missing_imports = true
+plugins = "pydantic.mypy"
```

### Comparing `validio_sdk-0.1.0/validio_sdk/code/apply.py` & `validio_sdk-0.2.0/validio_sdk/code/apply.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/code/plan.py` & `validio_sdk-0.2.0/validio_sdk/code/plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,38 +60,59 @@
         ["python", directory / scaffold.main_file_name],
         cwd=directory,
         env=process_env,
         capture_output=True,
     )
 
     if child.returncode != 0:
-        print(child.stderr.decode("unicode_escape"), file=sys.stderr)
-        print(
-            f"{scaffold.main_file_name} terminated with a non-zero exit code",
-            file=sys.stderr,
-        )
+        _dump_child_stderr(child)
         sys.exit(child.returncode)
 
     raw_output: str = child.stdout.decode("utf-8")
-    (_graph, ctx, captured_output) = _extract_resource_graph(raw_output)
+    (_graph, ctx, captured_output) = _extract_resource_graph(raw_output, child)
     if no_capture and captured_output:
         print(captured_output)
 
     return ctx
 
 
+def _dump_child_stderr(child: subprocess.CompletedProcess):
+    print(child.stderr.decode("unicode_escape"), file=sys.stderr)
+    print(
+        f"{scaffold.main_file_name} terminated with a non-zero exit code",
+        file=sys.stderr,
+    )
+
+
 # Parse the graph from the child program's output. Returns also any captured stdout
 # of the child program.
-def _extract_resource_graph(raw_output: str) -> tuple[ResourceGraph, DiffContext, str]:
+def _extract_resource_graph(
+    raw_output: str,
+    child: subprocess.CompletedProcess,
+) -> tuple[ResourceGraph, DiffContext, str]:
     preamble_start_idx: int = raw_output.find(graph_preamble_var)
     if preamble_start_idx < 0:
         return ResourceGraph(), DiffContext(), ""
 
     std_output = raw_output[:preamble_start_idx]
-    graph_json = json.loads(raw_output[preamble_start_idx + len(graph_preamble_var) :])
+
+    graph_str = raw_output[preamble_start_idx + len(graph_preamble_var) :].strip()
+    if len(graph_str) == 0:
+        _dump_child_stderr(child)
+        raise RuntimeError(
+            "BUG(internal): missing resource graph from manifest program"
+        )
+
+    try:
+        graph_json = json.loads(graph_str)
+    except Exception as e:
+        # We wrap the error here, because otherwise the exception thrown by
+        # JSON parser can be cryptic if it lands in the terminal on its own.
+        raise RuntimeError(f"failed to load resource graph output JSON: {e}")
+
     graph, ctx = ResourceGraph._decode(graph_json)
     return graph, ctx, std_output
 
 
 def _create_resource_diff_object(
     r: Resource | dict, show_secrets: bool, rewrites: dict[str, Any] | None = None
 ) -> dict[str, object]:
```

### Comparing `validio_sdk-0.1.0/validio_sdk/code/scaffold.py` & `validio_sdk-0.2.0/validio_sdk/code/scaffold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/config.py` & `validio_sdk-0.2.0/validio_sdk/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,36 +28,42 @@
         super().__init__("Configuration file is invalid.")
 
 
 class ValidioConfig:
     """Representation of configuration to use in the Validio system and SDK."""
 
     def __init__(
-        self, endpoint: str = "", access_key: str = "", access_secret: str = ""
+        self,
+        endpoint: str = "",
+        access_key: str = "",
+        access_secret: str = "",
+        default_namespace: str = "default",
     ):
         """
         Constructor for `ValidioConfig`.
 
         Will ensure we can construct an object with the exposed property
         `access_secret`.
         """
+        self.default_namespace = default_namespace
         self.endpoint = endpoint
         self.access_key = access_key
         self._access_secret = access_secret
 
     def asdict(self):
         """
         Return a dictionary representation of the class.
 
         This is used from our `ClassJSONEncoder` to ensure we save JSON
         representing the class with the external property names. By doing this
         we can also ensure that we can serialize the config by passing the JSON
         to the constructor.
         """
         return {
+            "default_namespace": self.default_namespace,
             "endpoint": self.endpoint,
             "access_key": self.access_key,
             "access_secret": self._access_secret,
         }
 
     @staticmethod
     def _none_or_hidden(maybe_value):
@@ -80,14 +86,15 @@
     def __repr__(self):
         """
         Representation of a `ValidioConfig`.
 
         Will ensure we don't print sensitive information.
         """
         return (
+            f'{"Default namespace":<20} | {self.default_namespace}\n'
             f'{"Endpoint":<20} | {self.endpoint}\n'
             f'{"Access key":<20} | {self.access_key}\n'
             f'{"Access secret":<20} | {self._none_or_hidden(self.access_secret)}\n'
         )
 
 
 class Config:
```

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/__init__.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,17 +85,17 @@
     CreateGcpPubSubSource,
     CreateGcpPubSubSourceGcpPubSubSourceCreate,
 )
 from .create_gcp_storage_source import (
     CreateGcpStorageSource,
     CreateGcpStorageSourceGcpStorageSourceCreate,
 )
-from .create_notification_rule_v2 import (
-    CreateNotificationRuleV2,
-    CreateNotificationRuleV2NotificationRuleV2Create,
+from .create_notification_rule import (
+    CreateNotificationRule,
+    CreateNotificationRuleNotificationRuleCreate,
 )
 from .create_numeric_anomaly_validator_with_dynamic_threshold import (
     CreateNumericAnomalyValidatorWithDynamicThreshold,
     CreateNumericAnomalyValidatorWithDynamicThresholdNumericAnomalyValidatorWithDynamicThresholdCreate,
 )
 from .create_numeric_anomaly_validator_with_fixed_threshold import (
     CreateNumericAnomalyValidatorWithFixedThreshold,
@@ -220,17 +220,17 @@
     DeleteDestinationsDestinationsDeleteErrors,
 )
 from .delete_identity import DeleteIdentity, DeleteIdentityIdentityDelete
 from .delete_identity_provider import (
     DeleteIdentityProvider,
     DeleteIdentityProviderIdentityProviderDelete,
 )
-from .delete_notification_rule_v2 import (
-    DeleteNotificationRuleV2,
-    DeleteNotificationRuleV2NotificationRuleV2Delete,
+from .delete_notification_rule import (
+    DeleteNotificationRule,
+    DeleteNotificationRuleNotificationRuleDelete,
 )
 from .delete_segmentation import (
     DeleteSegmentation,
     DeleteSegmentationSegmentationsDelete,
     DeleteSegmentationSegmentationsDeleteErrors,
 )
 from .delete_source import (
@@ -375,29 +375,29 @@
     IdentityProviderDeletion,
     IdentityProviderDeletionErrors,
     IdentityProviderUpdate,
     IdentityProviderUpdateErrors,
     IdentityProviderUpdateIdentityProviderIdentityProvider,
     IdentityProviderUpdateIdentityProviderSamlIdentityProvider,
     IdentityProviderUpdateIdentityProviderSamlIdentityProviderConfig,
-    NotificationRuleV2Creation,
-    NotificationRuleV2CreationErrors,
-    NotificationRuleV2CreationNotificationRule,
-    NotificationRuleV2Deletion,
-    NotificationRuleV2DeletionErrors,
-    NotificationRuleV2DeletionNotificationRule,
-    NotificationRuleV2Details,
-    NotificationRuleV2DetailsChannelChannel,
-    NotificationRuleV2DetailsChannelSlackChannel,
-    NotificationRuleV2DetailsChannelSlackChannelConfig,
-    NotificationRuleV2DetailsChannelWebhookChannel,
-    NotificationRuleV2DetailsChannelWebhookChannelConfig,
-    NotificationRuleV2Update,
-    NotificationRuleV2UpdateErrors,
-    NotificationRuleV2UpdateNotificationRule,
+    NotificationRuleCreation,
+    NotificationRuleCreationErrors,
+    NotificationRuleCreationNotificationRule,
+    NotificationRuleDeletion,
+    NotificationRuleDeletionErrors,
+    NotificationRuleDeletionNotificationRule,
+    NotificationRuleDetails,
+    NotificationRuleDetailsChannelChannel,
+    NotificationRuleDetailsChannelSlackChannel,
+    NotificationRuleDetailsChannelSlackChannelConfig,
+    NotificationRuleDetailsChannelWebhookChannel,
+    NotificationRuleDetailsChannelWebhookChannelConfig,
+    NotificationRuleUpdate,
+    NotificationRuleUpdateErrors,
+    NotificationRuleUpdateNotificationRule,
     ReferenceSourceConfigDetails,
     ReferenceSourceConfigDetailsSource,
     ReferenceSourceConfigDetailsWindow,
     SegmentationCreation,
     SegmentationCreationErrors,
     SegmentationCreationSegmentation,
     SegmentationDetails,
@@ -613,14 +613,20 @@
     ValidatorCreationValidatorVolumeValidatorConfigThresholdFixedThreshold,
     ValidatorCreationValidatorVolumeValidatorConfigThresholdMonotonicThreshold,
     ValidatorCreationValidatorVolumeValidatorDestination,
     ValidatorCreationValidatorVolumeValidatorSourceConfig,
     ValidatorCreationValidatorVolumeValidatorSourceConfigSegmentation,
     ValidatorCreationValidatorVolumeValidatorSourceConfigSource,
     ValidatorCreationValidatorVolumeValidatorSourceConfigWindow,
+    ValidatorIncidents,
+    ValidatorIncidentsMetricValidatorMetric,
+    ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold,
+    ValidatorIncidentsMetricValidatorMetricWithFixedThreshold,
+    ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold,
+    ValidatorIncidentsSegment,
     ValidatorRecommendationApplication,
     ValidatorRecommendationDismissal,
     ValidatorRecommendationDismissalErrors,
     ValidatorUpdate,
     ValidatorUpdateErrors,
     ValidatorUpdateValidatorCategoricalDistributionValidator,
     ValidatorUpdateValidatorCategoricalDistributionValidatorConfig,
@@ -794,30 +800,38 @@
 )
 from .get_identity_providers import (
     GetIdentityProviders,
     GetIdentityProvidersIdentityProvidersIdentityProvider,
     GetIdentityProvidersIdentityProvidersSamlIdentityProvider,
     GetIdentityProvidersIdentityProvidersSamlIdentityProviderConfig,
 )
-from .get_notification_rule_v2_by_resource_name import (
-    GetNotificationRuleV2ByResourceName,
-    GetNotificationRuleV2ByResourceNameNotificationRuleV2ByResourceName,
-)
-from .get_notification_rules_v2 import (
-    GetNotificationRulesV2,
-    GetNotificationRulesV2NotificationRulesV2,
+from .get_incidents import (
+    GetIncidents,
+    GetIncidentsIncidentsNotification,
+    GetIncidentsIncidentsSchemaChangeNotification,
+    GetIncidentsIncidentsSegmentLimitExceededNotification,
+    GetIncidentsIncidentsSegmentLimitExceededNotificationSegmentation,
+    GetIncidentsIncidentsValidatorThresholdFailureNotification,
+    GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetric,
+    GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithDynamicThreshold,
+    GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithFixedThreshold,
+    GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithMonotonicThreshold,
+    GetIncidentsIncidentsValidatorThresholdFailureNotificationSegment,
+)
+from .get_notification_rule_by_resource_name import (
+    GetNotificationRuleByResourceName,
+    GetNotificationRuleByResourceNameNotificationRuleByResourceName,
+)
+from .get_notification_rules import (
+    GetNotificationRules,
+    GetNotificationRulesNotificationRules,
 )
 from .get_segment_incidents import (
     GetSegmentIncidents,
     GetSegmentIncidentsSegmentIncidents,
-    GetSegmentIncidentsSegmentIncidentsMetricValidatorMetric,
-    GetSegmentIncidentsSegmentIncidentsMetricValidatorMetricWithDynamicThreshold,
-    GetSegmentIncidentsSegmentIncidentsMetricValidatorMetricWithFixedThreshold,
-    GetSegmentIncidentsSegmentIncidentsMetricValidatorMetricWithMonotonicThreshold,
-    GetSegmentIncidentsSegmentIncidentsSegment,
 )
 from .get_segmentation import GetSegmentation, GetSegmentationSegmentation
 from .get_segmentation_by_resource_name import (
     GetSegmentationByResourceName,
     GetSegmentationByResourceNameSegmentationByResourceName,
 )
 from .get_source import (
@@ -924,14 +938,20 @@
     GetSourceByResourceNameSourceByResourceNameSnowflakeSourceSegmentations,
     GetSourceByResourceNameSourceByResourceNameSnowflakeSourceWindows,
     GetSourceByResourceNameSourceByResourceNameSource,
     GetSourceByResourceNameSourceByResourceNameSourceCredential,
     GetSourceByResourceNameSourceByResourceNameSourceSegmentations,
     GetSourceByResourceNameSourceByResourceNameSourceWindows,
 )
+from .get_source_incidents import (
+    GetSourceIncidents,
+    GetSourceIncidentsSourceIncidentsSchemaChangeNotification,
+    GetSourceIncidentsSourceIncidentsSegmentLimitExceededNotification,
+    GetSourceIncidentsSourceIncidentsSegmentLimitExceededNotificationSegmentation,
+)
 from .get_source_recommended_validators import (
     GetSourceRecommendedValidators,
     GetSourceRecommendedValidatorsSource,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfig,
@@ -1171,28 +1191,18 @@
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSegmentation,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSource,
     GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigWindow,
 )
 from .get_validator_incidents import (
     GetValidatorIncidents,
     GetValidatorIncidentsValidatorIncidents,
-    GetValidatorIncidentsValidatorIncidentsMetricValidatorMetric,
-    GetValidatorIncidentsValidatorIncidentsMetricValidatorMetricWithDynamicThreshold,
-    GetValidatorIncidentsValidatorIncidentsMetricValidatorMetricWithFixedThreshold,
-    GetValidatorIncidentsValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold,
-    GetValidatorIncidentsValidatorIncidentsSegment,
 )
 from .get_validator_segment_incidents import (
     GetValidatorSegmentIncidents,
     GetValidatorSegmentIncidentsValidatorSegmentIncidents,
-    GetValidatorSegmentIncidentsValidatorSegmentIncidentsMetricValidatorMetric,
-    GetValidatorSegmentIncidentsValidatorSegmentIncidentsMetricValidatorMetricWithDynamicThreshold,
-    GetValidatorSegmentIncidentsValidatorSegmentIncidentsMetricValidatorMetricWithFixedThreshold,
-    GetValidatorSegmentIncidentsValidatorSegmentIncidentsMetricValidatorMetricWithMonotonicThreshold,
-    GetValidatorSegmentIncidentsValidatorSegmentIncidentsSegment,
 )
 from .get_validator_segment_metrics import (
     GetValidatorSegmentMetrics,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistory,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistoryValues,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistory,
     GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistoryValues,
@@ -1269,19 +1279,20 @@
     GcpPubSubSourceCreateInput,
     GcpPubSubSourceUpdateInput,
     GcpStorageInferSchemaInput,
     GcpStorageSourceCreateInput,
     GcpStorageSourceUpdateInput,
     IdentityDeleteInput,
     IdentityProviderDeleteInput,
+    IncidentsInput,
     LocalIdentityProviderUpdateInput,
     MonotonicThresholdCreateInput,
-    NotificationRuleV2CreateInput,
-    NotificationRuleV2DeleteInput,
-    NotificationRuleV2UpdateInput,
+    NotificationRuleCreateInput,
+    NotificationRuleDeleteInput,
+    NotificationRuleUpdateInput,
     NumericAnomalyValidatorCreateInput,
     NumericAnomalyValidatorUpdateInput,
     NumericDistributionValidatorCreateInput,
     NumericDistributionValidatorUpdateInput,
     NumericValidatorCreateInput,
     NumericValidatorUpdateInput,
     PostgreSqlCredentialCreateInput,
@@ -1311,14 +1322,15 @@
     SnowflakeDestinationCreateInput,
     SnowflakeDestinationUpdateInput,
     SnowflakeInferSchemaInput,
     SnowflakeSourceCreateInput,
     SnowflakeSourceUpdateInput,
     SourceConfigCreateInput,
     SourceConfigUpdateInput,
+    SourceIncidentsInput,
     TimeRangeInput,
     TumblingWindowCreateInput,
     TumblingWindowUpdateInput,
     UserCreateInput,
     UserDeleteInput,
     UserUpdateInput,
     ValidatorIncidentsInput,
@@ -1523,14 +1535,19 @@
     ListWindowsWindowsListWindow,
     ListWindowsWindowsListWindowSource,
 )
 from .postgre_sql_credential_secret_changed import (
     PostgreSqlCredentialSecretChanged,
     PostgreSqlCredentialSecretChangedPostgreSqlCredentialSecretChanged,
 )
+from .segments import Segments, SegmentsSegments
+from .segments_by_resource_name import (
+    SegmentsByResourceName,
+    SegmentsByResourceNameSegmentsByResourceName,
+)
 from .snowflake_credential_secret_changed import (
     SnowflakeCredentialSecretChanged,
     SnowflakeCredentialSecretChangedSnowflakeCredentialSecretChanged,
 )
 from .start_source import (
     StartSource,
     StartSourceSourceStart,
@@ -1594,17 +1611,17 @@
     UpdateGcpStorageSource,
     UpdateGcpStorageSourceGcpStorageSourceUpdate,
 )
 from .update_local_identity_provider import (
     UpdateLocalIdentityProvider,
     UpdateLocalIdentityProviderLocalIdentityProviderUpdate,
 )
-from .update_notification_rule_v2 import (
-    UpdateNotificationRuleV2,
-    UpdateNotificationRuleV2NotificationRuleV2Update,
+from .update_notification_rule import (
+    UpdateNotificationRule,
+    UpdateNotificationRuleNotificationRuleUpdate,
 )
 from .update_numeric_anomaly_validator import (
     UpdateNumericAnomalyValidator,
     UpdateNumericAnomalyValidatorNumericAnomalyValidatorUpdate,
 )
 from .update_numeric_distribution_validator import (
     UpdateNumericDistributionValidator,
@@ -2045,16 +2062,16 @@
     "CreateGcpCredentialGcpCredentialCreate",
     "CreateGcpPubSubLiteSource",
     "CreateGcpPubSubLiteSourceGcpPubSubLiteSourceCreate",
     "CreateGcpPubSubSource",
     "CreateGcpPubSubSourceGcpPubSubSourceCreate",
     "CreateGcpStorageSource",
     "CreateGcpStorageSourceGcpStorageSourceCreate",
-    "CreateNotificationRuleV2",
-    "CreateNotificationRuleV2NotificationRuleV2Create",
+    "CreateNotificationRule",
+    "CreateNotificationRuleNotificationRuleCreate",
     "CreateNumericAnomalyValidatorWithDynamicThreshold",
     "CreateNumericAnomalyValidatorWithDynamicThresholdNumericAnomalyValidatorWithDynamicThresholdCreate",
     "CreateNumericAnomalyValidatorWithFixedThreshold",
     "CreateNumericAnomalyValidatorWithFixedThresholdNumericAnomalyValidatorWithFixedThresholdCreate",
     "CreateNumericDistributionValidatorWithDynamicThreshold",
     "CreateNumericDistributionValidatorWithDynamicThresholdNumericDistributionValidatorWithDynamicThresholdCreate",
     "CreateNumericDistributionValidatorWithFixedThreshold",
@@ -2145,16 +2162,16 @@
     "DeleteDestinations",
     "DeleteDestinationsDestinationsDelete",
     "DeleteDestinationsDestinationsDeleteErrors",
     "DeleteIdentity",
     "DeleteIdentityIdentityDelete",
     "DeleteIdentityProvider",
     "DeleteIdentityProviderIdentityProviderDelete",
-    "DeleteNotificationRuleV2",
-    "DeleteNotificationRuleV2NotificationRuleV2Delete",
+    "DeleteNotificationRule",
+    "DeleteNotificationRuleNotificationRuleDelete",
     "DeleteSegmentation",
     "DeleteSegmentationSegmentationsDelete",
     "DeleteSegmentationSegmentationsDeleteErrors",
     "DeleteSource",
     "DeleteSourceSourcesDelete",
     "DeleteSourceSourcesDeleteErrors",
     "DeleteSources",
@@ -2267,25 +2284,31 @@
     "GetIdentityProviderByResourceNameIdentityProviderByResourceNameIdentityProvider",
     "GetIdentityProviderByResourceNameIdentityProviderByResourceNameSamlIdentityProvider",
     "GetIdentityProviderByResourceNameIdentityProviderByResourceNameSamlIdentityProviderConfig",
     "GetIdentityProviders",
     "GetIdentityProvidersIdentityProvidersIdentityProvider",
     "GetIdentityProvidersIdentityProvidersSamlIdentityProvider",
     "GetIdentityProvidersIdentityProvidersSamlIdentityProviderConfig",
-    "GetNotificationRuleV2ByResourceName",
-    "GetNotificationRuleV2ByResourceNameNotificationRuleV2ByResourceName",
-    "GetNotificationRulesV2",
-    "GetNotificationRulesV2NotificationRulesV2",
+    "GetIncidents",
+    "GetIncidentsIncidentsNotification",
+    "GetIncidentsIncidentsSchemaChangeNotification",
+    "GetIncidentsIncidentsSegmentLimitExceededNotification",
+    "GetIncidentsIncidentsSegmentLimitExceededNotificationSegmentation",
+    "GetIncidentsIncidentsValidatorThresholdFailureNotification",
+    "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetric",
+    "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithDynamicThreshold",
+    "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithFixedThreshold",
+    "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithMonotonicThreshold",
+    "GetIncidentsIncidentsValidatorThresholdFailureNotificationSegment",
+    "GetNotificationRuleByResourceName",
+    "GetNotificationRuleByResourceNameNotificationRuleByResourceName",
+    "GetNotificationRules",
+    "GetNotificationRulesNotificationRules",
     "GetSegmentIncidents",
     "GetSegmentIncidentsSegmentIncidents",
-    "GetSegmentIncidentsSegmentIncidentsMetricValidatorMetric",
-    "GetSegmentIncidentsSegmentIncidentsMetricValidatorMetricWithDynamicThreshold",
-    "GetSegmentIncidentsSegmentIncidentsMetricValidatorMetricWithFixedThreshold",
-    "GetSegmentIncidentsSegmentIncidentsMetricValidatorMetricWithMonotonicThreshold",
-    "GetSegmentIncidentsSegmentIncidentsSegment",
     "GetSegmentation",
     "GetSegmentationByResourceName",
     "GetSegmentationByResourceNameSegmentationByResourceName",
     "GetSegmentationSegmentation",
     "GetSource",
     "GetSourceByResourceName",
     "GetSourceByResourceNameSourceByResourceNameAwsKinesisSource",
@@ -2335,14 +2358,18 @@
     "GetSourceByResourceNameSourceByResourceNameSnowflakeSourceCredential",
     "GetSourceByResourceNameSourceByResourceNameSnowflakeSourceSegmentations",
     "GetSourceByResourceNameSourceByResourceNameSnowflakeSourceWindows",
     "GetSourceByResourceNameSourceByResourceNameSource",
     "GetSourceByResourceNameSourceByResourceNameSourceCredential",
     "GetSourceByResourceNameSourceByResourceNameSourceSegmentations",
     "GetSourceByResourceNameSourceByResourceNameSourceWindows",
+    "GetSourceIncidents",
+    "GetSourceIncidentsSourceIncidentsSchemaChangeNotification",
+    "GetSourceIncidentsSourceIncidentsSegmentLimitExceededNotification",
+    "GetSourceIncidentsSourceIncidentsSegmentLimitExceededNotificationSegmentation",
     "GetSourceRecommendedValidators",
     "GetSourceRecommendedValidatorsSource",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSegmentation",
@@ -2534,26 +2561,16 @@
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorDestination",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfig",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSegmentation",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigSource",
     "GetValidatorByResourceNameValidatorByResourceNameVolumeValidatorSourceConfigWindow",
     "GetValidatorIncidents",
     "GetValidatorIncidentsValidatorIncidents",
-    "GetValidatorIncidentsValidatorIncidentsMetricValidatorMetric",
-    "GetValidatorIncidentsValidatorIncidentsMetricValidatorMetricWithDynamicThreshold",
-    "GetValidatorIncidentsValidatorIncidentsMetricValidatorMetricWithFixedThreshold",
-    "GetValidatorIncidentsValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold",
-    "GetValidatorIncidentsValidatorIncidentsSegment",
     "GetValidatorSegmentIncidents",
     "GetValidatorSegmentIncidentsValidatorSegmentIncidents",
-    "GetValidatorSegmentIncidentsValidatorSegmentIncidentsMetricValidatorMetric",
-    "GetValidatorSegmentIncidentsValidatorSegmentIncidentsMetricValidatorMetricWithDynamicThreshold",
-    "GetValidatorSegmentIncidentsValidatorSegmentIncidentsMetricValidatorMetricWithFixedThreshold",
-    "GetValidatorSegmentIncidentsValidatorSegmentIncidentsMetricValidatorMetricWithMonotonicThreshold",
-    "GetValidatorSegmentIncidentsValidatorSegmentIncidentsSegment",
     "GetValidatorSegmentMetrics",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistory",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithDynamicThresholdHistoryValues",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistory",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithFixedThresholdHistoryValues",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithMonotonicThresholdHistory",
     "GetValidatorSegmentMetricsValidatorSegmentMetricsValidatorMetricWithMonotonicThresholdHistoryValues",
@@ -2681,14 +2698,15 @@
     "IdentityProviderDeletionErrors",
     "IdentityProviderUpdate",
     "IdentityProviderUpdateErrorCode",
     "IdentityProviderUpdateErrors",
     "IdentityProviderUpdateIdentityProviderIdentityProvider",
     "IdentityProviderUpdateIdentityProviderSamlIdentityProvider",
     "IdentityProviderUpdateIdentityProviderSamlIdentityProviderConfig",
+    "IncidentsInput",
     "InferAwsKinesisSchema",
     "InferAwsRedshiftSchema",
     "InferAwsS3Schema",
     "InferDemoSchema",
     "InferGcpBigQuerySchema",
     "InferGcpPubSubLiteSchema",
     "InferGcpPubSubSchema",
@@ -2873,32 +2891,32 @@
     "ListWindowsWindowsListTumblingWindow",
     "ListWindowsWindowsListTumblingWindowConfig",
     "ListWindowsWindowsListTumblingWindowSource",
     "ListWindowsWindowsListWindow",
     "ListWindowsWindowsListWindowSource",
     "LocalIdentityProviderUpdateInput",
     "MonotonicThresholdCreateInput",
-    "NotificationRuleV2CreateInput",
-    "NotificationRuleV2Creation",
-    "NotificationRuleV2CreationErrors",
-    "NotificationRuleV2CreationNotificationRule",
-    "NotificationRuleV2DeleteInput",
-    "NotificationRuleV2Deletion",
-    "NotificationRuleV2DeletionErrors",
-    "NotificationRuleV2DeletionNotificationRule",
-    "NotificationRuleV2Details",
-    "NotificationRuleV2DetailsChannelChannel",
-    "NotificationRuleV2DetailsChannelSlackChannel",
-    "NotificationRuleV2DetailsChannelSlackChannelConfig",
-    "NotificationRuleV2DetailsChannelWebhookChannel",
-    "NotificationRuleV2DetailsChannelWebhookChannelConfig",
-    "NotificationRuleV2Update",
-    "NotificationRuleV2UpdateErrors",
-    "NotificationRuleV2UpdateInput",
-    "NotificationRuleV2UpdateNotificationRule",
+    "NotificationRuleCreateInput",
+    "NotificationRuleCreation",
+    "NotificationRuleCreationErrors",
+    "NotificationRuleCreationNotificationRule",
+    "NotificationRuleDeleteInput",
+    "NotificationRuleDeletion",
+    "NotificationRuleDeletionErrors",
+    "NotificationRuleDeletionNotificationRule",
+    "NotificationRuleDetails",
+    "NotificationRuleDetailsChannelChannel",
+    "NotificationRuleDetailsChannelSlackChannel",
+    "NotificationRuleDetailsChannelSlackChannelConfig",
+    "NotificationRuleDetailsChannelWebhookChannel",
+    "NotificationRuleDetailsChannelWebhookChannelConfig",
+    "NotificationRuleUpdate",
+    "NotificationRuleUpdateErrors",
+    "NotificationRuleUpdateInput",
+    "NotificationRuleUpdateNotificationRule",
     "NotificationSeverity",
     "NotificationTypename",
     "NumericAnomalyMetric",
     "NumericAnomalyValidatorCreateInput",
     "NumericAnomalyValidatorUpdateInput",
     "NumericDistributionMetric",
     "NumericDistributionValidatorCreateInput",
@@ -2935,14 +2953,18 @@
     "SegmentationCreateInput",
     "SegmentationCreation",
     "SegmentationCreationErrors",
     "SegmentationCreationSegmentation",
     "SegmentationDetails",
     "SegmentationDetailsSource",
     "SegmentationSummary",
+    "Segments",
+    "SegmentsByResourceName",
+    "SegmentsByResourceNameSegmentsByResourceName",
+    "SegmentsSegments",
     "SessionizedWindowCreateInput",
     "SessionizedWindowUpdateInput",
     "SlackChannelCreateInput",
     "SlackChannelUpdateInput",
     "SnowflakeCredentialCreateInput",
     "SnowflakeCredentialSecretChanged",
     "SnowflakeCredentialSecretChangedInput",
@@ -3004,14 +3026,15 @@
     "SourceCreationSourceSnowflakeSourceCredential",
     "SourceCreationSourceSnowflakeSourceSegmentations",
     "SourceCreationSourceSnowflakeSourceWindows",
     "SourceCreationSourceSource",
     "SourceCreationSourceSourceCredential",
     "SourceCreationSourceSourceSegmentations",
     "SourceCreationSourceSourceWindows",
+    "SourceIncidentsInput",
     "SourceState",
     "SourceUpdate",
     "SourceUpdateErrors",
     "SourceUpdateSourceAwsKinesisSource",
     "SourceUpdateSourceAwsKinesisSourceConfig",
     "SourceUpdateSourceAwsKinesisSourceCredential",
     "SourceUpdateSourceAwsKinesisSourceSegmentations",
@@ -3099,16 +3122,16 @@
     "UpdateGcpPubSubLiteSourceGcpPubSubLiteSourceUpdate",
     "UpdateGcpPubSubSource",
     "UpdateGcpPubSubSourceGcpPubSubSourceUpdate",
     "UpdateGcpStorageSource",
     "UpdateGcpStorageSourceGcpStorageSourceUpdate",
     "UpdateLocalIdentityProvider",
     "UpdateLocalIdentityProviderLocalIdentityProviderUpdate",
-    "UpdateNotificationRuleV2",
-    "UpdateNotificationRuleV2NotificationRuleV2Update",
+    "UpdateNotificationRule",
+    "UpdateNotificationRuleNotificationRuleUpdate",
     "UpdateNumericAnomalyValidator",
     "UpdateNumericAnomalyValidatorNumericAnomalyValidatorUpdate",
     "UpdateNumericDistributionValidator",
     "UpdateNumericDistributionValidatorNumericDistributionValidatorUpdate",
     "UpdateNumericValidator",
     "UpdateNumericValidatorNumericValidatorUpdate",
     "UpdatePostgreSqlCredential",
@@ -3529,15 +3552,21 @@
     "ValidatorCreationValidatorVolumeValidatorConfigThresholdFixedThreshold",
     "ValidatorCreationValidatorVolumeValidatorConfigThresholdMonotonicThreshold",
     "ValidatorCreationValidatorVolumeValidatorDestination",
     "ValidatorCreationValidatorVolumeValidatorSourceConfig",
     "ValidatorCreationValidatorVolumeValidatorSourceConfigSegmentation",
     "ValidatorCreationValidatorVolumeValidatorSourceConfigSource",
     "ValidatorCreationValidatorVolumeValidatorSourceConfigWindow",
+    "ValidatorIncidents",
     "ValidatorIncidentsInput",
+    "ValidatorIncidentsMetricValidatorMetric",
+    "ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold",
+    "ValidatorIncidentsMetricValidatorMetricWithFixedThreshold",
+    "ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold",
+    "ValidatorIncidentsSegment",
     "ValidatorRecommendationApplication",
     "ValidatorRecommendationApplyInput",
     "ValidatorRecommendationDismissInput",
     "ValidatorRecommendationDismissal",
     "ValidatorRecommendationDismissalErrors",
     "ValidatorSegmentIncidentsInput",
     "ValidatorSegmentMetricsInput",
```

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/apply_validator_recommendation.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/apply_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/async_base_client.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,17 @@
     async def execute(
         self, query: str, variables: Optional[Dict[str, Any]] = None
     ) -> httpx.Response:
         payload: Dict[str, Any] = {"query": query}
         if variables:
             payload["variables"] = self._convert_dict_to_json_serializable(variables)
         content = json.dumps(payload, default=pydantic_encoder)
-        return await self.http_client.post(url=self.url, content=content)
+        return await self.http_client.post(
+            url=self.url, content=content, headers={"Content-Type": "application/json"}
+        )
 
     def get_data(self, response: httpx.Response) -> Dict[str, Any]:
         if not response.is_success:
             raise GraphQLClientHttpError(
                 status_code=response.status_code, response=response
             )
```

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/aws_credential_secret_changed.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/aws_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/backfill_source.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/backfill_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/base_model.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/client.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,17 +92,17 @@
     CreateGcpPubSubSource,
     CreateGcpPubSubSourceGcpPubSubSourceCreate,
 )
 from .create_gcp_storage_source import (
     CreateGcpStorageSource,
     CreateGcpStorageSourceGcpStorageSourceCreate,
 )
-from .create_notification_rule_v2 import (
-    CreateNotificationRuleV2,
-    CreateNotificationRuleV2NotificationRuleV2Create,
+from .create_notification_rule import (
+    CreateNotificationRule,
+    CreateNotificationRuleNotificationRuleCreate,
 )
 from .create_numeric_anomaly_validator_with_dynamic_threshold import (
     CreateNumericAnomalyValidatorWithDynamicThreshold,
     CreateNumericAnomalyValidatorWithDynamicThresholdNumericAnomalyValidatorWithDynamicThresholdCreate,
 )
 from .create_numeric_anomaly_validator_with_fixed_threshold import (
     CreateNumericAnomalyValidatorWithFixedThreshold,
@@ -214,17 +214,17 @@
     DeleteDestinationsDestinationsDelete,
 )
 from .delete_identity import DeleteIdentity, DeleteIdentityIdentityDelete
 from .delete_identity_provider import (
     DeleteIdentityProvider,
     DeleteIdentityProviderIdentityProviderDelete,
 )
-from .delete_notification_rule_v2 import (
-    DeleteNotificationRuleV2,
-    DeleteNotificationRuleV2NotificationRuleV2Delete,
+from .delete_notification_rule import (
+    DeleteNotificationRule,
+    DeleteNotificationRuleNotificationRuleDelete,
 )
 from .delete_segmentation import (
     DeleteSegmentation,
     DeleteSegmentationSegmentationsDelete,
 )
 from .delete_source import DeleteSource, DeleteSourceSourcesDelete
 from .delete_sources import DeleteSources, DeleteSourcesSourcesDelete
@@ -273,21 +273,28 @@
     GetIdentityProviderByResourceNameIdentityProviderByResourceNameSamlIdentityProvider,
 )
 from .get_identity_providers import (
     GetIdentityProviders,
     GetIdentityProvidersIdentityProvidersIdentityProvider,
     GetIdentityProvidersIdentityProvidersSamlIdentityProvider,
 )
-from .get_notification_rule_v2_by_resource_name import (
-    GetNotificationRuleV2ByResourceName,
-    GetNotificationRuleV2ByResourceNameNotificationRuleV2ByResourceName,
-)
-from .get_notification_rules_v2 import (
-    GetNotificationRulesV2,
-    GetNotificationRulesV2NotificationRulesV2,
+from .get_incidents import (
+    GetIncidents,
+    GetIncidentsIncidentsNotification,
+    GetIncidentsIncidentsSchemaChangeNotification,
+    GetIncidentsIncidentsSegmentLimitExceededNotification,
+    GetIncidentsIncidentsValidatorThresholdFailureNotification,
+)
+from .get_notification_rule_by_resource_name import (
+    GetNotificationRuleByResourceName,
+    GetNotificationRuleByResourceNameNotificationRuleByResourceName,
+)
+from .get_notification_rules import (
+    GetNotificationRules,
+    GetNotificationRulesNotificationRules,
 )
 from .get_segment_incidents import (
     GetSegmentIncidents,
     GetSegmentIncidentsSegmentIncidents,
 )
 from .get_segmentation import GetSegmentation, GetSegmentationSegmentation
 from .get_segmentation_by_resource_name import (
@@ -316,14 +323,19 @@
     GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSource,
     GetSourceByResourceNameSourceByResourceNameGcpPubSubSource,
     GetSourceByResourceNameSourceByResourceNameGcpStorageSource,
     GetSourceByResourceNameSourceByResourceNamePostgreSqlSource,
     GetSourceByResourceNameSourceByResourceNameSnowflakeSource,
     GetSourceByResourceNameSourceByResourceNameSource,
 )
+from .get_source_incidents import (
+    GetSourceIncidents,
+    GetSourceIncidentsSourceIncidentsSchemaChangeNotification,
+    GetSourceIncidentsSourceIncidentsSegmentLimitExceededNotification,
+)
 from .get_source_recommended_validators import (
     GetSourceRecommendedValidators,
     GetSourceRecommendedValidatorsSource,
 )
 from .get_user_by_resource_name import (
     GetUserByResourceName,
     GetUserByResourceNameUserByResourceName,
@@ -429,19 +441,20 @@
     GcpPubSubSourceCreateInput,
     GcpPubSubSourceUpdateInput,
     GcpStorageInferSchemaInput,
     GcpStorageSourceCreateInput,
     GcpStorageSourceUpdateInput,
     IdentityDeleteInput,
     IdentityProviderDeleteInput,
+    IncidentsInput,
     LocalIdentityProviderUpdateInput,
     MonotonicThresholdCreateInput,
-    NotificationRuleV2CreateInput,
-    NotificationRuleV2DeleteInput,
-    NotificationRuleV2UpdateInput,
+    NotificationRuleCreateInput,
+    NotificationRuleDeleteInput,
+    NotificationRuleUpdateInput,
     NumericAnomalyValidatorCreateInput,
     NumericAnomalyValidatorUpdateInput,
     NumericDistributionValidatorCreateInput,
     NumericDistributionValidatorUpdateInput,
     NumericValidatorCreateInput,
     NumericValidatorUpdateInput,
     PostgreSqlCredentialCreateInput,
@@ -467,14 +480,15 @@
     SnowflakeCredentialSecretChangedInput,
     SnowflakeCredentialUpdateInput,
     SnowflakeDestinationCreateInput,
     SnowflakeDestinationUpdateInput,
     SnowflakeInferSchemaInput,
     SnowflakeSourceCreateInput,
     SnowflakeSourceUpdateInput,
+    SourceIncidentsInput,
     TumblingWindowCreateInput,
     TumblingWindowUpdateInput,
     UserCreateInput,
     UserDeleteInput,
     UserUpdateInput,
     ValidatorIncidentsInput,
     ValidatorRecommendationApplyInput,
@@ -537,14 +551,19 @@
     ListWindowsWindowsListTumblingWindow,
     ListWindowsWindowsListWindow,
 )
 from .postgre_sql_credential_secret_changed import (
     PostgreSqlCredentialSecretChanged,
     PostgreSqlCredentialSecretChangedPostgreSqlCredentialSecretChanged,
 )
+from .segments import Segments, SegmentsSegments
+from .segments_by_resource_name import (
+    SegmentsByResourceName,
+    SegmentsByResourceNameSegmentsByResourceName,
+)
 from .snowflake_credential_secret_changed import (
     SnowflakeCredentialSecretChanged,
     SnowflakeCredentialSecretChangedSnowflakeCredentialSecretChanged,
 )
 from .start_source import StartSource, StartSourceSourceStart
 from .stop_source import StopSource, StopSourceSourceStop
 from .update_aws_credential import (
@@ -604,17 +623,17 @@
     UpdateGcpStorageSource,
     UpdateGcpStorageSourceGcpStorageSourceUpdate,
 )
 from .update_local_identity_provider import (
     UpdateLocalIdentityProvider,
     UpdateLocalIdentityProviderLocalIdentityProviderUpdate,
 )
-from .update_notification_rule_v2 import (
-    UpdateNotificationRuleV2,
-    UpdateNotificationRuleV2NotificationRuleV2Update,
+from .update_notification_rule import (
+    UpdateNotificationRule,
+    UpdateNotificationRuleNotificationRuleUpdate,
 )
 from .update_numeric_anomaly_validator import (
     UpdateNumericAnomalyValidator,
     UpdateNumericAnomalyValidatorNumericAnomalyValidatorUpdate,
 )
 from .update_numeric_distribution_validator import (
     UpdateNumericDistributionValidator,
@@ -3862,22 +3881,22 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateGcpStorageSource.parse_obj(data).gcp_storage_source_create
 
-    async def create_notification_rule_v2(
-        self, input: NotificationRuleV2CreateInput
-    ) -> CreateNotificationRuleV2NotificationRuleV2Create:
+    async def create_notification_rule(
+        self, input: NotificationRuleCreateInput
+    ) -> CreateNotificationRuleNotificationRuleCreate:
         query = gql(
             """
-            mutation CreateNotificationRuleV2($input: NotificationRuleV2CreateInput!) {
-              notificationRuleV2Create(input: $input) {
-                ...NotificationRuleV2Creation
+            mutation CreateNotificationRule($input: NotificationRuleCreateInput!) {
+              notificationRuleCreate(input: $input) {
+                ...NotificationRuleCreation
               }
             }
 
             fragment ChannelDetails on Channel {
               __typename
               id
               name
@@ -3897,25 +3916,25 @@
                   webhookUrl
                   applicationLinkUrl
                   authHeader
                 }
               }
             }
 
-            fragment NotificationRuleV2Creation on NotificationRuleV2CreateResult {
+            fragment NotificationRuleCreation on NotificationRuleCreateResult {
               errors {
                 code
                 message
               }
               notificationRule {
-                ...NotificationRuleV2Details
+                ...NotificationRuleDetails
               }
             }
 
-            fragment NotificationRuleV2Details on NotificationRuleV2 {
+            fragment NotificationRuleDetails on NotificationRule {
               __typename
               id
               name
               notificationTypenames
               createdAt
               updatedAt
               sources
@@ -3926,15 +3945,15 @@
               resourceNamespace
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return CreateNotificationRuleV2.parse_obj(data).notification_rule_v2_create
+        return CreateNotificationRule.parse_obj(data).notification_rule_create
 
     async def create_numeric_anomaly_validator_with_dynamic_threshold(
         self,
         input: NumericAnomalyValidatorCreateInput,
         threshold: DynamicThresholdCreateInput,
     ) -> CreateNumericAnomalyValidatorWithDynamicThresholdNumericAnomalyValidatorWithDynamicThresholdCreate:
         query = gql(
@@ -9906,26 +9925,26 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return DeleteIdentityProvider.parse_obj(data).identity_provider_delete
 
-    async def delete_notification_rule_v2(
-        self, input: NotificationRuleV2DeleteInput
-    ) -> DeleteNotificationRuleV2NotificationRuleV2Delete:
+    async def delete_notification_rule(
+        self, input: NotificationRuleDeleteInput
+    ) -> DeleteNotificationRuleNotificationRuleDelete:
         query = gql(
             """
-            mutation DeleteNotificationRuleV2($input: NotificationRuleV2DeleteInput!) {
-              notificationRuleV2Delete(input: $input) {
-                ...NotificationRuleV2Deletion
+            mutation DeleteNotificationRule($input: NotificationRuleDeleteInput!) {
+              notificationRuleDelete(input: $input) {
+                ...NotificationRuleDeletion
               }
             }
 
-            fragment NotificationRuleV2Deletion on NotificationRuleV2DeleteResult {
+            fragment NotificationRuleDeletion on NotificationRuleDeleteResult {
               errors {
                 code
                 message
               }
               notificationRule {
                 __typename
                 id
@@ -9933,15 +9952,15 @@
               }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return DeleteNotificationRuleV2.parse_obj(data).notification_rule_v2_delete
+        return DeleteNotificationRule.parse_obj(data).notification_rule_delete
 
     async def delete_segmentation(
         self, id: SegmentationId
     ) -> DeleteSegmentationSegmentationsDelete:
         query = gql(
             """
             mutation DeleteSegmentation($id: SegmentationId!) {
@@ -10531,25 +10550,102 @@
             """
         )
         variables: dict[str, object] = {"filter": filter}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetIdentityProviders.parse_obj(data).identity_providers
 
-    async def get_notification_rule_v2_by_resource_name(
+    async def get_incidents(
+        self, input: IncidentsInput
+    ) -> List[
+        Union[
+            GetIncidentsIncidentsNotification,
+            GetIncidentsIncidentsSchemaChangeNotification,
+            GetIncidentsIncidentsSegmentLimitExceededNotification,
+            GetIncidentsIncidentsValidatorThresholdFailureNotification,
+        ]
+    ]:
+        query = gql(
+            """
+            query GetIncidents($input: IncidentsInput!) {
+              incidents(input: $input) {
+                __typename
+                id
+                severity
+                ... on SchemaChangeNotification {
+                  createdAt
+                  payload
+                }
+                ... on SegmentLimitExceededNotification {
+                  createdAt
+                  limit
+                  segmentation {
+                    id
+                    name
+                  }
+                }
+                ... on ValidatorThresholdFailureNotification {
+                  segment {
+                    ...SegmentDetails
+                  }
+                  metric {
+                    ...ValidatorMetricDetails
+                  }
+                }
+              }
+            }
+
+            fragment SegmentDetails on Segment {
+              __typename
+              id
+              fields {
+                field
+                value
+              }
+              muted
+            }
+
+            fragment ValidatorMetricDetails on ValidatorMetric {
+              __typename
+              startTime
+              endTime
+              isIncident
+              value
+              ... on ValidatorMetricWithFixedThreshold {
+                operator
+                bound
+              }
+              ... on ValidatorMetricWithDynamicThreshold {
+                lowerBound
+                upperBound
+                decisionBoundsType
+                isBurnIn
+              }
+              ... on ValidatorMetricWithMonotonicThreshold {
+                operator
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return GetIncidents.parse_obj(data).incidents
+
+    async def get_notification_rule_by_resource_name(
         self, resource_name: str, resource_namespace: str
-    ) -> Optional[GetNotificationRuleV2ByResourceNameNotificationRuleV2ByResourceName]:
+    ) -> Optional[GetNotificationRuleByResourceNameNotificationRuleByResourceName]:
         query = gql(
             """
-            query GetNotificationRuleV2ByResourceName($resourceName: String!, $resourceNamespace: String! = "default") {
-              notificationRuleV2ByResourceName(
+            query GetNotificationRuleByResourceName($resourceName: String!, $resourceNamespace: String! = "default") {
+              notificationRuleByResourceName(
                 resourceName: $resourceName
                 resourceNamespace: $resourceNamespace
               ) {
-                ...NotificationRuleV2Details
+                ...NotificationRuleDetails
               }
             }
 
             fragment ChannelDetails on Channel {
               __typename
               id
               name
@@ -10569,15 +10665,15 @@
                   webhookUrl
                   applicationLinkUrl
                   authHeader
                 }
               }
             }
 
-            fragment NotificationRuleV2Details on NotificationRuleV2 {
+            fragment NotificationRuleDetails on NotificationRule {
               __typename
               id
               name
               notificationTypenames
               createdAt
               updatedAt
               sources
@@ -10591,26 +10687,26 @@
         )
         variables: dict[str, object] = {
             "resourceName": resource_name,
             "resourceNamespace": resource_namespace,
         }
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return GetNotificationRuleV2ByResourceName.parse_obj(
+        return GetNotificationRuleByResourceName.parse_obj(
             data
-        ).notification_rule_v2_by_resource_name
+        ).notification_rule_by_resource_name
 
-    async def get_notification_rules_v2(
+    async def get_notification_rules(
         self, filter: Union[Optional[ResourceFilter], UnsetType] = UNSET
-    ) -> List[GetNotificationRulesV2NotificationRulesV2]:
+    ) -> List[GetNotificationRulesNotificationRules]:
         query = gql(
             """
-            query GetNotificationRulesV2($filter: ResourceFilter) {
-              notificationRulesV2(filter: $filter) {
-                ...NotificationRuleV2Details
+            query GetNotificationRules($filter: ResourceFilter) {
+              notificationRules(filter: $filter) {
+                ...NotificationRuleDetails
               }
             }
 
             fragment ChannelDetails on Channel {
               __typename
               id
               name
@@ -10630,15 +10726,15 @@
                   webhookUrl
                   applicationLinkUrl
                   authHeader
                 }
               }
             }
 
-            fragment NotificationRuleV2Details on NotificationRuleV2 {
+            fragment NotificationRuleDetails on NotificationRule {
               __typename
               id
               name
               notificationTypenames
               createdAt
               updatedAt
               sources
@@ -10649,44 +10745,49 @@
               resourceNamespace
             }
             """
         )
         variables: dict[str, object] = {"filter": filter}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return GetNotificationRulesV2.parse_obj(data).notification_rules_v2
+        return GetNotificationRules.parse_obj(data).notification_rules
 
     async def get_segment_incidents(
         self, input: SegmentIncidentsInput
     ) -> List[GetSegmentIncidentsSegmentIncidents]:
         query = gql(
             """
             query GetSegmentIncidents($input: SegmentIncidentsInput!) {
               segmentIncidents(input: $input) {
-                id
-                severity
-                segment {
-                  ...SegmentDetails
-                }
-                metric {
-                  ...ValidatorMetricDetails
-                }
+                ...ValidatorIncidents
               }
             }
 
             fragment SegmentDetails on Segment {
               __typename
               id
               fields {
                 field
                 value
               }
               muted
             }
 
+            fragment ValidatorIncidents on ValidatorThresholdFailureNotification {
+              __typename
+              id
+              severity
+              segment {
+                ...SegmentDetails
+              }
+              metric {
+                ...ValidatorMetricDetails
+              }
+            }
+
             fragment ValidatorMetricDetails on ValidatorMetric {
               __typename
               startTime
               endTime
               isIncident
               value
               ... on ValidatorMetricWithFixedThreshold {
@@ -11082,14 +11183,56 @@
             "resourceName": resource_name,
             "resourceNamespace": resource_namespace,
         }
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetSourceByResourceName.parse_obj(data).source_by_resource_name
 
+    async def get_source_incidents(
+        self, input: SourceIncidentsInput
+    ) -> List[
+        Union[
+            GetSourceIncidentsSourceIncidentsSchemaChangeNotification,
+            GetSourceIncidentsSourceIncidentsSegmentLimitExceededNotification,
+        ]
+    ]:
+        query = gql(
+            """
+            query GetSourceIncidents($input: SourceIncidentsInput!) {
+              sourceIncidents(input: $input) {
+                ...SourceIncidents
+              }
+            }
+
+            fragment SourceIncidents on SourceIncidentNotification {
+              __typename
+              ... on SchemaChangeNotification {
+                id
+                severity
+                createdAt
+                payload
+              }
+              ... on SegmentLimitExceededNotification {
+                id
+                severity
+                createdAt
+                limit
+                segmentation {
+                  id
+                  name
+                }
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return GetSourceIncidents.parse_obj(data).source_incidents
+
     async def get_source_recommended_validators(
         self, id: SourceId
     ) -> Optional[GetSourceRecommendedValidatorsSource]:
         query = gql(
             """
             query GetSourceRecommendedValidators($id: SourceId!) {
               source(id: $id) {
@@ -11930,35 +12073,40 @@
     async def get_validator_incidents(
         self, input: ValidatorIncidentsInput
     ) -> List[GetValidatorIncidentsValidatorIncidents]:
         query = gql(
             """
             query GetValidatorIncidents($input: ValidatorIncidentsInput!) {
               validatorIncidents(input: $input) {
-                id
-                severity
-                segment {
-                  ...SegmentDetails
-                }
-                metric {
-                  ...ValidatorMetricDetails
-                }
+                ...ValidatorIncidents
               }
             }
 
             fragment SegmentDetails on Segment {
               __typename
               id
               fields {
                 field
                 value
               }
               muted
             }
 
+            fragment ValidatorIncidents on ValidatorThresholdFailureNotification {
+              __typename
+              id
+              severity
+              segment {
+                ...SegmentDetails
+              }
+              metric {
+                ...ValidatorMetricDetails
+              }
+            }
+
             fragment ValidatorMetricDetails on ValidatorMetric {
               __typename
               startTime
               endTime
               isIncident
               value
               ... on ValidatorMetricWithFixedThreshold {
@@ -11985,35 +12133,40 @@
     async def get_validator_segment_incidents(
         self, input: ValidatorSegmentIncidentsInput
     ) -> List[GetValidatorSegmentIncidentsValidatorSegmentIncidents]:
         query = gql(
             """
             query GetValidatorSegmentIncidents($input: ValidatorSegmentIncidentsInput!) {
               validatorSegmentIncidents(input: $input) {
-                id
-                severity
-                segment {
-                  ...SegmentDetails
-                }
-                metric {
-                  ...ValidatorMetricDetails
-                }
+                ...ValidatorIncidents
               }
             }
 
             fragment SegmentDetails on Segment {
               __typename
               id
               fields {
                 field
                 value
               }
               muted
             }
 
+            fragment ValidatorIncidents on ValidatorThresholdFailureNotification {
+              __typename
+              id
+              severity
+              segment {
+                ...SegmentDetails
+              }
+              metric {
+                ...ValidatorMetricDetails
+              }
+            }
+
             fragment ValidatorMetricDetails on ValidatorMetric {
               __typename
               startTime
               endTime
               isIncident
               value
               ... on ValidatorMetricWithFixedThreshold {
@@ -13019,14 +13172,72 @@
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return PostgreSqlCredentialSecretChanged.parse_obj(
             data
         ).postgre_sql_credential_secret_changed
 
+    async def segments(self, id: SegmentationId) -> List[SegmentsSegments]:
+        query = gql(
+            """
+            query Segments($id: SegmentationId!) {
+              segments(id: $id) {
+                ...SegmentDetails
+              }
+            }
+
+            fragment SegmentDetails on Segment {
+              __typename
+              id
+              fields {
+                field
+                value
+              }
+              muted
+            }
+            """
+        )
+        variables: dict[str, object] = {"id": id}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return Segments.parse_obj(data).segments
+
+    async def segments_by_resource_name(
+        self, resource_name: str, resource_namespace: str
+    ) -> List[SegmentsByResourceNameSegmentsByResourceName]:
+        query = gql(
+            """
+            query SegmentsByResourceName($resourceName: String!, $resourceNamespace: String! = "default") {
+              segmentsByResourceName(
+                resourceName: $resourceName
+                resourceNamespace: $resourceNamespace
+              ) {
+                ...SegmentDetails
+              }
+            }
+
+            fragment SegmentDetails on Segment {
+              __typename
+              id
+              fields {
+                field
+                value
+              }
+              muted
+            }
+            """
+        )
+        variables: dict[str, object] = {
+            "resourceName": resource_name,
+            "resourceNamespace": resource_namespace,
+        }
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return SegmentsByResourceName.parse_obj(data).segments_by_resource_name
+
     async def snowflake_credential_secret_changed(
         self, input: SnowflakeCredentialSecretChangedInput
     ) -> SnowflakeCredentialSecretChangedSnowflakeCredentialSecretChanged:
         query = gql(
             """
             query SnowflakeCredentialSecretChanged($input: SnowflakeCredentialSecretChangedInput!) {
               snowflakeCredentialSecretChanged(input: $input) {
@@ -15254,22 +15465,22 @@
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateLocalIdentityProvider.parse_obj(
             data
         ).local_identity_provider_update
 
-    async def update_notification_rule_v2(
-        self, input: NotificationRuleV2UpdateInput
-    ) -> UpdateNotificationRuleV2NotificationRuleV2Update:
+    async def update_notification_rule(
+        self, input: NotificationRuleUpdateInput
+    ) -> UpdateNotificationRuleNotificationRuleUpdate:
         query = gql(
             """
-            mutation UpdateNotificationRuleV2($input: NotificationRuleV2UpdateInput!) {
-              notificationRuleV2Update(input: $input) {
-                ...NotificationRuleV2Update
+            mutation UpdateNotificationRule($input: NotificationRuleUpdateInput!) {
+              notificationRuleUpdate(input: $input) {
+                ...NotificationRuleUpdate
               }
             }
 
             fragment ChannelDetails on Channel {
               __typename
               id
               name
@@ -15289,44 +15500,44 @@
                   webhookUrl
                   applicationLinkUrl
                   authHeader
                 }
               }
             }
 
-            fragment NotificationRuleV2Details on NotificationRuleV2 {
+            fragment NotificationRuleDetails on NotificationRule {
               __typename
               id
               name
               notificationTypenames
               createdAt
               updatedAt
               sources
               channel {
                 ...ChannelDetails
               }
               resourceName
               resourceNamespace
             }
 
-            fragment NotificationRuleV2Update on NotificationRuleV2UpdateResult {
+            fragment NotificationRuleUpdate on NotificationRuleUpdateResult {
               errors {
                 code
                 message
               }
               notificationRule {
-                ...NotificationRuleV2Details
+                ...NotificationRuleDetails
               }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
-        return UpdateNotificationRuleV2.parse_obj(data).notification_rule_v2_update
+        return UpdateNotificationRule.parse_obj(data).notification_rule_update
 
     async def update_numeric_anomaly_validator(
         self, input: NumericAnomalyValidatorUpdateInput
     ) -> UpdateNumericAnomalyValidatorNumericAnomalyValidatorUpdate:
         query = gql(
             """
             mutation UpdateNumericAnomalyValidator($input: NumericAnomalyValidatorUpdateInput!) {
```

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_aws_redshift_credential.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_postgre_sql_credential.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_saml_identity_provider.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_snowflake_destination.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_credential.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_credentials.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_destination.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_destinations.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_segmentation.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_segmentation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_source.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_sources.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_validators.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_window.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_window.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/delete_windows.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/delete_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/enums.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/enums.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/exceptions.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/fragments.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     CategoricalDistributionMetric,
     ComparisonOperator,
     DecisionBoundsType,
     IdentityDeleteErrorCode,
     IdentityProviderCreateErrorCode,
     IdentityProviderDeleteErrorCode,
     IdentityProviderUpdateErrorCode,
+    NotificationSeverity,
     NotificationTypename,
     NumericAnomalyMetric,
     NumericDistributionMetric,
     NumericMetric,
     RelativeTimeMetric,
     RelativeVolumeMetric,
     Role,
@@ -736,124 +737,124 @@
 
 class IdentityProviderUpdateIdentityProviderSamlIdentityProviderConfig(BaseModel):
     entry_point: str = Field(alias="entryPoint")
     entity_id: str = Field(alias="entityId")
     cert: str
 
 
-class NotificationRuleV2Details(BaseModel):
+class NotificationRuleDetails(BaseModel):
     typename__: str = Field(alias="__typename")
     id: Any
     name: str
     notification_typenames: List[NotificationTypename] = Field(
         alias="notificationTypenames"
     )
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     sources: List[Optional[SourceId]]
     channel: Union[
-        "NotificationRuleV2DetailsChannelChannel",
-        "NotificationRuleV2DetailsChannelSlackChannel",
-        "NotificationRuleV2DetailsChannelWebhookChannel",
+        "NotificationRuleDetailsChannelChannel",
+        "NotificationRuleDetailsChannelSlackChannel",
+        "NotificationRuleDetailsChannelWebhookChannel",
     ] = Field(discriminator="typename__")
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
 
 
-class NotificationRuleV2DetailsChannelChannel(BaseModel):
+class NotificationRuleDetailsChannelChannel(BaseModel):
     typename__: Literal["Channel"] = Field(alias="__typename")
     id: Any
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
 
 
-class NotificationRuleV2DetailsChannelSlackChannel(BaseModel):
+class NotificationRuleDetailsChannelSlackChannel(BaseModel):
     typename__: Literal["SlackChannel"] = Field(alias="__typename")
     id: Any
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
-    config: "NotificationRuleV2DetailsChannelSlackChannelConfig"
+    config: "NotificationRuleDetailsChannelSlackChannelConfig"
 
 
-class NotificationRuleV2DetailsChannelSlackChannelConfig(BaseModel):
+class NotificationRuleDetailsChannelSlackChannelConfig(BaseModel):
     webhook_url: str = Field(alias="webhookUrl")
     timezone: Optional[str]
     application_link_url: str = Field(alias="applicationLinkUrl")
 
 
-class NotificationRuleV2DetailsChannelWebhookChannel(BaseModel):
+class NotificationRuleDetailsChannelWebhookChannel(BaseModel):
     typename__: Literal["WebhookChannel"] = Field(alias="__typename")
     id: Any
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
-    config: "NotificationRuleV2DetailsChannelWebhookChannelConfig"
+    config: "NotificationRuleDetailsChannelWebhookChannelConfig"
 
 
-class NotificationRuleV2DetailsChannelWebhookChannelConfig(BaseModel):
+class NotificationRuleDetailsChannelWebhookChannelConfig(BaseModel):
     webhook_url: str = Field(alias="webhookUrl")
     application_link_url: str = Field(alias="applicationLinkUrl")
     auth_header: Optional[str] = Field(alias="authHeader")
 
 
-class NotificationRuleV2Creation(BaseModel):
-    errors: List["NotificationRuleV2CreationErrors"]
-    notification_rule: Optional["NotificationRuleV2CreationNotificationRule"] = Field(
+class NotificationRuleCreation(BaseModel):
+    errors: List["NotificationRuleCreationErrors"]
+    notification_rule: Optional["NotificationRuleCreationNotificationRule"] = Field(
         alias="notificationRule"
     )
 
 
-class NotificationRuleV2CreationErrors(BaseModel):
+class NotificationRuleCreationErrors(BaseModel):
     code: ApiErrorCode
     message: str
 
 
-class NotificationRuleV2CreationNotificationRule(NotificationRuleV2Details):
+class NotificationRuleCreationNotificationRule(NotificationRuleDetails):
     pass
 
 
-class NotificationRuleV2Deletion(BaseModel):
-    errors: List["NotificationRuleV2DeletionErrors"]
-    notification_rule: Optional["NotificationRuleV2DeletionNotificationRule"] = Field(
+class NotificationRuleDeletion(BaseModel):
+    errors: List["NotificationRuleDeletionErrors"]
+    notification_rule: Optional["NotificationRuleDeletionNotificationRule"] = Field(
         alias="notificationRule"
     )
 
 
-class NotificationRuleV2DeletionErrors(BaseModel):
+class NotificationRuleDeletionErrors(BaseModel):
     code: ApiErrorCode
     message: str
 
 
-class NotificationRuleV2DeletionNotificationRule(BaseModel):
-    typename__: Literal["NotificationRuleV2"] = Field(alias="__typename")
+class NotificationRuleDeletionNotificationRule(BaseModel):
+    typename__: Literal["NotificationRule"] = Field(alias="__typename")
     id: Any
     name: str
 
 
-class NotificationRuleV2Update(BaseModel):
-    errors: List["NotificationRuleV2UpdateErrors"]
-    notification_rule: Optional["NotificationRuleV2UpdateNotificationRule"] = Field(
+class NotificationRuleUpdate(BaseModel):
+    errors: List["NotificationRuleUpdateErrors"]
+    notification_rule: Optional["NotificationRuleUpdateNotificationRule"] = Field(
         alias="notificationRule"
     )
 
 
-class NotificationRuleV2UpdateErrors(BaseModel):
+class NotificationRuleUpdateErrors(BaseModel):
     code: ApiErrorCode
     message: str
 
 
-class NotificationRuleV2UpdateNotificationRule(NotificationRuleV2Details):
+class NotificationRuleUpdateNotificationRule(NotificationRuleDetails):
     pass
 
 
 class ReferenceSourceConfigDetails(BaseModel):
     source: "ReferenceSourceConfigDetailsSource"
     window: "ReferenceSourceConfigDetailsWindow"
     history: int
@@ -2845,14 +2846,74 @@
 ):
     id: WindowId
     name: str
     resource_name: str = Field(alias="resourceName")
     resource_namespace: str = Field(alias="resourceNamespace")
 
 
+class ValidatorIncidents(BaseModel):
+    typename__: str = Field(alias="__typename")
+    id: Any
+    severity: NotificationSeverity
+    segment: "ValidatorIncidentsSegment"
+    metric: Union[
+        "ValidatorIncidentsMetricValidatorMetric",
+        "ValidatorIncidentsMetricValidatorMetricWithFixedThreshold",
+        "ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold",
+        "ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold",
+    ] = Field(discriminator="typename__")
+
+
+class ValidatorIncidentsSegment(SegmentDetails):
+    pass
+
+
+class ValidatorIncidentsMetricValidatorMetric(BaseModel):
+    typename__: Literal["ValidatorMetric"] = Field(alias="__typename")
+    start_time: datetime = Field(alias="startTime")
+    end_time: datetime = Field(alias="endTime")
+    is_incident: bool = Field(alias="isIncident")
+    value: float
+
+
+class ValidatorIncidentsMetricValidatorMetricWithFixedThreshold(BaseModel):
+    typename__: Literal["ValidatorMetricWithFixedThreshold"] = Field(alias="__typename")
+    start_time: datetime = Field(alias="startTime")
+    end_time: datetime = Field(alias="endTime")
+    is_incident: bool = Field(alias="isIncident")
+    value: float
+    operator: ComparisonOperator
+    bound: float
+
+
+class ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold(BaseModel):
+    typename__: Literal["ValidatorMetricWithDynamicThreshold"] = Field(
+        alias="__typename"
+    )
+    start_time: datetime = Field(alias="startTime")
+    end_time: datetime = Field(alias="endTime")
+    is_incident: bool = Field(alias="isIncident")
+    value: float
+    lower_bound: float = Field(alias="lowerBound")
+    upper_bound: float = Field(alias="upperBound")
+    decision_bounds_type: DecisionBoundsType = Field(alias="decisionBoundsType")
+    is_burn_in: bool = Field(alias="isBurnIn")
+
+
+class ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold(BaseModel):
+    typename__: Literal["ValidatorMetricWithMonotonicThreshold"] = Field(
+        alias="__typename"
+    )
+    start_time: datetime = Field(alias="startTime")
+    end_time: datetime = Field(alias="endTime")
+    is_incident: bool = Field(alias="isIncident")
+    value: float
+    operator: ComparisonOperator
+
+
 class ValidatorRecommendationApplication(BaseModel):
     typename__: str = Field(alias="__typename")
     failed_ids: List[Any] = Field(alias="failedIds")
     success_ids: List[str] = Field(alias="successIds")
 
 
 class ValidatorRecommendationDismissal(BaseModel):
@@ -4023,29 +4084,29 @@
 IdentityProviderDeletion.update_forward_refs()
 IdentityProviderDeletionErrors.update_forward_refs()
 IdentityProviderUpdate.update_forward_refs()
 IdentityProviderUpdateErrors.update_forward_refs()
 IdentityProviderUpdateIdentityProviderIdentityProvider.update_forward_refs()
 IdentityProviderUpdateIdentityProviderSamlIdentityProvider.update_forward_refs()
 IdentityProviderUpdateIdentityProviderSamlIdentityProviderConfig.update_forward_refs()
-NotificationRuleV2Details.update_forward_refs()
-NotificationRuleV2DetailsChannelChannel.update_forward_refs()
-NotificationRuleV2DetailsChannelSlackChannel.update_forward_refs()
-NotificationRuleV2DetailsChannelSlackChannelConfig.update_forward_refs()
-NotificationRuleV2DetailsChannelWebhookChannel.update_forward_refs()
-NotificationRuleV2DetailsChannelWebhookChannelConfig.update_forward_refs()
-NotificationRuleV2Creation.update_forward_refs()
-NotificationRuleV2CreationErrors.update_forward_refs()
-NotificationRuleV2CreationNotificationRule.update_forward_refs()
-NotificationRuleV2Deletion.update_forward_refs()
-NotificationRuleV2DeletionErrors.update_forward_refs()
-NotificationRuleV2DeletionNotificationRule.update_forward_refs()
-NotificationRuleV2Update.update_forward_refs()
-NotificationRuleV2UpdateErrors.update_forward_refs()
-NotificationRuleV2UpdateNotificationRule.update_forward_refs()
+NotificationRuleDetails.update_forward_refs()
+NotificationRuleDetailsChannelChannel.update_forward_refs()
+NotificationRuleDetailsChannelSlackChannel.update_forward_refs()
+NotificationRuleDetailsChannelSlackChannelConfig.update_forward_refs()
+NotificationRuleDetailsChannelWebhookChannel.update_forward_refs()
+NotificationRuleDetailsChannelWebhookChannelConfig.update_forward_refs()
+NotificationRuleCreation.update_forward_refs()
+NotificationRuleCreationErrors.update_forward_refs()
+NotificationRuleCreationNotificationRule.update_forward_refs()
+NotificationRuleDeletion.update_forward_refs()
+NotificationRuleDeletionErrors.update_forward_refs()
+NotificationRuleDeletionNotificationRule.update_forward_refs()
+NotificationRuleUpdate.update_forward_refs()
+NotificationRuleUpdateErrors.update_forward_refs()
+NotificationRuleUpdateNotificationRule.update_forward_refs()
 ReferenceSourceConfigDetails.update_forward_refs()
 ReferenceSourceConfigDetailsSource.update_forward_refs()
 ReferenceSourceConfigDetailsWindow.update_forward_refs()
 SegmentDetails.update_forward_refs()
 SegmentDetailsFields.update_forward_refs()
 SegmentationDetails.update_forward_refs()
 SegmentationDetailsSource.update_forward_refs()
@@ -4261,14 +4322,20 @@
 ValidatorCreationValidatorRelativeVolumeValidatorConfig.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdDynamicThreshold.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdFixedThreshold.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorConfigThresholdMonotonicThreshold.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfig.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigSource.update_forward_refs()
 ValidatorCreationValidatorRelativeVolumeValidatorReferenceSourceConfigWindow.update_forward_refs()
+ValidatorIncidents.update_forward_refs()
+ValidatorIncidentsSegment.update_forward_refs()
+ValidatorIncidentsMetricValidatorMetric.update_forward_refs()
+ValidatorIncidentsMetricValidatorMetricWithFixedThreshold.update_forward_refs()
+ValidatorIncidentsMetricValidatorMetricWithDynamicThreshold.update_forward_refs()
+ValidatorIncidentsMetricValidatorMetricWithMonotonicThreshold.update_forward_refs()
 ValidatorRecommendationApplication.update_forward_refs()
 ValidatorRecommendationDismissal.update_forward_refs()
 ValidatorRecommendationDismissalErrors.update_forward_refs()
 ValidatorUpdate.update_forward_refs()
 ValidatorUpdateErrors.update_forward_refs()
 ValidatorUpdateValidatorValidator.update_forward_refs()
 ValidatorUpdateValidatorValidatorSourceConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_channel_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_channel_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_channels.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_credential_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_credential_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_destination_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_destination_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_identity_providers.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_identity_providers.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_notification_rule_v2_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
-from .fragments import NotificationRuleV2Details
+from .fragments import NotificationRuleDetails
 
 
-class GetNotificationRuleV2ByResourceName(BaseModel):
-    notification_rule_v2_by_resource_name: Optional[
-        "GetNotificationRuleV2ByResourceNameNotificationRuleV2ByResourceName"
-    ] = Field(alias="notificationRuleV2ByResourceName")
+class GetNotificationRuleByResourceName(BaseModel):
+    notification_rule_by_resource_name: Optional[
+        "GetNotificationRuleByResourceNameNotificationRuleByResourceName"
+    ] = Field(alias="notificationRuleByResourceName")
 
 
-class GetNotificationRuleV2ByResourceNameNotificationRuleV2ByResourceName(
-    NotificationRuleV2Details
+class GetNotificationRuleByResourceNameNotificationRuleByResourceName(
+    NotificationRuleDetails
 ):
     pass
 
 
-GetNotificationRuleV2ByResourceName.update_forward_refs()
-GetNotificationRuleV2ByResourceNameNotificationRuleV2ByResourceName.update_forward_refs()
+GetNotificationRuleByResourceName.update_forward_refs()
+GetNotificationRuleByResourceNameNotificationRuleByResourceName.update_forward_refs()
```

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_source.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_source_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_source_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_source_recommended_validators.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_source_recommended_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_validator_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_validator_segment_metrics.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_validator_segment_metrics.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/get_window_by_resource_name.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/get_window_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/input_types.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/input_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,40 +408,44 @@
     id: str
 
 
 class IdentityProviderDeleteInput(BaseModel):
     id: str
 
 
+class IncidentsInput(BaseModel):
+    time_range: "TimeRangeInput" = Field(alias="timeRange")
+
+
 class LocalIdentityProviderUpdateInput(BaseModel):
     disabled: bool
     id: str
     name: str
 
 
 class MonotonicThresholdCreateInput(BaseModel):
     operator: ComparisonOperator
 
 
-class NotificationRuleV2CreateInput(BaseModel):
+class NotificationRuleCreateInput(BaseModel):
     channel_id: Any = Field(alias="channelId")
     name: str
     notification_typenames: List[NotificationTypename] = Field(
         alias="notificationTypenames"
     )
     resource_name: Optional[str] = Field(alias="resourceName")
     resource_namespace: Optional[str] = Field(alias="resourceNamespace")
     sources: List[SourceId]
 
 
-class NotificationRuleV2DeleteInput(BaseModel):
+class NotificationRuleDeleteInput(BaseModel):
     id: Any
 
 
-class NotificationRuleV2UpdateInput(BaseModel):
+class NotificationRuleUpdateInput(BaseModel):
     id: Any
     name: Optional[str]
     notification_typenames: List[NotificationTypename] = Field(
         alias="notificationTypenames"
     )
     sources: List[SourceId]
 
@@ -768,14 +772,19 @@
     window_id: WindowId = Field(alias="windowId")
 
 
 class SourceConfigUpdateInput(BaseModel):
     filter: Optional[JsonFilterExpression]
 
 
+class SourceIncidentsInput(BaseModel):
+    source_id: SourceId = Field(alias="sourceId")
+    time_range: "TimeRangeInput" = Field(alias="timeRange")
+
+
 class TimeRangeInput(BaseModel):
     end: datetime
     start: datetime
 
 
 class TumblingWindowCreateInput(BaseModel):
     data_time_field: JsonPointer = Field(alias="dataTimeField")
@@ -822,14 +831,15 @@
 class ValidatorIncidentsInput(BaseModel):
     time_range: "TimeRangeInput" = Field(alias="timeRange")
     validator_id: ValidatorId = Field(alias="validatorId")
 
 
 class ValidatorRecommendationApplyInput(BaseModel):
     ids: List[Any]
+    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
 
 
 class ValidatorRecommendationDismissInput(BaseModel):
     ids: List[Any]
 
 
 class ValidatorSegmentIncidentsInput(BaseModel):
@@ -942,19 +952,20 @@
 GcpPubSubSourceCreateInput.update_forward_refs()
 GcpPubSubSourceUpdateInput.update_forward_refs()
 GcpStorageInferSchemaInput.update_forward_refs()
 GcpStorageSourceCreateInput.update_forward_refs()
 GcpStorageSourceUpdateInput.update_forward_refs()
 IdentityDeleteInput.update_forward_refs()
 IdentityProviderDeleteInput.update_forward_refs()
+IncidentsInput.update_forward_refs()
 LocalIdentityProviderUpdateInput.update_forward_refs()
 MonotonicThresholdCreateInput.update_forward_refs()
-NotificationRuleV2CreateInput.update_forward_refs()
-NotificationRuleV2DeleteInput.update_forward_refs()
-NotificationRuleV2UpdateInput.update_forward_refs()
+NotificationRuleCreateInput.update_forward_refs()
+NotificationRuleDeleteInput.update_forward_refs()
+NotificationRuleUpdateInput.update_forward_refs()
 NumericAnomalyValidatorCreateInput.update_forward_refs()
 NumericAnomalyValidatorUpdateInput.update_forward_refs()
 NumericDistributionValidatorCreateInput.update_forward_refs()
 NumericDistributionValidatorUpdateInput.update_forward_refs()
 NumericValidatorCreateInput.update_forward_refs()
 NumericValidatorUpdateInput.update_forward_refs()
 PostgreSqlCredentialCreateInput.update_forward_refs()
@@ -984,14 +995,15 @@
 SnowflakeDestinationCreateInput.update_forward_refs()
 SnowflakeDestinationUpdateInput.update_forward_refs()
 SnowflakeInferSchemaInput.update_forward_refs()
 SnowflakeSourceCreateInput.update_forward_refs()
 SnowflakeSourceUpdateInput.update_forward_refs()
 SourceConfigCreateInput.update_forward_refs()
 SourceConfigUpdateInput.update_forward_refs()
+SourceIncidentsInput.update_forward_refs()
 TimeRangeInput.update_forward_refs()
 TumblingWindowCreateInput.update_forward_refs()
 TumblingWindowUpdateInput.update_forward_refs()
 UserCreateInput.update_forward_refs()
 UserDeleteInput.update_forward_refs()
 UserUpdateInput.update_forward_refs()
 ValidatorIncidentsInput.update_forward_refs()
```

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/list_credentials.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/list_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/list_destinations.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/list_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/list_sources.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/list_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/list_validators.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/list_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/list_windows.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/list_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/scalars.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/scalars.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Any, Callable, Dict
 
 from validio_sdk.scalars import (
+    BooleanFilter,
     EnumFilter,
     NullFilter,
     StringFilter,
     ThresholdFilter,
     serialize_json_filter_expression,
 )
 
 SCALARS_PARSE_FUNCTIONS: Dict[Any, Callable[[Any], Any]] = {}
 SCALARS_SERIALIZE_FUNCTIONS: Dict[Any, Callable[[Any], Any]] = {
+    BooleanFilter: serialize_json_filter_expression,
     EnumFilter: serialize_json_filter_expression,
     NullFilter: serialize_json_filter_expression,
     StringFilter: serialize_json_filter_expression,
     ThresholdFilter: serialize_json_filter_expression,
 }
```

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/start_source.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/start_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/stop_source.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/stop_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_aws_redshift_credential.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_local_identity_provider.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_local_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_postgre_sql_credential.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_relative_time_validator.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_relative_time_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_relative_volume_validator.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_relative_volume_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_saml_identity_provider.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_snowflake_destination.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py` & `validio_sdk-0.2.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_diff.py` & `validio_sdk-0.2.0/validio_sdk/resource/_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from validio_sdk.resource._util import SourceSchemaReinference, _sanitize_error
 from validio_sdk.resource.credentials import Credential
 from validio_sdk.resource.sources import Source
 from validio_sdk.validio_client import ValidioAPIClient
 
 R = TypeVar("R", bound=Resource)
 
-
 """
 When we descend into nested objects, we set a limit on how deep we go.
 Otherwise, in a bad manifest configuration or due to a bug in our code, we
 could enter a cycle.
 """
 MAX_RESOURCE_DEPTH = 15
 
@@ -62,15 +61,15 @@
     credentials: dict[str, ResourceUpdate] = dataclasses.field(default_factory=dict)
     channels: dict[str, ResourceUpdate] = dataclasses.field(default_factory=dict)
     sources: dict[str, ResourceUpdate] = dataclasses.field(default_factory=dict)
     destinations: dict[str, ResourceUpdate] = dataclasses.field(default_factory=dict)
     windows: dict[str, ResourceUpdate] = dataclasses.field(default_factory=dict)
     segmentations: dict[str, ResourceUpdate] = dataclasses.field(default_factory=dict)
     validators: dict[str, ResourceUpdate] = dataclasses.field(default_factory=dict)
-    notification_rules_v2: dict[str, ResourceUpdate] = dataclasses.field(
+    notification_rules: dict[str, ResourceUpdate] = dataclasses.field(
         default_factory=dict
     )
 
 
 @dataclass
 class GraphDiff:
     to_create: DiffContext
@@ -161,25 +160,31 @@
         if source_field_selector:
             field_selector = source_field_selector
         elif filter_field_selector:
             field_selector = filter_field_selector
         else:
             continue
 
+        source = must_find_source(manifest_ctx, template.source_name)
+        if source.jtd_schema is None:
+            # If we have no schema then it means we're doing a diff where the
+            # source's credential has not yet been created - which means we can't
+            # do schema inference. As a result, we can't yet expand the selector.
+            continue
+
         if source_field_selector:
             delattr(template, "_field_selector")
         if reference_field_selector:
             delattr(template, "_reference_field_selector")
         if filter_field_selector:
             delattr(template.filter, "_field_selector")
 
         # Remove the placeholder validator.
         del manifest_ctx.validators[name]
 
-        source = must_find_source(manifest_ctx, template.source_name)
         fields = field_selector.field_selector._get_matching_fields(
             cast(Any, source.jtd_schema)
         )
 
         # We don't want to deep copy the entire resource graph
         resource_graph = template._resource_graph
         template._resource_graph = None  # type: ignore
@@ -461,14 +466,18 @@
 
 async def infer_schema_for_source(
     manifest_ctx: DiffContext,
     source: Source,
     client: ValidioAPIClient,
 ):
     credential = manifest_ctx.credentials[source.credential_name]
+    # If we don't yet have an ID (credential has not yet been created),
+    # we can't do schema inference. So schema will be unknown in the diff.
+    if credential._id.value is None:
+        return
     await source._api_infer_schema(credential, client)
 
 
 async def check_for_credential_secret_changes(
     manifest_ctx: DiffContext,
     graph: GraphDiff,
     client: ValidioAPIClient,
@@ -527,17 +536,15 @@
 def collect_resource_diff(
     manifest_resource: Resource,
     server_resource: Resource,
     extra_fields: set[str] | None = None,
     show_secrets: bool | None = None,
 ) -> ResourceUpdate:
     all_fields = {
-        *manifest_resource._immutable_fields(),
-        *manifest_resource._mutable_fields(),
-        *manifest_resource._nested_objects().keys(),
+        *manifest_resource._all_fields(),
         *(extra_fields if extra_fields else {}),
     }
     manifest_config = {f: getattr(manifest_resource, f) for f in all_fields}
     server_config = {f: getattr(server_resource, f) for f in all_fields}
 
     # When generating a diff - if there's a credential involved,
     # then mask it if requested.
@@ -558,11 +565,11 @@
     )
 
 
 def _check_namespace(namespace: str, server_resource: Resource):
     server_namespace = server_resource._must_namespace()
     if namespace != server_namespace:
         raise ManifestConfigurationError(
-            f"resource {server_resource.__class__.__name__} does not belong to the "
-            f"current namespace; resource namespace = {server_namespace}; "
-            f"current namespace = {namespace}"
+            f"resource {server_resource.__class__.__name__} '{server_resource.name}' "
+            "does not belong to the current namespace; "
+            f"resource namespace = {server_namespace}; current namespace = {namespace}"
         )
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_diff_util.py` & `validio_sdk-0.2.0/validio_sdk/resource/_diff_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_diffable.py` & `validio_sdk-0.2.0/validio_sdk/resource/_diffable.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from typing import Optional
 
 
-class Diffable:
+class Diffable(ABC):
     """
     An abstract class to be implemented by objects that can be diff-ed against the
     server version. All Resource instances implement this by default. And in some
     cases (like filters, thresholds etc.), nested objects of a resource need to be
     diff-ed and require such objects require an implementation of this base.
 
     NOTE: When adding/removing fields to any resource or object contained
@@ -27,7 +27,20 @@
     def _nested_objects(self) -> dict[str, Optional["Diffable"]]:
         """Returns any nested objects contained within this object.
 
         Nested objects will be diff-ed recursively.
         ...
         :returns dict[field, Optional[object]].
         """
+
+    def _ignored_fields(self) -> set[str]:
+        """Returns any fields on the object that can should not be diffed."""
+        return set({})
+
+    def _all_fields(self) -> set[str]:
+        """Return all fields of the resource."""
+        return {
+            *self._immutable_fields(),
+            *self._mutable_fields(),
+            *self._nested_objects().keys(),
+            *self._ignored_fields(),
+        }
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_errors.py` & `validio_sdk-0.2.0/validio_sdk/resource/_errors.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_field_selector.py` & `validio_sdk-0.2.0/validio_sdk/resource/_field_selector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import re
 from dataclasses import dataclass
 from enum import Enum
 from typing import TYPE_CHECKING, Any
 
-from validio_sdk.resource._errors import ManifestConfigurationError
-
 if TYPE_CHECKING:
     from validio_sdk.scalars import JsonTypeDefinition
 
 
 class FieldDataType(str, Enum):
     """Represents the datatype of a field."""
 
@@ -92,33 +90,29 @@
         return FromFieldSelector()
 
     def _encode(self) -> dict[str, object]:
         return self.__dict__
 
     def _get_matching_fields(self, schema: "JsonTypeDefinition") -> list[str]:
         matching_fields = []
-        properties: dict[str, dict[str, str]] = {}
+        properties: dict[str, dict[str, Any]] = {}
         for k in ["optionalProperties", "properties"]:
             if k in schema:
                 properties = {**properties, **schema[k]}
 
         for name, prop in properties.items():
-            for required_field in ["nullable"]:
-                if required_field not in prop:
-                    raise ManifestConfigurationError(
-                        "invalid JTD schema: missing required field"
-                        f" {required_field} in property {prop}"
-                    )
-
             if "type" not in prop or not FieldDataType[self.data_type]._matches(
                 prop["type"]
             ):
                 continue
 
-            if self.nullable and self.nullable != prop["nullable"]:
+            nullable_prop = True
+            if "nullable" in prop:
+                nullable_prop = prop["nullable"]
+            if self.nullable and self.nullable != nullable_prop:
                 continue
 
             if self.regex and not re.match(self.regex, name):
                 continue
 
             matching_fields.append(name)
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_resource.py` & `validio_sdk-0.2.0/validio_sdk/resource/_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 )
 from validio_sdk.validio_client import ValidioAPIClient
 
 if TYPE_CHECKING:
     from validio_sdk.resource.channels import Channel
     from validio_sdk.resource.credentials import Credential
     from validio_sdk.resource.destinations import Destination
-    from validio_sdk.resource.notification_rules_v2 import NotificationRuleV2
+    from validio_sdk.resource.notification_rules import NotificationRule
     from validio_sdk.resource.segmentations import Segmentation
     from validio_sdk.resource.sources import Source
     from validio_sdk.resource.validators import Validator
     from validio_sdk.resource.windows import Window
 
-
 R = TypeVar("R", bound="Resource")
 
 
 @dataclass
 class DiffContext:
     """
     Caches all objects of a graph to make it easier to
@@ -42,15 +41,15 @@
     credentials: dict[str, "Credential"] = dataclasses.field(default_factory=dict)
     channels: dict[str, "Channel"] = dataclasses.field(default_factory=dict)
     sources: dict[str, "Source"] = dataclasses.field(default_factory=dict)
     destinations: dict[str, "Destination"] = dataclasses.field(default_factory=dict)
     windows: dict[str, "Window"] = dataclasses.field(default_factory=dict)
     segmentations: dict[str, "Segmentation"] = dataclasses.field(default_factory=dict)
     validators: dict[str, "Validator"] = dataclasses.field(default_factory=dict)
-    notification_rules_v2: dict[str, "NotificationRuleV2"] = dataclasses.field(
+    notification_rules: dict[str, "NotificationRule"] = dataclasses.field(
         default_factory=dict
     )
 
     # Validators objects that are yet to be decoded
     pending_validators_raw: dict[str, tuple[type, dict[str, Any]]] = dataclasses.field(
         default_factory=dict
     )
@@ -118,14 +117,18 @@
         )
 
         # The graph must always come from the parent. Except for the root
         # node type (Credential) which will explicitly set a default if none
         # was provided.
         self._resource_graph: ResourceGraph = __internal__
 
+        # Flags whether this resource has been applied (created/deleted/updated)
+        # on the server.
+        self._applied = False
+
     def _must_id(self) -> str:
         if self._id.value is None:
             raise RuntimeError(
                 f"resource {self.__class__.__name__}(name={self.name}) "
                 "has unresolved ID"
             )
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_resource_graph.py` & `validio_sdk-0.2.0/validio_sdk/resource/_resource_graph.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import atexit
 import json
 import os
+import sys
 
 from validio_sdk.code.settings import dump_graph_var, graph_preamble_var
 from validio_sdk.resource._resource import ResourceGraph
 from validio_sdk.resource._serde import custom_resource_graph_encoder
 
 """
 This holds a 'global' instance of a resource graph. This is the graph
@@ -15,14 +16,23 @@
 RESOURCE_GRAPH: ResourceGraph = ResourceGraph()
 
 
 def _dump_graph():
     # Since we piggyback on stdout, we prefix the graph with a
     # preamble to identify the start of the relevant info in the stream.
     if dump_graph_var in os.environ:
-        print(graph_preamble_var)
-        print(
-            json.dumps(RESOURCE_GRAPH, default=custom_resource_graph_encoder, indent=2)
-        )
+        try:
+            print(graph_preamble_var)
+            print(
+                json.dumps(
+                    RESOURCE_GRAPH, default=custom_resource_graph_encoder, indent=2
+                )
+            )
+        except Exception as e:
+            # If we fail to parse the graph, write the error out to stderr
+            # since Python won't let us easily exit with an error from here.
+            # The parent process is set up to check stderr since we don't
+            # have a graph, so it will exit with the error instead.
+            print(e, file=sys.stderr)
 
 
 atexit.register(_dump_graph)
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_serde.py` & `validio_sdk-0.2.0/validio_sdk/resource/_serde.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 itself or other internal fields that we don't need to serialise. We ignore these
 during encoding.
 """
 SKIPPED_INTERNAL_FIELD_NAMES = {
     "_resource_names_by_type",
     "_resource_graph",
     "_id",
+    "_applied",
     "_namespace",
 }
 
 """
 Contains the type (unique hardcoded name) of the current node.
 Allows us know how to decode that node.
 """
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_server_resources.py` & `validio_sdk-0.2.0/validio_sdk/resource/_server_resources.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,33 +2,37 @@
 from typing import cast
 
 # We need to import the validio_sdk module due to the `eval`
 # ruff: noqa: F401
 import validio_sdk
 from validio_sdk.graphql_client import (
     GraphQLClientHttpError,
+    ListCredentialsCredentialsListAwsCredential,
     ListCredentialsCredentialsListAwsRedshiftCredential,
     ListCredentialsCredentialsListPostgreSqlCredential,
     ListCredentialsCredentialsListSnowflakeCredential,
     ReferenceSourceConfigDetails,
 )
 from validio_sdk.resource._diff import (
     DiffContext,
     GraphDiff,
     ResourceUpdates,
+    expand_validator_field_selectors,
+    infer_schema_for_source,
 )
 from validio_sdk.resource._diff_util import (
     must_find_destination,
     must_find_segmentation,
     must_find_source,
     must_find_window,
 )
 from validio_sdk.resource._resource import Resource, ResourceGraph
 from validio_sdk.resource._util import _sanitize_error
 from validio_sdk.resource.credentials import (
+    AwsCredential,
     AwsRedshiftCredential,
     Credential,
     DemoCredential,
     GcpCredential,
     PostgreSqlCredential,
     SnowflakeCredential,
 )
@@ -59,15 +63,15 @@
     await load_credentials(namespace, client, g, ctx)
     await load_channels(namespace, client, g, ctx)
     await load_destinations(namespace, client, ctx)
     await load_sources(namespace, client, ctx)
     await load_segmentations(namespace, client, ctx)
     await load_windows(namespace, client, ctx)
     await load_validators(namespace, client, ctx)
-    await load_notification_rules_v2(namespace, client, ctx)
+    await load_notification_rules(namespace, client, ctx)
 
     return ctx
 
 
 async def load_credentials(
     # ruff: noqa: ARG001
     namespace: str,
@@ -85,14 +89,22 @@
         match c.typename__:
             case "DemoCredential":
                 credential: Credential = DemoCredential(name=name, __internal__=g)
             case "GcpCredential":
                 credential = GcpCredential(
                     name=name, credential="UNSET", __internal__=g
                 )
+            case "AwsCredential":
+                c = cast(ListCredentialsCredentialsListAwsCredential, c)
+                credential = AwsCredential(
+                    name=name,
+                    access_key=c.config.access_key,
+                    secret_key="UNSET",
+                    __internal__=g,
+                )
             case "PostgreSqlCredential":
                 c = cast(ListCredentialsCredentialsListPostgreSqlCredential, c)
                 credential = PostgreSqlCredential(
                     name=name,
                     host=c.config.host,
                     port=c.config.port,
                     user=c.config.user,
@@ -114,14 +126,15 @@
             case "SnowflakeCredential":
                 c = cast(ListCredentialsCredentialsListSnowflakeCredential, c)
                 credential = SnowflakeCredential(
                     name=name,
                     account=c.config.account,
                     user=c.config.user,
                     password="UNSET",
+                    __internal__=g,
                 )
             case _:
                 raise RuntimeError(
                     f"unsupported credential '{name}' of type '{type(c)}'"
                 )
 
         credential._id.value = c.id
@@ -154,50 +167,50 @@
             }
         )
         channel._id.value = ch.id
         channel._namespace = ch.resource_namespace
         ctx.channels[name] = channel
 
 
-async def load_notification_rules_v2(
+async def load_notification_rules(
     namespace: str,
     client: ValidioAPIClient,
     ctx: DiffContext,
 ):
     # We need to import the module due to the `eval`
     # ruff: noqa: F401
-    from validio_sdk.resource import notification_rules_v2
+    from validio_sdk.resource import notification_rules
 
-    rules = await client.get_notification_rules_v2()
+    rules = await client.get_notification_rules()
 
     source_lookup_by_id = {s._must_id(): s for s in ctx.sources.values()}
     for r in rules:
         name = r.resource_name
 
-        cls = eval(f"validio_sdk.resource.notification_rules_v2.{r.typename__}")
+        cls = eval(f"validio_sdk.resource.notification_rules.{r.typename__}")
         fields = list(inspect.signature(cls).parameters)
         rule = cls(
             **{
                 **{
                     f: getattr(r, f)
                     for f in fields
                     if f not in {"name", "channel", "sources"}
                 },
                 "name": name,
                 "channel": ctx.channels[r.channel.resource_name],
                 "sources": [
-                    ctx.sources[sid]
+                    source_lookup_by_id[sid]
                     for sid in r.sources
                     if sid and sid in source_lookup_by_id
                 ],
             }
         )
         rule._id.value = r.id
         rule._namespace = r.resource_namespace
-        ctx.notification_rules_v2[name] = rule
+        ctx.notification_rules[name] = rule
 
 
 async def load_destinations(
     namespace: str,
     client: ValidioAPIClient,
     ctx: DiffContext,
 ):
@@ -300,15 +313,15 @@
         if cls is None:
             raise RuntimeError(
                 f"missing implementation for window type {w.__class__.__name__}"
             )
 
         window = cls(
             **{
-                **w.config.__dict__,  # type:ignore
+                **(w.config.__dict__ if hasattr(w, "config") else {}),  # type:ignore
                 "name": name,
                 "source": must_find_source(ctx, w.source.resource_name),
                 "data_time_field": w.data_time_field,
             }
         )
 
         window._id.value = w.id
@@ -440,65 +453,128 @@
     ctx: DiffContext,
     diff: GraphDiff,
     client: ValidioAPIClient,
     show_secrets: bool,
 ):
     try:
         await apply_deletes(namespace=namespace, deletes=diff.to_delete, client=client)
+
+        # We perform create operations in two batches. First here creates top
+        # level resources, then after performing updates, we create any remaining
+        # resources. We do this due to a couple scenarios
+        # - A resource potentially depends on the parent to be created first before
+        #   it can be updated. Example is a validator being updated to use a
+        #   destination that is to be created. Another is a notification rule that
+        #   is being updated to reference a Source that is to be created. In such
+        #   cases, we need to apply the create on parent resource before the update
+        #   on child resource.
+        # - Conversely, in some cases, a parent resource needs to be updated before
+        #   the child resource can be created. e.g a validator that is referencing a
+        #   new field in a schema needs the source to be updated first otherwise diver
+        #   will reject the validator as invalid because the field does not yet exist.
+        #
+        # So, here we create the top level resources first - ensuring that any child
+        # resource that relies on them are resolved properly.
+        # We start with creating credentials only. Since sources need them to infer
+        # schema.
         await apply_creates(
             namespace=namespace,
             manifest_ctx=ctx,
-            creates=diff.to_create,
+            creates=DiffContext(credentials=diff.to_create.credentials),
+            client=client,
+            show_secrets=show_secrets,
+        )
+
+        # Resolve any pending source schemas now that we have their credential.
+        for source in diff.to_create.sources.values():
+            if source.jtd_schema is None:
+                await infer_schema_for_source(
+                    manifest_ctx=ctx, source=source, client=client
+                )
+
+        # Create the remaining top level resources.
+        await apply_creates(
+            namespace=namespace,
+            manifest_ctx=ctx,
+            creates=DiffContext(
+                sources=diff.to_create.sources,
+                destinations=diff.to_create.destinations,
+                channels=diff.to_create.channels,
+            ),
             client=client,
             show_secrets=show_secrets,
         )
+
+        # Now we should have all source schemas available. We can expand
+        # field selectors.
+        expand_validator_field_selectors(ctx)
+
+        # Then apply updates.
         await apply_updates(
             namespace=namespace, manifest_ctx=ctx, updates=diff.to_update, client=client
         )
+
+        # Then apply remaining creates. Resources that have been created in
+        # the previous steps are marked as _applied, so they will be skipped this
+        # time around.
+        await apply_creates(
+            namespace=namespace,
+            manifest_ctx=ctx,
+            creates=diff.to_create,
+            client=client,
+            show_secrets=show_secrets,
+        )
     except GraphQLClientHttpError as e:
         raise RuntimeError(f"API error: ({e.status_code}: {e.response.json()})")
 
 
 async def apply_deletes(namespace: str, deletes: DiffContext, client: ValidioAPIClient):
     # Delete notification rules first These reference sources so we
     # remove them before removing the sources they reference.
-    for r in deletes.notification_rules_v2.values():
-        await r._api_delete(client)
+    for r in deletes.notification_rules.values():
+        await _delete_resource(r, client)
 
     # For pipeline resources, start with sources (This cascades deletes,
     # so we don't have to individually delete child resources).
     for s in deletes.sources.values():
-        await s._api_delete(client)
+        await _delete_resource(s, client)
 
     # For child resources, we only need to delete them if their parent
     # haven't been deleted.
     for w in deletes.windows.values():
         if w.source_name not in deletes.sources:
-            await w._api_delete(client)
+            await _delete_resource(w, client)
 
     for sg in deletes.segmentations.values():
         if sg.source_name not in deletes.sources:
-            await sg._api_delete(client)
+            await _delete_resource(sg, client)
 
     for v in deletes.validators.values():
         if v.source_name not in deletes.sources:
-            await v._api_delete(client)
+            await _delete_resource(v, client)
 
     # Next, delete destinations. Validators are deleted before we
     # delete potentially attached destinations.
     for d in deletes.destinations.values():
-        await d._api_delete(client)
+        await _delete_resource(d, client)
 
     # Finally delete credentials - these do not cascade so the api rejects any
     # delete requests if there are existing child resources attached to a credential.
     for c in deletes.credentials.values():
-        await c._api_delete(client)
+        await _delete_resource(c, client)
 
     for ch in deletes.channels.values():
-        await ch._api_delete(client)
+        await _delete_resource(ch, client)
+
+
+async def _delete_resource(resource: Resource, client: ValidioAPIClient):
+    if resource._applied:
+        return
+    resource._applied = True
+    await resource._api_delete(client)
 
 
 async def apply_creates(
     namespace: str,
     manifest_ctx: DiffContext,
     creates: DiffContext,
     client: ValidioAPIClient,
@@ -509,18 +585,22 @@
         list(creates.credentials.values()),
         list(creates.sources.values()),
         list(creates.destinations.values()),
         list(creates.segmentations.values()),
         list(creates.windows.values()),
         list(creates.validators.values()),
         list(creates.channels.values()),
-        list(creates.notification_rules_v2.values()),
+        list(creates.notification_rules.values()),
     ]
     for resources in all_resources:
         for r in resources:
+            if r._applied:
+                continue
+            r._applied = True
+
             try:
                 await r._api_create(namespace, client, manifest_ctx)
             except GraphQLClientHttpError as e:
                 raise (
                     _sanitize_error(e, show_secrets) if isinstance(r, Credential) else e
                 )
 
@@ -535,13 +615,17 @@
         list(updates.credentials.values()),
         list(updates.destinations.values()),
         list(updates.sources.values()),
         list(updates.segmentations.values()),
         list(updates.windows.values()),
         list(updates.validators.values()),
         list(updates.channels.values()),
-        list(updates.notification_rules_v2.values()),
+        list(updates.notification_rules.values()),
     ]
 
     for up in all_updates:
         for u in up:
+            if u.manifest.resource._applied:
+                continue
+            u.manifest.resource._applied = True
+
             await u.manifest.resource._api_update(namespace, client, manifest_ctx)
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/_util.py` & `validio_sdk-0.2.0/validio_sdk/resource/_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/channels.py` & `validio_sdk-0.2.0/validio_sdk/resource/channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,37 +61,37 @@
     @staticmethod
     def _decode(
         ctx: "DiffContext",
         cls: type,
         obj: dict[str, dict[str, object]],
         g: ResourceGraph,
     ) -> "Channel":
-        from validio_sdk.resource.notification_rules_v2 import NotificationRuleV2
+        from validio_sdk.resource.notification_rules import NotificationRule
 
         channel = cls(**with_resource_graph_info(obj[CONFIG_FIELD_NAME], g))
 
         # Decode notification rules
         children_obj = cast(dict[str, dict[str, object]], get_children_node(obj))
         notification_rules_obj = cast(
             dict[str, dict[str, object]],
             (
-                children_obj[NotificationRuleV2.__name__]
-                if NotificationRuleV2.__name__ in children_obj
+                children_obj[NotificationRule.__name__]
+                if NotificationRule.__name__ in children_obj
                 else {}
             ),
         )
 
         notification_rules = {}
         for rule_name, value in notification_rules_obj.items():
-            rule = NotificationRuleV2._decode(ctx, channel, value)
+            rule = NotificationRule._decode(ctx, channel, value)
             notification_rules[rule_name] = rule
-            ctx.notification_rules_v2[rule_name] = rule
+            ctx.notification_rules[rule_name] = rule
 
         if len(notification_rules) > 0:
-            channel._children[NotificationRuleV2.__name__] = cast(
+            channel._children[NotificationRule.__name__] = cast(
                 dict[str, Resource], notification_rules
             )
 
         return channel
 
 
 class SlackChannel(Channel):
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/credentials.py` & `validio_sdk-0.2.0/validio_sdk/resource/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         self.access_key = access_key
         self.secret_key = secret_key
 
     def _immutable_fields(self) -> set[str]:
         return set({})
 
     def _mutable_fields(self) -> set[str]:
-        return set({})
+        return {"access_key"}
 
     def _secret_fields(self) -> set[str] | None:
         return {"secret_key"}
 
 
 class SnowflakeCredential(Credential):
     """A credential resource that can be used to connect to a Snowflake table."""
@@ -206,15 +206,15 @@
         self.user = user
         self.password = password
 
     def _immutable_fields(self) -> set[str]:
         return set({})
 
     def _mutable_fields(self) -> set[str]:
-        return {"account", "user", "password"}
+        return {"account", "user"}
 
     def _secret_fields(self) -> set[str] | None:
         return {"password"}
 
 
 class PostgresLikeCredential(Credential):
     """
@@ -249,15 +249,15 @@
         self.password = password
         self.default_database = default_database
 
     def _immutable_fields(self) -> set[str]:
         return set({})
 
     def _mutable_fields(self) -> set[str]:
-        return {"host", "port", "user", "password", "default_database"}
+        return {"host", "port", "user", "default_database"}
 
     def _secret_fields(self) -> set[str] | None:
         return {"password"}
 
 
 class PostgreSqlCredential(PostgresLikeCredential):
     """
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/destinations.py` & `validio_sdk-0.2.0/validio_sdk/resource/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/filters.py` & `validio_sdk-0.2.0/validio_sdk/resource/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,14 +61,43 @@
     def _api_create_input(self) -> dict[str, object]:
         return {
             "__typename": f"{self.__class__.__name__}Expression",
             **self.__dict__,
         }
 
 
+class BooleanFilterOperator(str, Enum):
+    """
+    Configures the behavior of a Boolean filter.
+
+    IS_TRUE: Allow values equal to TRUE
+    IS_FALSE: Allow values equal to FALSE
+    """
+
+    IS_TRUE = "IS_TRUE"
+    IS_FALSE = "IS_FALSE"
+
+
+@dataclass
+class BooleanFilter(Filter):
+    """A Boolean filter configuration.
+
+    https://docs.validio.io/docs/filters#boolean-filter
+    """
+
+    field: Union[str, "FieldSelector"]
+    operator: BooleanFilterOperator
+
+    def __post_init__(self):
+        """Post init for filter."""
+        self.field = self._maybe_set_field_selector("field", self.field)
+        if not isinstance(self.operator, BooleanFilterOperator):
+            self.operator = BooleanFilterOperator(self.operator)
+
+
 class NullFilterOperator(str, Enum):
     """
     Configures the behavior of a Null filter.
 
     IS: Filter in NULL values
     IS_NOT: Filter in Non-NULL values
     """
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/notification_rules_v2.py` & `validio_sdk-0.2.0/validio_sdk/resource/notification_rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Notification rule configuration."""
 from typing import TYPE_CHECKING, Any
 
-from validio_sdk.graphql_client import NotificationRuleV2DeleteInput
+from validio_sdk.graphql_client import (
+    NotificationRuleDeleteInput,
+    NotificationTypename,
+)
 from validio_sdk.resource._resource import Resource
 from validio_sdk.resource._serde import (
     CONFIG_FIELD_NAME,
     _api_create_input_params,
     _api_update_input_params,
     _encode_resource,
 )
@@ -13,27 +16,27 @@
 from validio_sdk.resource.sources import Source
 from validio_sdk.validio_client import ValidioAPIClient
 
 if TYPE_CHECKING:
     from validio_sdk.resource._diff import DiffContext
 
 
-class NotificationRuleV2(Resource):
+class NotificationRule(Resource):
     """
     A notification rule.
 
     https://docs.validio.io/docs/notifications
     """
 
     def __init__(
         self,
         name: str,
         channel: Channel,
         sources: list[Source] | None = None,
-        notification_typenames: list[str] | None = None,
+        notification_typenames: list[NotificationTypename] | None = None,
     ):
         """
         Constructor.
 
         :param name: Unique resource name assigned to the window
         :param channel: The channel to attach the rule to
         :param sources: An optional list of sources to apply the rule onto.
@@ -46,17 +49,24 @@
         self.channel_name = channel.name
 
         # We turn the names into a set and back to list as a means
         # to dedupe the names.
         self.source_names = list(
             {source.name for source in sources} if sources is not None else {}
         )
-        self.notification_typenames = list(
-            set(notification_typenames) if notification_typenames is not None else {}
+
+        typenames = (
+            [
+                n if isinstance(n, NotificationTypename) else NotificationTypename(n)
+                for n in notification_typenames
+            ]
+            if notification_typenames is not None
+            else []
         )
+        self.notification_typenames = list(set(typenames))
 
         # Sort so that we can compare two lists when we look for diffs.
         self.source_names.sort()
         self.notification_typenames.sort()
 
         channel.add(name, self)
 
@@ -64,15 +74,15 @@
         return {"channel_name"}
 
     def _mutable_fields(self) -> set[str]:
         return {"source_names", "notification_typenames"}
 
     def resource_class_name(self) -> str:
         """Returns the base class name."""
-        return "NotificationRuleV2"
+        return "NotificationRule"
 
     def _api_create_response_field_name(self) -> str:
         return "notification_rule"
 
     def _api_create_input(self, namespace: str, ctx: "DiffContext") -> Any:
         return _api_create_input_params(
             self,
@@ -88,20 +98,20 @@
             self,
             overrides={
                 "sources": self._extract_source_ids_from_ctx(ctx),
             },
         )
 
     async def _api_delete(self, client: ValidioAPIClient) -> Any:
-        response = await client.delete_notification_rule_v2(
-            NotificationRuleV2DeleteInput(id=self._must_id())
+        response = await client.delete_notification_rule(
+            NotificationRuleDeleteInput(id=self._must_id())
         )
         return self._check_graphql_response(
             response=response,
-            method_name="delete_notification_rule_v2",
+            method_name="delete_notification_rule",
             response_field=None,
         )
 
     def _extract_source_ids_from_ctx(self, ctx: "DiffContext") -> list[str]:
         ids = []
         for source_name in self.source_names:
             ids.append(ctx.sources[source_name]._must_id())
@@ -112,27 +122,27 @@
         # Drop fields here that are not part of the constructor for when
         # we deserialize back. They will be reinitialized by the constructor.
         return _encode_resource(self, skip_fields={"channel_name"})
 
     @staticmethod
     def _decode(
         ctx: "DiffContext", channel: Channel, obj: dict[str, Any]
-    ) -> "NotificationRuleV2":
+    ) -> "NotificationRule":
         config_obj = obj[CONFIG_FIELD_NAME]
         sources = [
             ctx.sources[source_name] for source_name in config_obj["source_names"]
         ]
         obj = {
             # Drop fields that are not part of the constructor, we will
             # reinitialize them in the constructor.
             k: v
             for k, v in config_obj.items()
             if k not in {"source_names"}
         }
 
-        return NotificationRuleV2(
+        return NotificationRule(
             **{
                 **obj,
                 "channel": channel,
                 "sources": sources,
             }  # type: ignore
         )
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/segmentations.py` & `validio_sdk-0.2.0/validio_sdk/resource/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/sources.py` & `validio_sdk-0.2.0/validio_sdk/resource/sources.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Sources."""
+import inspect
+import json
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, Optional, Union, cast
 
 from camel_converter import to_snake
 
 # We need validio_sdk in scope due to eval.
 # ruff: noqa: F401
 import validio_sdk
 from validio_sdk.graphql_client import (
     CsvParserInput,
 )
 from validio_sdk.resource._diffable import Diffable
-from validio_sdk.resource._errors import ManifestConfigurationError
 from validio_sdk.resource._resource import Resource
 from validio_sdk.resource._serde import (
     CONFIG_FIELD_NAME,
     NODE_TYPE_FIELD_NAME,
     _api_create_input_params,
     _api_update_input_params,
     _encode_resource,
@@ -68,21 +69,21 @@
         self.credential_name: str = credential.name
         self.jtd_schema = jtd_schema
         _sanitize_jtd_schema(self.jtd_schema)
 
         credential.add(name, self)
 
     def _immutable_fields(self) -> set[str]:
-        return set({})
+        return {"credential_name"}
 
     def _mutable_fields(self) -> set[str]:
         # Note: jtd_schema is a mutable field but is handled specially in the diff
         # process - since schemas can be managed automatically. So it's not listed
         # here
-        return {"credential_name"}
+        return set({})
 
     def resource_class_name(self) -> str:
         """Returns the base class name."""
         return "Source"
 
     def _api_create_input(self, namespace: str, ctx: "DiffContext") -> Any:
         return _api_create_input_params(
@@ -225,42 +226,22 @@
         Return the fields (as defined in the graphql ...InferSchemaInput as well
         as their values. The credential id is provided by the caller so that's
         ignored here. If None is returned (Demo), then the inference method is
         assumed to take no parameters (not even a credential id).
         """
 
 
-def _validate_lookback(name: str, lookback_days: int):
-    if lookback_days > MAX_LOOKBACK_DAYS:
-        raise ManifestConfigurationError(
-            f"resource {name}: lookback_days {lookback_days} cannot "
-            f"exceed {MAX_LOOKBACK_DAYS} days"
-        )
-
-
 def _sanitize_jtd_schema(jtd_schema: JsonTypeDefinition | None):
     # TODO VR-2073:
     # The jtd python lib for some reason wants this property to be a string
     # even though the spec and all other language libraries say it's a bool.
     if jtd_schema and "additionalProperties" in jtd_schema:
         del jtd_schema["additionalProperties"]
 
 
-def _sanity_check_cron_schedule(name: str, schedule: str):
-    if len(schedule.split()) != CRON_DIGITS:
-        raise ManifestConfigurationError(
-            f"resource {name}: schedule '{schedule}' must be a 5-digit cron expression"
-        )
-
-
-def _warehouse_checks(name: str, lookback_days: int, schedule: str):
-    _validate_lookback(name, lookback_days)
-    _sanity_check_cron_schedule(name, schedule)
-
-
 class DemoSource(Source):
     """A Demo source configuration."""
 
     def __init__(
         self,
         name: str,
         credential: DemoCredential,
@@ -303,16 +284,14 @@
         :param lookback_days: How far back in time to start data monitoring
             from. (max 365)
         :param schedule: A 5-digit cron expression specifying how when the source
             polls for new data. Example: '0 0 * * *' to poll daily at midnight.
         """
         super().__init__(name, credential, jtd_schema)
 
-        _warehouse_checks(name, lookback_days, schedule)
-
         self.project = project
         self.dataset = dataset
         self.table = table
         self.cursor_field = cursor_field
         self.lookback_days = lookback_days
         self.schedule = schedule
 
@@ -364,41 +343,46 @@
         warehouse: str | None = None,
         role: str | None = None,
         jtd_schema: JsonTypeDefinition | None = None,
     ):
         """
         Constructor.
 
-        :param database: Name of the snowflake database to connect to .
+        :param database: Name of the snowflake database to connect to (immutable).
         :param db_schema: Name of the schema in the database that contains the
-            table to monitor.
-        :param table: Name of table to monitor.
-        :param warehouse: Snowflake virtual warehouse to use to run queries.
-        :param role: Snowflake role to assume when running queries.
+            table to monitor (immutable).
+        :param table: Name of table to monitor (immutable).
+        :param warehouse: Snowflake virtual warehouse to use to run queries (immutable).
+        :param role: Snowflake role to assume when running queries (immutable).
         :param cursor_field: Timestamp column specifying when each row in the table
-            was added/updated.
+            was added/updated (immutable).
             https://docs.validio.io/docs/data-warehouse#general-considerations
         :param lookback_days: How far back in time to start data ingestion
             from. (max 365)
         :param schedule: A 5-digit cron expression specifying how when the source
             polls for new data. Example: '0 0 * * *' to poll daily at midnight.
         """
         super().__init__(name, credential, jtd_schema)
 
-        _warehouse_checks(name, lookback_days, schedule)
-
         self.database = database
         self.db_schema = db_schema
         self.table = table
         self.warehouse = warehouse
         self.role = role
         self.cursor_field = cursor_field
         self.lookback_days = lookback_days
         self.schedule = schedule
 
+    def __getattr__(self, name):
+        """Getter for field aliases."""
+        # schema is called db_schema
+        if name == "schema":
+            return self.db_schema
+        raise AttributeError
+
     def _immutable_fields(self) -> set[str]:
         return {
             *super()._immutable_fields(),
             *{
                 "db_schema",
                 "database",
                 "table",
@@ -453,23 +437,28 @@
         :param lookback_days: How far back in time to start data ingestion
             from. (max 365)
         :param schedule: A 5-digit cron expression specifying how when the source
             polls for new data. Example: '0 0 * * *' to poll daily at midnight.
         """
         super().__init__(name, credential, jtd_schema)
 
-        _warehouse_checks(name, lookback_days, schedule)
-
         self.db_schema = db_schema
         self.table = table
         self.database = database
         self.cursor_field = cursor_field
         self.lookback_days = lookback_days
         self.schedule = schedule
 
+    def __getattr__(self, name):
+        """Getter for field aliases."""
+        # schema is called db_schema
+        if name == "schema":
+            return self.db_schema
+        raise AttributeError
+
     def _immutable_fields(self) -> set[str]:
         return {
             *super()._immutable_fields(),
             *{
                 "db_schema",
                 "database",
                 "table",
@@ -504,25 +493,25 @@
 class AwsRedshiftSource(PostgresLikeSource):
     """A Redshift source configuration.
 
     https://docs.validio.io/docs/redshift
     """
 
 
-class AwsKinesis(Source):
+class AwsKinesisSource(Source):
     """
     A Kinesis source configuration.
 
     https://docs.validio.io/docs/kinesis
     """
 
     def __init__(
         self,
         name: str,
-        credential: SnowflakeCredential,
+        credential: AwsCredential,
         region: str,
         stream_name: str,
         jtd_schema: JsonTypeDefinition | None = None,
     ):
         """
         Constructor.
 
@@ -546,47 +535,158 @@
     def _api_infer_schema_input(self) -> dict[str, object] | None:
         return {
             "region": self.region,
             "stream_name": self.stream_name,
         }
 
 
+class GcpPubSubBaseSource(Source, ABC):
+    """Base definition for PubSub source configuration."""
+
+    def __init__(
+        self,
+        name: str,
+        credential: GcpCredential,
+        project: str,
+        subscription_id: str,
+        jtd_schema: JsonTypeDefinition | None = None,
+    ):
+        """
+        Constructor.
+
+        :param project: The GCP project where the pubsub topic resides.
+        :param subscription_id: The subscription ID of the subscription
+            to use to consumer messages from the topic.
+            https://cloud.google.com/pubsub/docs/create-subscription
+        """
+        super().__init__(name, credential, jtd_schema)
+
+        self.project = project
+        self.subscription_id = subscription_id
+
+    def _immutable_fields(self) -> set[str]:
+        return {
+            *super()._immutable_fields(),
+            *{
+                "project",
+                "subscription_id",
+            },
+        }
+
+    def _api_infer_schema_input(self) -> dict[str, object] | None:
+        return {
+            "project": self.project,
+            "subscription_id": self.subscription_id,
+        }
+
+
+class GcpPubSubSource(GcpPubSubBaseSource):
+    """A PubSub source configuration. See GcpPubSubBase for properties."""
+
+
+class GcpPubSubLiteSource(GcpPubSubBaseSource):
+    """A PubSubLite source configuration."""
+
+    def __init__(
+        self,
+        name: str,
+        credential: GcpCredential,
+        project: str,
+        location: str,
+        subscription_id: str,
+        jtd_schema: JsonTypeDefinition | None = None,
+    ):
+        """
+        Constructor.
+
+        :param project: The GCP project where the pubsub topic resides.
+        :param location: The region where the pubsub topic resides: e.g
+            e.g. europe-west3-a
+            https://cloud.google.com/pubsub/lite/docs/locations
+        :param subscription_id: The subscription ID of the subscription
+            to use to consumer messages from the stream.
+            https://cloud.google.com/pubsub/docs/create-subscription
+        """
+        super().__init__(
+            name=name,
+            credential=credential,
+            jtd_schema=jtd_schema,
+            project=project,
+            subscription_id=subscription_id,
+        )
+
+        self.location = location
+
+    def _immutable_fields(self) -> set[str]:
+        return {
+            *super()._immutable_fields(),
+            *{"location"},
+        }
+
+    def _api_infer_schema_input(self) -> dict[str, object] | None:
+        return {
+            **(super()._api_infer_schema_input() or {}),
+            "location": self.location,
+        }
+
+
 # Object storages
 
 
 class CsvParserConfig(Diffable):
     """CSV configuration for a source."""
 
     def __init__(
         self,
-        null_marker: str | None,
+        null_marker: str | None = None,
         delimiter: str = ",",
     ):
         """
         Constructor.
 
         :param null_marker: Specifies what character sequence represents
             NULL (defaults to empty string)
         :param delimiter: Delimiter used in the csv file
         """
         self.null_marker = null_marker
         self.delimiter = delimiter
 
+    @staticmethod
+    def _from_any(other: Any) -> "CsvParserConfig":
+        if isinstance(other, CsvParserConfig):
+            return other
+        if isinstance(other, dict):
+            return CsvParserConfig(**other)
+
+        params = {
+            f: getattr(other, f)
+            for f in list(inspect.signature(CsvParserConfig).parameters)
+        }
+        return CsvParserConfig(**params)
+
     def _immutable_fields(self) -> set[str]:
         return set({})
 
     def _mutable_fields(self) -> set[str]:
         return {
             "null_marker",
             "delimiter",
         }
 
     def _nested_objects(self) -> dict[str, Diffable | None]:
         return {}
 
+    def _encode(self) -> dict[str, object]:
+        return json.loads(
+            json.dumps(
+                self.__dict__,
+                default=lambda o: o._encode(),
+            )
+        )
+
 
 class ObjectStorageSource(Source, ABC):
     """
     Base class for object storage source configuration.
 
     https://docs.validio.io/docs/s3
     """
@@ -608,36 +708,36 @@
         :param file_pattern: Glob pattern against file names, used to filter in
             what files are eligible for ingestion.
         :param schedule: A 5-digit cron expression specifying how when the source
             polls for new data. Example: '0 0 * * *' to poll daily at midnight.
         """
         super().__init__(name, credential, jtd_schema)
 
-        _sanity_check_cron_schedule(name, schedule)
-
         self.bucket = bucket
         self.file_pattern = file_pattern
         self.schedule = schedule
         self.csv = (
-            CsvParserConfig(null_marker=None, delimiter=",") if csv is None else csv
+            CsvParserConfig(null_marker=None, delimiter=",")
+            if csv is None
+            else CsvParserConfig._from_any(csv)
         )
 
     def _immutable_fields(self) -> set[str]:
         return {
             *super()._immutable_fields(),
             *{
                 "bucket",
+                "file_pattern",
             },
         }
 
     def _mutable_fields(self) -> set[str]:
         return {
             *super()._mutable_fields(),
             *{
-                "file_pattern",
                 "schedule",
             },
         }
 
     def _nested_objects(self) -> dict[str, Diffable | None]:
         return {
             "csv": self.csv,
@@ -646,14 +746,19 @@
     def _csv_parser_input(self) -> CsvParserInput:
         return CsvParserInput(
             delimiter=self.csv.delimiter,
             # type: ignore[call-arg]
             null_marker=self.csv.null_marker,
         )
 
+    def _api_input_overrides(self) -> dict[str, Any]:
+        return {
+            "csv": self._csv_parser_input(),
+        }
+
 
 class AwsS3Source(ObjectStorageSource):
     """
     An AWS S3 source configuration.
 
     https://docs.validio.io/docs/s3
     """
@@ -692,19 +797,14 @@
         return {
             *super()._immutable_fields(),
             *{
                 "prefix",
             },
         }
 
-    def _api_input_overrides(self) -> dict[str, Any]:
-        return {
-            "csv": self._csv_parser_input(),
-        }
-
     def _api_infer_schema_input(self) -> dict[str, object] | None:
         return {
             "bucket": self.bucket,
             "prefix": self.prefix,
             "file_pattern": self.file_pattern,
             "csv": self._csv_parser_input(),
         }
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/tests/test__diff.py` & `validio_sdk-0.2.0/validio_sdk/resource/tests/test__diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from validio_sdk.resource._errors import ManifestConfigurationError
 from validio_sdk.resource._resource import Resource, ResourceGraph
 from validio_sdk.resource.channels import Channel, SlackChannel
 from validio_sdk.resource.credentials import Credential, DemoCredential
 from validio_sdk.resource.destinations import Destination, GcpBigQueryDestination
 from validio_sdk.resource.filters import NullFilter
-from validio_sdk.resource.notification_rules_v2 import NotificationRuleV2
+from validio_sdk.resource.notification_rules import NotificationRule
 from validio_sdk.resource.segmentations import Segmentation
 from validio_sdk.resource.sources import DemoSource, Source
 from validio_sdk.resource.thresholds import DynamicThreshold
 from validio_sdk.resource.validators import (
     NumericDistributionValidator,
     NumericValidator,
     Reference,
@@ -44,47 +44,47 @@
     credentials: dict[str, Credential] | None = None,
     channels: dict[str, Channel] | None = None,
     destinations: dict[str, Destination] | None = None,
     sources: dict[str, Source] | None = None,
     windows: dict[str, Window] | None = None,
     segmentations: dict[str, Segmentation] | None = None,
     validators: dict[str, Validator] | None = None,
-    notification_rules_v2: dict[str, NotificationRuleV2] | None = None,
+    notification_rules: dict[str, NotificationRule] | None = None,
 ) -> DiffContext:
     return DiffContext(
         credentials=credentials or {},
         channels=channels or {},
         destinations=destinations or {},
         sources=sources or {},
         windows=windows or {},
         segmentations=segmentations or {},
         validators=validators or {},
-        notification_rules_v2=notification_rules_v2 or {},
+        notification_rules=notification_rules or {},
     )
 
 
 def create_resource_updates(
     credentials: dict[str, ResourceUpdate] | None = None,
     channels: dict[str, ResourceUpdate] | None = None,
     destinations: dict[str, ResourceUpdate] | None = None,
     sources: dict[str, ResourceUpdate] | None = None,
     windows: dict[str, ResourceUpdate] | None = None,
     segmentations: dict[str, ResourceUpdate] | None = None,
     validators: dict[str, ResourceUpdate] | None = None,
-    notification_rules_v2: dict[str, ResourceUpdate] | None = None,
+    notification_rules: dict[str, ResourceUpdate] | None = None,
 ) -> ResourceUpdates:
     return ResourceUpdates(
         credentials=credentials or {},
         channels=channels or {},
         destinations=destinations or {},
         sources=sources or {},
         windows=windows or {},
         segmentations=segmentations or {},
         validators=validators or {},
-        notification_rules_v2=notification_rules_v2 or {},
+        notification_rules=notification_rules or {},
     )
 
 
 def create_graph_diff(
     to_create: DiffContext | None = None,
     to_delete: DiffContext | None = None,
     to_update: ResourceUpdates | None = None,
@@ -93,19 +93,15 @@
         to_create=to_create or DiffContext(),
         to_delete=to_delete or DiffContext(),
         to_update=to_update or create_resource_updates(),
     )
 
 
 def collect_resource_config(manifest: Resource, server: Resource) -> ResourceUpdate:
-    all_fields = {
-        *manifest._immutable_fields(),
-        *manifest._mutable_fields(),
-        *manifest._nested_objects().keys(),
-    }
+    all_fields = manifest._all_fields()
     manifest_config = {f: getattr(manifest, f) for f in all_fields}
     server_config = {f: getattr(server, f) for f in all_fields}
     return ResourceUpdate(
         manifest=ResourceWithRepr(resource=manifest, repr=manifest_config),
         server=ResourceWithRepr(resource=server, repr=server_config),
     )
 
@@ -147,17 +143,17 @@
         manifest_seg1,
         NumericMetric.MEAN,
         "b",
     )  # To be created
     manifest_ch1 = SlackChannel("ch1", "app", "web", "tz", manifest_g)
     manifest_ch2 = SlackChannel("ch2", "app", "web", "tz", manifest_g)  # To be created
     manifest_ch3 = SlackChannel("ch3", "app", "web", None, manifest_g)  # To be updated
-    manifest_r1 = NotificationRuleV2("r1", manifest_ch1, [manifest_s1])
-    manifest_r2 = NotificationRuleV2("r2", manifest_ch1, [manifest_s1])  # To be created
-    manifest_r3 = NotificationRuleV2("r3", manifest_ch1, [manifest_s1])  # To be updated
+    manifest_r1 = NotificationRule("r1", manifest_ch1, [manifest_s1])
+    manifest_r2 = NotificationRule("r2", manifest_ch1, [manifest_s1])  # To be created
+    manifest_r3 = NotificationRule("r3", manifest_ch1, [manifest_s1])  # To be updated
 
     server_c1 = DemoCredential("c1", server_g)
     server_d1 = GcpBigQueryDestination("d1", cast(Any, server_c1), "a", "b", "c")
     server_d2 = GcpBigQueryDestination("d2", cast(Any, server_c1), "d", "f", "g")
     server_d4 = GcpBigQueryDestination(
         "d4", cast(Any, server_c1), "x", "y", "z"
     )  # To be deleted
@@ -173,17 +169,17 @@
     server_v1 = NumericValidator("v1", server_w1, server_seg1, NumericMetric.MAX, "a")
     server_v3 = NumericValidator(
         "v3", server_w1, server_seg1, NumericMetric.MAX, "d"
     )  # Delete
     server_ch1 = SlackChannel("ch1", "app", "web", "tz", server_g)
     server_ch3 = SlackChannel("ch3", "app", "web", "tz", server_g)
     server_ch4 = SlackChannel("ch4", "app", "web", "tz", server_g)  # To be deleted
-    server_r1 = NotificationRuleV2("r1", server_ch1, [server_s1])
-    server_r3 = NotificationRuleV2("r3", server_ch1, [])
-    server_r4 = NotificationRuleV2("r4", server_ch1, [server_s1])  # To be deleted
+    server_r1 = NotificationRule("r1", server_ch1, [server_s1])
+    server_r3 = NotificationRule("r3", server_ch1, [])
+    server_r4 = NotificationRule("r4", server_ch1, [server_s1])  # To be deleted
 
     manifest_ctx = create_diff_context(
         credentials={manifest_c1.name: manifest_c1},
         destinations={
             manifest_d1.name: manifest_d1,
             manifest_d2.name: manifest_d2,
             manifest_d3.name: manifest_d3,
@@ -206,15 +202,15 @@
             manifest_v2.name: manifest_v2,
         },
         channels={
             manifest_ch1.name: manifest_ch1,
             manifest_ch2.name: manifest_ch2,
             manifest_ch3.name: manifest_ch3,
         },
-        notification_rules_v2={
+        notification_rules={
             manifest_r1.name: manifest_r1,
             manifest_r2.name: manifest_r2,
             manifest_r3.name: manifest_r3,
         },
     )
 
     server_ctx = create_diff_context(
@@ -242,39 +238,39 @@
             server_v3.name: server_v3,
         },
         channels={
             server_ch1.name: server_ch1,
             server_ch3.name: server_ch3,
             server_ch4.name: server_ch4,
         },
-        notification_rules_v2={
+        notification_rules={
             server_r1.name: server_r1,
             server_r3.name: server_r3,
             server_r4.name: server_r4,
         },
     )
 
     expected = create_graph_diff(
         to_create=DiffContext(
             destinations={manifest_d3.name: manifest_d3},
             sources={manifest_s2.name: manifest_s2},
             segmentations={manifest_seg2.name: manifest_seg2},
             windows={manifest_w2.name: manifest_w2},
             validators={manifest_v2.name: manifest_v2},
             channels={manifest_ch2.name: manifest_ch2},
-            notification_rules_v2={manifest_r2.name: manifest_r2},
+            notification_rules={manifest_r2.name: manifest_r2},
         ),
         to_delete=DiffContext(
             destinations={server_d4.name: server_d4},
             sources={server_s3.name: server_s3},
             segmentations={server_seg3.name: server_seg3},
             windows={server_w4.name: server_w4},
             validators={server_v3.name: server_v3},
             channels={server_ch4.name: server_ch4},
-            notification_rules_v2={server_r4.name: server_r4},
+            notification_rules={server_r4.name: server_r4},
         ),
         to_update=create_resource_updates(
             destinations={
                 server_d2.name: collect_resource_config(
                     manifest_d2,
                     server_d2,
                 )
@@ -287,15 +283,15 @@
             },
             channels={
                 manifest_ch3.name: collect_resource_config(
                     manifest_ch3,
                     server_ch3,
                 ),
             },
-            notification_rules_v2={
+            notification_rules={
                 manifest_r3.name: collect_resource_config(
                     manifest_r3,
                     server_r3,
                 )
             },
         ),
     )
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/tests/test__field_selector.py` & `validio_sdk-0.2.0/validio_sdk/resource/tests/test__field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/tests/test__resource.py` & `validio_sdk-0.2.0/validio_sdk/resource/tests/test__resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     WindowTimeUnit,
 )
 from validio_sdk.resource import (
     FieldSelector,
     channels,
     credentials,
     destinations,
-    notification_rules_v2,
+    notification_rules,
     segmentations,
     sources,
     validators,
     windows,
 )
 from validio_sdk.resource._field_selector import FieldDataType
 from validio_sdk.resource._resource import ResourceGraph
@@ -129,21 +129,21 @@
         "null_count",
         window=w1,
         segmentation=seg1,
         metric=VolumeMetric.COUNT,
         filter=NullFilter(field=FieldSelector(data_type=FieldDataType.BOOLEAN)),
     )
 
-    notification_rules_v2.NotificationRuleV2(
+    notification_rules.NotificationRule(
         name="r1",
         channel=ch1,
         sources=[s1, s3],
         notification_typenames=["SchemaChangeNotification"],
     )
-    notification_rules_v2.NotificationRuleV2(
+    notification_rules.NotificationRule(
         name="r2",
         channel=ch2,
     )
 
     expected_config = """
 {
   "sub_graphs": {
@@ -409,17 +409,17 @@
           "name": "ch1",
           "application_link_url": "foo",
           "webhook_url": "bar",
           "timezone": "utc"
         },
         "_children": {
           "_node_type": "_children",
-          "NotificationRuleV2": {
+          "NotificationRule": {
             "r1": {
-              "_node_type": "NotificationRuleV2",
+              "_node_type": "NotificationRule",
               "config_field": {
                 "name": "r1",
                 "source_names": [
                   "s1",
                   "s3"
                 ],
                 "notification_typenames": [
@@ -436,17 +436,17 @@
           "name": "ch2",
           "application_link_url": "foo",
           "webhook_url": "bar",
           "auth_header": "secretz"
         },
         "_children": {
           "_node_type": "_children",
-          "NotificationRuleV2": {
+          "NotificationRule": {
             "r2": {
-              "_node_type": "NotificationRuleV2",
+              "_node_type": "NotificationRule",
               "config_field": {
                 "name": "r2",
                 "source_names": [],
                 "notification_typenames": []
               }
             }
           }
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/thresholds.py` & `validio_sdk-0.2.0/validio_sdk/resource/thresholds.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/validators.py` & `validio_sdk-0.2.0/validio_sdk/resource/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,24 +301,35 @@
             "threshold": self.threshold,
         }
 
     def _immutable_fields(self) -> set[str]:
         fields = {
             "window_name",
             "segmentation_name",
-            "metric",
-            "initialize_with_backfill",
         }
+
+        if not isinstance(self, FreshnessValidator):
+            fields.add("metric")
+
         if hasattr(self, "destination_name"):
             fields.add("destination_name")
         return fields
 
     def _mutable_fields(self) -> set[str]:
         return set({})
 
+    def _ignored_fields(self) -> set[str]:
+        return {
+            # initialize_with_backfill is treated as a hint on the backend.
+            # So what the client sets is not necessarily what the server will
+            # return back. The field is also unused after validator creation
+            # so that it doesn't matter to diff it. So we ignore it always.
+            "initialize_with_backfill",
+        }
+
     def resource_class_name(self) -> str:
         """Returns the base class name."""
         return "Validator"
 
     def _source_config_create_input(
         self, ctx: "DiffContext"
     ) -> SourceConfigCreateInput:
```

### Comparing `validio_sdk-0.1.0/validio_sdk/resource/windows.py` & `validio_sdk-0.2.0/validio_sdk/resource/windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/scalars.py` & `validio_sdk-0.2.0/validio_sdk/scalars.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 """Scalars used in our GraphQL schemas."""
 
 from dataclasses import fields
 from enum import Enum
 from typing import Union
 
-from validio_sdk import EnumFilter, NullFilter, StringFilter, ThresholdFilter
+from validio_sdk import (
+    BooleanFilter,
+    EnumFilter,
+    NullFilter,
+    StringFilter,
+    ThresholdFilter,
+)
 
 ValidioId = str
 CredentialId = ValidioId
 DestinationId = ValidioId
 SegmentationId = ValidioId
 SourceId = ValidioId
 ValidatorId = ValidioId
 WindowId = ValidioId
 
 CronExpression = str
 
 # Raw JSON, used for filters
-JsonFilterExpression = Union[EnumFilter, NullFilter, StringFilter, ThresholdFilter]
+JsonFilterExpression = Union[
+    BooleanFilter, EnumFilter, NullFilter, StringFilter, ThresholdFilter
+]
 
 # JTD schema definition
 JsonTypeDefinition = dict
 
 # A JSONPath expression specifying a field within a datapoint.
 # Examples:
 #   user.address.street for nested structures.
```

### Comparing `validio_sdk-0.1.0/validio_sdk/util.py` & `validio_sdk-0.2.0/validio_sdk/util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.1.0/validio_sdk/validio_client.py` & `validio_sdk-0.2.0/validio_sdk/validio_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,18 +41,15 @@
         :returns: A `ValidioAPIClient` object
         """
         if validio_config is None:
             validio_config = Config().read()
 
         base_url = validio_config.endpoint
         graphql_endpoint = f"{base_url}/graphql"
-        base_headers = {
-            "user-agent": f"validio-sdk@{validio_sdk.metadata.version()}",
-            "Content-type": "application/json",
-        }
+        base_headers = {"user-agent": f"validio-sdk@{validio_sdk.metadata.version()}"}
         http_client = httpx.AsyncClient(
             headers=base_headers,
             auth=_add_api_token_auth_header(validio_config),
             timeout=30,
             event_hooks={"response": [_handle_unauthorized]},
         )
```

