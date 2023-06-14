# Comparing `tmp/pulumi_aiven-6.4.0a1686633780.tar.gz` & `tmp/pulumi_aiven-6.4.0a1686760738.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.4.0a1686633780.tar", last modified: Tue Jun 13 05:31:16 2023, max compression
+gzip compressed data, was "pulumi_aiven-6.4.0a1686760738.tar", last modified: Wed Jun 14 16:43:47 2023, max compression
```

## Comparing `pulumi_aiven-6.4.0a1686633780.tar` & `pulumi_aiven-6.4.0a1686760738.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:31:16.674225 pulumi_aiven-6.4.0a1686633780/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-13 05:31:16.674225 pulumi_aiven-6.4.0a1686633780/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:31:16.674225 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   595384 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    74463 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    74126 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:31:16.674225 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    74148 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21638 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21714 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22363 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    21870 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22139 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21817 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    21406 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21707 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    21219 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10493 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    75717 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    74178 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    79009 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    77110 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    77666 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19784 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    76510 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    75396 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    76019 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    75139 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)   891068 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72557 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75515 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    22097 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:31:16.674225 pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:31:16.674225 pulumi_aiven-6.4.0a1686633780/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-13 05:31:16.000000 pulumi_aiven-6.4.0a1686633780/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:47.436717 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   596968 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29700 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74463 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74126 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74148 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30205 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12455 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21536 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21292 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21768 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21715 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21228 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21271 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17872 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75717 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74178 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79009 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77110 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77666 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76510 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75396 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76019 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75139 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   892923 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72557 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37913 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75515 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 16:43:47.000000 pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:43:47.440717 pulumi_aiven-6.4.0a1686760738/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-14 16:43:46.000000 pulumi_aiven-6.4.0a1686760738/setup.py
```

### Comparing `pulumi_aiven-6.4.0a1686633780/PKG-INFO` & `pulumi_aiven-6.4.0a1686760738/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.4.0a1686633780
+Version: 6.4.0a1686760738
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.4.0a1686633780/README.md` & `pulumi_aiven-6.4.0a1686760738/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/__init__.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -5357,27 +5357,30 @@
     def __init__(__self__, *,
                  consumer_enable_auto_commit: Optional[pulumi.Input[bool]] = None,
                  consumer_request_max_bytes: Optional[pulumi.Input[int]] = None,
                  consumer_request_timeout_ms: Optional[pulumi.Input[int]] = None,
                  producer_acks: Optional[pulumi.Input[str]] = None,
                  producer_compression_type: Optional[pulumi.Input[str]] = None,
                  producer_linger_ms: Optional[pulumi.Input[int]] = None,
+                 producer_max_request_size: Optional[pulumi.Input[int]] = None,
                  simpleconsumer_pool_size_max: Optional[pulumi.Input[int]] = None):
         if consumer_enable_auto_commit is not None:
             pulumi.set(__self__, "consumer_enable_auto_commit", consumer_enable_auto_commit)
         if consumer_request_max_bytes is not None:
             pulumi.set(__self__, "consumer_request_max_bytes", consumer_request_max_bytes)
         if consumer_request_timeout_ms is not None:
             pulumi.set(__self__, "consumer_request_timeout_ms", consumer_request_timeout_ms)
         if producer_acks is not None:
             pulumi.set(__self__, "producer_acks", producer_acks)
         if producer_compression_type is not None:
             pulumi.set(__self__, "producer_compression_type", producer_compression_type)
         if producer_linger_ms is not None:
             pulumi.set(__self__, "producer_linger_ms", producer_linger_ms)
+        if producer_max_request_size is not None:
+            pulumi.set(__self__, "producer_max_request_size", producer_max_request_size)
         if simpleconsumer_pool_size_max is not None:
             pulumi.set(__self__, "simpleconsumer_pool_size_max", simpleconsumer_pool_size_max)
 
     @property
     @pulumi.getter(name="consumerEnableAutoCommit")
     def consumer_enable_auto_commit(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "consumer_enable_auto_commit")
@@ -5428,14 +5431,23 @@
         return pulumi.get(self, "producer_linger_ms")
 
     @producer_linger_ms.setter
     def producer_linger_ms(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "producer_linger_ms", value)
 
     @property
+    @pulumi.getter(name="producerMaxRequestSize")
+    def producer_max_request_size(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "producer_max_request_size")
+
+    @producer_max_request_size.setter
+    def producer_max_request_size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "producer_max_request_size", value)
+
+    @property
     @pulumi.getter(name="simpleconsumerPoolSizeMax")
     def simpleconsumer_pool_size_max(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "simpleconsumer_pool_size_max")
 
     @simpleconsumer_pool_size_max.setter
     def simpleconsumer_pool_size_max(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "simpleconsumer_pool_size_max", value)
@@ -6198,15 +6210,15 @@
         :param pulumi.Input[bool] preallocate: preallocate value
         :param pulumi.Input[str] retention_bytes: retention.bytes value
         :param pulumi.Input[str] retention_ms: retention.ms value
         :param pulumi.Input[str] segment_bytes: segment.bytes value
         :param pulumi.Input[str] segment_index_bytes: segment.index.bytes value
         :param pulumi.Input[str] segment_jitter_ms: segment.jitter.ms value
         :param pulumi.Input[str] segment_ms: segment.ms value
-        :param pulumi.Input[bool] unclean_leader_election_enable: unclean.leader.election.enable value
+        :param pulumi.Input[bool] unclean_leader_election_enable: unclean.leader.election.enable value; This field is deprecated and no longer functional.
         """
         if cleanup_policy is not None:
             pulumi.set(__self__, "cleanup_policy", cleanup_policy)
         if compression_type is not None:
             pulumi.set(__self__, "compression_type", compression_type)
         if delete_retention_ms is not None:
             pulumi.set(__self__, "delete_retention_ms", delete_retention_ms)
@@ -6247,14 +6259,17 @@
         if segment_index_bytes is not None:
             pulumi.set(__self__, "segment_index_bytes", segment_index_bytes)
         if segment_jitter_ms is not None:
             pulumi.set(__self__, "segment_jitter_ms", segment_jitter_ms)
         if segment_ms is not None:
             pulumi.set(__self__, "segment_ms", segment_ms)
         if unclean_leader_election_enable is not None:
+            warnings.warn("""This field is deprecated and no longer functional.""", DeprecationWarning)
+            pulumi.log.warn("""unclean_leader_election_enable is deprecated: This field is deprecated and no longer functional.""")
+        if unclean_leader_election_enable is not None:
             pulumi.set(__self__, "unclean_leader_election_enable", unclean_leader_election_enable)
 
     @property
     @pulumi.getter(name="cleanupPolicy")
     def cleanup_policy(self) -> Optional[pulumi.Input[str]]:
         """
         cleanup.policy value
@@ -6529,15 +6544,15 @@
     def segment_ms(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "segment_ms", value)
 
     @property
     @pulumi.getter(name="uncleanLeaderElectionEnable")
     def unclean_leader_election_enable(self) -> Optional[pulumi.Input[bool]]:
         """
-        unclean.leader.election.enable value
+        unclean.leader.election.enable value; This field is deprecated and no longer functional.
         """
         return pulumi.get(self, "unclean_leader_election_enable")
 
     @unclean_leader_election_enable.setter
     def unclean_leader_election_enable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "unclean_leader_election_enable", value)
 
@@ -14082,22 +14097,25 @@
 
 @pulumi.input_type
 class ServiceIntegrationKafkaMirrormakerUserConfigKafkaMirrormakerArgs:
     def __init__(__self__, *,
                  consumer_fetch_min_bytes: Optional[pulumi.Input[int]] = None,
                  producer_batch_size: Optional[pulumi.Input[int]] = None,
                  producer_buffer_memory: Optional[pulumi.Input[int]] = None,
+                 producer_compression_type: Optional[pulumi.Input[str]] = None,
                  producer_linger_ms: Optional[pulumi.Input[int]] = None,
                  producer_max_request_size: Optional[pulumi.Input[int]] = None):
         if consumer_fetch_min_bytes is not None:
             pulumi.set(__self__, "consumer_fetch_min_bytes", consumer_fetch_min_bytes)
         if producer_batch_size is not None:
             pulumi.set(__self__, "producer_batch_size", producer_batch_size)
         if producer_buffer_memory is not None:
             pulumi.set(__self__, "producer_buffer_memory", producer_buffer_memory)
+        if producer_compression_type is not None:
+            pulumi.set(__self__, "producer_compression_type", producer_compression_type)
         if producer_linger_ms is not None:
             pulumi.set(__self__, "producer_linger_ms", producer_linger_ms)
         if producer_max_request_size is not None:
             pulumi.set(__self__, "producer_max_request_size", producer_max_request_size)
 
     @property
     @pulumi.getter(name="consumerFetchMinBytes")
@@ -14123,14 +14141,23 @@
         return pulumi.get(self, "producer_buffer_memory")
 
     @producer_buffer_memory.setter
     def producer_buffer_memory(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "producer_buffer_memory", value)
 
     @property
+    @pulumi.getter(name="producerCompressionType")
+    def producer_compression_type(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "producer_compression_type")
+
+    @producer_compression_type.setter
+    def producer_compression_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "producer_compression_type", value)
+
+    @property
     @pulumi.getter(name="producerLingerMs")
     def producer_linger_ms(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "producer_linger_ms")
 
     @producer_linger_ms.setter
     def producer_linger_ms(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "producer_linger_ms", value)
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account_team.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/flink.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_aws_privatelink.py`

 * *Files 11% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_aws_privatelink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    foo = aiven.get_aws_privatelink(project=data["aiven_project"]["foo"]["project"],
+        service_name=aiven_kafka["bar"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
@@ -148,16 +148,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_aws_privatelink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    foo = aiven.get_aws_privatelink(project=data["aiven_project"]["foo"]["project"],
+        service_name=aiven_kafka["bar"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_aws_vpc_peering_connection(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    foo = aiven.get_aws_vpc_peering_connection(vpc_id=data["aiven_project_vpc"]["vpc"]["id"],
         aws_account_id="XXXXX",
         aws_vpc_id="XXXXX")
     ```
 
 
     :param str aws_account_id: AWS account ID. This property cannot be changed, doing so forces recreation of the resource.
     :param str aws_vpc_id: AWS VPC ID. This property cannot be changed, doing so forces recreation of the resource.
@@ -183,15 +183,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_aws_vpc_peering_connection(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    foo = aiven.get_aws_vpc_peering_connection(vpc_id=data["aiven_project_vpc"]["vpc"]["id"],
         aws_account_id="XXXXX",
         aws_vpc_id="XXXXX")
     ```
 
 
     :param str aws_account_id: AWS account ID. This property cannot be changed, doing so forces recreation of the resource.
     :param str aws_vpc_id: AWS VPC ID. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_azure_privatelink.py`

 * *Files 10% similar despite different names*

```diff
@@ -136,16 +136,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_azure_privatelink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    foo = aiven.get_azure_privatelink(project=data["aiven_project"]["foo"]["project"],
+        service_name=aiven_kafka["bar"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
@@ -174,16 +174,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_azure_privatelink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    foo = aiven.get_azure_privatelink(project=data["aiven_project"]["foo"]["project"],
+        service_name=aiven_kafka["bar"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassanda.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    bar = aiven.get_cassandra(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    bar = aiven.get_cassandra(project=data["aiven_project"]["foo"]["project"],
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -438,15 +438,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    bar = aiven.get_cassandra(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    bar = aiven.get_cassandra(project=data["aiven_project"]["foo"]["project"],
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassandra.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    bar = aiven.get_cassandra(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    bar = aiven.get_cassandra(project=data["aiven_project"]["foo"]["project"],
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    bar = aiven.get_cassandra(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    bar = aiven.get_cassandra(project=data["aiven_project"]["foo"]["project"],
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    clickhouse = aiven.get_clickhouse(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    clickhouse = aiven.get_clickhouse(project=data["aiven_project"]["pr1"]["project"],
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    clickhouse = aiven.get_clickhouse(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    clickhouse = aiven.get_clickhouse(project=data["aiven_project"]["pr1"]["project"],
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influxdb_database.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,57 +6,57 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetClickhouseDatabaseResult',
-    'AwaitableGetClickhouseDatabaseResult',
-    'get_clickhouse_database',
-    'get_clickhouse_database_output',
+    'GetInfluxdbDatabaseResult',
+    'AwaitableGetInfluxdbDatabaseResult',
+    'get_influxdb_database',
+    'get_influxdb_database_output',
 ]
 
 @pulumi.output_type
-class GetClickhouseDatabaseResult:
+class GetInfluxdbDatabaseResult:
     """
-    A collection of values returned by getClickhouseDatabase.
+    A collection of values returned by getInfluxdbDatabase.
     """
-    def __init__(__self__, id=None, name=None, project=None, service_name=None, termination_protection=None):
+    def __init__(__self__, database_name=None, id=None, project=None, service_name=None, termination_protection=None):
+        if database_name and not isinstance(database_name, str):
+            raise TypeError("Expected argument 'database_name' to be a str")
+        pulumi.set(__self__, "database_name", database_name)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
         if termination_protection and not isinstance(termination_protection, bool):
             raise TypeError("Expected argument 'termination_protection' to be a bool")
         pulumi.set(__self__, "termination_protection", termination_protection)
 
     @property
-    @pulumi.getter
-    def id(self) -> str:
+    @pulumi.getter(name="databaseName")
+    def database_name(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "database_name")
 
     @property
     @pulumi.getter
-    def name(self) -> str:
+    def id(self) -> str:
         """
-        The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
+        The provider-assigned unique ID for this managed resource.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -72,83 +72,61 @@
 
     @property
     @pulumi.getter(name="terminationProtection")
     def termination_protection(self) -> bool:
         return pulumi.get(self, "termination_protection")
 
 
-class AwaitableGetClickhouseDatabaseResult(GetClickhouseDatabaseResult):
+class AwaitableGetInfluxdbDatabaseResult(GetInfluxdbDatabaseResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetClickhouseDatabaseResult(
+        return GetInfluxdbDatabaseResult(
+            database_name=self.database_name,
             id=self.id,
-            name=self.name,
             project=self.project,
             service_name=self.service_name,
             termination_protection=self.termination_protection)
 
 
-def get_clickhouse_database(name: Optional[str] = None,
-                            project: Optional[str] = None,
-                            service_name: Optional[str] = None,
-                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClickhouseDatabaseResult:
+def get_influxdb_database(database_name: Optional[str] = None,
+                          project: Optional[str] = None,
+                          service_name: Optional[str] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInfluxdbDatabaseResult:
     """
-    The Clickhouse database data source provides information about the existing Aiven Clickhouse Database.
+    The InfluxDB Database data source provides information about the existing Aiven InfluxDB Database.
 
-    ## Example Usage
 
-    ```python
-    import pulumi
-    import pulumi_aiven as aiven
-
-    clickhouse_db = aiven.get_clickhouse_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        name="my-ch-db")
-    ```
-
-
-    :param str name: The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
+    :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
-    __args__['name'] = name
+    __args__['databaseName'] = database_name
     __args__['project'] = project
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getClickhouseDatabase:getClickhouseDatabase', __args__, opts=opts, typ=GetClickhouseDatabaseResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getInfluxdbDatabase:getInfluxdbDatabase', __args__, opts=opts, typ=GetInfluxdbDatabaseResult).value
 
-    return AwaitableGetClickhouseDatabaseResult(
+    return AwaitableGetInfluxdbDatabaseResult(
+        database_name=__ret__.database_name,
         id=__ret__.id,
-        name=__ret__.name,
         project=__ret__.project,
         service_name=__ret__.service_name,
         termination_protection=__ret__.termination_protection)
 
 
-@_utilities.lift_output_func(get_clickhouse_database)
-def get_clickhouse_database_output(name: Optional[pulumi.Input[str]] = None,
-                                   project: Optional[pulumi.Input[str]] = None,
-                                   service_name: Optional[pulumi.Input[str]] = None,
-                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClickhouseDatabaseResult]:
+@_utilities.lift_output_func(get_influxdb_database)
+def get_influxdb_database_output(database_name: Optional[pulumi.Input[str]] = None,
+                                 project: Optional[pulumi.Input[str]] = None,
+                                 service_name: Optional[pulumi.Input[str]] = None,
+                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInfluxdbDatabaseResult]:
     """
-    The Clickhouse database data source provides information about the existing Aiven Clickhouse Database.
-
-    ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_aiven as aiven
-
-    clickhouse_db = aiven.get_clickhouse_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        name="my-ch-db")
-    ```
+    The InfluxDB Database data source provides information about the existing Aiven InfluxDB Database.
 
 
-    :param str name: The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
+    :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3db_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,178 +6,165 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetClickhouseUserResult',
-    'AwaitableGetClickhouseUserResult',
-    'get_clickhouse_user',
-    'get_clickhouse_user_output',
+    'GetM3dbUserResult',
+    'AwaitableGetM3dbUserResult',
+    'get_m3db_user',
+    'get_m3db_user_output',
 ]
 
 @pulumi.output_type
-class GetClickhouseUserResult:
+class GetM3dbUserResult:
     """
-    A collection of values returned by getClickhouseUser.
+    A collection of values returned by getM3dbUser.
     """
-    def __init__(__self__, id=None, password=None, project=None, required=None, service_name=None, username=None, uuid=None):
+    def __init__(__self__, id=None, password=None, project=None, service_name=None, type=None, username=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if password and not isinstance(password, str):
             raise TypeError("Expected argument 'password' to be a str")
         pulumi.set(__self__, "password", password)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
-        if required and not isinstance(required, bool):
-            raise TypeError("Expected argument 'required' to be a bool")
-        pulumi.set(__self__, "required", required)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
         if username and not isinstance(username, str):
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
-        if uuid and not isinstance(uuid, str):
-            raise TypeError("Expected argument 'uuid' to be a str")
-        pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        The password of the clickhouse user.
+        The password of the M3DB User.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter
-    def required(self) -> bool:
-        """
-        Indicates if a clickhouse user is required
-        """
-        return pulumi.get(self, "required")
-
-    @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter
-    def username(self) -> str:
+    def type(self) -> str:
         """
-        The actual name of the Clickhouse user. This property cannot be changed, doing so forces recreation of the resource.
+        Type of the user account. Tells whether the user is the primary account or a regular account.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
-    def uuid(self) -> str:
+    def username(self) -> str:
         """
-        UUID of the clickhouse user.
+        The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "uuid")
+        return pulumi.get(self, "username")
 
 
-class AwaitableGetClickhouseUserResult(GetClickhouseUserResult):
+class AwaitableGetM3dbUserResult(GetM3dbUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetClickhouseUserResult(
+        return GetM3dbUserResult(
             id=self.id,
             password=self.password,
             project=self.project,
-            required=self.required,
             service_name=self.service_name,
-            username=self.username,
-            uuid=self.uuid)
+            type=self.type,
+            username=self.username)
 
 
-def get_clickhouse_user(project: Optional[str] = None,
-                        service_name: Optional[str] = None,
-                        username: Optional[str] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClickhouseUserResult:
+def get_m3db_user(project: Optional[str] = None,
+                  service_name: Optional[str] = None,
+                  username: Optional[str] = None,
+                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetM3dbUserResult:
     """
-    The Clickhouse User data source provides information about the existing Aiven Clickhouse User.
+    The M3DB User data source provides information about the existing Aiven M3DB User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    ch_user = aiven.get_clickhouse_user(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        username="<USERNAME>")
+    user = aiven.get_m3db_user(project="my-project",
+        service_name="my-service",
+        username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Clickhouse user. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getClickhouseUser:getClickhouseUser', __args__, opts=opts, typ=GetClickhouseUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getM3dbUser:getM3dbUser', __args__, opts=opts, typ=GetM3dbUserResult).value
 
-    return AwaitableGetClickhouseUserResult(
+    return AwaitableGetM3dbUserResult(
         id=__ret__.id,
         password=__ret__.password,
         project=__ret__.project,
-        required=__ret__.required,
         service_name=__ret__.service_name,
-        username=__ret__.username,
-        uuid=__ret__.uuid)
+        type=__ret__.type,
+        username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_clickhouse_user)
-def get_clickhouse_user_output(project: Optional[pulumi.Input[str]] = None,
-                               service_name: Optional[pulumi.Input[str]] = None,
-                               username: Optional[pulumi.Input[str]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClickhouseUserResult]:
+@_utilities.lift_output_func(get_m3db_user)
+def get_m3db_user_output(project: Optional[pulumi.Input[str]] = None,
+                         service_name: Optional[pulumi.Input[str]] = None,
+                         username: Optional[pulumi.Input[str]] = None,
+                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetM3dbUserResult]:
     """
-    The Clickhouse User data source provides information about the existing Aiven Clickhouse User.
+    The M3DB User data source provides information about the existing Aiven M3DB User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    ch_user = aiven.get_clickhouse_user(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        username="<USERNAME>")
+    user = aiven.get_m3db_user(project="my-project",
+        service_name="my-service",
+        username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Clickhouse user. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,101 +6,93 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetConnectionPoolResult',
-    'AwaitableGetConnectionPoolResult',
-    'get_connection_pool',
-    'get_connection_pool_output',
+    'GetPgUserResult',
+    'AwaitableGetPgUserResult',
+    'get_pg_user',
+    'get_pg_user_output',
 ]
 
 @pulumi.output_type
-class GetConnectionPoolResult:
+class GetPgUserResult:
     """
-    A collection of values returned by getConnectionPool.
+    A collection of values returned by getPgUser.
     """
-    def __init__(__self__, connection_uri=None, database_name=None, id=None, pool_mode=None, pool_name=None, pool_size=None, project=None, service_name=None, username=None):
-        if connection_uri and not isinstance(connection_uri, str):
-            raise TypeError("Expected argument 'connection_uri' to be a str")
-        pulumi.set(__self__, "connection_uri", connection_uri)
-        if database_name and not isinstance(database_name, str):
-            raise TypeError("Expected argument 'database_name' to be a str")
-        pulumi.set(__self__, "database_name", database_name)
+    def __init__(__self__, access_cert=None, access_key=None, id=None, password=None, pg_allow_replication=None, project=None, service_name=None, type=None, username=None):
+        if access_cert and not isinstance(access_cert, str):
+            raise TypeError("Expected argument 'access_cert' to be a str")
+        pulumi.set(__self__, "access_cert", access_cert)
+        if access_key and not isinstance(access_key, str):
+            raise TypeError("Expected argument 'access_key' to be a str")
+        pulumi.set(__self__, "access_key", access_key)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if pool_mode and not isinstance(pool_mode, str):
-            raise TypeError("Expected argument 'pool_mode' to be a str")
-        pulumi.set(__self__, "pool_mode", pool_mode)
-        if pool_name and not isinstance(pool_name, str):
-            raise TypeError("Expected argument 'pool_name' to be a str")
-        pulumi.set(__self__, "pool_name", pool_name)
-        if pool_size and not isinstance(pool_size, int):
-            raise TypeError("Expected argument 'pool_size' to be a int")
-        pulumi.set(__self__, "pool_size", pool_size)
+        if password and not isinstance(password, str):
+            raise TypeError("Expected argument 'password' to be a str")
+        pulumi.set(__self__, "password", password)
+        if pg_allow_replication and not isinstance(pg_allow_replication, bool):
+            raise TypeError("Expected argument 'pg_allow_replication' to be a bool")
+        pulumi.set(__self__, "pg_allow_replication", pg_allow_replication)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
+        if type and not isinstance(type, str):
+            raise TypeError("Expected argument 'type' to be a str")
+        pulumi.set(__self__, "type", type)
         if username and not isinstance(username, str):
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
 
     @property
-    @pulumi.getter(name="connectionUri")
-    def connection_uri(self) -> str:
+    @pulumi.getter(name="accessCert")
+    def access_cert(self) -> str:
         """
-        The URI for connecting to the pool
+        Access certificate for the user
         """
-        return pulumi.get(self, "connection_uri")
+        return pulumi.get(self, "access_cert")
 
     @property
-    @pulumi.getter(name="databaseName")
-    def database_name(self) -> str:
+    @pulumi.getter(name="accessKey")
+    def access_key(self) -> str:
         """
-        The name of the database the pool connects to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        Access certificate key for the user
         """
-        return pulumi.get(self, "database_name")
+        return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="poolMode")
-    def pool_mode(self) -> str:
-        """
-        The mode the pool operates in. The possible values are `session`, `transaction` and `statement`. The default value is `transaction`.
-        """
-        return pulumi.get(self, "pool_mode")
-
-    @property
-    @pulumi.getter(name="poolName")
-    def pool_name(self) -> str:
+    @pulumi.getter
+    def password(self) -> str:
         """
-        The name of the created pool. This property cannot be changed, doing so forces recreation of the resource.
+        The password of the PG User ( not applicable for all services ).
         """
-        return pulumi.get(self, "pool_name")
+        return pulumi.get(self, "password")
 
     @property
-    @pulumi.getter(name="poolSize")
-    def pool_size(self) -> int:
+    @pulumi.getter(name="pgAllowReplication")
+    def pg_allow_replication(self) -> bool:
         """
-        The number of connections the pool may create towards the backend server. This does not affect the number of incoming connections, which is always a much larger number. The default value is `10`.
+        Defines whether replication is allowed. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "pool_size")
+        return pulumi.get(self, "pg_allow_replication")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -112,98 +104,106 @@
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter
+    def type(self) -> str:
+        """
+        Type of the user account. Tells whether the user is the primary account or a regular account.
+        """
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter
     def username(self) -> str:
         """
-        The name of the service user used to connect to the database. To set up proper dependencies please refer to this variable as a reference.
+        The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
 
-class AwaitableGetConnectionPoolResult(GetConnectionPoolResult):
+class AwaitableGetPgUserResult(GetPgUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetConnectionPoolResult(
-            connection_uri=self.connection_uri,
-            database_name=self.database_name,
+        return GetPgUserResult(
+            access_cert=self.access_cert,
+            access_key=self.access_key,
             id=self.id,
-            pool_mode=self.pool_mode,
-            pool_name=self.pool_name,
-            pool_size=self.pool_size,
+            password=self.password,
+            pg_allow_replication=self.pg_allow_replication,
             project=self.project,
             service_name=self.service_name,
+            type=self.type,
             username=self.username)
 
 
-def get_connection_pool(pool_name: Optional[str] = None,
-                        project: Optional[str] = None,
-                        service_name: Optional[str] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetConnectionPoolResult:
+def get_pg_user(project: Optional[str] = None,
+                service_name: Optional[str] = None,
+                username: Optional[str] = None,
+                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPgUserResult:
     """
-    The Connection Pool data source provides information about the existing Aiven Connection Pool.
+    The PG User data source provides information about the existing Aiven PG User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestpool = aiven.get_connection_pool(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        pool_name="mypool")
+    user = aiven.get_pg_user(project="my-project",
+        service_name="my-service",
+        username="user1")
     ```
 
 
-    :param str pool_name: The name of the created pool. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
-    __args__['poolName'] = pool_name
     __args__['project'] = project
     __args__['serviceName'] = service_name
+    __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getConnectionPool:getConnectionPool', __args__, opts=opts, typ=GetConnectionPoolResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getPgUser:getPgUser', __args__, opts=opts, typ=GetPgUserResult).value
 
-    return AwaitableGetConnectionPoolResult(
-        connection_uri=__ret__.connection_uri,
-        database_name=__ret__.database_name,
+    return AwaitableGetPgUserResult(
+        access_cert=__ret__.access_cert,
+        access_key=__ret__.access_key,
         id=__ret__.id,
-        pool_mode=__ret__.pool_mode,
-        pool_name=__ret__.pool_name,
-        pool_size=__ret__.pool_size,
+        password=__ret__.password,
+        pg_allow_replication=__ret__.pg_allow_replication,
         project=__ret__.project,
         service_name=__ret__.service_name,
+        type=__ret__.type,
         username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_connection_pool)
-def get_connection_pool_output(pool_name: Optional[pulumi.Input[str]] = None,
-                               project: Optional[pulumi.Input[str]] = None,
-                               service_name: Optional[pulumi.Input[str]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetConnectionPoolResult]:
+@_utilities.lift_output_func(get_pg_user)
+def get_pg_user_output(project: Optional[pulumi.Input[str]] = None,
+                       service_name: Optional[pulumi.Input[str]] = None,
+                       username: Optional[pulumi.Input[str]] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPgUserResult]:
     """
-    The Connection Pool data source provides information about the existing Aiven Connection Pool.
+    The PG User data source provides information about the existing Aiven PG User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestpool = aiven.get_connection_pool(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        pool_name="mypool")
+    user = aiven.get_pg_user(project="my-project",
+        service_name="my-service",
+        username="user1")
     ```
 
 
-    :param str pool_name: The name of the created pool. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    flink = aiven.get_flink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    flink = aiven.get_flink(project=data["aiven_project"]["pr1"]["project"],
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    flink = aiven.get_flink(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    flink = aiven.get_flink(project=data["aiven_project"]["pr1"]["project"],
         service_name="<SERVICE_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink_application.py`

 * *Files 4% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    app1 = aiven.get_flink_application(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    app1 = aiven.get_flink_application(project=data["aiven_project"]["pr1"]["project"],
         service_name="<SERVICE_NAME>",
         name="<APPLICATION_NAME>")
     ```
 
 
     :param str name: Application name
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
@@ -192,15 +192,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    app1 = aiven.get_flink_application(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    app1 = aiven.get_flink_application(project=data["aiven_project"]["pr1"]["project"],
         service_name="<SERVICE_NAME>",
         name="<APPLICATION_NAME>")
     ```
 
 
     :param str name: Application name
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_flink_application_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,15 +199,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    app1 = aiven.get_flink_application_version(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    app1 = aiven.get_flink_application_version(project=data["aiven_project"]["pr1"]["project"],
         service_name="<SERVICE_NAME>",
         application_id="<APPLICATION_ID>",
         application_version_id="<APPLICATION_VERSION_ID>")
     ```
 
 
     :param str application_id: Application ID
@@ -250,15 +250,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    app1 = aiven.get_flink_application_version(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    app1 = aiven.get_flink_application_version(project=data["aiven_project"]["pr1"]["project"],
         service_name="<SERVICE_NAME>",
         application_id="<APPLICATION_ID>",
         application_version_id="<APPLICATION_VERSION_ID>")
     ```
 
 
     :param str application_id: Application ID
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_gcp_vpc_peering_connection(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    foo = aiven.get_gcp_vpc_peering_connection(vpc_id=data["aiven_project_vpc"]["vpc"]["id"],
         gcp_project_id="xxxx",
         peer_vpc="xxxx")
     ```
 
 
     :param str gcp_project_id: GCP project ID. This property cannot be changed, doing so forces recreation of the resource.
     :param str peer_vpc: GCP VPC network name. This property cannot be changed, doing so forces recreation of the resource.
@@ -166,15 +166,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    foo = aiven.get_gcp_vpc_peering_connection(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    foo = aiven.get_gcp_vpc_peering_connection(vpc_id=data["aiven_project_vpc"]["vpc"]["id"],
         gcp_project_id="xxxx",
         peer_vpc="xxxx")
     ```
 
 
     :param str gcp_project_id: GCP project ID. This property cannot be changed, doing so forces recreation of the resource.
     :param str peer_vpc: GCP VPC network name. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_grafana.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    gr1 = aiven.get_grafana(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    gr1 = aiven.get_grafana(project=data["aiven_project"]["ps1"]["project"],
         service_name="my-gr1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    gr1 = aiven.get_grafana(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    gr1 = aiven.get_grafana(project=data["aiven_project"]["ps1"]["project"],
         service_name="my-gr1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influx_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    inf1 = aiven.get_influx_db(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    inf1 = aiven.get_influx_db(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-inf1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    inf1 = aiven.get_influx_db(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    inf1 = aiven.get_influx_db(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-inf1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mysql_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetInfluxdbDatabaseResult',
-    'AwaitableGetInfluxdbDatabaseResult',
-    'get_influxdb_database',
-    'get_influxdb_database_output',
+    'GetMysqlDatabaseResult',
+    'AwaitableGetMysqlDatabaseResult',
+    'get_mysql_database',
+    'get_mysql_database_output',
 ]
 
 @pulumi.output_type
-class GetInfluxdbDatabaseResult:
+class GetMysqlDatabaseResult:
     """
-    A collection of values returned by getInfluxdbDatabase.
+    A collection of values returned by getMysqlDatabase.
     """
     def __init__(__self__, database_name=None, id=None, project=None, service_name=None, termination_protection=None):
         if database_name and not isinstance(database_name, str):
             raise TypeError("Expected argument 'database_name' to be a str")
         pulumi.set(__self__, "database_name", database_name)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
@@ -72,61 +72,83 @@
 
     @property
     @pulumi.getter(name="terminationProtection")
     def termination_protection(self) -> bool:
         return pulumi.get(self, "termination_protection")
 
 
-class AwaitableGetInfluxdbDatabaseResult(GetInfluxdbDatabaseResult):
+class AwaitableGetMysqlDatabaseResult(GetMysqlDatabaseResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetInfluxdbDatabaseResult(
+        return GetMysqlDatabaseResult(
             database_name=self.database_name,
             id=self.id,
             project=self.project,
             service_name=self.service_name,
             termination_protection=self.termination_protection)
 
 
-def get_influxdb_database(database_name: Optional[str] = None,
-                          project: Optional[str] = None,
-                          service_name: Optional[str] = None,
-                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInfluxdbDatabaseResult:
-    """
-    The InfluxDB Database data source provides information about the existing Aiven InfluxDB Database.
+def get_mysql_database(database_name: Optional[str] = None,
+                       project: Optional[str] = None,
+                       service_name: Optional[str] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMysqlDatabaseResult:
+    """
+    The MySQL Database data source provides information about the existing Aiven MySQL Database.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_aiven as aiven
+
+    mydatabase = aiven.get_mysql_database(project=aiven_project["myproject"]["project"],
+        service_name=aiven_mysql["mymysql"]["service_name"],
+        database_name="<DATABASE_NAME>")
+    ```
 
 
     :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['databaseName'] = database_name
     __args__['project'] = project
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getInfluxdbDatabase:getInfluxdbDatabase', __args__, opts=opts, typ=GetInfluxdbDatabaseResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getMysqlDatabase:getMysqlDatabase', __args__, opts=opts, typ=GetMysqlDatabaseResult).value
 
-    return AwaitableGetInfluxdbDatabaseResult(
+    return AwaitableGetMysqlDatabaseResult(
         database_name=__ret__.database_name,
         id=__ret__.id,
         project=__ret__.project,
         service_name=__ret__.service_name,
         termination_protection=__ret__.termination_protection)
 
 
-@_utilities.lift_output_func(get_influxdb_database)
-def get_influxdb_database_output(database_name: Optional[pulumi.Input[str]] = None,
-                                 project: Optional[pulumi.Input[str]] = None,
-                                 service_name: Optional[pulumi.Input[str]] = None,
-                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInfluxdbDatabaseResult]:
-    """
-    The InfluxDB Database data source provides information about the existing Aiven InfluxDB Database.
+@_utilities.lift_output_func(get_mysql_database)
+def get_mysql_database_output(database_name: Optional[pulumi.Input[str]] = None,
+                              project: Optional[pulumi.Input[str]] = None,
+                              service_name: Optional[pulumi.Input[str]] = None,
+                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMysqlDatabaseResult]:
+    """
+    The MySQL Database data source provides information about the existing Aiven MySQL Database.
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_aiven as aiven
+
+    mydatabase = aiven.get_mysql_database(project=aiven_project["myproject"]["project"],
+        service_name=aiven_mysql["mymysql"]["service_name"],
+        database_name="<DATABASE_NAME>")
+    ```
 
 
     :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,15 +401,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kafka1 = aiven.get_kafka(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    kafka1 = aiven.get_kafka(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-kafka1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -461,15 +461,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kafka1 = aiven.get_kafka(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    kafka1 = aiven.get_kafka(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-kafka1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_acl.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,16 +127,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestacl = aiven.get_kafka_acl(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mytestacl = aiven.get_kafka_acl(project=aiven_project["myproject"]["project"],
+        service_name=aiven_kafka["mykafka"]["service_name"],
         topic="<TOPIC_NAME_PATTERN>",
         permission="<PERMISSON>",
         username="<USERNAME_PATTERN>")
     ```
 
 
     :param str permission: Kafka permission to grant. The possible values are `admin`, `read`, `readwrite` and `write`. This property cannot be changed, doing so forces recreation of the resource.
@@ -176,16 +176,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestacl = aiven.get_kafka_acl(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mytestacl = aiven.get_kafka_acl(project=aiven_project["myproject"]["project"],
+        service_name=aiven_kafka["mykafka"]["service_name"],
         topic="<TOPIC_NAME_PATTERN>",
         permission="<PERMISSON>",
         username="<USERNAME_PATTERN>")
     ```
 
 
     :param str permission: Kafka permission to grant. The possible values are `admin`, `read`, `readwrite` and `write`. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kc1 = aiven.get_kafka_connect(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    kc1 = aiven.get_kafka_connect(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-kc1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kc1 = aiven.get_kafka_connect(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    kc1 = aiven.get_kafka_connect(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-kc1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -186,16 +186,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kafka_es_con1 = aiven.get_kafka_connector(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    kafka_es_con1 = aiven.get_kafka_connector(project=aiven_project["kafka-con-project1"]["project"],
+        service_name=aiven_kafka["kafka-service1"]["service_name"],
         connector_name="kafka-es-con1")
     ```
 
 
     :param str connector_name: The kafka connector name. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
@@ -232,16 +232,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    kafka_es_con1 = aiven.get_kafka_connector(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    kafka_es_con1 = aiven.get_kafka_connector(project=aiven_project["kafka-con-project1"]["project"],
+        service_name=aiven_kafka["kafka-service1"]["service_name"],
         connector_name="kafka-es-con1")
     ```
 
 
     :param str connector_name: The kafka connector name. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mm1 = aiven.get_kafka_mirror_maker(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mm1 = aiven.get_kafka_mirror_maker(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-mm1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mm1 = aiven.get_kafka_mirror_maker(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mm1 = aiven.get_kafka_mirror_maker(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-mm1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -137,16 +137,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    config = aiven.get_kafka_schema_configuration(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    config = aiven.get_kafka_schema_configuration(project=aiven_project["kafka-schemas-project1"]["project"],
+        service_name=aiven_kafka["kafka-service1"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str subject_name: The Kafka Schema Subject name. This property cannot be changed, doing so forces recreation of the resource.
     """
@@ -178,16 +178,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    config = aiven.get_kafka_schema_configuration(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    config = aiven.get_kafka_schema_configuration(project=aiven_project["kafka-schemas-project1"]["project"],
+        service_name=aiven_kafka["kafka-service1"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str subject_name: The Kafka Schema Subject name. This property cannot be changed, doing so forces recreation of the resource.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_topic.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,16 +147,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytesttopic = aiven.get_kafka_topic(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mytesttopic = aiven.get_kafka_topic(project=aiven_project["myproject"]["project"],
+        service_name=aiven_kafka["myservice"]["service_name"],
         topic_name="<TOPIC_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str topic_name: The name of the topic. This property cannot be changed, doing so forces recreation of the resource.
@@ -190,16 +190,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytesttopic = aiven.get_kafka_topic(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mytesttopic = aiven.get_kafka_topic(project=aiven_project["myproject"]["project"],
+        service_name=aiven_kafka["myservice"]["service_name"],
         topic_name="<TOPIC_NAME>")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str topic_name: The name of the topic. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3_aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    m3a = aiven.get_m3_aggregator(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    m3a = aiven.get_m3_aggregator(project=data["aiven_project"]["foo"]["project"],
         service_name="my-m3a")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    m3a = aiven.get_m3_aggregator(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    m3a = aiven.get_m3_aggregator(project=data["aiven_project"]["foo"]["project"],
         service_name="my-m3a")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_m3_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    m3 = aiven.get_m3_db(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    m3 = aiven.get_m3_db(project=data["aiven_project"]["foo"]["project"],
         service_name="my-m3db")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    m3 = aiven.get_m3_db(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    m3 = aiven.get_m3_db(project=data["aiven_project"]["foo"]["project"],
         service_name="my-m3db")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_opensearch_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetM3dbUserResult',
-    'AwaitableGetM3dbUserResult',
-    'get_m3db_user',
-    'get_m3db_user_output',
+    'GetOpensearchUserResult',
+    'AwaitableGetOpensearchUserResult',
+    'get_opensearch_user',
+    'get_opensearch_user_output',
 ]
 
 @pulumi.output_type
-class GetM3dbUserResult:
+class GetOpensearchUserResult:
     """
-    A collection of values returned by getM3dbUser.
+    A collection of values returned by getOpensearchUser.
     """
     def __init__(__self__, id=None, password=None, project=None, service_name=None, type=None, username=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if password and not isinstance(password, str):
             raise TypeError("Expected argument 'password' to be a str")
@@ -49,15 +49,15 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        The password of the M3DB User.
+        The password of the Opensearch User.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
@@ -81,90 +81,90 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
 
-class AwaitableGetM3dbUserResult(GetM3dbUserResult):
+class AwaitableGetOpensearchUserResult(GetOpensearchUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetM3dbUserResult(
+        return GetOpensearchUserResult(
             id=self.id,
             password=self.password,
             project=self.project,
             service_name=self.service_name,
             type=self.type,
             username=self.username)
 
 
-def get_m3db_user(project: Optional[str] = None,
-                  service_name: Optional[str] = None,
-                  username: Optional[str] = None,
-                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetM3dbUserResult:
+def get_opensearch_user(project: Optional[str] = None,
+                        service_name: Optional[str] = None,
+                        username: Optional[str] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpensearchUserResult:
     """
-    The M3DB User data source provides information about the existing Aiven M3DB User.
+    The Opensearch User data source provides information about the existing Aiven Cassandra User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_m3db_user(project="my-project",
+    user = aiven.get_opensearch_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getM3dbUser:getM3dbUser', __args__, opts=opts, typ=GetM3dbUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getOpensearchUser:getOpensearchUser', __args__, opts=opts, typ=GetOpensearchUserResult).value
 
-    return AwaitableGetM3dbUserResult(
+    return AwaitableGetOpensearchUserResult(
         id=__ret__.id,
         password=__ret__.password,
         project=__ret__.project,
         service_name=__ret__.service_name,
         type=__ret__.type,
         username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_m3db_user)
-def get_m3db_user_output(project: Optional[pulumi.Input[str]] = None,
-                         service_name: Optional[pulumi.Input[str]] = None,
-                         username: Optional[pulumi.Input[str]] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetM3dbUserResult]:
+@_utilities.lift_output_func(get_opensearch_user)
+def get_opensearch_user_output(project: Optional[pulumi.Input[str]] = None,
+                               service_name: Optional[pulumi.Input[str]] = None,
+                               username: Optional[pulumi.Input[str]] = None,
+                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpensearchUserResult]:
     """
-    The M3DB User data source provides information about the existing Aiven M3DB User.
+    The Opensearch User data source provides information about the existing Aiven Cassandra User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_m3db_user(project="my-project",
+    user = aiven.get_opensearch_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the M3DB User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files 9% similar despite different names*

```diff
@@ -198,18 +198,18 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    f1 = aiven.get_mirror_maker_replication_flow(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        source_cluster=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        target_cluster=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    f1 = aiven.get_mirror_maker_replication_flow(project=aiven_project["kafka-mm-project1"]["project"],
+        service_name=aiven_kafka["mm"]["service_name"],
+        source_cluster=aiven_kafka["source"]["service_name"],
+        target_cluster=aiven_kafka["target"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str source_cluster: Source cluster alias. Maximum length: `128`.
     :param str target_cluster: Target cluster alias. Maximum length: `128`.
@@ -249,18 +249,18 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    f1 = aiven.get_mirror_maker_replication_flow(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        source_cluster=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        target_cluster=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    f1 = aiven.get_mirror_maker_replication_flow(project=aiven_project["kafka-mm-project1"]["project"],
+        service_name=aiven_kafka["mm"]["service_name"],
+        source_cluster=aiven_kafka["source"]["service_name"],
+        target_cluster=aiven_kafka["target"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str source_cluster: Source cluster alias. Maximum length: `128`.
     :param str target_cluster: Target cluster alias. Maximum length: `128`.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_my_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mysql1 = aiven.get_my_sql(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mysql1 = aiven.get_my_sql(project=data["aiven_project"]["foo"]["project"],
         service_name="my-mysql1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mysql1 = aiven.get_my_sql(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mysql1 = aiven.get_my_sql(project=data["aiven_project"]["foo"]["project"],
         service_name="my-mysql1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg_database.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,32 +6,38 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetMysqlDatabaseResult',
-    'AwaitableGetMysqlDatabaseResult',
-    'get_mysql_database',
-    'get_mysql_database_output',
+    'GetPgDatabaseResult',
+    'AwaitableGetPgDatabaseResult',
+    'get_pg_database',
+    'get_pg_database_output',
 ]
 
 @pulumi.output_type
-class GetMysqlDatabaseResult:
+class GetPgDatabaseResult:
     """
-    A collection of values returned by getMysqlDatabase.
+    A collection of values returned by getPgDatabase.
     """
-    def __init__(__self__, database_name=None, id=None, project=None, service_name=None, termination_protection=None):
+    def __init__(__self__, database_name=None, id=None, lc_collate=None, lc_ctype=None, project=None, service_name=None, termination_protection=None):
         if database_name and not isinstance(database_name, str):
             raise TypeError("Expected argument 'database_name' to be a str")
         pulumi.set(__self__, "database_name", database_name)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if lc_collate and not isinstance(lc_collate, str):
+            raise TypeError("Expected argument 'lc_collate' to be a str")
+        pulumi.set(__self__, "lc_collate", lc_collate)
+        if lc_ctype and not isinstance(lc_ctype, str):
+            raise TypeError("Expected argument 'lc_ctype' to be a str")
+        pulumi.set(__self__, "lc_ctype", lc_ctype)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
         if termination_protection and not isinstance(termination_protection, bool):
@@ -51,14 +57,30 @@
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="lcCollate")
+    def lc_collate(self) -> str:
+        """
+        Default string sort order (`LC_COLLATE`) of the database. The default value is `en_US.UTF-8`. This property cannot be changed, doing so forces recreation of the resource.
+        """
+        return pulumi.get(self, "lc_collate")
+
+    @property
+    @pulumi.getter(name="lcCtype")
+    def lc_ctype(self) -> str:
+        """
+        Default character classification (`LC_CTYPE`) of the database. The default value is `en_US.UTF-8`. This property cannot be changed, doing so forces recreation of the resource.
+        """
+        return pulumi.get(self, "lc_ctype")
+
+    @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "project")
 
@@ -72,81 +94,85 @@
 
     @property
     @pulumi.getter(name="terminationProtection")
     def termination_protection(self) -> bool:
         return pulumi.get(self, "termination_protection")
 
 
-class AwaitableGetMysqlDatabaseResult(GetMysqlDatabaseResult):
+class AwaitableGetPgDatabaseResult(GetPgDatabaseResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetMysqlDatabaseResult(
+        return GetPgDatabaseResult(
             database_name=self.database_name,
             id=self.id,
+            lc_collate=self.lc_collate,
+            lc_ctype=self.lc_ctype,
             project=self.project,
             service_name=self.service_name,
             termination_protection=self.termination_protection)
 
 
-def get_mysql_database(database_name: Optional[str] = None,
-                       project: Optional[str] = None,
-                       service_name: Optional[str] = None,
-                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMysqlDatabaseResult:
+def get_pg_database(database_name: Optional[str] = None,
+                    project: Optional[str] = None,
+                    service_name: Optional[str] = None,
+                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPgDatabaseResult:
     """
-    The MySQL Database data source provides information about the existing Aiven MySQL Database.
+    The PG Database data source provides information about the existing Aiven PostgreSQL Database.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mydatabase = aiven.get_mysql_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mydatabase = aiven.get_pg_database(project=aiven_project["myproject"]["project"],
+        service_name=aiven_pg["mypg"]["service_name"],
         database_name="<DATABASE_NAME>")
     ```
 
 
     :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['databaseName'] = database_name
     __args__['project'] = project
     __args__['serviceName'] = service_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getMysqlDatabase:getMysqlDatabase', __args__, opts=opts, typ=GetMysqlDatabaseResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getPgDatabase:getPgDatabase', __args__, opts=opts, typ=GetPgDatabaseResult).value
 
-    return AwaitableGetMysqlDatabaseResult(
+    return AwaitableGetPgDatabaseResult(
         database_name=__ret__.database_name,
         id=__ret__.id,
+        lc_collate=__ret__.lc_collate,
+        lc_ctype=__ret__.lc_ctype,
         project=__ret__.project,
         service_name=__ret__.service_name,
         termination_protection=__ret__.termination_protection)
 
 
-@_utilities.lift_output_func(get_mysql_database)
-def get_mysql_database_output(database_name: Optional[pulumi.Input[str]] = None,
-                              project: Optional[pulumi.Input[str]] = None,
-                              service_name: Optional[pulumi.Input[str]] = None,
-                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMysqlDatabaseResult]:
+@_utilities.lift_output_func(get_pg_database)
+def get_pg_database_output(database_name: Optional[pulumi.Input[str]] = None,
+                           project: Optional[pulumi.Input[str]] = None,
+                           service_name: Optional[pulumi.Input[str]] = None,
+                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPgDatabaseResult]:
     """
-    The MySQL Database data source provides information about the existing Aiven MySQL Database.
+    The PG Database data source provides information about the existing Aiven PostgreSQL Database.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mydatabase = aiven.get_mysql_database(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mydatabase = aiven.get_pg_database(project=aiven_project["myproject"]["project"],
+        service_name=aiven_pg["mypg"]["service_name"],
         database_name="<DATABASE_NAME>")
     ```
 
 
     :param str database_name: The name of the service database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os1 = aiven.get_open_search(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    os1 = aiven.get_open_search(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-os1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os1 = aiven.get_open_search(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    os1 = aiven.get_open_search(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-os1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search_acl_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -100,16 +100,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os_acl_config = aiven.get_open_search_acl_config(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    os_acl_config = aiven.get_open_search_acl_config(project=aiven_project["os-project"]["project"],
+        service_name=aiven_opensearch["os"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
@@ -135,16 +135,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os_acl_config = aiven.get_open_search_acl_config(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    os_acl_config = aiven.get_open_search_acl_config(project=aiven_project["os-project"]["project"],
+        service_name=aiven_opensearch["os"]["service_name"])
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,16 +115,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os_acl_rule = aiven.get_open_search_acl_rule(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    os_acl_rule = aiven.get_open_search_acl_rule(project=aiven_opensearch_acl_config["os_acls_config"]["project"],
+        service_name=aiven_opensearch_acl_config["os_acls_config"]["service_name"],
         username="<USERNAME>",
         index="<INDEX>")
     ```
 
 
     :param str index: The index pattern for this ACL entry. Maximum length: `249`. This property cannot be changed, doing so forces recreation of the resource.
     :param str permission: The permissions for this ACL entry. The possible values are `deny`, `admin`, `read`, `readwrite` and `write`.
@@ -162,16 +162,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    os_acl_rule = aiven.get_open_search_acl_rule(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    os_acl_rule = aiven.get_open_search_acl_rule(project=aiven_opensearch_acl_config["os_acls_config"]["project"],
+        service_name=aiven_opensearch_acl_config["os_acls_config"]["service_name"],
         username="<USERNAME>",
         index="<INDEX>")
     ```
 
 
     :param str index: The index pattern for this ACL entry. Maximum length: `249`. This property cannot be changed, doing so forces recreation of the resource.
     :param str permission: The permissions for this ACL entry. The possible values are `deny`, `admin`, `read`, `readwrite` and `write`.
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_clickhouse_database.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,60 +6,57 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetOpensearchUserResult',
-    'AwaitableGetOpensearchUserResult',
-    'get_opensearch_user',
-    'get_opensearch_user_output',
+    'GetClickhouseDatabaseResult',
+    'AwaitableGetClickhouseDatabaseResult',
+    'get_clickhouse_database',
+    'get_clickhouse_database_output',
 ]
 
 @pulumi.output_type
-class GetOpensearchUserResult:
+class GetClickhouseDatabaseResult:
     """
-    A collection of values returned by getOpensearchUser.
+    A collection of values returned by getClickhouseDatabase.
     """
-    def __init__(__self__, id=None, password=None, project=None, service_name=None, type=None, username=None):
+    def __init__(__self__, id=None, name=None, project=None, service_name=None, termination_protection=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if password and not isinstance(password, str):
-            raise TypeError("Expected argument 'password' to be a str")
-        pulumi.set(__self__, "password", password)
+        if name and not isinstance(name, str):
+            raise TypeError("Expected argument 'name' to be a str")
+        pulumi.set(__self__, "name", name)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
-        if username and not isinstance(username, str):
-            raise TypeError("Expected argument 'username' to be a str")
-        pulumi.set(__self__, "username", username)
+        if termination_protection and not isinstance(termination_protection, bool):
+            raise TypeError("Expected argument 'termination_protection' to be a bool")
+        pulumi.set(__self__, "termination_protection", termination_protection)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
-    def password(self) -> str:
+    def name(self) -> str:
         """
-        The password of the Opensearch User.
+        The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def project(self) -> str:
         """
         Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -70,101 +67,88 @@
     def service_name(self) -> str:
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "service_name")
 
     @property
-    @pulumi.getter
-    def type(self) -> str:
-        """
-        Type of the user account. Tells whether the user is the primary account or a regular account.
-        """
-        return pulumi.get(self, "type")
-
-    @property
-    @pulumi.getter
-    def username(self) -> str:
-        """
-        The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-        """
-        return pulumi.get(self, "username")
+    @pulumi.getter(name="terminationProtection")
+    def termination_protection(self) -> bool:
+        return pulumi.get(self, "termination_protection")
 
 
-class AwaitableGetOpensearchUserResult(GetOpensearchUserResult):
+class AwaitableGetClickhouseDatabaseResult(GetClickhouseDatabaseResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetOpensearchUserResult(
+        return GetClickhouseDatabaseResult(
             id=self.id,
-            password=self.password,
+            name=self.name,
             project=self.project,
             service_name=self.service_name,
-            type=self.type,
-            username=self.username)
+            termination_protection=self.termination_protection)
 
 
-def get_opensearch_user(project: Optional[str] = None,
-                        service_name: Optional[str] = None,
-                        username: Optional[str] = None,
-                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOpensearchUserResult:
+def get_clickhouse_database(name: Optional[str] = None,
+                            project: Optional[str] = None,
+                            service_name: Optional[str] = None,
+                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClickhouseDatabaseResult:
     """
-    The Opensearch User data source provides information about the existing Aiven Cassandra User.
+    The Clickhouse database data source provides information about the existing Aiven Clickhouse Database.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_opensearch_user(project="my-project",
-        service_name="my-service",
-        username="user1")
+    clickhouse_db = aiven.get_clickhouse_database(project=aiven_clickhouse["ch"]["project"],
+        service_name=aiven_clickhouse["ch"]["service_name"],
+        name="my-ch-db")
     ```
 
 
+    :param str name: The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
+    __args__['name'] = name
     __args__['project'] = project
     __args__['serviceName'] = service_name
-    __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getOpensearchUser:getOpensearchUser', __args__, opts=opts, typ=GetOpensearchUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getClickhouseDatabase:getClickhouseDatabase', __args__, opts=opts, typ=GetClickhouseDatabaseResult).value
 
-    return AwaitableGetOpensearchUserResult(
+    return AwaitableGetClickhouseDatabaseResult(
         id=__ret__.id,
-        password=__ret__.password,
+        name=__ret__.name,
         project=__ret__.project,
         service_name=__ret__.service_name,
-        type=__ret__.type,
-        username=__ret__.username)
+        termination_protection=__ret__.termination_protection)
 
 
-@_utilities.lift_output_func(get_opensearch_user)
-def get_opensearch_user_output(project: Optional[pulumi.Input[str]] = None,
-                               service_name: Optional[pulumi.Input[str]] = None,
-                               username: Optional[pulumi.Input[str]] = None,
-                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOpensearchUserResult]:
+@_utilities.lift_output_func(get_clickhouse_database)
+def get_clickhouse_database_output(name: Optional[pulumi.Input[str]] = None,
+                                   project: Optional[pulumi.Input[str]] = None,
+                                   service_name: Optional[pulumi.Input[str]] = None,
+                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClickhouseDatabaseResult]:
     """
-    The Opensearch User data source provides information about the existing Aiven Cassandra User.
+    The Clickhouse database data source provides information about the existing Aiven Clickhouse Database.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_opensearch_user(project="my-project",
-        service_name="my-service",
-        username="user1")
+    clickhouse_db = aiven.get_clickhouse_database(project=aiven_clickhouse["ch"]["project"],
+        service_name=aiven_clickhouse["ch"]["service_name"],
+        name="my-ch-db")
     ```
 
 
+    :param str name: The name of the Clickhouse database. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Opensearch User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_organization.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_organizational_unit.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_pg.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    pg = aiven.get_pg(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    pg = aiven.get_pg(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-pg1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    pg = aiven.get_pg(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    pg = aiven.get_pg(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-pg1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_redis_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,101 +6,112 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetPgUserResult',
-    'AwaitableGetPgUserResult',
-    'get_pg_user',
-    'get_pg_user_output',
+    'GetRedisUserResult',
+    'AwaitableGetRedisUserResult',
+    'get_redis_user',
+    'get_redis_user_output',
 ]
 
 @pulumi.output_type
-class GetPgUserResult:
+class GetRedisUserResult:
     """
-    A collection of values returned by getPgUser.
+    A collection of values returned by getRedisUser.
     """
-    def __init__(__self__, access_cert=None, access_key=None, id=None, password=None, pg_allow_replication=None, project=None, service_name=None, type=None, username=None):
-        if access_cert and not isinstance(access_cert, str):
-            raise TypeError("Expected argument 'access_cert' to be a str")
-        pulumi.set(__self__, "access_cert", access_cert)
-        if access_key and not isinstance(access_key, str):
-            raise TypeError("Expected argument 'access_key' to be a str")
-        pulumi.set(__self__, "access_key", access_key)
+    def __init__(__self__, id=None, password=None, project=None, redis_acl_categories=None, redis_acl_channels=None, redis_acl_commands=None, redis_acl_keys=None, service_name=None, type=None, username=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if password and not isinstance(password, str):
             raise TypeError("Expected argument 'password' to be a str")
         pulumi.set(__self__, "password", password)
-        if pg_allow_replication and not isinstance(pg_allow_replication, bool):
-            raise TypeError("Expected argument 'pg_allow_replication' to be a bool")
-        pulumi.set(__self__, "pg_allow_replication", pg_allow_replication)
         if project and not isinstance(project, str):
             raise TypeError("Expected argument 'project' to be a str")
         pulumi.set(__self__, "project", project)
+        if redis_acl_categories and not isinstance(redis_acl_categories, list):
+            raise TypeError("Expected argument 'redis_acl_categories' to be a list")
+        pulumi.set(__self__, "redis_acl_categories", redis_acl_categories)
+        if redis_acl_channels and not isinstance(redis_acl_channels, list):
+            raise TypeError("Expected argument 'redis_acl_channels' to be a list")
+        pulumi.set(__self__, "redis_acl_channels", redis_acl_channels)
+        if redis_acl_commands and not isinstance(redis_acl_commands, list):
+            raise TypeError("Expected argument 'redis_acl_commands' to be a list")
+        pulumi.set(__self__, "redis_acl_commands", redis_acl_commands)
+        if redis_acl_keys and not isinstance(redis_acl_keys, list):
+            raise TypeError("Expected argument 'redis_acl_keys' to be a list")
+        pulumi.set(__self__, "redis_acl_keys", redis_acl_keys)
         if service_name and not isinstance(service_name, str):
             raise TypeError("Expected argument 'service_name' to be a str")
         pulumi.set(__self__, "service_name", service_name)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
         if username and not isinstance(username, str):
             raise TypeError("Expected argument 'username' to be a str")
         pulumi.set(__self__, "username", username)
 
     @property
-    @pulumi.getter(name="accessCert")
-    def access_cert(self) -> str:
+    @pulumi.getter
+    def id(self) -> str:
         """
-        Access certificate for the user
+        The provider-assigned unique ID for this managed resource.
         """
-        return pulumi.get(self, "access_cert")
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="accessKey")
-    def access_key(self) -> str:
+    @pulumi.getter
+    def password(self) -> str:
         """
-        Access certificate key for the user
+        The password of the Redis User.
         """
-        return pulumi.get(self, "access_key")
+        return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def project(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter
-    def password(self) -> str:
+    @pulumi.getter(name="redisAclCategories")
+    def redis_acl_categories(self) -> Sequence[str]:
         """
-        The password of the PG User ( not applicable for all services ).
+        Defines command category rules. The field is required with`redis_acl_commands` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "redis_acl_categories")
 
     @property
-    @pulumi.getter(name="pgAllowReplication")
-    def pg_allow_replication(self) -> bool:
+    @pulumi.getter(name="redisAclChannels")
+    def redis_acl_channels(self) -> Sequence[str]:
         """
-        Defines whether replication is allowed. This property cannot be changed, doing so forces recreation of the resource.
+        Defines the permitted pub/sub channel patterns. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "pg_allow_replication")
+        return pulumi.get(self, "redis_acl_channels")
 
     @property
-    @pulumi.getter
-    def project(self) -> str:
+    @pulumi.getter(name="redisAclCommands")
+    def redis_acl_commands(self) -> Sequence[str]:
         """
-        Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        Defines rules for individual commands. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "redis_acl_commands")
+
+    @property
+    @pulumi.getter(name="redisAclKeys")
+    def redis_acl_keys(self) -> Sequence[str]:
+        """
+        Defines key access rules. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
+        """
+        return pulumi.get(self, "redis_acl_keys")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
         """
         Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -114,96 +125,98 @@
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "username")
 
 
-class AwaitableGetPgUserResult(GetPgUserResult):
+class AwaitableGetRedisUserResult(GetRedisUserResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetPgUserResult(
-            access_cert=self.access_cert,
-            access_key=self.access_key,
+        return GetRedisUserResult(
             id=self.id,
             password=self.password,
-            pg_allow_replication=self.pg_allow_replication,
             project=self.project,
+            redis_acl_categories=self.redis_acl_categories,
+            redis_acl_channels=self.redis_acl_channels,
+            redis_acl_commands=self.redis_acl_commands,
+            redis_acl_keys=self.redis_acl_keys,
             service_name=self.service_name,
             type=self.type,
             username=self.username)
 
 
-def get_pg_user(project: Optional[str] = None,
-                service_name: Optional[str] = None,
-                username: Optional[str] = None,
-                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPgUserResult:
+def get_redis_user(project: Optional[str] = None,
+                   service_name: Optional[str] = None,
+                   username: Optional[str] = None,
+                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRedisUserResult:
     """
-    The PG User data source provides information about the existing Aiven PG User.
+    The Redis User data source provides information about the existing Aiven Redis User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_pg_user(project="my-project",
+    user = aiven.get_redis_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
     __args__['project'] = project
     __args__['serviceName'] = service_name
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getPgUser:getPgUser', __args__, opts=opts, typ=GetPgUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getRedisUser:getRedisUser', __args__, opts=opts, typ=GetRedisUserResult).value
 
-    return AwaitableGetPgUserResult(
-        access_cert=__ret__.access_cert,
-        access_key=__ret__.access_key,
+    return AwaitableGetRedisUserResult(
         id=__ret__.id,
         password=__ret__.password,
-        pg_allow_replication=__ret__.pg_allow_replication,
         project=__ret__.project,
+        redis_acl_categories=__ret__.redis_acl_categories,
+        redis_acl_channels=__ret__.redis_acl_channels,
+        redis_acl_commands=__ret__.redis_acl_commands,
+        redis_acl_keys=__ret__.redis_acl_keys,
         service_name=__ret__.service_name,
         type=__ret__.type,
         username=__ret__.username)
 
 
-@_utilities.lift_output_func(get_pg_user)
-def get_pg_user_output(project: Optional[pulumi.Input[str]] = None,
-                       service_name: Optional[pulumi.Input[str]] = None,
-                       username: Optional[pulumi.Input[str]] = None,
-                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPgUserResult]:
+@_utilities.lift_output_func(get_redis_user)
+def get_redis_user_output(project: Optional[pulumi.Input[str]] = None,
+                          service_name: Optional[pulumi.Input[str]] = None,
+                          username: Optional[pulumi.Input[str]] = None,
+                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRedisUserResult]:
     """
-    The PG User data source provides information about the existing Aiven PG User.
+    The Redis User data source provides information about the existing Aiven Redis User.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_pg_user(project="my-project",
+    user = aiven.get_redis_user(project="my-project",
         service_name="my-service",
         username="user1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the PG User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str username: The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_project.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestuser = aiven.get_project_user(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mytestuser = aiven.get_project_user(project=aiven_project["myproject"]["project"],
         email="john.doe@example.com")
     ```
 
 
     :param str email: Email address of the user. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
@@ -135,15 +135,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    mytestuser = aiven.get_project_user(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    mytestuser = aiven.get_project_user(project=aiven_project["myproject"]["project"],
         email="john.doe@example.com")
     ```
 
 
     :param str email: Email address of the user. This property cannot be changed, doing so forces recreation of the resource.
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_project_vpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -113,17 +113,17 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myvpc = aiven.get_project_vpc(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    myvpc = aiven.get_project_vpc(project=aiven_project["myproject"]["project"],
         cloud_name="google-europe-west1")
-    myvpc_id = aiven.get_project_vpc(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    myvpc_id = aiven.get_project_vpc(vpc_id=aiven_project_vpc["vpc"]["id"])
     ```
 
 
     :param str cloud_name: Defines where the cloud provider and region where the service is hosted in. See the Service resource for additional information.
     :param str project: Identifies the project this resource belongs to.
     :param str vpc_id: ID of the VPC. This can be used to filter out the specific VPC if there are more than one datasource returned.
     """
@@ -153,17 +153,17 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myvpc = aiven.get_project_vpc(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    myvpc = aiven.get_project_vpc(project=aiven_project["myproject"]["project"],
         cloud_name="google-europe-west1")
-    myvpc_id = aiven.get_project_vpc(vpc_id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    myvpc_id = aiven.get_project_vpc(vpc_id=aiven_project_vpc["vpc"]["id"])
     ```
 
 
     :param str cloud_name: Defines where the cloud provider and region where the service is hosted in. See the Service resource for additional information.
     :param str project: Identifies the project this resource belongs to.
     :param str vpc_id: ID of the VPC. This can be used to filter out the specific VPC if there are more than one datasource returned.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    redis1 = aiven.get_redis(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    redis1 = aiven.get_redis(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-redis1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
@@ -435,15 +435,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    redis1 = aiven.get_redis(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    redis1 = aiven.get_redis(project=data["aiven_project"]["pr1"]["project"],
         service_name="my-redis1")
     ```
 
 
     :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     :param str service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,217 +6,204 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetRedisUserResult',
-    'AwaitableGetRedisUserResult',
-    'get_redis_user',
-    'get_redis_user_output',
+    'GetTransitGatewayVpcAttachmentResult',
+    'AwaitableGetTransitGatewayVpcAttachmentResult',
+    'get_transit_gateway_vpc_attachment',
+    'get_transit_gateway_vpc_attachment_output',
 ]
 
 @pulumi.output_type
-class GetRedisUserResult:
+class GetTransitGatewayVpcAttachmentResult:
     """
-    A collection of values returned by getRedisUser.
+    A collection of values returned by getTransitGatewayVpcAttachment.
     """
-    def __init__(__self__, id=None, password=None, project=None, redis_acl_categories=None, redis_acl_channels=None, redis_acl_commands=None, redis_acl_keys=None, service_name=None, type=None, username=None):
+    def __init__(__self__, id=None, peer_cloud_account=None, peer_region=None, peer_vpc=None, peering_connection_id=None, state=None, state_info=None, user_peer_network_cidrs=None, vpc_id=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if password and not isinstance(password, str):
-            raise TypeError("Expected argument 'password' to be a str")
-        pulumi.set(__self__, "password", password)
-        if project and not isinstance(project, str):
-            raise TypeError("Expected argument 'project' to be a str")
-        pulumi.set(__self__, "project", project)
-        if redis_acl_categories and not isinstance(redis_acl_categories, list):
-            raise TypeError("Expected argument 'redis_acl_categories' to be a list")
-        pulumi.set(__self__, "redis_acl_categories", redis_acl_categories)
-        if redis_acl_channels and not isinstance(redis_acl_channels, list):
-            raise TypeError("Expected argument 'redis_acl_channels' to be a list")
-        pulumi.set(__self__, "redis_acl_channels", redis_acl_channels)
-        if redis_acl_commands and not isinstance(redis_acl_commands, list):
-            raise TypeError("Expected argument 'redis_acl_commands' to be a list")
-        pulumi.set(__self__, "redis_acl_commands", redis_acl_commands)
-        if redis_acl_keys and not isinstance(redis_acl_keys, list):
-            raise TypeError("Expected argument 'redis_acl_keys' to be a list")
-        pulumi.set(__self__, "redis_acl_keys", redis_acl_keys)
-        if service_name and not isinstance(service_name, str):
-            raise TypeError("Expected argument 'service_name' to be a str")
-        pulumi.set(__self__, "service_name", service_name)
-        if type and not isinstance(type, str):
-            raise TypeError("Expected argument 'type' to be a str")
-        pulumi.set(__self__, "type", type)
-        if username and not isinstance(username, str):
-            raise TypeError("Expected argument 'username' to be a str")
-        pulumi.set(__self__, "username", username)
+        if peer_cloud_account and not isinstance(peer_cloud_account, str):
+            raise TypeError("Expected argument 'peer_cloud_account' to be a str")
+        pulumi.set(__self__, "peer_cloud_account", peer_cloud_account)
+        if peer_region and not isinstance(peer_region, str):
+            raise TypeError("Expected argument 'peer_region' to be a str")
+        pulumi.set(__self__, "peer_region", peer_region)
+        if peer_vpc and not isinstance(peer_vpc, str):
+            raise TypeError("Expected argument 'peer_vpc' to be a str")
+        pulumi.set(__self__, "peer_vpc", peer_vpc)
+        if peering_connection_id and not isinstance(peering_connection_id, str):
+            raise TypeError("Expected argument 'peering_connection_id' to be a str")
+        pulumi.set(__self__, "peering_connection_id", peering_connection_id)
+        if state and not isinstance(state, str):
+            raise TypeError("Expected argument 'state' to be a str")
+        pulumi.set(__self__, "state", state)
+        if state_info and not isinstance(state_info, dict):
+            raise TypeError("Expected argument 'state_info' to be a dict")
+        pulumi.set(__self__, "state_info", state_info)
+        if user_peer_network_cidrs and not isinstance(user_peer_network_cidrs, list):
+            raise TypeError("Expected argument 'user_peer_network_cidrs' to be a list")
+        pulumi.set(__self__, "user_peer_network_cidrs", user_peer_network_cidrs)
+        if vpc_id and not isinstance(vpc_id, str):
+            raise TypeError("Expected argument 'vpc_id' to be a str")
+        pulumi.set(__self__, "vpc_id", vpc_id)
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter
-    def password(self) -> str:
+    @pulumi.getter(name="peerCloudAccount")
+    def peer_cloud_account(self) -> str:
         """
-        The password of the Redis User.
+        AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "peer_cloud_account")
 
     @property
-    @pulumi.getter
-    def project(self) -> str:
+    @pulumi.getter(name="peerRegion")
+    def peer_region(self) -> str:
         """
-        Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        AWS region of the peered VPC (if not in the same region as Aiven VPC)
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "peer_region")
 
     @property
-    @pulumi.getter(name="redisAclCategories")
-    def redis_acl_categories(self) -> Sequence[str]:
+    @pulumi.getter(name="peerVpc")
+    def peer_vpc(self) -> str:
         """
-        Defines command category rules. The field is required with`redis_acl_commands` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
+        Transit gateway ID. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "redis_acl_categories")
+        return pulumi.get(self, "peer_vpc")
 
     @property
-    @pulumi.getter(name="redisAclChannels")
-    def redis_acl_channels(self) -> Sequence[str]:
+    @pulumi.getter(name="peeringConnectionId")
+    def peering_connection_id(self) -> str:
         """
-        Defines the permitted pub/sub channel patterns. This property cannot be changed, doing so forces recreation of the resource.
+        Cloud provider identifier for the peering connection if available
         """
-        return pulumi.get(self, "redis_acl_channels")
+        return pulumi.get(self, "peering_connection_id")
 
     @property
-    @pulumi.getter(name="redisAclCommands")
-    def redis_acl_commands(self) -> Sequence[str]:
-        """
-        Defines rules for individual commands. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
-        """
-        return pulumi.get(self, "redis_acl_commands")
-
-    @property
-    @pulumi.getter(name="redisAclKeys")
-    def redis_acl_keys(self) -> Sequence[str]:
+    @pulumi.getter
+    def state(self) -> str:
         """
-        Defines key access rules. The field is required with`redis_acl_categories` and `redis_acl_keys`. This property cannot be changed, doing so forces recreation of the resource.
+        State of the peering connection
         """
-        return pulumi.get(self, "redis_acl_keys")
+        return pulumi.get(self, "state")
 
     @property
-    @pulumi.getter(name="serviceName")
-    def service_name(self) -> str:
+    @pulumi.getter(name="stateInfo")
+    def state_info(self) -> Mapping[str, Any]:
         """
-        Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        State-specific help or error information
         """
-        return pulumi.get(self, "service_name")
+        return pulumi.get(self, "state_info")
 
     @property
-    @pulumi.getter
-    def type(self) -> str:
+    @pulumi.getter(name="userPeerNetworkCidrs")
+    def user_peer_network_cidrs(self) -> Sequence[str]:
         """
-        Type of the user account. Tells whether the user is the primary account or a regular account.
+        List of private IPv4 ranges to route through the peering connection
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "user_peer_network_cidrs")
 
     @property
-    @pulumi.getter
-    def username(self) -> str:
+    @pulumi.getter(name="vpcId")
+    def vpc_id(self) -> str:
         """
-        The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        The VPC the peering connection belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "vpc_id")
 
 
-class AwaitableGetRedisUserResult(GetRedisUserResult):
+class AwaitableGetTransitGatewayVpcAttachmentResult(GetTransitGatewayVpcAttachmentResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetRedisUserResult(
+        return GetTransitGatewayVpcAttachmentResult(
             id=self.id,
-            password=self.password,
-            project=self.project,
-            redis_acl_categories=self.redis_acl_categories,
-            redis_acl_channels=self.redis_acl_channels,
-            redis_acl_commands=self.redis_acl_commands,
-            redis_acl_keys=self.redis_acl_keys,
-            service_name=self.service_name,
-            type=self.type,
-            username=self.username)
-
-
-def get_redis_user(project: Optional[str] = None,
-                   service_name: Optional[str] = None,
-                   username: Optional[str] = None,
-                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRedisUserResult:
+            peer_cloud_account=self.peer_cloud_account,
+            peer_region=self.peer_region,
+            peer_vpc=self.peer_vpc,
+            peering_connection_id=self.peering_connection_id,
+            state=self.state,
+            state_info=self.state_info,
+            user_peer_network_cidrs=self.user_peer_network_cidrs,
+            vpc_id=self.vpc_id)
+
+
+def get_transit_gateway_vpc_attachment(peer_cloud_account: Optional[str] = None,
+                                       peer_vpc: Optional[str] = None,
+                                       vpc_id: Optional[str] = None,
+                                       opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTransitGatewayVpcAttachmentResult:
     """
-    The Redis User data source provides information about the existing Aiven Redis User.
+    The Transit Gateway VPC Attachment resource allows the creation and management Transit Gateway VPC Attachment VPC peering connection between Aiven and AWS.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_redis_user(project="my-project",
-        service_name="my-service",
-        username="user1")
+    attachment = aiven.get_transit_gateway_vpc_attachment(vpc_id=aiven_project_vpc["bar"]["id"],
+        peer_cloud_account="<PEER_ACCOUNT_ID>",
+        peer_vpc="google-project1")
     ```
 
 
-    :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str peer_cloud_account: AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
+    :param str peer_vpc: Transit gateway ID. This property cannot be changed, doing so forces recreation of the resource.
+    :param str vpc_id: The VPC the peering connection belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     __args__ = dict()
-    __args__['project'] = project
-    __args__['serviceName'] = service_name
-    __args__['username'] = username
+    __args__['peerCloudAccount'] = peer_cloud_account
+    __args__['peerVpc'] = peer_vpc
+    __args__['vpcId'] = vpc_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('aiven:index/getRedisUser:getRedisUser', __args__, opts=opts, typ=GetRedisUserResult).value
+    __ret__ = pulumi.runtime.invoke('aiven:index/getTransitGatewayVpcAttachment:getTransitGatewayVpcAttachment', __args__, opts=opts, typ=GetTransitGatewayVpcAttachmentResult).value
 
-    return AwaitableGetRedisUserResult(
+    return AwaitableGetTransitGatewayVpcAttachmentResult(
         id=__ret__.id,
-        password=__ret__.password,
-        project=__ret__.project,
-        redis_acl_categories=__ret__.redis_acl_categories,
-        redis_acl_channels=__ret__.redis_acl_channels,
-        redis_acl_commands=__ret__.redis_acl_commands,
-        redis_acl_keys=__ret__.redis_acl_keys,
-        service_name=__ret__.service_name,
-        type=__ret__.type,
-        username=__ret__.username)
-
-
-@_utilities.lift_output_func(get_redis_user)
-def get_redis_user_output(project: Optional[pulumi.Input[str]] = None,
-                          service_name: Optional[pulumi.Input[str]] = None,
-                          username: Optional[pulumi.Input[str]] = None,
-                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRedisUserResult]:
+        peer_cloud_account=__ret__.peer_cloud_account,
+        peer_region=__ret__.peer_region,
+        peer_vpc=__ret__.peer_vpc,
+        peering_connection_id=__ret__.peering_connection_id,
+        state=__ret__.state,
+        state_info=__ret__.state_info,
+        user_peer_network_cidrs=__ret__.user_peer_network_cidrs,
+        vpc_id=__ret__.vpc_id)
+
+
+@_utilities.lift_output_func(get_transit_gateway_vpc_attachment)
+def get_transit_gateway_vpc_attachment_output(peer_cloud_account: Optional[pulumi.Input[str]] = None,
+                                              peer_vpc: Optional[pulumi.Input[str]] = None,
+                                              vpc_id: Optional[pulumi.Input[str]] = None,
+                                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTransitGatewayVpcAttachmentResult]:
     """
-    The Redis User data source provides information about the existing Aiven Redis User.
+    The Transit Gateway VPC Attachment resource allows the creation and management Transit Gateway VPC Attachment VPC peering connection between Aiven and AWS.
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    user = aiven.get_redis_user(project="my-project",
-        service_name="my-service",
-        username="user1")
+    attachment = aiven.get_transit_gateway_vpc_attachment(vpc_id=aiven_project_vpc["bar"]["id"],
+        peer_cloud_account="<PEER_ACCOUNT_ID>",
+        peer_vpc="google-project1")
     ```
 
 
-    :param str project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
-    :param str username: The actual name of the Redis User. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+    :param str peer_cloud_account: AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
+    :param str peer_vpc: Transit gateway ID. This property cannot be changed, doing so forces recreation of the resource.
+    :param str vpc_id: The VPC the peering connection belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
     """
     ...
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,16 +167,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    sc1 = aiven.get_service_component(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    sc1 = aiven.get_service_component(project=aiven_kafka["project1"]["project"],
+        service_name=aiven_kafka["service1"]["service_name"],
         component="kafka",
         route="dynamic",
         kafka_authentication_method="certificate")
     ```
 
 
     :param str component: Service component name
@@ -227,16 +227,16 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    sc1 = aiven.get_service_component(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
-        service_name=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    sc1 = aiven.get_service_component(project=aiven_kafka["project1"]["project"],
+        service_name=aiven_kafka["service1"]["service_name"],
         component="kafka",
         route="dynamic",
         kafka_authentication_method="certificate")
     ```
 
 
     :param str component: Service component name
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myintegration = aiven.get_service_integration(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    myintegration = aiven.get_service_integration(project=aiven_project["myproject"]["project"],
         destination_service_name="<DESTINATION_SERVICE_NAME>",
         integration_type="datadog",
         source_service_name="<SOURCE_SERVICE_NAME>")
     ```
 
 
     :param str destination_service_name: Destination service for the integration (if any)
@@ -306,15 +306,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myintegration = aiven.get_service_integration(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    myintegration = aiven.get_service_integration(project=aiven_project["myproject"]["project"],
         destination_service_name="<DESTINATION_SERVICE_NAME>",
         integration_type="datadog",
         source_service_name="<SOURCE_SERVICE_NAME>")
     ```
 
 
     :param str destination_service_name: Destination service for the integration (if any)
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myendpoint = aiven.get_service_integration_endpoint(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    myendpoint = aiven.get_service_integration_endpoint(project=aiven_project["myproject"]["project"],
         endpoint_name="<ENDPOINT_NAME>")
     ```
 
 
     :param str endpoint_name: Name of the service integration endpoint
     :param str project: Project the service integration endpoint belongs to
     """
@@ -279,15 +279,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_aiven as aiven
 
-    myendpoint = aiven.get_service_integration_endpoint(project=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference),
+    myendpoint = aiven.get_service_integration_endpoint(project=aiven_project["myproject"]["project"],
         endpoint_name="<ENDPOINT_NAME>")
     ```
 
 
     :param str endpoint_name: Name of the service integration endpoint
     :param str project: Project the service integration endpoint belongs to
     """
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/grafana.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_acl.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,28 @@
 @pulumi.input_type
 class KafkaAclArgs:
     def __init__(__self__, *,
                  permission: pulumi.Input[str],
                  project: pulumi.Input[str],
                  service_name: pulumi.Input[str],
                  topic: pulumi.Input[str],
-                 username: pulumi.Input[str],
-                 acl_id: Optional[pulumi.Input[str]] = None):
+                 username: pulumi.Input[str]):
         """
         The set of arguments for constructing a KafkaAcl resource.
         :param pulumi.Input[str] permission: Kafka permission to grant. The possible values are `admin`, `read`, `readwrite` and `write`. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] topic: Topic name pattern for the ACL entry. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: Username pattern for the ACL entry. This property cannot be changed, doing so forces recreation of the resource.
-        :param pulumi.Input[str] acl_id: Kafka ACL ID
         """
         pulumi.set(__self__, "permission", permission)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "service_name", service_name)
         pulumi.set(__self__, "topic", topic)
         pulumi.set(__self__, "username", username)
-        if acl_id is not None:
-            pulumi.set(__self__, "acl_id", acl_id)
 
     @property
     @pulumi.getter
     def permission(self) -> pulumi.Input[str]:
         """
         Kafka permission to grant. The possible values are `admin`, `read`, `readwrite` and `write`. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -93,26 +89,14 @@
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
-    @property
-    @pulumi.getter(name="aclId")
-    def acl_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Kafka ACL ID
-        """
-        return pulumi.get(self, "acl_id")
-
-    @acl_id.setter
-    def acl_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "acl_id", value)
-
 
 @pulumi.input_type
 class _KafkaAclState:
     def __init__(__self__, *,
                  acl_id: Optional[pulumi.Input[str]] = None,
                  permission: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
@@ -215,15 +199,14 @@
 
 
 class KafkaAcl(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 acl_id: Optional[pulumi.Input[str]] = None,
                  permission: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  topic: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
@@ -247,15 +230,14 @@
 
         ```sh
          $ pulumi import aiven:index/kafkaAcl:KafkaAcl mytestacl project/service_name/id
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] acl_id: Kafka ACL ID
         :param pulumi.Input[str] permission: Kafka permission to grant. The possible values are `admin`, `read`, `readwrite` and `write`. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] topic: Topic name pattern for the ACL entry. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: Username pattern for the ACL entry. This property cannot be changed, doing so forces recreation of the resource.
         """
         ...
@@ -298,30 +280,28 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 acl_id: Optional[pulumi.Input[str]] = None,
                  permission: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  topic: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KafkaAclArgs.__new__(KafkaAclArgs)
 
-            __props__.__dict__["acl_id"] = acl_id
             if permission is None and not opts.urn:
                 raise TypeError("Missing required property 'permission'")
             __props__.__dict__["permission"] = permission
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             if service_name is None and not opts.urn:
@@ -329,14 +309,15 @@
             __props__.__dict__["service_name"] = service_name
             if topic is None and not opts.urn:
                 raise TypeError("Missing required property 'topic'")
             __props__.__dict__["topic"] = topic
             if username is None and not opts.urn:
                 raise TypeError("Missing required property 'username'")
             __props__.__dict__["username"] = username
+            __props__.__dict__["acl_id"] = None
         super(KafkaAcl, __self__).__init__(
             'aiven:index/kafkaAcl:KafkaAcl',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,32 +14,28 @@
 @pulumi.input_type
 class KafkaSchemaRegistryAclArgs:
     def __init__(__self__, *,
                  permission: pulumi.Input[str],
                  project: pulumi.Input[str],
                  resource: pulumi.Input[str],
                  service_name: pulumi.Input[str],
-                 username: pulumi.Input[str],
-                 acl_id: Optional[pulumi.Input[str]] = None):
+                 username: pulumi.Input[str]):
         """
         The set of arguments for constructing a KafkaSchemaRegistryAcl resource.
         :param pulumi.Input[str] permission: Kafka Schema Registry permission to grant. The possible values are `schema_registry_read` and `schema_registry_write`. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] resource: Resource name pattern for the Schema Registry ACL entry. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: Username pattern for the ACL entry. This property cannot be changed, doing so forces recreation of the resource.
-        :param pulumi.Input[str] acl_id: Kafka Schema Registry ACL ID
         """
         pulumi.set(__self__, "permission", permission)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "resource", resource)
         pulumi.set(__self__, "service_name", service_name)
         pulumi.set(__self__, "username", username)
-        if acl_id is not None:
-            pulumi.set(__self__, "acl_id", acl_id)
 
     @property
     @pulumi.getter
     def permission(self) -> pulumi.Input[str]:
         """
         Kafka Schema Registry permission to grant. The possible values are `schema_registry_read` and `schema_registry_write`. This property cannot be changed, doing so forces recreation of the resource.
         """
@@ -93,26 +89,14 @@
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
-    @property
-    @pulumi.getter(name="aclId")
-    def acl_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Kafka Schema Registry ACL ID
-        """
-        return pulumi.get(self, "acl_id")
-
-    @acl_id.setter
-    def acl_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "acl_id", value)
-
 
 @pulumi.input_type
 class _KafkaSchemaRegistryAclState:
     def __init__(__self__, *,
                  acl_id: Optional[pulumi.Input[str]] = None,
                  permission: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
@@ -215,27 +199,25 @@
 
 
 class KafkaSchemaRegistryAcl(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 acl_id: Optional[pulumi.Input[str]] = None,
                  permission: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  resource: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The Resource Kafka Schema Registry ACL resource allows the creation and management of Schema Registry ACLs for an Aiven Kafka service.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] acl_id: Kafka Schema Registry ACL ID
         :param pulumi.Input[str] permission: Kafka Schema Registry permission to grant. The possible values are `schema_registry_read` and `schema_registry_write`. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] resource: Resource name pattern for the Schema Registry ACL entry. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the name of the service that this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] username: Username pattern for the ACL entry. This property cannot be changed, doing so forces recreation of the resource.
         """
         ...
@@ -258,30 +240,28 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 acl_id: Optional[pulumi.Input[str]] = None,
                  permission: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  resource: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = KafkaSchemaRegistryAclArgs.__new__(KafkaSchemaRegistryAclArgs)
 
-            __props__.__dict__["acl_id"] = acl_id
             if permission is None and not opts.urn:
                 raise TypeError("Missing required property 'permission'")
             __props__.__dict__["permission"] = permission
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             if resource is None and not opts.urn:
@@ -289,14 +269,15 @@
             __props__.__dict__["resource"] = resource
             if service_name is None and not opts.urn:
                 raise TypeError("Missing required property 'service_name'")
             __props__.__dict__["service_name"] = service_name
             if username is None and not opts.urn:
                 raise TypeError("Missing required property 'username'")
             __props__.__dict__["username"] = username
+            __props__.__dict__["acl_id"] = None
         super(KafkaSchemaRegistryAcl, __self__).__init__(
             'aiven:index/kafkaSchemaRegistryAcl:KafkaSchemaRegistryAcl',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/open_search.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/organization.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/organizational_unit.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/outputs.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -5252,14 +5252,16 @@
             suggest = "consumer_request_timeout_ms"
         elif key == "producerAcks":
             suggest = "producer_acks"
         elif key == "producerCompressionType":
             suggest = "producer_compression_type"
         elif key == "producerLingerMs":
             suggest = "producer_linger_ms"
+        elif key == "producerMaxRequestSize":
+            suggest = "producer_max_request_size"
         elif key == "simpleconsumerPoolSizeMax":
             suggest = "simpleconsumer_pool_size_max"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in KafkaKafkaUserConfigKafkaRestConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
@@ -5273,27 +5275,30 @@
     def __init__(__self__, *,
                  consumer_enable_auto_commit: Optional[bool] = None,
                  consumer_request_max_bytes: Optional[int] = None,
                  consumer_request_timeout_ms: Optional[int] = None,
                  producer_acks: Optional[str] = None,
                  producer_compression_type: Optional[str] = None,
                  producer_linger_ms: Optional[int] = None,
+                 producer_max_request_size: Optional[int] = None,
                  simpleconsumer_pool_size_max: Optional[int] = None):
         if consumer_enable_auto_commit is not None:
             pulumi.set(__self__, "consumer_enable_auto_commit", consumer_enable_auto_commit)
         if consumer_request_max_bytes is not None:
             pulumi.set(__self__, "consumer_request_max_bytes", consumer_request_max_bytes)
         if consumer_request_timeout_ms is not None:
             pulumi.set(__self__, "consumer_request_timeout_ms", consumer_request_timeout_ms)
         if producer_acks is not None:
             pulumi.set(__self__, "producer_acks", producer_acks)
         if producer_compression_type is not None:
             pulumi.set(__self__, "producer_compression_type", producer_compression_type)
         if producer_linger_ms is not None:
             pulumi.set(__self__, "producer_linger_ms", producer_linger_ms)
+        if producer_max_request_size is not None:
+            pulumi.set(__self__, "producer_max_request_size", producer_max_request_size)
         if simpleconsumer_pool_size_max is not None:
             pulumi.set(__self__, "simpleconsumer_pool_size_max", simpleconsumer_pool_size_max)
 
     @property
     @pulumi.getter(name="consumerEnableAutoCommit")
     def consumer_enable_auto_commit(self) -> Optional[bool]:
         return pulumi.get(self, "consumer_enable_auto_commit")
@@ -5320,14 +5325,19 @@
 
     @property
     @pulumi.getter(name="producerLingerMs")
     def producer_linger_ms(self) -> Optional[int]:
         return pulumi.get(self, "producer_linger_ms")
 
     @property
+    @pulumi.getter(name="producerMaxRequestSize")
+    def producer_max_request_size(self) -> Optional[int]:
+        return pulumi.get(self, "producer_max_request_size")
+
+    @property
     @pulumi.getter(name="simpleconsumerPoolSizeMax")
     def simpleconsumer_pool_size_max(self) -> Optional[int]:
         return pulumi.get(self, "simpleconsumer_pool_size_max")
 
 
 @pulumi.output_type
 class KafkaKafkaUserConfigPrivateAccess(dict):
@@ -6139,15 +6149,15 @@
         :param bool preallocate: preallocate value
         :param str retention_bytes: retention.bytes value
         :param str retention_ms: retention.ms value
         :param str segment_bytes: segment.bytes value
         :param str segment_index_bytes: segment.index.bytes value
         :param str segment_jitter_ms: segment.jitter.ms value
         :param str segment_ms: segment.ms value
-        :param bool unclean_leader_election_enable: unclean.leader.election.enable value
+        :param bool unclean_leader_election_enable: unclean.leader.election.enable value; This field is deprecated and no longer functional.
         """
         if cleanup_policy is not None:
             pulumi.set(__self__, "cleanup_policy", cleanup_policy)
         if compression_type is not None:
             pulumi.set(__self__, "compression_type", compression_type)
         if delete_retention_ms is not None:
             pulumi.set(__self__, "delete_retention_ms", delete_retention_ms)
@@ -6378,15 +6388,15 @@
         """
         return pulumi.get(self, "segment_ms")
 
     @property
     @pulumi.getter(name="uncleanLeaderElectionEnable")
     def unclean_leader_election_enable(self) -> Optional[bool]:
         """
-        unclean.leader.election.enable value
+        unclean.leader.election.enable value; This field is deprecated and no longer functional.
         """
         return pulumi.get(self, "unclean_leader_election_enable")
 
 
 @pulumi.output_type
 class KafkaTopicTag(dict):
     def __init__(__self__, *,
@@ -13327,14 +13337,16 @@
         suggest = None
         if key == "consumerFetchMinBytes":
             suggest = "consumer_fetch_min_bytes"
         elif key == "producerBatchSize":
             suggest = "producer_batch_size"
         elif key == "producerBufferMemory":
             suggest = "producer_buffer_memory"
+        elif key == "producerCompressionType":
+            suggest = "producer_compression_type"
         elif key == "producerLingerMs":
             suggest = "producer_linger_ms"
         elif key == "producerMaxRequestSize":
             suggest = "producer_max_request_size"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServiceIntegrationKafkaMirrormakerUserConfigKafkaMirrormaker. Access the value via the '{suggest}' property getter instead.")
@@ -13347,22 +13359,25 @@
         ServiceIntegrationKafkaMirrormakerUserConfigKafkaMirrormaker.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  consumer_fetch_min_bytes: Optional[int] = None,
                  producer_batch_size: Optional[int] = None,
                  producer_buffer_memory: Optional[int] = None,
+                 producer_compression_type: Optional[str] = None,
                  producer_linger_ms: Optional[int] = None,
                  producer_max_request_size: Optional[int] = None):
         if consumer_fetch_min_bytes is not None:
             pulumi.set(__self__, "consumer_fetch_min_bytes", consumer_fetch_min_bytes)
         if producer_batch_size is not None:
             pulumi.set(__self__, "producer_batch_size", producer_batch_size)
         if producer_buffer_memory is not None:
             pulumi.set(__self__, "producer_buffer_memory", producer_buffer_memory)
+        if producer_compression_type is not None:
+            pulumi.set(__self__, "producer_compression_type", producer_compression_type)
         if producer_linger_ms is not None:
             pulumi.set(__self__, "producer_linger_ms", producer_linger_ms)
         if producer_max_request_size is not None:
             pulumi.set(__self__, "producer_max_request_size", producer_max_request_size)
 
     @property
     @pulumi.getter(name="consumerFetchMinBytes")
@@ -13376,14 +13391,19 @@
 
     @property
     @pulumi.getter(name="producerBufferMemory")
     def producer_buffer_memory(self) -> Optional[int]:
         return pulumi.get(self, "producer_buffer_memory")
 
     @property
+    @pulumi.getter(name="producerCompressionType")
+    def producer_compression_type(self) -> Optional[str]:
+        return pulumi.get(self, "producer_compression_type")
+
+    @property
     @pulumi.getter(name="producerLingerMs")
     def producer_linger_ms(self) -> Optional[int]:
         return pulumi.get(self, "producer_linger_ms")
 
     @property
     @pulumi.getter(name="producerMaxRequestSize")
     def producer_max_request_size(self) -> Optional[int]:
@@ -17231,27 +17251,30 @@
     def __init__(__self__, *,
                  consumer_enable_auto_commit: Optional[bool] = None,
                  consumer_request_max_bytes: Optional[int] = None,
                  consumer_request_timeout_ms: Optional[int] = None,
                  producer_acks: Optional[str] = None,
                  producer_compression_type: Optional[str] = None,
                  producer_linger_ms: Optional[int] = None,
+                 producer_max_request_size: Optional[int] = None,
                  simpleconsumer_pool_size_max: Optional[int] = None):
         if consumer_enable_auto_commit is not None:
             pulumi.set(__self__, "consumer_enable_auto_commit", consumer_enable_auto_commit)
         if consumer_request_max_bytes is not None:
             pulumi.set(__self__, "consumer_request_max_bytes", consumer_request_max_bytes)
         if consumer_request_timeout_ms is not None:
             pulumi.set(__self__, "consumer_request_timeout_ms", consumer_request_timeout_ms)
         if producer_acks is not None:
             pulumi.set(__self__, "producer_acks", producer_acks)
         if producer_compression_type is not None:
             pulumi.set(__self__, "producer_compression_type", producer_compression_type)
         if producer_linger_ms is not None:
             pulumi.set(__self__, "producer_linger_ms", producer_linger_ms)
+        if producer_max_request_size is not None:
+            pulumi.set(__self__, "producer_max_request_size", producer_max_request_size)
         if simpleconsumer_pool_size_max is not None:
             pulumi.set(__self__, "simpleconsumer_pool_size_max", simpleconsumer_pool_size_max)
 
     @property
     @pulumi.getter(name="consumerEnableAutoCommit")
     def consumer_enable_auto_commit(self) -> Optional[bool]:
         return pulumi.get(self, "consumer_enable_auto_commit")
@@ -17278,14 +17301,19 @@
 
     @property
     @pulumi.getter(name="producerLingerMs")
     def producer_linger_ms(self) -> Optional[int]:
         return pulumi.get(self, "producer_linger_ms")
 
     @property
+    @pulumi.getter(name="producerMaxRequestSize")
+    def producer_max_request_size(self) -> Optional[int]:
+        return pulumi.get(self, "producer_max_request_size")
+
+    @property
     @pulumi.getter(name="simpleconsumerPoolSizeMax")
     def simpleconsumer_pool_size_max(self) -> Optional[int]:
         return pulumi.get(self, "simpleconsumer_pool_size_max")
 
 
 @pulumi.output_type
 class GetKafkaKafkaUserConfigPrivateAccessResult(dict):
@@ -22745,22 +22773,25 @@
 
 @pulumi.output_type
 class GetServiceIntegrationKafkaMirrormakerUserConfigKafkaMirrormakerResult(dict):
     def __init__(__self__, *,
                  consumer_fetch_min_bytes: Optional[int] = None,
                  producer_batch_size: Optional[int] = None,
                  producer_buffer_memory: Optional[int] = None,
+                 producer_compression_type: Optional[str] = None,
                  producer_linger_ms: Optional[int] = None,
                  producer_max_request_size: Optional[int] = None):
         if consumer_fetch_min_bytes is not None:
             pulumi.set(__self__, "consumer_fetch_min_bytes", consumer_fetch_min_bytes)
         if producer_batch_size is not None:
             pulumi.set(__self__, "producer_batch_size", producer_batch_size)
         if producer_buffer_memory is not None:
             pulumi.set(__self__, "producer_buffer_memory", producer_buffer_memory)
+        if producer_compression_type is not None:
+            pulumi.set(__self__, "producer_compression_type", producer_compression_type)
         if producer_linger_ms is not None:
             pulumi.set(__self__, "producer_linger_ms", producer_linger_ms)
         if producer_max_request_size is not None:
             pulumi.set(__self__, "producer_max_request_size", producer_max_request_size)
 
     @property
     @pulumi.getter(name="consumerFetchMinBytes")
@@ -22774,14 +22805,19 @@
 
     @property
     @pulumi.getter(name="producerBufferMemory")
     def producer_buffer_memory(self) -> Optional[int]:
         return pulumi.get(self, "producer_buffer_memory")
 
     @property
+    @pulumi.getter(name="producerCompressionType")
+    def producer_compression_type(self) -> Optional[str]:
+        return pulumi.get(self, "producer_compression_type")
+
+    @property
     @pulumi.getter(name="producerLingerMs")
     def producer_linger_ms(self) -> Optional[int]:
         return pulumi.get(self, "producer_linger_ms")
 
     @property
     @pulumi.getter(name="producerMaxRequestSize")
     def producer_max_request_size(self) -> Optional[int]:
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/pg.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/project.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,41 +15,37 @@
 
 @pulumi.input_type
 class ProjectArgs:
     def __init__(__self__, *,
                  project: pulumi.Input[str],
                  account_id: Optional[pulumi.Input[str]] = None,
                  add_account_owners_admin_access: Optional[pulumi.Input[bool]] = None,
-                 available_credits: Optional[pulumi.Input[str]] = None,
                  billing_group: Optional[pulumi.Input[str]] = None,
                  copy_from_project: Optional[pulumi.Input[str]] = None,
                  default_cloud: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagArgs']]]] = None,
                  technical_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_source_project_billing_group: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Project resource.
         :param pulumi.Input[str] project: Defines the name of the project. Name must be globally unique (between all Aiven customers) and cannot be changed later without destroying and re-creating the project, including all sub-resources.
         :param pulumi.Input[str] account_id: An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[bool] add_account_owners_admin_access: If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
-        :param pulumi.Input[str] available_credits: The amount of platform credits available to the project. This could be your free trial or other promotional credits.
         :param pulumi.Input[str] billing_group: The id of the billing group that is linked to this project. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] copy_from_project: is the name of another project used to copy billing information and some other project attributes like technical contacts from. This is mostly relevant when an existing project has billing type set to invoice and that needs to be copied over to a new project. (Setting billing is otherwise not allowed over the API.) This only has effect when the project is created. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] default_cloud: Defines the default cloud provider and region where services are hosted. This can be changed freely after the project is created. This will not affect existing services.
         :param pulumi.Input[Sequence[pulumi.Input['ProjectTagArgs']]] tags: Tags are key-value pairs that allow you to categorize projects.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] technical_emails: Defines the email addresses that will receive alerts about upcoming maintenance updates or warnings about service instability. It is  good practice to keep this up-to-date to be aware of any potential issues with your project.
         :param pulumi.Input[bool] use_source_project_billing_group: Use the same billing group that is used in source project.
         """
         pulumi.set(__self__, "project", project)
         if account_id is not None:
             pulumi.set(__self__, "account_id", account_id)
         if add_account_owners_admin_access is not None:
             pulumi.set(__self__, "add_account_owners_admin_access", add_account_owners_admin_access)
-        if available_credits is not None:
-            pulumi.set(__self__, "available_credits", available_credits)
         if billing_group is not None:
             pulumi.set(__self__, "billing_group", billing_group)
         if copy_from_project is not None:
             pulumi.set(__self__, "copy_from_project", copy_from_project)
         if default_cloud is not None:
             pulumi.set(__self__, "default_cloud", default_cloud)
         if tags is not None:
@@ -92,26 +88,14 @@
         return pulumi.get(self, "add_account_owners_admin_access")
 
     @add_account_owners_admin_access.setter
     def add_account_owners_admin_access(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "add_account_owners_admin_access", value)
 
     @property
-    @pulumi.getter(name="availableCredits")
-    def available_credits(self) -> Optional[pulumi.Input[str]]:
-        """
-        The amount of platform credits available to the project. This could be your free trial or other promotional credits.
-        """
-        return pulumi.get(self, "available_credits")
-
-    @available_credits.setter
-    def available_credits(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "available_credits", value)
-
-    @property
     @pulumi.getter(name="billingGroup")
     def billing_group(self) -> Optional[pulumi.Input[str]]:
         """
         The id of the billing group that is linked to this project. To set up proper dependencies please refer to this variable as a reference.
         """
         return pulumi.get(self, "billing_group")
 
@@ -399,15 +383,14 @@
 class Project(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_id: Optional[pulumi.Input[str]] = None,
                  add_account_owners_admin_access: Optional[pulumi.Input[bool]] = None,
-                 available_credits: Optional[pulumi.Input[str]] = None,
                  billing_group: Optional[pulumi.Input[str]] = None,
                  copy_from_project: Optional[pulumi.Input[str]] = None,
                  default_cloud: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagArgs']]]]] = None,
                  technical_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_source_project_billing_group: Optional[pulumi.Input[bool]] = None,
@@ -421,15 +404,14 @@
          $ pulumi import aiven:index/project:Project myproject project
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] account_id: An optional property to link a project to already an existing account by using account ID. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[bool] add_account_owners_admin_access: If account_id is set, grant account owner team admin access to the new project. The default value is `true`.
-        :param pulumi.Input[str] available_credits: The amount of platform credits available to the project. This could be your free trial or other promotional credits.
         :param pulumi.Input[str] billing_group: The id of the billing group that is linked to this project. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] copy_from_project: is the name of another project used to copy billing information and some other project attributes like technical contacts from. This is mostly relevant when an existing project has billing type set to invoice and that needs to be copied over to a new project. (Setting billing is otherwise not allowed over the API.) This only has effect when the project is created. To set up proper dependencies please refer to this variable as a reference.
         :param pulumi.Input[str] default_cloud: Defines the default cloud provider and region where services are hosted. This can be changed freely after the project is created. This will not affect existing services.
         :param pulumi.Input[str] project: Defines the name of the project. Name must be globally unique (between all Aiven customers) and cannot be changed later without destroying and re-creating the project, including all sub-resources.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagArgs']]]] tags: Tags are key-value pairs that allow you to categorize projects.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] technical_emails: Defines the email addresses that will receive alerts about upcoming maintenance updates or warnings about service instability. It is  good practice to keep this up-to-date to be aware of any potential issues with your project.
         :param pulumi.Input[bool] use_source_project_billing_group: Use the same billing group that is used in source project.
@@ -462,15 +444,14 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  account_id: Optional[pulumi.Input[str]] = None,
                  add_account_owners_admin_access: Optional[pulumi.Input[bool]] = None,
-                 available_credits: Optional[pulumi.Input[str]] = None,
                  billing_group: Optional[pulumi.Input[str]] = None,
                  copy_from_project: Optional[pulumi.Input[str]] = None,
                  default_cloud: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagArgs']]]]] = None,
                  technical_emails: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_source_project_billing_group: Optional[pulumi.Input[bool]] = None,
@@ -481,24 +462,24 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectArgs.__new__(ProjectArgs)
 
             __props__.__dict__["account_id"] = account_id
             __props__.__dict__["add_account_owners_admin_access"] = add_account_owners_admin_access
-            __props__.__dict__["available_credits"] = available_credits
             __props__.__dict__["billing_group"] = billing_group
             __props__.__dict__["copy_from_project"] = copy_from_project
             __props__.__dict__["default_cloud"] = default_cloud
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             __props__.__dict__["tags"] = tags
             __props__.__dict__["technical_emails"] = technical_emails
             __props__.__dict__["use_source_project_billing_group"] = use_source_project_billing_group
+            __props__.__dict__["available_credits"] = None
             __props__.__dict__["ca_cert"] = None
             __props__.__dict__["estimated_balance"] = None
             __props__.__dict__["payment_method"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["caCert"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Project, __self__).__init__(
             'aiven:index/project:Project',
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/project_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/provider.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/redis.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,57 +11,49 @@
 
 __all__ = ['TransitGatewayVpcAttachmentArgs', 'TransitGatewayVpcAttachment']
 
 @pulumi.input_type
 class TransitGatewayVpcAttachmentArgs:
     def __init__(__self__, *,
                  peer_cloud_account: pulumi.Input[str],
-                 peer_region: pulumi.Input[str],
                  peer_vpc: pulumi.Input[str],
                  user_peer_network_cidrs: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 vpc_id: pulumi.Input[str]):
+                 vpc_id: pulumi.Input[str],
+                 peer_region: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a TransitGatewayVpcAttachment resource.
         :param pulumi.Input[str] peer_cloud_account: AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
-        :param pulumi.Input[str] peer_region: AWS region of the peered VPC (if not in the same region as Aiven VPC)
         :param pulumi.Input[str] peer_vpc: Transit gateway ID. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] user_peer_network_cidrs: List of private IPv4 ranges to route through the peering connection
         :param pulumi.Input[str] vpc_id: The VPC the peering connection belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
+        :param pulumi.Input[str] peer_region: AWS region of the peered VPC (if not in the same region as Aiven VPC)
         """
         pulumi.set(__self__, "peer_cloud_account", peer_cloud_account)
-        pulumi.set(__self__, "peer_region", peer_region)
         pulumi.set(__self__, "peer_vpc", peer_vpc)
         pulumi.set(__self__, "user_peer_network_cidrs", user_peer_network_cidrs)
         pulumi.set(__self__, "vpc_id", vpc_id)
+        if peer_region is not None:
+            warnings.warn("""This field is deprecated and will be removed in the next major release.""", DeprecationWarning)
+            pulumi.log.warn("""peer_region is deprecated: This field is deprecated and will be removed in the next major release.""")
+        if peer_region is not None:
+            pulumi.set(__self__, "peer_region", peer_region)
 
     @property
     @pulumi.getter(name="peerCloudAccount")
     def peer_cloud_account(self) -> pulumi.Input[str]:
         """
         AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "peer_cloud_account")
 
     @peer_cloud_account.setter
     def peer_cloud_account(self, value: pulumi.Input[str]):
         pulumi.set(self, "peer_cloud_account", value)
 
     @property
-    @pulumi.getter(name="peerRegion")
-    def peer_region(self) -> pulumi.Input[str]:
-        """
-        AWS region of the peered VPC (if not in the same region as Aiven VPC)
-        """
-        return pulumi.get(self, "peer_region")
-
-    @peer_region.setter
-    def peer_region(self, value: pulumi.Input[str]):
-        pulumi.set(self, "peer_region", value)
-
-    @property
     @pulumi.getter(name="peerVpc")
     def peer_vpc(self) -> pulumi.Input[str]:
         """
         Transit gateway ID. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "peer_vpc")
 
@@ -89,14 +81,26 @@
         """
         return pulumi.get(self, "vpc_id")
 
     @vpc_id.setter
     def vpc_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "vpc_id", value)
 
+    @property
+    @pulumi.getter(name="peerRegion")
+    def peer_region(self) -> Optional[pulumi.Input[str]]:
+        """
+        AWS region of the peered VPC (if not in the same region as Aiven VPC)
+        """
+        return pulumi.get(self, "peer_region")
+
+    @peer_region.setter
+    def peer_region(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "peer_region", value)
+
 
 @pulumi.input_type
 class _TransitGatewayVpcAttachmentState:
     def __init__(__self__, *,
                  peer_cloud_account: Optional[pulumi.Input[str]] = None,
                  peer_region: Optional[pulumi.Input[str]] = None,
                  peer_vpc: Optional[pulumi.Input[str]] = None,
@@ -115,14 +119,17 @@
         :param pulumi.Input[Mapping[str, Any]] state_info: State-specific help or error information
         :param pulumi.Input[Sequence[pulumi.Input[str]]] user_peer_network_cidrs: List of private IPv4 ranges to route through the peering connection
         :param pulumi.Input[str] vpc_id: The VPC the peering connection belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         """
         if peer_cloud_account is not None:
             pulumi.set(__self__, "peer_cloud_account", peer_cloud_account)
         if peer_region is not None:
+            warnings.warn("""This field is deprecated and will be removed in the next major release.""", DeprecationWarning)
+            pulumi.log.warn("""peer_region is deprecated: This field is deprecated and will be removed in the next major release.""")
+        if peer_region is not None:
             pulumi.set(__self__, "peer_region", peer_region)
         if peer_vpc is not None:
             pulumi.set(__self__, "peer_vpc", peer_vpc)
         if peering_connection_id is not None:
             pulumi.set(__self__, "peering_connection_id", peering_connection_id)
         if state is not None:
             pulumi.set(__self__, "state", state)
@@ -329,16 +336,17 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TransitGatewayVpcAttachmentArgs.__new__(TransitGatewayVpcAttachmentArgs)
 
             if peer_cloud_account is None and not opts.urn:
                 raise TypeError("Missing required property 'peer_cloud_account'")
             __props__.__dict__["peer_cloud_account"] = peer_cloud_account
-            if peer_region is None and not opts.urn:
-                raise TypeError("Missing required property 'peer_region'")
+            if peer_region is not None and not opts.urn:
+                warnings.warn("""This field is deprecated and will be removed in the next major release.""", DeprecationWarning)
+                pulumi.log.warn("""peer_region is deprecated: This field is deprecated and will be removed in the next major release.""")
             __props__.__dict__["peer_region"] = peer_region
             if peer_vpc is None and not opts.urn:
                 raise TypeError("Missing required property 'peer_vpc'")
             __props__.__dict__["peer_vpc"] = peer_vpc
             if user_peer_network_cidrs is None and not opts.urn:
                 raise TypeError("Missing required property 'user_peer_network_cidrs'")
             __props__.__dict__["user_peer_network_cidrs"] = user_peer_network_cidrs
@@ -402,15 +410,15 @@
         """
         AWS account ID or GCP project ID of the peered VPC. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "peer_cloud_account")
 
     @property
     @pulumi.getter(name="peerRegion")
-    def peer_region(self) -> pulumi.Output[str]:
+    def peer_region(self) -> pulumi.Output[Optional[str]]:
         """
         AWS region of the peered VPC (if not in the same region as Aiven VPC)
         """
         return pulumi.get(self, "peer_region")
 
     @property
     @pulumi.getter(name="peerVpc")
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-aiven
-Version: 6.4.0a1686633780
+Version: 6.4.0a1686760738
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.4.0a1686633780/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.4.0a1686760738/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.4.0a1686633780/setup.py` & `pulumi_aiven-6.4.0a1686760738/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.4.0a1686633780"
-PLUGIN_VERSION = "6.4.0-alpha.1686633780+6e1d1057"
+VERSION = "6.4.0a1686760738"
+PLUGIN_VERSION = "6.4.0-alpha.1686760738+a70dcde0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aiven', PLUGIN_VERSION])
         except OSError as error:
```

