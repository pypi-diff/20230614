# Comparing `tmp/cloud-governance-1.1.98.tar.gz` & `tmp/cloud-governance-1.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-governance-1.1.98.tar", last modified: Tue May 16 18:38:37 2023, max compression
+gzip compressed data, was "cloud-governance-1.1.99.tar", last modified: Thu May 18 13:04:16 2023, max compression
```

## Comparing `cloud-governance-1.1.98.tar` & `cloud-governance-1.1.99.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.143784 cloud-governance-1.1.98/cloud_governance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/short_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cost_explorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18246 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/sts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/aws/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/cost_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/gcp/google_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/account/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/classic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/google_drive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/google_drive/google_drive_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/jira/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/jira/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/jira/jira_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/ldap/ldap_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/logger/init_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/logger/logger_time_stamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/mails/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/mails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/mails/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)    16489 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/mails/mail_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/mails/postfix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.151784 cloud-governance-1.1.98/cloud_governance/common/tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/common/tool/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/environment_variables_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/es_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/main/main_common_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/cost_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ebs_in_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ebs_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/empty_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/ip_unattached.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/monthly_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/s3_inactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/skipped_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/unused_nat_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/aws/zombie_snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/azure/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/common_policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/common_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/common_policies/send_aggregated_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/gcp/cost_billing_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/tag_baremetal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/ibm/tag_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.155784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gitleaks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.159784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/cloud_governance/policy/policy_runners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/cloud_governance/policy/policy_runners/common_policy_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:38:37.147784 cloud-governance-1.1.98/cloud_governance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 18:38:37.000000 cloud-governance-1.1.98/cloud_governance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 18:38:37.163784 cloud-governance-1.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-16 18:38:20.000000 cloud-governance-1.1.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.647628 cloud-governance-1.1.99/cloud_governance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.647628 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.647628 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.647628 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.647628 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/short_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/short_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/short_run/ec2_short_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.647628 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18246 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/price/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/price/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/price/resources_pricing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/sts/sts_oprations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/aws/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/azure/cost_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/azure/cost_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/azure/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/azure/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/gcp/google_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/account/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.651628 cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/common/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/common/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/google_drive/google_drive_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/google_drive/upload_to_gsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/common/jira/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/jira/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/jira/jira_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/common/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/ldap/ldap_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/common/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/logger/init_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/logger/logger_time_stamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/common/mails/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/mails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/mails/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16489 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/mails/mail_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/mails/postfix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/common/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/common/tool/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18195 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/main/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/main/environment_variables_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/main/es_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/main/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/main/main_common_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.655628 cloud-governance-1.1.99/cloud_governance/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/cost_billing_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/cost_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15608 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/cost_explorer_payer_billings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/ebs_in_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/ebs_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/ec2_idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/ec2_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/ec2_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/empty_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/ip_unattached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/monthly_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/s3_inactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/skipped_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/unused_nat_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51727 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/aws/zombie_snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/azure/cost_billing_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/common_policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/common_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/common_policies/send_aggregated_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/gcp/cost_billing_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/ibm/cost_billing_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/ibm/ibm_cost_over_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/ibm/ibm_cost_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/ibm/tag_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/cost_expenditure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41938 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.659628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27642 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17153 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/gitleaks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/gitleaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/ibm_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/tagging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/cloud_governance/policy/policy_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/cloud_governance/policy/policy_runners/common_policy_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 13:04:16.647628 cloud-governance-1.1.99/cloud_governance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-05-18 13:04:16.000000 cloud-governance-1.1.99/cloud_governance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-18 13:04:16.000000 cloud-governance-1.1.99/cloud_governance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:04:16.000000 cloud-governance-1.1.99/cloud_governance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 13:04:16.000000 cloud-governance-1.1.99/cloud_governance.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-18 13:04:16.000000 cloud-governance-1.1.99/cloud_governance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 13:04:16.000000 cloud-governance-1.1.99/cloud_governance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 13:04:16.663628 cloud-governance-1.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-18 13:03:59.000000 cloud-governance-1.1.99/setup.py
```

### Comparing `cloud-governance-1.1.98/LICENSE` & `cloud-governance-1.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/PKG-INFO` & `cloud-governance-1.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.98
+Version: 1.1.99
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloud-governance-1.1.98/README.md` & `cloud-governance-1.1.99/README.md`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py` & `cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/ec2_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py` & `cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_in_progress_issues.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py` & `cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/monitor_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py` & `cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/aws/long_run/tag_long_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py` & `cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/common/ec2_monitor_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py` & `cloud-governance-1.1.99/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/iam/iam_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/iam/iam_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/price.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/price/price.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/price/resources_pricing.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/price/resources_pricing.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/aws/utils/utils.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/aws/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/gcp/google_account.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/gcp/google_account.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/account/ibm_account.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/account/ibm_account.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/clouds/ibm/classic/classic_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/clouds/ibm/classic/classic_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elastic_upload.py` & `cloud-governance-1.1.99/cloud_governance/common/elasticsearch/elastic_upload.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/elasticsearch/elasticsearch_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/elasticsearch/elasticsearch_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/google_drive/google_drive_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/google_drive/upload_to_gsheet.py` & `cloud-governance-1.1.99/cloud_governance/common/google_drive/upload_to_gsheet.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/jira/jira.py` & `cloud-governance-1.1.99/cloud_governance/common/jira/jira.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/jira/jira_operations.py` & `cloud-governance-1.1.99/cloud_governance/common/jira/jira_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/ldap/ldap_search.py` & `cloud-governance-1.1.99/cloud_governance/common/ldap/ldap_search.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/logger/logger_time_stamp.py` & `cloud-governance-1.1.99/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/mails/gmail.py` & `cloud-governance-1.1.99/cloud_governance/common/mails/gmail.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/mails/mail_message.py` & `cloud-governance-1.1.99/cloud_governance/common/mails/mail_message.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/common/mails/postfix.py` & `cloud-governance-1.1.99/cloud_governance/common/mails/postfix.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/main/environment_variables.py` & `cloud-governance-1.1.99/cloud_governance/main/environment_variables.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/main/es_uploader.py` & `cloud-governance-1.1.99/cloud_governance/main/es_uploader.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/main/main.py` & `cloud-governance-1.1.99/cloud_governance/main/main.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/cost_billing_reports.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/cost_explorer.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/cost_explorer.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/cost_explorer_payer_billings.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/cost_explorer_payer_billings.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/cost_over_usage.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/ebs_in_use.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/ebs_in_use.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/ebs_unattached.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_idle.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/ec2_idle.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_run.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/ec2_run.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/ec2_stop.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/ec2_stop.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/empty_roles.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/empty_roles.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/ip_unattached.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/ip_unattached.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/monthly_report.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/monthly_report.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/s3_inactive.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/s3_inactive.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/skipped_resources.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/skipped_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/unused_nat_gateway.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/unused_nat_gateway.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/zombie_cluster_resource.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/aws/zombie_snapshots.py` & `cloud-governance-1.1.99/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/azure/cost_billing_reports.py` & `cloud-governance-1.1.99/cloud_governance/policy/azure/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/common_policies/send_aggregated_alerts.py` & `cloud-governance-1.1.99/cloud_governance/policy/common_policies/send_aggregated_alerts.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/gcp/cost_billing_reports.py` & `cloud-governance-1.1.99/cloud_governance/policy/gcp/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/ibm/cost_billing_reports.py` & `cloud-governance-1.1.99/cloud_governance/policy/ibm/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/ibm/ibm_cost_over_usage.py` & `cloud-governance-1.1.99/cloud_governance/policy/ibm/ibm_cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/ibm/ibm_cost_report.py` & `cloud-governance-1.1.99/cloud_governance/policy/ibm/ibm_cost_report.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/ibm/tag_baremetal.py` & `cloud-governance-1.1.99/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/ibm/tag_vm.py` & `cloud-governance-1.1.99/cloud_governance/policy/ibm/tag_vm.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance/policy/policy_runners/common_policy_runner.py` & `cloud-governance-1.1.99/cloud_governance/policy/policy_runners/common_policy_runner.py`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance.egg-info/PKG-INFO` & `cloud-governance-1.1.99/cloud_governance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-governance
-Version: 1.1.98
+Version: 1.1.99
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cloud-governance-1.1.98/cloud_governance.egg-info/SOURCES.txt` & `cloud-governance-1.1.99/cloud_governance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/cloud_governance.egg-info/requires.txt` & `cloud-governance-1.1.99/cloud_governance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cloud-governance-1.1.98/setup.py` & `cloud-governance-1.1.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.1.98'
+__version__ = '1.1.99'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

