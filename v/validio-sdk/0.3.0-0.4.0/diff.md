# Comparing `tmp/validio_sdk-0.3.0.tar.gz` & `tmp/validio_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_sdk-0.3.0.tar", max compression
+gzip compressed data, was "validio_sdk-0.4.0.tar", max compression
```

## Comparing `validio_sdk-0.3.0.tar` & `validio_sdk-0.4.0.tar`

### file list

```diff
@@ -1,202 +1,202 @@
--rw-r--r--   0        0        0    11340 2023-06-14 12:04:50.154055 validio_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0      302 2023-06-14 12:04:50.154055 validio_sdk-0.3.0/README_PUBLIC.md
--rw-r--r--   0        0        0     4665 2023-06-14 12:05:00.925900 validio_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      588 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/code/__init__.py
--rw-r--r--   0        0        0      551 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/code/apply.py
--rw-r--r--   0        0        0     4767 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/code/plan.py
--rw-r--r--   0        0        0     1565 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/code/scaffold.py
--rw-r--r--   0        0        0      305 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/code/settings.py
--rw-r--r--   0        0        0     5891 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/config.py
--rw-r--r--   0        0        0   245071 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/__init__.py
--rw-r--r--   0        0        0      573 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/apply_validator_recommendation.py
--rw-r--r--   0        0        0     7319 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      526 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/aws_credential_secret_changed.py
--rw-r--r--   0        0        0      613 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
--rw-r--r--   0        0        0      614 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/backfill_source.py
--rw-r--r--   0        0        0     1899 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/base_model.py
--rw-r--r--   0        0        0   584680 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/client.py
--rw-r--r--   0        0        0      445 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_aws_credential.py
--rw-r--r--   0        0        0      528 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py
--rw-r--r--   0        0        0      468 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_aws_kinesis_source.py
--rw-r--r--   0        0        0      526 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_aws_redshift_credential.py
--rw-r--r--   0        0        0      480 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_aws_redshift_source.py
--rw-r--r--   0        0        0      418 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_aws_s3_source.py
--rw-r--r--   0        0        0      843 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      823 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      455 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_demo_credential.py
--rw-r--r--   0        0        0      407 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_demo_source.py
--rw-r--r--   0        0        0      407 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_file_window.py
--rw-r--r--   0        0        0      468 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_fixed_batch_window.py
--rw-r--r--   0        0        0      702 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      682 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      539 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py
--rw-r--r--   0        0        0      481 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_gcp_big_query_source.py
--rw-r--r--   0        0        0      445 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_gcp_credential.py
--rw-r--r--   0        0        0      500 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      459 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      468 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_gcp_storage_source.py
--rw-r--r--   0        0        0      487 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_notification_rule.py
--rw-r--r--   0        0        0      753 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      803 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      783 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      823 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      682 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      662 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      702 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      516 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_postgre_sql_credential.py
--rw-r--r--   0        0        0      468 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_postgre_sql_source.py
--rw-r--r--   0        0        0      733 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      713 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      753 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      753 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      528 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_saml_identity_provider.py
--rw-r--r--   0        0        0      438 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_segmentation.py
--rw-r--r--   0        0        0      477 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_sessionized_window.py
--rw-r--r--   0        0        0      429 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_slack_channel.py
--rw-r--r--   0        0        0      505 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_snowflake_credential.py
--rw-r--r--   0        0        0      517 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_snowflake_destination.py
--rw-r--r--   0        0        0      457 2023-06-14 12:04:50.158055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_snowflake_source.py
--rw-r--r--   0        0        0      447 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_tumbling_window.py
--rw-r--r--   0        0        0      328 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_user.py
--rw-r--r--   0        0        0      672 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      652 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      449 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/create_webhook_channel.py
--rw-r--r--   0        0        0      364 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_channel.py
--rw-r--r--   0        0        0      614 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_credential.py
--rw-r--r--   0        0        0      622 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_credentials.py
--rw-r--r--   0        0        0      630 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_destination.py
--rw-r--r--   0        0        0      638 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_destinations.py
--rw-r--r--   0        0        0      376 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_identity.py
--rw-r--r--   0        0        0      487 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_identity_provider.py
--rw-r--r--   0        0        0      487 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_notification_rule.py
--rw-r--r--   0        0        0      646 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_segmentation.py
--rw-r--r--   0        0        0      536 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_source.py
--rw-r--r--   0        0        0      544 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_sources.py
--rw-r--r--   0        0        0      328 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_user.py
--rw-r--r--   0        0        0      606 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_validators.py
--rw-r--r--   0        0        0      536 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_window.py
--rw-r--r--   0        0        0      544 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/delete_windows.py
--rw-r--r--   0        0        0      589 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py
--rw-r--r--   0        0        0     3065 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/enums.py
--rw-r--r--   0        0        0     2314 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/exceptions.py
--rw-r--r--   0        0        0   175196 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/fragments.py
--rw-r--r--   0        0        0      526 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py
--rw-r--r--   0        0        0     2896 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_channel_by_resource_name.py
--rw-r--r--   0        0        0     2427 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_channels.py
--rw-r--r--   0        0        0     4965 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_credential_by_resource_name.py
--rw-r--r--   0        0        0     5997 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_destination_by_resource_name.py
--rw-r--r--   0        0        0     2218 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
--rw-r--r--   0        0        0     2033 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_identity_providers.py
--rw-r--r--   0        0        0     5368 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_incidents.py
--rw-r--r--   0        0        0      627 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_notification_rules.py
--rw-r--r--   0        0        0      460 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_segment_incidents.py
--rw-r--r--   0        0        0      357 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_segmentation.py
--rw-r--r--   0        0        0      572 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
--rw-r--r--   0        0        0    20258 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_source.py
--rw-r--r--   0        0        0    24833 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_source_by_resource_name.py
--rw-r--r--   0        0        0     1727 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_source_incidents.py
--rw-r--r--   0        0        0    21532 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_source_recommended_validators.py
--rw-r--r--   0        0        0      476 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_user_by_resource_name.py
--rw-r--r--   0        0        0      300 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_users.py
--rw-r--r--   0        0        0    40168 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator.py
--rw-r--r--   0        0        0    48254 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator_incidents.py
--rw-r--r--   0        0        0      551 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator_segment_incidents.py
--rw-r--r--   0        0        0     3986 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator_segment_metrics.py
--rw-r--r--   0        0        0     5711 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/get_window_by_resource_name.py
--rw-r--r--   0        0        0      290 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
--rw-r--r--   0        0        0      308 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_aws_redshift_schema.py
--rw-r--r--   0        0        0      270 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_aws_s3_schema.py
--rw-r--r--   0        0        0      265 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_demo_schema.py
--rw-r--r--   0        0        0      309 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
--rw-r--r--   0        0        0      318 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
--rw-r--r--   0        0        0      287 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
--rw-r--r--   0        0        0      290 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_gcp_storage_schema.py
--rw-r--r--   0        0        0      290 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_postgre_sql_schema.py
--rw-r--r--   0        0        0      285 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/infer_snowflake_schema.py
--rw-r--r--   0        0        0    34411 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/input_types.py
--rw-r--r--   0        0        0     4316 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/list_credentials.py
--rw-r--r--   0        0        0     5202 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/list_destinations.py
--rw-r--r--   0        0        0      457 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/list_segmentations.py
--rw-r--r--   0        0        0    21364 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/list_sources.py
--rw-r--r--   0        0        0    42237 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/list_validators.py
--rw-r--r--   0        0        0     4976 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/list_windows.py
--rw-r--r--   0        0        0      603 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
--rw-r--r--   0        0        0      594 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/scalars.py
--rw-r--r--   0        0        0      288 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/segments.py
--rw-r--r--   0        0        0      499 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/segments_by_resource_name.py
--rw-r--r--   0        0        0      592 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
--rw-r--r--   0        0        0      566 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/start_source.py
--rw-r--r--   0        0        0      550 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/stop_source.py
--rw-r--r--   0        0        0      441 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_aws_credential.py
--rw-r--r--   0        0        0      524 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py
--rw-r--r--   0        0        0      464 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_aws_kinesis_source.py
--rw-r--r--   0        0        0      522 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_aws_redshift_credential.py
--rw-r--r--   0        0        0      476 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_aws_redshift_source.py
--rw-r--r--   0        0        0      414 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_aws_s3_source.py
--rw-r--r--   0        0        0      636 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py
--rw-r--r--   0        0        0      464 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_fixed_batch_window.py
--rw-r--r--   0        0        0      491 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_freshness_validator.py
--rw-r--r--   0        0        0      535 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py
--rw-r--r--   0        0        0      477 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_gcp_big_query_source.py
--rw-r--r--   0        0        0      441 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_gcp_credential.py
--rw-r--r--   0        0        0      496 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      455 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      464 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_gcp_storage_source.py
--rw-r--r--   0        0        0      534 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_local_identity_provider.py
--rw-r--r--   0        0        0      483 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_notification_rule.py
--rw-r--r--   0        0        0      540 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
--rw-r--r--   0        0        0      596 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_numeric_validator.py
--rw-r--r--   0        0        0      512 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_postgre_sql_credential.py
--rw-r--r--   0        0        0      464 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_postgre_sql_source.py
--rw-r--r--   0        0        0      520 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_relative_time_validator.py
--rw-r--r--   0        0        0      540 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_relative_volume_validator.py
--rw-r--r--   0        0        0      524 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_saml_identity_provider.py
--rw-r--r--   0        0        0      473 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_sessionized_window.py
--rw-r--r--   0        0        0      425 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_slack_channel.py
--rw-r--r--   0        0        0      501 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_snowflake_credential.py
--rw-r--r--   0        0        0      513 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_snowflake_destination.py
--rw-r--r--   0        0        0      453 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_snowflake_source.py
--rw-r--r--   0        0        0      443 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_tumbling_window.py
--rw-r--r--   0        0        0      324 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_user.py
--rw-r--r--   0        0        0    57176 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0    56052 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0    58306 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      459 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_volume_validator.py
--rw-r--r--   0        0        0      445 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/graphql_client/update_webhook_channel.py
--rw-r--r--   0        0        0      265 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/metadata.py
--rw-r--r--   0        0        0        0 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/py.typed
--rw-r--r--   0        0        0      135 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/__init__.py
--rw-r--r--   0        0        0    21078 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_diff.py
--rw-r--r--   0        0        0     1208 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_diff_util.py
--rw-r--r--   0        0        0     1657 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_diffable.py
--rw-r--r--   0        0        0     1579 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_errors.py
--rw-r--r--   0        0        0     4002 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_field_selector.py
--rw-r--r--   0        0        0    17790 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_resource.py
--rw-r--r--   0        0        0     1355 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_resource_graph.py
--rw-r--r--   0        0        0     5366 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_serde.py
--rw-r--r--   0        0        0    21047 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_server_resources.py
--rw-r--r--   0        0        0      844 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/_util.py
--rw-r--r--   0        0        0     5027 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/channels.py
--rw-r--r--   0        0        0     7692 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/credentials.py
--rw-r--r--   0        0        0     5398 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/destinations.py
--rw-r--r--   0        0        0     6255 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/filters.py
--rw-r--r--   0        0        0     4846 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/notification_rules.py
--rw-r--r--   0        0        0     2040 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/segmentations.py
--rw-r--r--   0        0        0    25856 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/sources.py
--rw-r--r--   0        0        0        0 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/tests/__init__.py
--rw-r--r--   0        0        0    15408 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/tests/test__diff.py
--rw-r--r--   0        0        0     1905 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/tests/test__field_selector.py
--rw-r--r--   0        0        0    16357 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/tests/test__resource.py
--rw-r--r--   0        0        0     5638 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/thresholds.py
--rw-r--r--   0        0        0    32563 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/validators.py
--rw-r--r--   0        0        0     5995 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/resource/windows.py
--rw-r--r--   0        0        0     1377 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/scalars.py
--rw-r--r--   0        0        0     1813 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/util.py
--rw-r--r--   0        0        0     2382 2023-06-14 12:04:50.162055 validio_sdk-0.3.0/validio_sdk/validio_client.py
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 validio_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-06-14 13:46:50.060746 validio_sdk-0.4.0/LICENSE
+-rw-r--r--   0        0        0      308 2023-06-14 13:46:50.060746 validio_sdk-0.4.0/README_PUBLIC.md
+-rw-r--r--   0        0        0     4847 2023-06-14 13:47:01.312598 validio_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-06-14 13:46:50.064746 validio_sdk-0.4.0/validio_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:46:50.064746 validio_sdk-0.4.0/validio_sdk/code/__init__.py
+-rw-r--r--   0        0        0      551 2023-06-14 13:46:50.064746 validio_sdk-0.4.0/validio_sdk/code/apply.py
+-rw-r--r--   0        0        0     4767 2023-06-14 13:46:50.064746 validio_sdk-0.4.0/validio_sdk/code/plan.py
+-rw-r--r--   0        0        0     1565 2023-06-14 13:46:50.064746 validio_sdk-0.4.0/validio_sdk/code/scaffold.py
+-rw-r--r--   0        0        0      305 2023-06-14 13:46:50.064746 validio_sdk-0.4.0/validio_sdk/code/settings.py
+-rw-r--r--   0        0        0     5891 2023-06-14 13:46:50.064746 validio_sdk-0.4.0/validio_sdk/config.py
+-rw-r--r--   0        0        0   245071 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/__init__.py
+-rw-r--r--   0        0        0      573 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/apply_validator_recommendation.py
+-rw-r--r--   0        0        0     7319 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      526 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/aws_credential_secret_changed.py
+-rw-r--r--   0        0        0      613 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
+-rw-r--r--   0        0        0      614 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/backfill_source.py
+-rw-r--r--   0        0        0     1899 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/base_model.py
+-rw-r--r--   0        0        0   584680 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/client.py
+-rw-r--r--   0        0        0      445 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_aws_credential.py
+-rw-r--r--   0        0        0      528 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      468 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_aws_kinesis_source.py
+-rw-r--r--   0        0        0      526 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_aws_redshift_credential.py
+-rw-r--r--   0        0        0      480 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_aws_redshift_source.py
+-rw-r--r--   0        0        0      418 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_aws_s3_source.py
+-rw-r--r--   0        0        0      843 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      823 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      455 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_demo_credential.py
+-rw-r--r--   0        0        0      407 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_demo_source.py
+-rw-r--r--   0        0        0      407 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_file_window.py
+-rw-r--r--   0        0        0      468 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_fixed_batch_window.py
+-rw-r--r--   0        0        0      702 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      682 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      539 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      481 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_gcp_big_query_source.py
+-rw-r--r--   0        0        0      445 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_gcp_credential.py
+-rw-r--r--   0        0        0      500 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      459 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      468 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_gcp_storage_source.py
+-rw-r--r--   0        0        0      487 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_notification_rule.py
+-rw-r--r--   0        0        0      753 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      803 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      783 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      823 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      682 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      662 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      702 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      516 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_postgre_sql_credential.py
+-rw-r--r--   0        0        0      468 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_postgre_sql_source.py
+-rw-r--r--   0        0        0      733 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      713 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      753 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      753 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      528 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_saml_identity_provider.py
+-rw-r--r--   0        0        0      438 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_segmentation.py
+-rw-r--r--   0        0        0      477 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_sessionized_window.py
+-rw-r--r--   0        0        0      429 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_slack_channel.py
+-rw-r--r--   0        0        0      505 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_snowflake_credential.py
+-rw-r--r--   0        0        0      517 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_snowflake_destination.py
+-rw-r--r--   0        0        0      457 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_snowflake_source.py
+-rw-r--r--   0        0        0      447 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_tumbling_window.py
+-rw-r--r--   0        0        0      328 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_user.py
+-rw-r--r--   0        0        0      672 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      652 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      449 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/create_webhook_channel.py
+-rw-r--r--   0        0        0      364 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_channel.py
+-rw-r--r--   0        0        0      614 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_credential.py
+-rw-r--r--   0        0        0      622 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_credentials.py
+-rw-r--r--   0        0        0      630 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_destination.py
+-rw-r--r--   0        0        0      638 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_destinations.py
+-rw-r--r--   0        0        0      376 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_identity.py
+-rw-r--r--   0        0        0      487 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_identity_provider.py
+-rw-r--r--   0        0        0      487 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_notification_rule.py
+-rw-r--r--   0        0        0      646 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_segmentation.py
+-rw-r--r--   0        0        0      536 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_source.py
+-rw-r--r--   0        0        0      544 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_sources.py
+-rw-r--r--   0        0        0      328 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_user.py
+-rw-r--r--   0        0        0      606 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_validators.py
+-rw-r--r--   0        0        0      536 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_window.py
+-rw-r--r--   0        0        0      544 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/delete_windows.py
+-rw-r--r--   0        0        0      589 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py
+-rw-r--r--   0        0        0     3065 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/enums.py
+-rw-r--r--   0        0        0     2314 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/exceptions.py
+-rw-r--r--   0        0        0   175196 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/fragments.py
+-rw-r--r--   0        0        0      526 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py
+-rw-r--r--   0        0        0     2896 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_channel_by_resource_name.py
+-rw-r--r--   0        0        0     2427 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_channels.py
+-rw-r--r--   0        0        0     4965 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_credential_by_resource_name.py
+-rw-r--r--   0        0        0     5997 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_destination_by_resource_name.py
+-rw-r--r--   0        0        0     2218 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
+-rw-r--r--   0        0        0     2033 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_identity_providers.py
+-rw-r--r--   0        0        0     5368 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_incidents.py
+-rw-r--r--   0        0        0      627 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_notification_rules.py
+-rw-r--r--   0        0        0      460 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_segment_incidents.py
+-rw-r--r--   0        0        0      357 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_segmentation.py
+-rw-r--r--   0        0        0      572 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
+-rw-r--r--   0        0        0    20258 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_source.py
+-rw-r--r--   0        0        0    24833 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_source_by_resource_name.py
+-rw-r--r--   0        0        0     1727 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_source_incidents.py
+-rw-r--r--   0        0        0    21532 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_source_recommended_validators.py
+-rw-r--r--   0        0        0      476 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_user_by_resource_name.py
+-rw-r--r--   0        0        0      300 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_users.py
+-rw-r--r--   0        0        0    40168 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator.py
+-rw-r--r--   0        0        0    48254 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator_incidents.py
+-rw-r--r--   0        0        0      551 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator_segment_incidents.py
+-rw-r--r--   0        0        0     3986 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator_segment_metrics.py
+-rw-r--r--   0        0        0     5711 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/get_window_by_resource_name.py
+-rw-r--r--   0        0        0      290 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
+-rw-r--r--   0        0        0      308 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_aws_redshift_schema.py
+-rw-r--r--   0        0        0      270 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_aws_s3_schema.py
+-rw-r--r--   0        0        0      265 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_demo_schema.py
+-rw-r--r--   0        0        0      309 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
+-rw-r--r--   0        0        0      318 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
+-rw-r--r--   0        0        0      287 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
+-rw-r--r--   0        0        0      290 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_gcp_storage_schema.py
+-rw-r--r--   0        0        0      290 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_postgre_sql_schema.py
+-rw-r--r--   0        0        0      285 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/infer_snowflake_schema.py
+-rw-r--r--   0        0        0    34411 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/input_types.py
+-rw-r--r--   0        0        0     4316 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/list_credentials.py
+-rw-r--r--   0        0        0     5202 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/list_destinations.py
+-rw-r--r--   0        0        0      457 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/list_segmentations.py
+-rw-r--r--   0        0        0    21364 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/list_sources.py
+-rw-r--r--   0        0        0    42237 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/list_validators.py
+-rw-r--r--   0        0        0     4976 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/list_windows.py
+-rw-r--r--   0        0        0      603 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
+-rw-r--r--   0        0        0      594 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/scalars.py
+-rw-r--r--   0        0        0      288 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/segments.py
+-rw-r--r--   0        0        0      499 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/segments_by_resource_name.py
+-rw-r--r--   0        0        0      592 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
+-rw-r--r--   0        0        0      566 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/start_source.py
+-rw-r--r--   0        0        0      550 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/stop_source.py
+-rw-r--r--   0        0        0      441 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_aws_credential.py
+-rw-r--r--   0        0        0      524 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      464 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_aws_kinesis_source.py
+-rw-r--r--   0        0        0      522 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_aws_redshift_credential.py
+-rw-r--r--   0        0        0      476 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_aws_redshift_source.py
+-rw-r--r--   0        0        0      414 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_aws_s3_source.py
+-rw-r--r--   0        0        0      636 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py
+-rw-r--r--   0        0        0      464 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_fixed_batch_window.py
+-rw-r--r--   0        0        0      491 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_freshness_validator.py
+-rw-r--r--   0        0        0      535 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      477 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_gcp_big_query_source.py
+-rw-r--r--   0        0        0      441 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_gcp_credential.py
+-rw-r--r--   0        0        0      496 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      455 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      464 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_gcp_storage_source.py
+-rw-r--r--   0        0        0      534 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_local_identity_provider.py
+-rw-r--r--   0        0        0      483 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_notification_rule.py
+-rw-r--r--   0        0        0      540 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
+-rw-r--r--   0        0        0      596 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_numeric_validator.py
+-rw-r--r--   0        0        0      512 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_postgre_sql_credential.py
+-rw-r--r--   0        0        0      464 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_postgre_sql_source.py
+-rw-r--r--   0        0        0      520 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_relative_time_validator.py
+-rw-r--r--   0        0        0      540 2023-06-14 13:46:50.068746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_relative_volume_validator.py
+-rw-r--r--   0        0        0      524 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_saml_identity_provider.py
+-rw-r--r--   0        0        0      473 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_sessionized_window.py
+-rw-r--r--   0        0        0      425 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_slack_channel.py
+-rw-r--r--   0        0        0      501 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_snowflake_credential.py
+-rw-r--r--   0        0        0      513 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_snowflake_destination.py
+-rw-r--r--   0        0        0      453 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_snowflake_source.py
+-rw-r--r--   0        0        0      443 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_tumbling_window.py
+-rw-r--r--   0        0        0      324 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_user.py
+-rw-r--r--   0        0        0    57176 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0    56052 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0    58306 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      459 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_volume_validator.py
+-rw-r--r--   0        0        0      445 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/graphql_client/update_webhook_channel.py
+-rw-r--r--   0        0        0      265 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/metadata.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/py.typed
+-rw-r--r--   0        0        0      135 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/__init__.py
+-rw-r--r--   0        0        0    21078 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_diff.py
+-rw-r--r--   0        0        0     1208 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_diff_util.py
+-rw-r--r--   0        0        0     1657 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_diffable.py
+-rw-r--r--   0        0        0     1579 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_errors.py
+-rw-r--r--   0        0        0     4002 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_field_selector.py
+-rw-r--r--   0        0        0    17790 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_resource.py
+-rw-r--r--   0        0        0     1355 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_resource_graph.py
+-rw-r--r--   0        0        0     5366 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_serde.py
+-rw-r--r--   0        0        0    21047 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_server_resources.py
+-rw-r--r--   0        0        0      847 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/_util.py
+-rw-r--r--   0        0        0     5027 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/channels.py
+-rw-r--r--   0        0        0     7692 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/credentials.py
+-rw-r--r--   0        0        0     5398 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/destinations.py
+-rw-r--r--   0        0        0     6255 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/filters.py
+-rw-r--r--   0        0        0     4846 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/notification_rules.py
+-rw-r--r--   0        0        0     2040 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/segmentations.py
+-rw-r--r--   0        0        0    25856 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/sources.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/tests/__init__.py
+-rw-r--r--   0        0        0    15408 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/tests/test__diff.py
+-rw-r--r--   0        0        0     1905 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/tests/test__field_selector.py
+-rw-r--r--   0        0        0    16357 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/tests/test__resource.py
+-rw-r--r--   0        0        0     5638 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/thresholds.py
+-rw-r--r--   0        0        0    32563 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/validators.py
+-rw-r--r--   0        0        0     5995 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/resource/windows.py
+-rw-r--r--   0        0        0     1377 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/scalars.py
+-rw-r--r--   0        0        0     1813 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/util.py
+-rw-r--r--   0        0        0     2382 2023-06-14 13:46:50.072746 validio_sdk-0.4.0/validio_sdk/validio_client.py
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 validio_sdk-0.4.0/PKG-INFO
```

### Comparing `validio_sdk-0.3.0/LICENSE` & `validio_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/pyproject.toml` & `validio_sdk-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [tool.poetry]
 name = "validio-sdk"
-version = "0.3.0"
+# This version does not represent the released version or any tag. For each
+# release we automatically bump this before building and publishing so this
+# should be kept at 0.0.1dev1
+version = "0.4.0"
 description = "SDK to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
 packages = [{ include = "validio_sdk" }]
 exclude = ["./validio_sdk/bin/pull_graphql.py", "./schema/**", "./plugins/**", "./examples/**"]
```

### Comparing `validio_sdk-0.3.0/validio_sdk/__init__.py` & `validio_sdk-0.4.0/validio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/code/apply.py` & `validio_sdk-0.4.0/validio_sdk/code/apply.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/code/plan.py` & `validio_sdk-0.4.0/validio_sdk/code/plan.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/code/scaffold.py` & `validio_sdk-0.4.0/validio_sdk/code/scaffold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/config.py` & `validio_sdk-0.4.0/validio_sdk/config.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/__init__.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/apply_validator_recommendation.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/apply_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/async_base_client.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/aws_credential_secret_changed.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/aws_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/backfill_source.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/backfill_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/base_model.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/client.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_aws_redshift_credential.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_postgre_sql_credential.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_saml_identity_provider.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_snowflake_destination.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_credential.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_credentials.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_destination.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_destinations.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_segmentation.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_segmentation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_source.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_sources.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_validators.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_window.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_window.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/delete_windows.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/delete_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/enums.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/enums.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/exceptions.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/fragments.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/fragments.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_channel_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_channel_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_channels.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_credential_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_credential_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_destination_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_destination_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_identity_providers.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_identity_providers.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_incidents.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_source.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_source_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_source_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_source_incidents.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_source_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_source_recommended_validators.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_source_recommended_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator_segment_incidents.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator_segment_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_validator_segment_metrics.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_validator_segment_metrics.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/get_window_by_resource_name.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/get_window_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/input_types.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/input_types.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/list_credentials.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/list_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/list_destinations.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/list_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/list_sources.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/list_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/list_validators.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/list_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/list_windows.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/list_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/scalars.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/start_source.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/start_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/stop_source.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/stop_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_aws_redshift_credential.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_local_identity_provider.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_local_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_postgre_sql_credential.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_relative_time_validator.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_relative_time_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_relative_volume_validator.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_relative_volume_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_saml_identity_provider.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_snowflake_destination.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py` & `validio_sdk-0.4.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_diff.py` & `validio_sdk-0.4.0/validio_sdk/resource/_diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_diff_util.py` & `validio_sdk-0.4.0/validio_sdk/resource/_diff_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from validio_sdk.resource.segmentations import Segmentation
 from validio_sdk.resource.sources import Source
 from validio_sdk.resource.windows import Window
 
 
 def must_find_source(ctx: DiffContext, name: str) -> Source:
     if name not in ctx.sources:
-        raise RuntimeError(f"could not find source '{name}' in server resource list")
+        raise RuntimeError(f"could not find Source '{name}' in server resource list")
     return ctx.sources[name]
 
 
 def must_find_window(ctx: DiffContext, name: str) -> Window:
     if name not in ctx.windows:
-        raise RuntimeError(f"could not find window '{name}' in server resource list")
+        raise RuntimeError(f"could not find Window '{name}' in server resource list")
     return ctx.windows[name]
 
 
 def must_find_segmentation(ctx: DiffContext, name: str) -> Segmentation:
     if name not in ctx.segmentations:
         raise RuntimeError(
-            f"could not find segmentation '{name}' in server resource list"
+            f"could not find Segmentation '{name}' in server resource list"
         )
     return ctx.segmentations[name]
 
 
 def must_find_destination(ctx: DiffContext, name: str) -> Destination:
     if name not in ctx.destinations:
         raise RuntimeError(
-            f"could not find destination '{name}' in server resource list"
+            f"could not find Destination '{name}' in server resource list"
         )
     return ctx.destinations[name]
```

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_diffable.py` & `validio_sdk-0.4.0/validio_sdk/resource/_diffable.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_errors.py` & `validio_sdk-0.4.0/validio_sdk/resource/_errors.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_field_selector.py` & `validio_sdk-0.4.0/validio_sdk/resource/_field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_resource.py` & `validio_sdk-0.4.0/validio_sdk/resource/_resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_resource_graph.py` & `validio_sdk-0.4.0/validio_sdk/resource/_resource_graph.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_serde.py` & `validio_sdk-0.4.0/validio_sdk/resource/_serde.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_server_resources.py` & `validio_sdk-0.4.0/validio_sdk/resource/_server_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,15 @@
         for c in WINDOW_CLASSES:
             if w.typename__ == c.__name__:
                 cls = c
                 break
 
         if cls is None:
             raise RuntimeError(
-                f"missing implementation for window type {w.__class__.__name__}"
+                f"missing implementation for Window type {w.__class__.__name__}"
             )
 
         window = cls(
             **{
                 **(w.config.__dict__ if hasattr(w, "config") else {}),  # type:ignore
                 "name": name,
                 "source": must_find_source(ctx, w.source.resource_name),
@@ -377,15 +377,15 @@
             for c in VALIDATOR_CLASSES:
                 if v.typename__ == c.__name__:
                     cls = c
                     break
 
             if cls is None:
                 raise RuntimeError(
-                    f"missing implementation for validator type {v.typename__}"
+                    f"missing implementation for Validator type {v.typename__}"
                 )
 
             window = must_find_window(ctx, v.source_config.window.resource_name)
             segmentation = must_find_segmentation(
                 ctx, v.source_config.segmentation.resource_name
             )
             maybe_destination = (
```

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/_util.py` & `validio_sdk-0.4.0/validio_sdk/resource/_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     show_secrets: bool,
 ) -> Exception:
     if show_secrets:
         return e
     raise RuntimeError(
         f"API error: status code {e.status_code}: The error message has been "
         "suppressed because it potentially contains sensitive information; "
-        "If you would like to view the error message, re-run with --show-secrets"
+        "If you would like to view the error message, run again with --show-secrets"
     )
```

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/channels.py` & `validio_sdk-0.4.0/validio_sdk/resource/channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/credentials.py` & `validio_sdk-0.4.0/validio_sdk/resource/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/destinations.py` & `validio_sdk-0.4.0/validio_sdk/resource/destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/filters.py` & `validio_sdk-0.4.0/validio_sdk/resource/filters.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/notification_rules.py` & `validio_sdk-0.4.0/validio_sdk/resource/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/segmentations.py` & `validio_sdk-0.4.0/validio_sdk/resource/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/sources.py` & `validio_sdk-0.4.0/validio_sdk/resource/sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/tests/test__diff.py` & `validio_sdk-0.4.0/validio_sdk/resource/tests/test__diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/tests/test__field_selector.py` & `validio_sdk-0.4.0/validio_sdk/resource/tests/test__field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/tests/test__resource.py` & `validio_sdk-0.4.0/validio_sdk/resource/tests/test__resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/thresholds.py` & `validio_sdk-0.4.0/validio_sdk/resource/thresholds.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/validators.py` & `validio_sdk-0.4.0/validio_sdk/resource/validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/resource/windows.py` & `validio_sdk-0.4.0/validio_sdk/resource/windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/scalars.py` & `validio_sdk-0.4.0/validio_sdk/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/util.py` & `validio_sdk-0.4.0/validio_sdk/util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/validio_sdk/validio_client.py` & `validio_sdk-0.4.0/validio_sdk/validio_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.3.0/PKG-INFO` & `validio_sdk-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: SDK to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Project-URL: Documentation, https://docs.validio.io/
 Description-Content-Type: text/markdown
 
 # validio-sdk
 
 This SDK is maintained by [Validio] to enable users to integrate with the Validio platform in a programmatic way.
 
-See the [SDK docs] for more information.
+For more information, refer to the [SDK docs].
 
 ## Installation
 
 ```sh
 pip install validio-sdk
 ```
```

