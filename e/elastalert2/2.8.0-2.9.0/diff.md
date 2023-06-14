# Comparing `tmp/elastalert2-2.8.0.tar.gz` & `tmp/elastalert2-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastalert2-2.8.0.tar", last modified: Fri Oct 21 16:09:32 2022, max compression
+gzip compressed data, was "elastalert2-2.9.0.tar", last modified: Fri Dec  2 12:24:32 2022, max compression
```

## Comparing `elastalert2-2.8.0.tar` & `elastalert2-2.9.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.791885 elastalert2-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11359 2022-10-21 16:09:23.000000 elastalert2-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-21 16:09:32.791885 elastalert2-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-10-21 16:09:23.000000 elastalert2-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.771884 elastalert2-2.8.0/elastalert/
--rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.779884 elastalert2-2.8.0/elastalert/alerters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5762 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/alerta.py
--rw-r--r--   0 runner    (1001) docker     (121)     3702 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/alertmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/chatwork.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/datadog.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/dingtalk.py
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/discord.py
--rw-r--r--   0 runner    (1001) docker     (121)     5943 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/email.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/exotel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/gitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/googlechat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/httppost.py
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/httppost2.py
--rw-r--r--   0 runner    (1001) docker     (121)    20096 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/jira.py
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/line.py
--rw-r--r--   0 runner    (1001) docker     (121)     7688 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/mattermost.py
--rw-r--r--   0 runner    (1001) docker     (121)     8229 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/opsgenie.py
--rw-r--r--   0 runner    (1001) docker     (121)     7705 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/pagerduty.py
--rw-r--r--   0 runner    (1001) docker     (121)     1491 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/pagertree.py
--rw-r--r--   0 runner    (1001) docker     (121)     5644 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/rocketchat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/servicenow.py
--rw-r--r--   0 runner    (1001) docker     (121)     4305 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/ses.py
--rw-r--r--   0 runner    (1001) docker     (121)     8182 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/slack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/sns.py
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/stomp.py
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/telegram.py
--rw-r--r--   0 runner    (1001) docker     (121)     9470 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/tencentsms.py
--rw-r--r--   0 runner    (1001) docker     (121)     6841 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/thehive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/twilio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/victorops.py
--rw-r--r--   0 runner    (1001) docker     (121)     5041 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerters/zabbix.py
--rw-r--r--   0 runner    (1001) docker     (121)    14633 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/alerts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11600 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/create_index.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    86577 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/elastalert.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/enhancements.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.767884 elastalert2-2.8.0/elastalert/es_mappings/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.779884 elastalert2-2.8.0/elastalert/es_mappings/7/
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/7/elastalert.json
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/7/elastalert_error.json
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/7/elastalert_status.json
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/7/past_elastalert.json
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/7/silence.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.779884 elastalert2-2.8.0/elastalert/es_mappings/8/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/8/elastalert.json
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/8/elastalert_error.json
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/8/elastalert_status.json
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/8/past_elastalert.json
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/es_mappings/8/silence.json
--rw-r--r--   0 runner    (1001) docker     (121)     5549 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/kibana_discover.py
--rw-r--r--   0 runner    (1001) docker     (121)     5165 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/kibana_external_url_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)    26663 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     2901 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/prometheus_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    62336 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/ruletypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    22839 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19326 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/test_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    19582 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-21 16:09:23.000000 elastalert2-2.8.0/elastalert/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.779884 elastalert2-2.8.0/elastalert2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-21 16:09:32.000000 elastalert2-2.8.0/elastalert2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3202 2022-10-21 16:09:32.000000 elastalert2-2.8.0/elastalert2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 16:09:32.000000 elastalert2-2.8.0/elastalert2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-21 16:09:32.000000 elastalert2-2.8.0/elastalert2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-10-21 16:09:32.000000 elastalert2-2.8.0/elastalert2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-21 16:09:32.000000 elastalert2-2.8.0/elastalert2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-21 16:09:32.791885 elastalert2-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-10-21 16:09:23.000000 elastalert2-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.767884 elastalert2-2.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:32.791885 elastalert2-2.8.0/tests/alerters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30175 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/alerta_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12596 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/alertmanager_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7396 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/chatwork_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5791 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/command_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/datadog_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/debug_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12081 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/dingtalk_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10055 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/discord_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    24478 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/email_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6121 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/exotel_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4781 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/gitter_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10101 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/googlechat_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    30671 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/httppost2_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10906 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/httppost_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    19767 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/jira_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/line_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    37425 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/mattermost_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    37081 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/opsgenie_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    32432 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/pagerduty_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5578 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/pagertree_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    28819 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/rocketchat_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10751 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/servicenow_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3737 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/ses_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    43171 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/slack_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/stomp_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    16252 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/teams_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9345 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/telegram_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7808 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/tencentsms_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    20660 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/thehive_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6903 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/twilio_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    11028 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/victorops_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2022-10-21 16:09:23.000000 elastalert2-2.8.0/tests/alerters/zabbix_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.219302 elastalert2-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2022-12-02 12:24:24.000000 elastalert2-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2022-12-02 12:24:32.219302 elastalert2-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2022-12-02 12:24:24.000000 elastalert2-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.211302 elastalert2-2.9.0/elastalert/
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.211302 elastalert2-2.9.0/elastalert/alerters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/alerta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/alertmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/chatwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/datadog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/dingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/exotel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/gitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/googlechat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/httppost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/httppost2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20096 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/mattermost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/opsgenie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/pagerduty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/pagertree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/rocketchat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/servicenow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/ses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/stomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/tencentsms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/thehive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/victorops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerters/zabbix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/create_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    86591 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/elastalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/enhancements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.207302 elastalert2-2.9.0/elastalert/es_mappings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.215302 elastalert2-2.9.0/elastalert/es_mappings/7/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/7/elastalert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/7/elastalert_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/7/elastalert_status.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/7/past_elastalert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/7/silence.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.215302 elastalert2-2.9.0/elastalert/es_mappings/8/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/8/elastalert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/8/elastalert_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/8/elastalert_status.json
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/8/past_elastalert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/es_mappings/8/silence.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/kibana_discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/kibana_external_url_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26716 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/prometheus_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62336 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/ruletypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22959 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    19326 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/test_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-02 12:24:24.000000 elastalert2-2.9.0/elastalert/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.215302 elastalert2-2.9.0/elastalert2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2022-12-02 12:24:32.000000 elastalert2-2.9.0/elastalert2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2022-12-02 12:24:32.000000 elastalert2-2.9.0/elastalert2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 12:24:32.000000 elastalert2-2.9.0/elastalert2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-02 12:24:32.000000 elastalert2-2.9.0/elastalert2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2022-12-02 12:24:32.000000 elastalert2-2.9.0/elastalert2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-02 12:24:32.000000 elastalert2-2.9.0/elastalert2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-02 12:24:32.219302 elastalert2-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2022-12-02 12:24:24.000000 elastalert2-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.207302 elastalert2-2.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:32.219302 elastalert2-2.9.0/tests/alerters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30175 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/alerta_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/alertmanager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/chatwork_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/datadog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/debug_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/dingtalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/discord_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/email_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/exotel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/gitter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/googlechat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30671 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/httppost2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/httppost_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/jira_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/line_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38149 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/mattermost_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37081 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/opsgenie_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32432 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/pagerduty_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/pagertree_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28819 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/rocketchat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/servicenow_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/ses_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43171 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/slack_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/stomp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16252 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/teams_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/telegram_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/tencentsms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/thehive_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/twilio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/victorops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2022-12-02 12:24:24.000000 elastalert2-2.9.0/tests/alerters/zabbix_test.py
```

### Comparing `elastalert2-2.8.0/LICENSE` & `elastalert2-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/PKG-INFO` & `elastalert2-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: elastalert2
-Version: 2.8.0
+Version: 2.9.0
 Summary: Automated rule-based alerting for Elasticsearch
 Home-page: https://github.com/jertel/elastalert2
 License: Apache 2.0
 Project-URL: Documentation, https://elastalert2.readthedocs.io
 Project-URL: Source Code, https://github.com/jertel/elastalert2
 Project-URL: Discussion Forum, https://github.com/jertel/elastalert2/discussions
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ElastAlert 2
```

### Comparing `elastalert2-2.8.0/README.md` & `elastalert2-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/__init__.py` & `elastalert2-2.9.0/elastalert/__init__.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/alerta.py` & `elastalert2-2.9.0/elastalert/alerters/alerta.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/alertmanager.py` & `elastalert2-2.9.0/elastalert/alerters/alertmanager.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/chatwork.py` & `elastalert2-2.9.0/elastalert/alerters/chatwork.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/command.py` & `elastalert2-2.9.0/elastalert/alerters/command.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/datadog.py` & `elastalert2-2.9.0/elastalert/alerters/datadog.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/debug.py` & `elastalert2-2.9.0/elastalert/alerters/debug.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/dingtalk.py` & `elastalert2-2.9.0/elastalert/alerters/dingtalk.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/discord.py` & `elastalert2-2.9.0/elastalert/alerters/discord.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/email.py` & `elastalert2-2.9.0/elastalert/alerters/email.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/exotel.py` & `elastalert2-2.9.0/elastalert/alerters/exotel.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/gitter.py` & `elastalert2-2.9.0/elastalert/alerters/gitter.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/googlechat.py` & `elastalert2-2.9.0/elastalert/alerters/googlechat.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/httppost.py` & `elastalert2-2.9.0/elastalert/alerters/httppost.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/httppost2.py` & `elastalert2-2.9.0/elastalert/alerters/httppost2.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/jira.py` & `elastalert2-2.9.0/elastalert/alerters/jira.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/line.py` & `elastalert2-2.9.0/elastalert/alerters/line.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/mattermost.py` & `elastalert2-2.9.0/elastalert/alerters/mattermost.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         self.mattermost_ignore_ssl_errors = self.rule.get('mattermost_ignore_ssl_errors', False)
 
         # Override webhook config
         self.mattermost_username_override = self.rule.get('mattermost_username_override', 'elastalert')
         self.mattermost_channel_override = self.rule.get('mattermost_channel_override', '')
         if isinstance(self.mattermost_channel_override, str):
             self.mattermost_channel_override = [self.mattermost_channel_override]
+        self.mattermost_emoji_override = self.rule.get('mattermost_emoji_override', ':ghost:')
         self.mattermost_icon_url_override = self.rule.get('mattermost_icon_url_override', '')
 
         # Message properties
         self.mattermost_msg_pretext = self.rule.get('mattermost_msg_pretext', '')
         self.mattermost_msg_color = self.rule.get('mattermost_msg_color', 'danger')
         self.mattermost_msg_fields = self.rule.get('mattermost_msg_fields', '')
         self.mattermost_image_url = self.rule.get('mattermost_image_url', '')
@@ -100,14 +101,16 @@
             payload['text'] = body
 
         if self.mattermost_msg_fields != '':
             payload['attachments'][0]['fields'] = self.populate_fields(matches)
 
         if self.mattermost_icon_url_override != '':
             payload['icon_url'] = self.mattermost_icon_url_override
+        else:
+            payload['icon_emoji'] = self.mattermost_emoji_override
 
         if self.mattermost_title != '':
             payload['attachments'][0]['title'] = self.mattermost_title
 
         if self.mattermost_title_link != '':
             payload['attachments'][0]['title_link'] = self.mattermost_title_link
```

### Comparing `elastalert2-2.8.0/elastalert/alerters/opsgenie.py` & `elastalert2-2.9.0/elastalert/alerters/opsgenie.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/pagerduty.py` & `elastalert2-2.9.0/elastalert/alerters/pagerduty.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/pagertree.py` & `elastalert2-2.9.0/elastalert/alerters/pagertree.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/rocketchat.py` & `elastalert2-2.9.0/elastalert/alerters/rocketchat.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/servicenow.py` & `elastalert2-2.9.0/elastalert/alerters/servicenow.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/ses.py` & `elastalert2-2.9.0/elastalert/alerters/ses.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/slack.py` & `elastalert2-2.9.0/elastalert/alerters/slack.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/sns.py` & `elastalert2-2.9.0/elastalert/alerters/sns.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def alert(self, matches):
         body = self.create_alert_body(matches)
 
         try:
             if self.profile is None:
                 session = boto3.Session(
                     aws_access_key_id=self.sns_aws_access_key_id,
-                    aws_secret_access_key=self.sns_aws_access_key_id,
+                    aws_secret_access_key=self.sns_aws_secret_access_key,
                     region_name=self.sns_aws_region
                 )
             else:
                 session = boto3.Session(profile_name=self.profile)
 
             sns_client = session.client('sns')
             sns_client.publish(
```

### Comparing `elastalert2-2.8.0/elastalert/alerters/stomp.py` & `elastalert2-2.9.0/elastalert/alerters/stomp.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/teams.py` & `elastalert2-2.9.0/elastalert/alerters/teams.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/telegram.py` & `elastalert2-2.9.0/elastalert/alerters/telegram.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/tencentsms.py` & `elastalert2-2.9.0/elastalert/alerters/tencentsms.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/thehive.py` & `elastalert2-2.9.0/elastalert/alerters/thehive.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/twilio.py` & `elastalert2-2.9.0/elastalert/alerters/twilio.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/victorops.py` & `elastalert2-2.9.0/elastalert/alerters/victorops.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerters/zabbix.py` & `elastalert2-2.9.0/elastalert/alerters/zabbix.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/alerts.py` & `elastalert2-2.9.0/elastalert/alerts.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/auth.py` & `elastalert2-2.9.0/elastalert/auth.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/config.py` & `elastalert2-2.9.0/elastalert/config.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/create_index.py` & `elastalert2-2.9.0/elastalert/create_index.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/elastalert.py` & `elastalert2-2.9.0/elastalert/elastalert.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,15 +876,15 @@
             match = rule['type'].matches.pop(0)
             match['num_hits'] = self.thread_data.cumulative_hits
             match['num_matches'] = num_matches
 
             # If realert is set, silence the rule for that duration
             # Silence is cached by query_key, if it exists
             # Default realert time is 0 seconds
-            silence_cache_key = rule['name']
+            silence_cache_key = rule['realert_key']
             query_key_value = self.get_query_key_value(rule, match)
             if query_key_value is not None:
                 silence_cache_key += '.' + query_key_value
 
             if self.is_silenced(rule['name'] + "._silence") or self.is_silenced(silence_cache_key):
                 elastalert_logger.info('Ignoring match for silenced rule %s' % (silence_cache_key,))
                 continue
@@ -1671,15 +1671,15 @@
         if not self.args.rule:
             elastalert_logger.error('--silence must be used with --rule')
             exit(1)
 
         # With --rule, self.rules will only contain that specific rule
         if not silence_cache_key:
             if self.args.silence_qk_value:
-                silence_cache_key = self.rules[0]['name'] + "." + self.args.silence_qk_value
+                silence_cache_key = self.rules[0]['realert_key'] + "." + self.args.silence_qk_value
             else:
                 silence_cache_key = self.rules[0]['name'] + "._silence"
 
         try:
             silence_ts = parse_deadline(self.args.silence)
         except (ValueError, TypeError):
             elastalert_logger.error('%s is not a valid time period' % (self.args.silence))
```

### Comparing `elastalert2-2.8.0/elastalert/enhancements.py` & `elastalert2-2.9.0/elastalert/enhancements.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/es_mappings/7/elastalert.json` & `elastalert2-2.9.0/elastalert/es_mappings/7/elastalert.json`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/es_mappings/8/elastalert.json` & `elastalert2-2.9.0/elastalert/es_mappings/8/elastalert.json`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/kibana_discover.py` & `elastalert2-2.9.0/elastalert/kibana_discover.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .util import lookup_es_key
 from .util import ts_add
 
 kibana_default_timedelta = datetime.timedelta(minutes=10)
 
 kibana_versions = frozenset([
         '7.0', '7.1', '7.2', '7.3', '7.4', '7.5', '7.6', '7.7', '7.8', '7.9', '7.10', '7.11', '7.12', '7.13', '7.14', '7.15', '7.16', '7.17', 
-        '8.0', '8.1', '8.2', '8.3', '8.4'
+        '8.0', '8.1', '8.2', '8.3', '8.4', '8.5'
         ])
 
 def generate_kibana_discover_url(rule, match):
     ''' Creates a link for a kibana discover app. '''
 
     discover_app_url = rule.get('kibana_discover_app_url')
     if not discover_app_url:
```

### Comparing `elastalert2-2.8.0/elastalert/kibana_external_url_formatter.py` & `elastalert2-2.9.0/elastalert/kibana_external_url_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,20 @@
         if self.security_tenant:
             url = append_security_tenant(url, self.security_tenant)
         return url
 
 class ShortKibanaExternalUrlFormatter(KibanaExternalUrlFormatter):
     '''Formats external urls using the Kibana Shorten URL API'''
 
-    def __init__(self, base_url: str, auth: AuthBase, security_tenant: str, new_shortener: bool) -> None:
+    def __init__(self, base_url: str, auth: AuthBase, security_tenant: str, new_shortener: bool, verify: bool) -> None:
         self.auth = auth
         self.security_tenant = security_tenant
         self.goto_url = urljoin(base_url, 'goto/')
         self.use_new_shortener = new_shortener
+        self.verify = verify
 
         if self.use_new_shortener:
             path = 'api/short_url'
         else:
             path = 'api/shorten_url'
 
         shorten_url = urljoin(base_url, path)
@@ -79,15 +80,16 @@
             response = requests.post(
                 url=self.shorten_url,
                 auth=self.auth,
                 headers={
                     'kbn-xsrf': 'elastalert',
                     'osd-xsrf': 'elastalert'
                 },
-                json=json
+                json=json,
+                verify=self.verify
             )
             response.raise_for_status()
         except RequestException as e:
             raise EAException("Failed to invoke Kibana Shorten URL API: %s" % e)
 
         response_body = response.json()
         url_id = response_body.get(response_param)
@@ -146,11 +148,12 @@
 ) -> KibanaExternalUrlFormatter:
     '''Creates a Kibana external url formatter'''
 
     base_url = rule.get('kibana_url')
     new_shortener = is_kibana_atleastsevensixteen(rule.get('kibana_discover_version', '0.0'))
 
     if shorten:
+        verify = rule.get('kibana_verify_certs', True)
         auth = create_kibana_auth(base_url, rule)
-        return ShortKibanaExternalUrlFormatter(base_url, auth, security_tenant, new_shortener)
+        return ShortKibanaExternalUrlFormatter(base_url, auth, security_tenant, new_shortener, verify)
 
     return AbsoluteKibanaExternalUrlFormatter(base_url, security_tenant)
```

### Comparing `elastalert2-2.8.0/elastalert/loaders.py` & `elastalert2-2.9.0/elastalert/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,14 +329,15 @@
             raise EAException('Invalid time format used: %s' % e)
 
         # Set defaults, copy defaults from config.yaml
         for key, val in list(self.base_config.items()):
             rule.setdefault(key, val)
         rule.setdefault('name', os.path.splitext(filename)[0])
         rule.setdefault('realert', datetime.timedelta(seconds=0))
+        rule.setdefault('realert_key', rule['name'])
         rule.setdefault('aggregation', datetime.timedelta(seconds=0))
         rule.setdefault('query_delay', datetime.timedelta(seconds=0))
         rule.setdefault('timestamp_field', '@timestamp')
         rule.setdefault('filter', [])
         rule.setdefault('timestamp_type', 'iso')
         rule.setdefault('timestamp_format', '%Y-%m-%dT%H:%M:%SZ')
         rule.setdefault('_source_enabled', True)
```

### Comparing `elastalert2-2.8.0/elastalert/prometheus_wrapper.py` & `elastalert2-2.9.0/elastalert/prometheus_wrapper.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/ruletypes.py` & `elastalert2-2.9.0/elastalert/ruletypes.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/schema.yaml` & `elastalert2-2.9.0/elastalert/schema.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,15 @@
     anyOf:
       - type: array
         items:
           type: string
       - type: string
   aggregation: *timeframe
   realert: *timeframe
+  realert_key: {type: string}
   exponential_realert: *timeframe
 
   buffer_time: *timeframe
   query_delay: *timeframe
   max_query_size: {type: integer}
   max_scrolling: {type: integer}
   max_threads: {type: integer}
@@ -256,14 +257,15 @@
   include: {type: array, items: {type: string}}
   top_count_keys: {type: array, items: {type: string}}
   top_count_number: {type: integer}
   raw_count_keys: {type: boolean}
   kibana_url: {type: string, format: uri}
   kibana_username: {type: string}
   kibana_password: {type: string}
+  kibana_verify_certs: {type: boolean}
   use_local_time: {type: boolean}
   custom_pretty_ts_format: {type: string}
   match_enhancements: {type: array, items: {type: string}}
   query_key: *arrayOfString
   replace_dots_in_field_names: {type: boolean}
   scan_entire_timeframe: {type: boolean}
 
@@ -274,15 +276,15 @@
   summary_prefix: {type: string}
   summary_suffix: {type: string}
 
   ### Kibana Discover App Link
   generate_kibana_discover_url: {type: boolean}
   shorten_kibana_discover_url: {type: boolean}
   kibana_discover_app_url: {type: string}
-  kibana_discover_version: {type: string, enum: ['8.4', '8.3', '8.2', '8.1', '8.0', '7.17', '7.16', '7.15', '7.14', '7.13', '7.12', '7.11', '7.10', '7.9', '7.8', '7.7', '7.6', '7.5', '7.4', '7.3', '7.2', '7.1', '7.0']}
+  kibana_discover_version: {type: string, enum: ['8.5', '8.4', '8.3', '8.2', '8.1', '8.0', '7.17', '7.16', '7.15', '7.14', '7.13', '7.12', '7.11', '7.10', '7.9', '7.8', '7.7', '7.6', '7.5', '7.4', '7.3', '7.2', '7.1', '7.0']}
   kibana_discover_index_pattern_id: {type: string, minLength: 1}
   kibana_discover_columns: {type: array, items: {type: string, minLength: 1}, minItems: 1}
   kibana_discover_from_timedelta: *timedelta
   kibana_discover_to_timedelta: *timedelta
   kibana_discover_security_tenant: {type:string}
 
   # Alert Content
@@ -502,14 +504,15 @@
 
   ### Mattermost
   mattermost_webhook_url: *arrayOfString
   mattermost_proxy: {type: string}
   mattermost_ignore_ssl_errors: {type: boolean}
   mattermost_username_override: {type: string}
   mattermost_channel_override: *arrayOfString
+  mattermost_emoji_override: {type: string}
   mattermost_icon_url_override: {type: string}
   mattermost_msg_pretext: {type: string}
   mattermost_msg_color: {enum: [good, warning, danger]}
   mattermost_msg_fields: *arrayOfMattermostField
   mattermost_title: {type: string}
   mattermost_title_link: {type: string}
   mattermost_footer: {type: string}
```

### Comparing `elastalert2-2.8.0/elastalert/test_rule.py` & `elastalert2-2.9.0/elastalert/test_rule.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert/util.py` & `elastalert2-2.9.0/elastalert/util.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/elastalert2.egg-info/PKG-INFO` & `elastalert2-2.9.0/elastalert2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: elastalert2
-Version: 2.8.0
+Version: 2.9.0
 Summary: Automated rule-based alerting for Elasticsearch
 Home-page: https://github.com/jertel/elastalert2
 License: Apache 2.0
 Project-URL: Documentation, https://elastalert2.readthedocs.io
 Project-URL: Source Code, https://github.com/jertel/elastalert2
 Project-URL: Discussion Forum, https://github.com/jertel/elastalert2/discussions
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ElastAlert 2
```

### Comparing `elastalert2-2.8.0/elastalert2.egg-info/SOURCES.txt` & `elastalert2-2.9.0/elastalert2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/setup.py` & `elastalert2-2.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
 base_dir = os.path.dirname(__file__)
 setup(
     name='elastalert2',
-    version='2.8.0',
+    version='2.9.0',
     description='Automated rule-based alerting for Elasticsearch',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/jertel/elastalert2",
     setup_requires='setuptools',
     license='Apache 2.0',
     project_urls={
         "Documentation": "https://elastalert2.readthedocs.io",
         "Source Code": "https://github.com/jertel/elastalert2",
         "Discussion Forum": "https://github.com/jertel/elastalert2/discussions",
     },
     classifiers=[
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
     ],
     entry_points={
         'console_scripts': ['elastalert-create-index=elastalert.create_index:main',
                             'elastalert-test-rule=elastalert.test_rule:main',
                             'elastalert=elastalert.elastalert:main']},
```

### Comparing `elastalert2-2.8.0/tests/alerters/alerta_test.py` & `elastalert2-2.9.0/tests/alerters/alerta_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/alertmanager_test.py` & `elastalert2-2.9.0/tests/alerters/alertmanager_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/chatwork_test.py` & `elastalert2-2.9.0/tests/alerters/chatwork_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/command_test.py` & `elastalert2-2.9.0/tests/alerters/command_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/datadog_test.py` & `elastalert2-2.9.0/tests/alerters/datadog_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/debug_test.py` & `elastalert2-2.9.0/tests/alerters/debug_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/dingtalk_test.py` & `elastalert2-2.9.0/tests/alerters/dingtalk_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/discord_test.py` & `elastalert2-2.9.0/tests/alerters/discord_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/email_test.py` & `elastalert2-2.9.0/tests/alerters/email_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/exotel_test.py` & `elastalert2-2.9.0/tests/alerters/exotel_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/gitter_test.py` & `elastalert2-2.9.0/tests/alerters/gitter_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/googlechat_test.py` & `elastalert2-2.9.0/tests/alerters/googlechat_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/httppost2_test.py` & `elastalert2-2.9.0/tests/alerters/httppost2_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/httppost_test.py` & `elastalert2-2.9.0/tests/alerters/httppost_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/jira_test.py` & `elastalert2-2.9.0/tests/alerters/jira_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/line_test.py` & `elastalert2-2.9.0/tests/alerters/line_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/mattermost_test.py` & `elastalert2-2.9.0/tests/alerters/mattermost_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n'
             }
         ],
         'username': 'elastalert',
         'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -92,14 +93,15 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n'
             }
         ],
         'username': 'elastalert',
         'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -139,15 +141,16 @@
                 'title': 'Test Mattermost',
                 'pretext': 'aaaaa',
                 'fields': []
             }
         ],
         'text': 'Test Mattermost Rule\n\n',
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -203,15 +206,16 @@
                     {'title': 'Stack', 'value': '<MISSING VALUE> <MISSING VALUE>', 'short': False},
                     {'title': 'Name', 'value': 'static field', 'short': False}
                 ],
                 'text': 'Test Mattermost Rule\n\n'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -302,15 +306,16 @@
                 'title': 'Test Mattermost',
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n'
             }
         ],
         'username': 'elastalert',
-        'channel': 'test channel'
+        'channel': 'test channel',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -351,15 +356,16 @@
                 'title': 'Test Mattermost',
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=False,
@@ -402,15 +408,16 @@
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'title': 'mattermost.title',
                 'title_link': 'http://title.url'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -452,15 +459,16 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'footer': 'Mattermost footer'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -502,15 +510,16 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'footer_icon': 'http://icon.url'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -552,15 +561,16 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'image_url': 'http://image.url'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -602,15 +612,16 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'thumb_url': 'http://thumb.url'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -652,15 +663,16 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'author_name': 'author name'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -702,15 +714,16 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'author_link': 'http://author.link.url'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -752,15 +765,16 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'author_icon': 'http://author.icon.url'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -855,15 +869,16 @@
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n',
                 'author_icon': 'http://author.icon.url'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -960,15 +975,16 @@
             {
                 'color': '#ec4b98',
                 'title': 'Discover in Kibana',
                 'title_link': 'http://localhost:5601/app/discover#/'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
         proxies=None
@@ -1004,15 +1020,16 @@
                 'title': 'Test Rule',
                 'pretext': '',
                 'fields': [],
                 'text': 'Test Rule\n\n'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
         proxies=None
@@ -1055,15 +1072,16 @@
             {
                 'color': '#ec4b98',
                 'title': 'Click to discover in Kibana',
                 'title_link': 'http://localhost:5601/app/discover#/'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
         proxies=None
@@ -1106,15 +1124,16 @@
             {
                 'color': 'blue',
                 'title': 'Discover in Kibana',
                 'title_link': 'http://localhost:5601/app/discover#/'
             }
         ],
         'username': 'elastalert',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
         proxies=None
@@ -1154,15 +1173,16 @@
                 'title': 'Test Mattermost',
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n'
             }
         ],
         'username': 'test user',
-        'channel': ''
+        'channel': '',
+        'icon_emoji': ':ghost:'
     }
 
     mock_post_request.assert_called_once_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
@@ -1203,29 +1223,31 @@
                 'title': 'Test Mattermost',
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n'
             }
         ],
         'username': 'elastalert',
-        'channel': '#test-alert'
+        'channel': '#test-alert',
+        'icon_emoji': ':ghost:'
     }
     expected_data2 = {
         'attachments': [
             {
                 'fallback': 'Test Mattermost: aaaaa',
                 'color': 'danger',
                 'title': 'Test Mattermost',
                 'pretext': 'aaaaa',
                 'fields': [],
                 'text': 'Test Mattermost Rule\n\n'
             }
         ],
         'username': 'elastalert',
-        'channel': '#test-alert2'
+        'channel': '#test-alert2',
+        'icon_emoji': ':ghost:'
     }
     mock_post_request.assert_called_with(
         rule['mattermost_webhook_url'],
         data=mock.ANY,
         headers={'content-type': 'application/json'},
         verify=True,
         proxies=None
```

### Comparing `elastalert2-2.8.0/tests/alerters/opsgenie_test.py` & `elastalert2-2.9.0/tests/alerters/opsgenie_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/pagerduty_test.py` & `elastalert2-2.9.0/tests/alerters/pagerduty_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/pagertree_test.py` & `elastalert2-2.9.0/tests/alerters/pagertree_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/rocketchat_test.py` & `elastalert2-2.9.0/tests/alerters/rocketchat_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/servicenow_test.py` & `elastalert2-2.9.0/tests/alerters/servicenow_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/ses_test.py` & `elastalert2-2.9.0/tests/alerters/ses_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/slack_test.py` & `elastalert2-2.9.0/tests/alerters/slack_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/sns_test.py` & `elastalert2-2.9.0/tests/alerters/sns_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/stomp_test.py` & `elastalert2-2.9.0/tests/alerters/stomp_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/teams_test.py` & `elastalert2-2.9.0/tests/alerters/teams_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/telegram_test.py` & `elastalert2-2.9.0/tests/alerters/telegram_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/tencentsms_test.py` & `elastalert2-2.9.0/tests/alerters/tencentsms_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/thehive_test.py` & `elastalert2-2.9.0/tests/alerters/thehive_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/twilio_test.py` & `elastalert2-2.9.0/tests/alerters/twilio_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/victorops_test.py` & `elastalert2-2.9.0/tests/alerters/victorops_test.py`

 * *Files identical despite different names*

### Comparing `elastalert2-2.8.0/tests/alerters/zabbix_test.py` & `elastalert2-2.9.0/tests/alerters/zabbix_test.py`

 * *Files identical despite different names*

