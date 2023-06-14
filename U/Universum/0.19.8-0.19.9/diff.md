# Comparing `tmp/Universum-0.19.8.tar.gz` & `tmp/Universum-0.19.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Universum-0.19.8.tar", last modified: Tue Jun 15 09:05:50 2021, max compression
+gzip compressed data, was "Universum-0.19.9.tar", last modified: Mon Oct 11 11:07:03 2021, max compression
```

## Comparing `Universum-0.19.8.tar` & `Universum-0.19.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.516667 Universum-0.19.8/
--rw-rw-r--   0 user      (1000) user      (1000)    11369 2021-06-15 09:05:50.516667 Universum-0.19.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     9380 2021-04-28 11:45:14.000000 Universum-0.19.8/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.392662 Universum-0.19.8/Universum.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    11369 2021-06-15 09:05:49.000000 Universum-0.19.8/Universum.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1915 2021-06-15 09:05:49.000000 Universum-0.19.8/Universum.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2021-06-15 09:05:49.000000 Universum-0.19.8/Universum.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      427 2021-06-15 09:05:49.000000 Universum-0.19.8/Universum.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       14 2021-06-15 09:05:49.000000 Universum-0.19.8/Universum.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.392662 Universum-0.19.8/doc/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-28 11:45:14.000000 Universum-0.19.8/doc/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5602 2021-04-28 11:45:14.000000 Universum-0.19.8/doc/conf.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2021-06-15 09:05:50.516667 Universum-0.19.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1513 2021-06-15 08:44:55.000000 Universum-0.19.8/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.444664 Universum-0.19.8/universum/
--rw-rw-r--   0 user      (1000) user      (1000)       47 2021-06-15 08:44:55.000000 Universum-0.19.8/universum/__init__.py
--rwxrwxr-x   0 user      (1000) user      (1000)     3701 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/__main__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.444664 Universum-0.19.8/universum/analyzers/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/analyzers/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1435 2021-06-15 08:44:55.000000 Universum-0.19.8/universum/analyzers/mypy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1433 2021-06-15 08:44:55.000000 Universum-0.19.8/universum/analyzers/pylint.py
--rw-rw-r--   0 user      (1000) user      (1000)     1719 2021-06-15 08:44:55.000000 Universum-0.19.8/universum/analyzers/scan_build_report.py
--rwxrwxr-x   0 user      (1000) user      (1000)     7045 2021-06-15 08:44:55.000000 Universum-0.19.8/universum/analyzers/uncrustify.py
--rw-rw-r--   0 user      (1000) user      (1000)     5327 2021-06-15 08:44:55.000000 Universum-0.19.8/universum/analyzers/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     1134 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/api.py
--rw-rw-r--   0 user      (1000) user      (1000)     1149 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/config_creator.py
--rw-rw-r--   0 user      (1000) user      (1000)    32494 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/configuration_support.py
--rw-rw-r--   0 user      (1000) user      (1000)     6728 2021-05-19 11:41:29.000000 Universum-0.19.8/universum/github_handler.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.448664 Universum-0.19.8/universum/lib/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/lib/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      432 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/lib/ci_exception.py
--rw-rw-r--   0 user      (1000) user      (1000)     4933 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/lib/gravity.py
--rw-rw-r--   0 user      (1000) user      (1000)     4646 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/lib/module_arguments.py
--rw-rw-r--   0 user      (1000) user      (1000)     6926 2021-05-19 11:41:29.000000 Universum-0.19.8/universum/lib/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     5231 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/main.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.464665 Universum-0.19.8/universum/modules/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2157 2021-05-12 07:42:39.000000 Universum-0.19.8/universum/modules/api_support.py
--rw-rw-r--   0 user      (1000) user      (1000)    10966 2021-05-12 07:42:39.000000 Universum-0.19.8/universum/modules/artifact_collector.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.468665 Universum-0.19.8/universum/modules/automation_server/
--rw-rw-r--   0 user      (1000) user      (1000)       33 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/automation_server/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2888 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/automation_server/automation_server.py
--rw-rw-r--   0 user      (1000) user      (1000)      932 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/automation_server/base_server.py
--rw-rw-r--   0 user      (1000) user      (1000)     2807 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/automation_server/jenkins_server.py
--rw-rw-r--   0 user      (1000) user      (1000)      399 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/automation_server/local_server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5456 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/automation_server/teamcity_server.py
--rw-rw-r--   0 user      (1000) user      (1000)     3155 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/code_report_collector.py
--rw-rw-r--   0 user      (1000) user      (1000)     1909 2021-05-19 11:41:29.000000 Universum-0.19.8/universum/modules/error_state.py
--rw-rw-r--   0 user      (1000) user      (1000)    16749 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/launcher.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.468665 Universum-0.19.8/universum/modules/output/
--rw-rw-r--   0 user      (1000) user      (1000)       22 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/output/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      926 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/output/base_output.py
--rw-rw-r--   0 user      (1000) user      (1000)     3280 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/output/output.py
--rw-rw-r--   0 user      (1000) user      (1000)     1545 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/output/teamcity_output.py
--rw-rw-r--   0 user      (1000) user      (1000)     2586 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/output/terminal_based_output.py
--rw-rw-r--   0 user      (1000) user      (1000)      850 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/project_directory.py
--rw-rw-r--   0 user      (1000) user      (1000)     5995 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/reporter.py
--rw-rw-r--   0 user      (1000) user      (1000)     9279 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/structure_handler.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-06-15 09:05:50.504667 Universum-0.19.8/universum/modules/vcs/
--rw-rw-r--   0 user      (1000) user      (1000)       19 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/vcs/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2942 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/vcs/base_vcs.py
--rw-rw-r--   0 user      (1000) user      (1000)     7619 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/vcs/gerrit_vcs.py
--rw-rw-r--   0 user      (1000) user      (1000)    13851 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/vcs/git_vcs.py
--rw-rw-r--   0 user      (1000) user      (1000)    11409 2021-05-19 11:41:29.000000 Universum-0.19.8/universum/modules/vcs/github_vcs.py
--rw-rw-r--   0 user      (1000) user      (1000)     2721 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/vcs/local_vcs.py
--rw-rw-r--   0 user      (1000) user      (1000)    28919 2021-06-15 08:44:55.000000 Universum-0.19.8/universum/modules/vcs/perforce_vcs.py
--rw-rw-r--   0 user      (1000) user      (1000)    10894 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/vcs/swarm.py
--rw-rw-r--   0 user      (1000) user      (1000)     8241 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/modules/vcs/vcs.py
--rw-rw-r--   0 user      (1000) user      (1000)      958 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/nonci.py
--rw-rw-r--   0 user      (1000) user      (1000)     2821 2021-04-28 11:45:14.000000 Universum-0.19.8/universum/poll.py
--rw-rw-r--   0 user      (1000) user      (1000)     3500 2021-06-15 08:44:55.000000 Universum-0.19.8/universum/submit.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.290788 Universum-0.19.9/
+-rw-rw-r--   0 user      (1000) user      (1000)    11912 2021-10-11 11:07:03.290788 Universum-0.19.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     9859 2021-10-11 11:01:00.000000 Universum-0.19.9/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.282788 Universum-0.19.9/Universum.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    11912 2021-10-11 11:07:02.000000 Universum-0.19.9/Universum.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1914 2021-10-11 11:07:02.000000 Universum-0.19.9/Universum.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2021-10-11 11:07:02.000000 Universum-0.19.9/Universum.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      436 2021-10-11 11:07:02.000000 Universum-0.19.9/Universum.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       14 2021-10-11 11:07:02.000000 Universum-0.19.9/Universum.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.282788 Universum-0.19.9/doc/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-28 11:45:14.000000 Universum-0.19.9/doc/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5602 2021-04-28 11:45:14.000000 Universum-0.19.9/doc/conf.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2021-10-11 11:07:03.290788 Universum-0.19.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2021-10-11 11:01:00.000000 Universum-0.19.9/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.286788 Universum-0.19.9/universum/
+-rw-rw-r--   0 user      (1000) user      (1000)       47 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     3665 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/__main__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.286788 Universum-0.19.9/universum/analyzers/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/analyzers/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1435 2021-06-23 14:07:44.000000 Universum-0.19.9/universum/analyzers/mypy.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1433 2021-06-23 14:07:44.000000 Universum-0.19.9/universum/analyzers/pylint.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     7111 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/analyzers/uncrustify.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5370 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/analyzers/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1134 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/api.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1159 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/config_creator.py
+-rw-rw-r--   0 user      (1000) user      (1000)    32494 2021-07-22 15:10:31.000000 Universum-0.19.9/universum/configuration_support.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6987 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/github_handler.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.286788 Universum-0.19.9/universum/lib/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/lib/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      432 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/lib/ci_exception.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4925 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/lib/gravity.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4634 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/lib/module_arguments.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6937 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/lib/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5231 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/main.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.286788 Universum-0.19.9/universum/modules/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2157 2021-06-23 14:07:44.000000 Universum-0.19.9/universum/modules/api_support.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11384 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/artifact_collector.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.290788 Universum-0.19.9/universum/modules/automation_server/
+-rw-rw-r--   0 user      (1000) user      (1000)       33 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/automation_server/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2888 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/automation_server/automation_server.py
+-rw-rw-r--   0 user      (1000) user      (1000)      932 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/automation_server/base_server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2805 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/automation_server/jenkins_server.py
+-rw-rw-r--   0 user      (1000) user      (1000)      399 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/automation_server/local_server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5421 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/automation_server/teamcity_server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5630 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/code_report_collector.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1927 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/error_state.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17073 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/launcher.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.290788 Universum-0.19.9/universum/modules/output/
+-rw-rw-r--   0 user      (1000) user      (1000)       22 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/output/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1416 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/output/base_output.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4919 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/output/html_output.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5049 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/output/output.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1476 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/output/teamcity_output.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2586 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/output/terminal_based_output.py
+-rw-rw-r--   0 user      (1000) user      (1000)      850 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/project_directory.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6257 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/reporter.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9099 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/structure_handler.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-10-11 11:07:03.290788 Universum-0.19.9/universum/modules/vcs/
+-rw-rw-r--   0 user      (1000) user      (1000)       19 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/vcs/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2941 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/vcs/base_vcs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7619 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/modules/vcs/gerrit_vcs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13827 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/vcs/git_vcs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11601 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/vcs/github_vcs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2723 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/vcs/local_vcs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    29386 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/vcs/perforce_vcs.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10876 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/vcs/swarm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8205 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/modules/vcs/vcs.py
+-rw-rw-r--   0 user      (1000) user      (1000)      958 2021-04-28 11:45:14.000000 Universum-0.19.9/universum/nonci.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2833 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/poll.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3853 2021-10-11 11:01:00.000000 Universum-0.19.9/universum/submit.py
```

### Comparing `Universum-0.19.8/PKG-INFO` & `Universum-0.19.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Universum
-Version: 0.19.8
+Version: 0.19.9
 Summary: Unifier of Continuous Integration
 Home-page: UNKNOWN
 Author: Ivan Keliukh <i.keliukh@samsung.com>, Kateryna Dovgan <k.dovgan@samsung.com>
 License: BSD
 Description: # Project 'Universum'
         [![Documentation Status](https://readthedocs.org/projects/universum/badge/?version=latest)](
         https://universum.readthedocs.io/en/latest/?badge=latest)
@@ -50,19 +50,20 @@
         1. Install all of the VCS extras as described in the [Universum installation manual](
            https://universum.readthedocs.io/en/latest/install.html#vcs-related-extras),
            (including installation of Git and P4 CLI)
         2. Install Docker (`docker-ce`, `docker-ce-cli`) as described in the [official installation manual](
            https://docs.docker.com/engine/installation/linux/ubuntu/#install-using-the-repository)
         
            * Also add current user to 'docker' group (use `sudo usermod -a -G docker $USER` and then relogin)
+        3. Install Mozilla WebDriver: `sudo apt install firefox-geckodriver`
         
         Further commands:
         ```bash
         python3.7 -m venv virtual-environment-python3.7
-        source ./virtual-environment/bin/activate
+        source ./virtual-environment-python3.7/bin/activate
         git clone https://github.com/Samsung/Universum.git universum-working-dir
         cd universum-working-dir
         git checkout master
         pip install -U .[test]
         make images
         ```
         And after this the `pytest` or `make test` commands can be executed (see below).
@@ -78,14 +79,16 @@
             * `pytest`
             * `pylint`
             * `pytest-pylint`
             * `teamcity-messages` (is not actually used in manual testing, but is there for CI)
             * `pytest-cov`
             * `coverage`
             * `mypy`
+            * `types-requests`
+            * `selenium`
         
         Although it is possible to get these modules via `pip3.7 install -U universum[test]`, it might be more convenient
         to checkout the Universum branch you are currently working on, change working directory to project root and
         run a `pip3.7 install -U .[test]` command from there for more flexibility. Using virtual environment (via `venv`
         command) allows to separate test environment from system and provides even more control over additional modules.
         
         Uninstalling Universum via `pip uninstall universum` will not uninstall all the dependencies installed along with it.
@@ -110,14 +113,19 @@
         pip install -U nox
         cd universum-working-dir
         nox
         ```
         This will launch the testing scenario, described in `noxfile.py`. This scenario includes rebuilding docker images
         for every supported Python version and running all the tests for corresponding Python.
         
+        Also, setting up "REUSE_DOCKER_CONTAINERS" environment variable (or running tests in PyCharm) will let tests
+        reuse already created and initialized containers, which speeds up the testing process. But do note that this is
+        recommended for development purposes only. Without recreating containers, the remnants of previous test runs
+        may affect the current test run.
+        
         
         ## Project contents
         
         `universum` is main project folder, that is being copied to Python libraries location
         (e.g. `dist-packages` or `site-packages`) when installed.
         It contains `__main__.py` script, that is the main entry point to the whole project.
         It also contains the following modules:
@@ -130,15 +138,15 @@
         * `lib` - utility functions libraries
         
           * `ci_exception` - internal exceptions
           * `module_arguments` - handles [command line](
             https://universum.readthedocs.io/en/latest/args.html) and other parameters
           * `gravity` - inter-module communication
           * `utils` - miscellaneous
-          
+        
         * `modules` - independent packages
         
           * `api_support` - 'main' mode module to answer API requests
           * `automation_server` - drivers for CI systems (e.g. Jenkins)
           * `artifact_collector` - implements [build artifacts](
             https://universum.readthedocs.io/en/latest/configuring.html#common-variations-keys)
           * `code_report_collector` - support for [external 'code report' modules](
@@ -153,15 +161,15 @@
         
         Also there are 'base' modules/classes for driver implementation standardization,
         and 'main' modules/classes for automated driver choosing based on environment and settings.
         
         `doc` directory contains sources for [project documentation](
         https://universum.readthedocs.io/en/latest/index.html). It can be generated
         locally with running `make` from root directory using Sphinx.
-          
+        
         `tests` directory contains test system, based on PyTest. Full tests can be started
         from root directory via `make tests` command, otherwise use standard PyTest syntax.
         *Commits failing any of project tests should not be merged into 'master' branch!*
         
         `examples` contains various examples of [project configuration files](
         https://universum.readthedocs.io/en/latest/configuring.html). Usage of such files
         is illustrated in `run_basic_example.sh` script.
```

### Comparing `Universum-0.19.8/README.md` & `Universum-0.19.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,19 +43,20 @@
 1. Install all of the VCS extras as described in the [Universum installation manual](
    https://universum.readthedocs.io/en/latest/install.html#vcs-related-extras),
    (including installation of Git and P4 CLI)
 2. Install Docker (`docker-ce`, `docker-ce-cli`) as described in the [official installation manual](
    https://docs.docker.com/engine/installation/linux/ubuntu/#install-using-the-repository)
 
    * Also add current user to 'docker' group (use `sudo usermod -a -G docker $USER` and then relogin)
+3. Install Mozilla WebDriver: `sudo apt install firefox-geckodriver`
 
 Further commands:
 ```bash
 python3.7 -m venv virtual-environment-python3.7
-source ./virtual-environment/bin/activate
+source ./virtual-environment-python3.7/bin/activate
 git clone https://github.com/Samsung/Universum.git universum-working-dir
 cd universum-working-dir
 git checkout master
 pip install -U .[test]
 make images
 ```
 And after this the `pytest` or `make test` commands can be executed (see below).
@@ -71,14 +72,16 @@
     * `pytest`
     * `pylint`
     * `pytest-pylint`
     * `teamcity-messages` (is not actually used in manual testing, but is there for CI)
     * `pytest-cov`
     * `coverage`
     * `mypy`
+    * `types-requests`
+    * `selenium`
 
 Although it is possible to get these modules via `pip3.7 install -U universum[test]`, it might be more convenient
 to checkout the Universum branch you are currently working on, change working directory to project root and
 run a `pip3.7 install -U .[test]` command from there for more flexibility. Using virtual environment (via `venv`
 command) allows to separate test environment from system and provides even more control over additional modules.
 
 Uninstalling Universum via `pip uninstall universum` will not uninstall all the dependencies installed along with it.
@@ -103,14 +106,19 @@
 pip install -U nox
 cd universum-working-dir
 nox
 ```
 This will launch the testing scenario, described in `noxfile.py`. This scenario includes rebuilding docker images
 for every supported Python version and running all the tests for corresponding Python.
 
+Also, setting up "REUSE_DOCKER_CONTAINERS" environment variable (or running tests in PyCharm) will let tests
+reuse already created and initialized containers, which speeds up the testing process. But do note that this is
+recommended for development purposes only. Without recreating containers, the remnants of previous test runs
+may affect the current test run.
+
 
 ## Project contents
 
 `universum` is main project folder, that is being copied to Python libraries location
 (e.g. `dist-packages` or `site-packages`) when installed.
 It contains `__main__.py` script, that is the main entry point to the whole project.
 It also contains the following modules:
@@ -123,15 +131,15 @@
 * `lib` - utility functions libraries
 
   * `ci_exception` - internal exceptions
   * `module_arguments` - handles [command line](
     https://universum.readthedocs.io/en/latest/args.html) and other parameters
   * `gravity` - inter-module communication
   * `utils` - miscellaneous
-  
+
 * `modules` - independent packages
 
   * `api_support` - 'main' mode module to answer API requests
   * `automation_server` - drivers for CI systems (e.g. Jenkins)
   * `artifact_collector` - implements [build artifacts](
     https://universum.readthedocs.io/en/latest/configuring.html#common-variations-keys)
   * `code_report_collector` - support for [external 'code report' modules](
@@ -146,15 +154,15 @@
 
 Also there are 'base' modules/classes for driver implementation standardization,
 and 'main' modules/classes for automated driver choosing based on environment and settings.
 
 `doc` directory contains sources for [project documentation](
 https://universum.readthedocs.io/en/latest/index.html). It can be generated
 locally with running `make` from root directory using Sphinx.
-  
+
 `tests` directory contains test system, based on PyTest. Full tests can be started
 from root directory via `make tests` command, otherwise use standard PyTest syntax.
 *Commits failing any of project tests should not be merged into 'master' branch!*
 
 `examples` contains various examples of [project configuration files](
 https://universum.readthedocs.io/en/latest/configuring.html). Usage of such files
 is illustrated in `run_basic_example.sh` script.
```

### Comparing `Universum-0.19.8/Universum.egg-info/PKG-INFO` & `Universum-0.19.9/Universum.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Universum
-Version: 0.19.8
+Version: 0.19.9
 Summary: Unifier of Continuous Integration
 Home-page: UNKNOWN
 Author: Ivan Keliukh <i.keliukh@samsung.com>, Kateryna Dovgan <k.dovgan@samsung.com>
 License: BSD
 Description: # Project 'Universum'
         [![Documentation Status](https://readthedocs.org/projects/universum/badge/?version=latest)](
         https://universum.readthedocs.io/en/latest/?badge=latest)
@@ -50,19 +50,20 @@
         1. Install all of the VCS extras as described in the [Universum installation manual](
            https://universum.readthedocs.io/en/latest/install.html#vcs-related-extras),
            (including installation of Git and P4 CLI)
         2. Install Docker (`docker-ce`, `docker-ce-cli`) as described in the [official installation manual](
            https://docs.docker.com/engine/installation/linux/ubuntu/#install-using-the-repository)
         
            * Also add current user to 'docker' group (use `sudo usermod -a -G docker $USER` and then relogin)
+        3. Install Mozilla WebDriver: `sudo apt install firefox-geckodriver`
         
         Further commands:
         ```bash
         python3.7 -m venv virtual-environment-python3.7
-        source ./virtual-environment/bin/activate
+        source ./virtual-environment-python3.7/bin/activate
         git clone https://github.com/Samsung/Universum.git universum-working-dir
         cd universum-working-dir
         git checkout master
         pip install -U .[test]
         make images
         ```
         And after this the `pytest` or `make test` commands can be executed (see below).
@@ -78,14 +79,16 @@
             * `pytest`
             * `pylint`
             * `pytest-pylint`
             * `teamcity-messages` (is not actually used in manual testing, but is there for CI)
             * `pytest-cov`
             * `coverage`
             * `mypy`
+            * `types-requests`
+            * `selenium`
         
         Although it is possible to get these modules via `pip3.7 install -U universum[test]`, it might be more convenient
         to checkout the Universum branch you are currently working on, change working directory to project root and
         run a `pip3.7 install -U .[test]` command from there for more flexibility. Using virtual environment (via `venv`
         command) allows to separate test environment from system and provides even more control over additional modules.
         
         Uninstalling Universum via `pip uninstall universum` will not uninstall all the dependencies installed along with it.
@@ -110,14 +113,19 @@
         pip install -U nox
         cd universum-working-dir
         nox
         ```
         This will launch the testing scenario, described in `noxfile.py`. This scenario includes rebuilding docker images
         for every supported Python version and running all the tests for corresponding Python.
         
+        Also, setting up "REUSE_DOCKER_CONTAINERS" environment variable (or running tests in PyCharm) will let tests
+        reuse already created and initialized containers, which speeds up the testing process. But do note that this is
+        recommended for development purposes only. Without recreating containers, the remnants of previous test runs
+        may affect the current test run.
+        
         
         ## Project contents
         
         `universum` is main project folder, that is being copied to Python libraries location
         (e.g. `dist-packages` or `site-packages`) when installed.
         It contains `__main__.py` script, that is the main entry point to the whole project.
         It also contains the following modules:
@@ -130,15 +138,15 @@
         * `lib` - utility functions libraries
         
           * `ci_exception` - internal exceptions
           * `module_arguments` - handles [command line](
             https://universum.readthedocs.io/en/latest/args.html) and other parameters
           * `gravity` - inter-module communication
           * `utils` - miscellaneous
-          
+        
         * `modules` - independent packages
         
           * `api_support` - 'main' mode module to answer API requests
           * `automation_server` - drivers for CI systems (e.g. Jenkins)
           * `artifact_collector` - implements [build artifacts](
             https://universum.readthedocs.io/en/latest/configuring.html#common-variations-keys)
           * `code_report_collector` - support for [external 'code report' modules](
@@ -153,15 +161,15 @@
         
         Also there are 'base' modules/classes for driver implementation standardization,
         and 'main' modules/classes for automated driver choosing based on environment and settings.
         
         `doc` directory contains sources for [project documentation](
         https://universum.readthedocs.io/en/latest/index.html). It can be generated
         locally with running `make` from root directory using Sphinx.
-          
+        
         `tests` directory contains test system, based on PyTest. Full tests can be started
         from root directory via `make tests` command, otherwise use standard PyTest syntax.
         *Commits failing any of project tests should not be merged into 'master' branch!*
         
         `examples` contains various examples of [project configuration files](
         https://universum.readthedocs.io/en/latest/configuring.html). Usage of such files
         is illustrated in `run_basic_example.sh` script.
```

### Comparing `Universum-0.19.8/Universum.egg-info/SOURCES.txt` & `Universum-0.19.9/Universum.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 universum/main.py
 universum/nonci.py
 universum/poll.py
 universum/submit.py
 universum/analyzers/__init__.py
 universum/analyzers/mypy.py
 universum/analyzers/pylint.py
-universum/analyzers/scan_build_report.py
 universum/analyzers/uncrustify.py
 universum/analyzers/utils.py
 universum/lib/__init__.py
 universum/lib/ci_exception.py
 universum/lib/gravity.py
 universum/lib/module_arguments.py
 universum/lib/utils.py
@@ -41,14 +40,15 @@
 universum/modules/automation_server/automation_server.py
 universum/modules/automation_server/base_server.py
 universum/modules/automation_server/jenkins_server.py
 universum/modules/automation_server/local_server.py
 universum/modules/automation_server/teamcity_server.py
 universum/modules/output/__init__.py
 universum/modules/output/base_output.py
+universum/modules/output/html_output.py
 universum/modules/output/output.py
 universum/modules/output/teamcity_output.py
 universum/modules/output/terminal_based_output.py
 universum/modules/vcs/__init__.py
 universum/modules/vcs/base_vcs.py
 universum/modules/vcs/gerrit_vcs.py
 universum/modules/vcs/git_vcs.py
```

### Comparing `Universum-0.19.8/doc/conf.py` & `Universum-0.19.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/setup.py` & `Universum-0.19.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 import universum
 
 
 def readme():
-    with open('README.md') as f:
+    with open('README.md', encoding="utf-8") as f:
         return f.read()
 
 
 p4 = ('pip>=19', 'p4python>=2019.1')
 
 git = 'gitpython>=3.0.5'
 
@@ -50,15 +50,16 @@
             'pytest',
             'pylint',
             'pytest-pylint',
             'teamcity-messages',
             'pytest-cov',
             'coverage',
             'mypy',
-            'types-requests'
+            'types-requests',
+            'selenium'
         ]
     }
 )
 
 
 if __name__ == "__main__":
     print("Please use 'sudo pip install .' instead of launching this script")
```

### Comparing `Universum-0.19.8/universum/__main__.py` & `Universum-0.19.9/universum/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     result = 0
     error_state_module = construct_component(GlobalErrorState, settings)
     main_module = construct_component(settings.main_class, settings)
 
     if error_state_module.is_in_error_state():
         raise IncorrectParameterError(("\n\n"+"-"*80 + "\n").join(error_state_module.get_errors()))
 
-    main_module.out.log("{} {} started execution".format(__title__, __version__))
+    main_module.out.log_execution_start(__title__, __version__)
 
     def signal_handler(signal_number, stack_frame):
         raise KeyboardInterrupt
 
     signal.signal(signal.SIGTERM, signal_handler)
 
     try:
@@ -69,15 +69,15 @@
 
     except Exception as e:
         ex_traceback = sys.exc_info()[2]
         main_module.out.log_exception("Unexpected error.\n" + format_traceback(e, ex_traceback))
         main_module.out.report_build_problem("Unexpected error while executing script.")
         result = 2
 
-    main_module.out.log("{} {} finished execution".format(__title__, __version__))
+    main_module.out.log_execution_finish(__title__, __version__)
     return result
 
 
 def main(args: Optional[List[str]] = None) -> int:
     parser = define_arguments()
     settings = parser.parse_args(args)
     settings.main_class = getattr(settings, "main_class", Main)
```

### Comparing `Universum-0.19.8/universum/analyzers/mypy.py` & `Universum-0.19.9/universum/analyzers/mypy.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/analyzers/pylint.py` & `Universum-0.19.9/universum/analyzers/pylint.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/analyzers/uncrustify.py` & `Universum-0.19.9/universum/analyzers/uncrustify.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,37 +56,37 @@
     def __init__(self, target_folder: Path, wrapcolumn: int, tabsize: int) -> None:
         self.target_folder = target_folder
         self.differ = difflib.HtmlDiff(tabsize=tabsize, wrapcolumn=wrapcolumn)
 
     def __call__(self, file: Path, src: List[str], target: List[str]) -> None:
         file_relative = file.relative_to(Path.cwd())
         out_file_name: str = str(file_relative).replace('/', '_') + '.html'
-        with open(self.target_folder.joinpath(out_file_name), 'w') as out_file:
+        with open(self.target_folder.joinpath(out_file_name), 'w', encoding="utf-8") as out_file:
             out_file.write(self.differ.make_file(src, target, context=False))
 
 
 def uncrustify_output_parser(files: List[Tuple[Path, Path]],
                              write_diff_file: Optional[Callable[[Path, List[str], List[str]], None]]
                              ) -> List[utils.ReportData]:
     result: List[utils.ReportData] = []
     for src_file, uncrustify_file in files:
-        with open(src_file) as src:
+        with open(src_file, encoding="utf-8") as src:
             src_lines = src.readlines()
-        with open(uncrustify_file) as fixed:
+        with open(uncrustify_file, encoding="utf-8") as fixed:
             fixed_lines = fixed.readlines()
 
         issues = _get_issues_from_diff(src_file, src_lines, fixed_lines)
         if issues and write_diff_file:
             write_diff_file(src_file, src_lines, fixed_lines)
         result.extend(issues)
     return result
 
 
 def _get_wrapcolumn_tabsize(cfg_file: str) -> Tuple[int, int]:
-    with open(cfg_file) as config:
+    with open(cfg_file, encoding="utf-8") as config:
         for line in config.readlines():
             if line.startswith("code_width"):
                 wrapcolumn = int(line.split()[2])
             if line.startswith("input_tab_size"):
                 tabsize = int(line.split()[2])
     return wrapcolumn, tabsize
 
@@ -146,14 +146,14 @@
 
 
 def _get_text_for_block(start: int, end: int, lines: List[str]) -> str:
     return _replace_invisible_symbols(''.join(lines[start: end]))
 
 
 def _replace_invisible_symbols(line: str) -> str:
-    for old_str, new_str in zip([u" ", u"\t", u"\n"], [u"\u00b7", u"\u2192\u2192\u2192\u2192", u"\u2193\u000a"]):
+    for old_str, new_str in zip([" ", "\t", "\n"], ["\u00b7", "\u2192\u2192\u2192\u2192", "\u2193\u000a"]):
         line = line.replace(old_str, new_str)
     return line
 
 
 if __name__ == "__main__":
     main()  # pylint: disable=no-value-for-parameter  # see https://github.com/PyCQA/pylint/issues/259
```

### Comparing `Universum-0.19.8/universum/analyzers/utils.py` & `Universum-0.19.9/universum/analyzers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,16 @@
                              "For example, if the version is 3.7, it uses the following command: "
                              "'python3.7 -m pylint <...>'")
 
 
 def report_to_file(issues: List[ReportData], json_file: str = None) -> None:
     issues_json = json.dumps(issues, indent=4)
     if json_file:
-        open(json_file, "w").write(issues_json)
+        with open(json_file, "w", encoding="utf-8") as f:
+            f.write(issues_json)
     else:
         sys.stdout.write(issues_json)
 
 
 def normalize(file: str) -> pathlib.Path:
     file_path = pathlib.Path(file)
     return file_path if file_path.is_absolute() else pathlib.Path.cwd().joinpath(file_path)
```

### Comparing `Universum-0.19.8/universum/api.py` & `Universum-0.19.9/universum/api.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/config_creator.py` & `Universum-0.19.9/universum/config_creator.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,21 +16,21 @@
         self.out = MinimalOut()
 
     def execute(self) -> None:
         config_name = ".universum.py"
         self.out.log(f"Creating an example configuration file '{config_name}'")
 
         config = Path(config_name)
-        config.write_text("""#!/usr/bin/env {}
+        config.write_text(f"""#!/usr/bin/env {PYTHON_VERSION}
 
 from universum.configuration_support import Configuration, Step
 
 configs = Configuration([Step(name='Show directory contents', command=['ls', '-la']),
                          Step(name='Print a line', command=['bash', '-c', 'echo Hello world'])])
 
 if __name__ == '__main__':
     print(configs.dump())
-""".format(PYTHON_VERSION))
+""", encoding="utf-8")
         self.out.log(f"To run with Universum, execute the following command:\n$ {PYTHON_VERSION} -m universum run")
 
     def finalize(self) -> None:
         pass
```

### Comparing `Universum-0.19.8/universum/configuration_support.py` & `Universum-0.19.9/universum/configuration_support.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/github_handler.py` & `Universum-0.19.9/universum/github_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
     @staticmethod
     def define_arguments(argument_parser):
         argument_parser.add_argument('--event', '-e', dest='event', metavar="GITHUB_EVENT",
                                      help='Currently parsed from "x-github-event" header of received web-hook')
         argument_parser.add_argument('--payload', '-pl', dest='payload', metavar="GITHUB_PAYLOAD",
                                      help='Full contents of web-hook received; pass a JSON file path, starting it '
-                                          'with "@" character, or use an environment variable for convenience')
+                                          'with "@" character, or use an environment variable for convenience. '
+                                          'Please note, that when passing a file, it is expected to be '
+                                          'in UTF-8 encoding')
         argument_parser.add_argument('--trigger-url', '-tu', dest='trigger_url', metavar="TRIGGER_URL",
                                      help='URL for GET request to trigger the CI build and pass all parameters '
                                           'parsed from payload; if any constant parameters (like token) are '
                                           'required, include them in this string as well, e.g.: '
                                           '"http://jenkins.com/job/JobName/build?token=MYTOKEN"')
         argument_parser.add_argument('--suite-name', '-sn', dest='suite_name', metavar="SUITE_NAME", default="CI tests",
                                      help='GitHub check suite name, default is "CI tests"')
@@ -53,15 +55,16 @@
         self.payload = self.read_and_check_multiline_option("payload", """
             GitHub web-hook payload JSON is not specified.
 
             Please pass incoming web-hook request payload to this parameter directly via
             '--payload' ('-pl') command line parameter or by setting GITHUB_PAYLOAD
             environment variable, or by passing file path as the argument value (start
             filename with '@' character, e.g. '@/tmp/file.json' or '@payload.json' for
-            relative path starting at current directory)
+            relative path starting at current directory). Please note, that when passing
+            a file, it's expected to be in UTF-8 encoding
             """)
 
     @make_block("Analysing trigger payload")
     def execute(self):
         try:
             payload = json.loads(self.payload)
         except json.decoder.JSONDecodeError as error:
```

### Comparing `Universum-0.19.8/universum/lib/gravity.py` & `Universum-0.19.9/universum/lib/gravity.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 ComponentType = TypeVar('ComponentType', bound=Module)
 
 
 def construct_component(cls: Type[ComponentType], main_settings: 'HasModulesMapping', *args, **kwargs) -> ComponentType:
     if not getattr(main_settings, "active_modules", None):
-        main_settings.active_modules = dict()
+        main_settings.active_modules = {}
 
     if cls not in main_settings.active_modules:
         cls.settings = Settings(cls)
         instance: 'Module' = cls.__new__(cls, main_settings=main_settings)
         # https://github.com/python/mypy/blob/master/mypy/checkmember.py#180
         # Accessing __init__ in statically typed code would compromise
         # type safety unless used via super().
@@ -103,15 +103,15 @@
         def constructor_function(*args, **kwargs) -> DependencyType:
             return construct_component(self.cls, instance.main_settings, *args, **kwargs)
         return constructor_function
 
 
 def get_dependencies(cls: Type[Module], result: Optional[List[Type[Module]]] = None) -> List[Type[Module]]:
     if result is None:
-        result = list()
+        result = []
 
     result.append(cls)
 
     # parent classes
     all_dependencies: List[Type[Module]]
     all_dependencies = [x for x in cls.__mro__ if issubclass(x, Module) and x != Module and x != cls]
     # dependencies
```

### Comparing `Universum-0.19.8/universum/lib/module_arguments.py` & `Universum-0.19.9/universum/lib/module_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.container = container
         super().__init__(container, *args, **kwargs)
 
     def _add_action(self, action):
         if action.metavar is not None:
             try:
                 if 'sphinx' in sys.modules:
-                    action.help += "\n\nEnvironment variable: ${}".format(action.metavar)
+                    action.help += f"\n\nEnvironment variable: ${action.metavar}"
                 else:
                     if not isinstance(action, argparse._SubParsersAction):
                         action.help += f" [env: {action.metavar}]"
             except TypeError:
                 action.help = f"Also available as [env: {action.metavar}]"
             default = os.environ.get(action.metavar, action.default)
 
@@ -67,15 +67,15 @@
         self.container.prepend_dest(action)
 
 
 # noinspection PyProtectedMember
 class ModuleArgumentParser(argparse.ArgumentParser):
 
     def __init__(self, **kwargs):
-        self.groups = dict()
+        self.groups = {}
         self.dest_prefix = ''
         argparse.ArgumentParser.__init__(self, **kwargs)
 
     def add_argument_group(self, *args, **kwargs):
         group = ModuleArgumentGroup(self, *args, **kwargs)
         self._action_groups.append(group)
         return group
```

### Comparing `Universum-0.19.8/universum/lib/utils.py` & `Universum-0.19.9/universum/lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 raise CriticalCiException(str(e)) from e
         return function_to_run
     return decorated_function
 
 
 def trim_and_convert_to_unicode(line: Union[bytes, str]) -> str:
     if isinstance(line, bytes):
-        line = line.decode("utf-8")
+        line = line.decode("utf-8", "replace")
     elif not isinstance(line, str):
         line = str(line)
 
     if line.endswith("\n"):
         line = line[:-1]
 
     return line
```

### Comparing `Universum-0.19.8/universum/main.py` & `Universum-0.19.9/universum/main.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/modules/api_support.py` & `Universum-0.19.9/universum/modules/api_support.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/modules/artifact_collector.py` & `Universum-0.19.9/universum/modules/artifact_collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from ..lib.utils import make_block
 from ..lib import utils
 from .automation_server import AutomationServerForHostingBuild
 from .output import HasOutput
 from .project_directory import ProjectDirectory
 from .reporter import Reporter
 from .structure_handler import HasStructure
+from .output.html_output import HtmlOutput
+
 
 __all__ = [
     "ArtifactCollector"
 ]
 
 
 def make_big_archive(target, source):
@@ -55,14 +57,15 @@
 
     return filename
 
 
 class ArtifactCollector(ProjectDirectory, HasOutput, HasStructure):
     reporter_factory = Dependency(Reporter)
     automation_server_factory = Dependency(AutomationServerForHostingBuild)
+    html_output_factory = Dependency(HtmlOutput)
 
     @staticmethod
     def define_arguments(argument_parser):
         parser = argument_parser.get_or_create_group("Artifact collection",
                                                      "Parameters of archiving and collecting of build artifacts")
 
         parser.add_argument("--artifact-dir", "-ad", dest="artifact_dir", metavar="ARTIFACT_DIR",
@@ -87,14 +90,18 @@
         self.artifact_dir = self.settings.artifact_dir
 
         if not self.artifact_dir:
             self.artifact_dir = os.path.join(os.getcwd(), "artifacts")
         if not os.path.exists(self.artifact_dir):
             os.makedirs(self.artifact_dir)
 
+        self.html_output = self.html_output_factory()
+        self.html_output.set_artifact_dir(self.artifact_dir)
+        self.html_output.artifact_dir_ready = False
+
     def make_file_name(self, name):
         return utils.calculate_file_absolute_path(self.artifact_dir, name)
 
     # TODO: using codecs is legacy from Python2; this function needs to be refactored
     def create_text_file(self, name):
         try:
             file_name = self.make_file_name(name)
@@ -128,37 +135,39 @@
                     for matching_path in matches:
                         try:
                             os.remove(matching_path)  # TODO: use shutil by default
                         except OSError as e:
                             if "Is a directory" not in e.strerror:
                                 raise
                             shutil.rmtree(matching_path)
+                        self.out.log(f"Cleaned up '{matching_path}'")
                 elif not ignore_already_existing:
                     text = "Build artifacts, such as"
                     for matching_path in matches:
-                        text += "\n * '" + os.path.basename(matching_path) + "'"
-                    text += "\nalready exist in '" + os.path.dirname(item["path"]) + "' directory."
+                        text += f"\n * '{os.path.basename(matching_path)}'"
+                    text += f"\nalready exist in '{os.path.dirname(item['path'])}' directory."
                     text += "\nPossible reason of this error: previous build results in working directory"
                     raise CriticalCiException(text)
 
             # Check existence in 'artifacts' directory: wildcards NOT applied
             path_to_check1 = os.path.join(self.artifact_dir, os.path.basename(item["path"]))
             path_to_check2 = os.path.join(path_to_check1 + ".zip")
             if os.path.exists(path_to_check1) or os.path.exists(path_to_check2):
-                text = "Build artifact '" + os.path.basename(item["path"]) + "' already present in artifact directory."
+                text = f"Build artifact '{os.path.basename(item['path'])}' already present in artifact directory."
                 text += "\nPossible reason of this error: previous build results in working directory"
                 raise CriticalCiException(text)
 
             dir_list.add(item["path"])
         new_artifact_list = list(dir_list)
         new_artifact_list.sort(key=len, reverse=True)
         return new_artifact_list
 
     @make_block("Preprocessing artifact lists")
     def set_and_clean_artifacts(self, project_configs: Configuration, ignore_existing_artifacts: bool = False) -> None:
+        self.html_output.artifact_dir_ready = True
         artifact_list = []
         report_artifact_list = []
         for configuration in project_configs.all():
             if configuration.artifacts:
                 path = utils.parse_path(configuration.artifacts, self.settings.project_root)
                 artifact_list.append(dict(path=path, clean=configuration.artifact_prebuild_clean))
             if configuration.report_artifacts:
@@ -224,7 +233,8 @@
 
     def clean_artifacts_silently(self):
         try:
             shutil.rmtree(self.artifact_dir)
         except OSError:
             pass
         os.makedirs(self.artifact_dir)
+        self.html_output.artifact_dir_ready = True
```

### Comparing `Universum-0.19.8/universum/modules/automation_server/automation_server.py` & `Universum-0.19.9/universum/modules/automation_server/automation_server.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/modules/automation_server/base_server.py` & `Universum-0.19.9/universum/modules/automation_server/base_server.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/modules/automation_server/jenkins_server.py` & `Universum-0.19.9/universum/modules/automation_server/jenkins_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             
             Please specify the url by using '--jenkins-trigger-url' ('-jtu') command-line
             option or URL environment variable.
             """)
 
     def trigger_build(self, revision: str) -> None:
         processed_url = self.settings.trigger_url % revision
-        self.out.log("Triggering url %s" % processed_url)
+        self.out.log(f"Triggering url {processed_url}")
         utils.make_request(processed_url)
 
 
 class JenkinsServerForHostingBuild(BaseServerForHostingBuild, HasErrorState):
 
     @staticmethod
     def define_arguments(argument_parser: ModuleArgumentParser) -> None:
```

### Comparing `Universum-0.19.8/universum/modules/automation_server/teamcity_server.py` & `Universum-0.19.9/universum/modules/automation_server/teamcity_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,11 +93,10 @@
         return "Here is the link to TeamCity build: " + tc_build_link
 
     def artifact_path(self, local_artifacts_dir: str, item: str) -> str:
         return self.settings.server_url + "/repository/download/" + self.settings.configuration_id + "/" + \
                self.settings.build_id + ":id/" + item
 
     def add_build_tag(self, tag: str) -> Response:
-        return requests.post("%s/httpAuth/app/rest/builds/id:%s/tags" %
-                             (self.settings.server_url, self.settings.build_id),
+        return requests.post(f"{self.settings.server_url}/httpAuth/app/rest/builds/id:{self.settings.build_id}/tags",
                              auth=(self.settings.user_id, self.settings.passwd),
                              data=tag, headers={'Content-Type': 'text/plain'}, verify=False)
```

### Comparing `Universum-0.19.8/universum/modules/error_state.py` & `Universum-0.19.9/universum/modules/error_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def read_multiline_option(self, setting_name: str) -> str:
         value: str = getattr(self.settings, setting_name, None)
         if not value:
             return ""
         if value.startswith('@'):
             try:
-                with open(value.lstrip('@')) as value_file:
+                with open(value.lstrip('@'), encoding="utf-8") as value_file:
                     return value_file.read()
             except FileNotFoundError as e:
                 self.error(f"Error reading argument {setting_name} from file {e.filename}: no such file")
                 return ""
         return value
 
     def read_and_check_multiline_option(self, setting_name: str, error_message: str) -> str:
```

### Comparing `Universum-0.19.8/universum/modules/launcher.py` & `Universum-0.19.9/universum/modules/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,31 +163,33 @@
     # TODO: change to non-singleton module and get all dependencies by ourselves
     def __init__(self, item: configuration_support.Step,
                  out: Output,
                  fail_block: Callable[[str], None],
                  send_tag: Callable[[str], Response],
                  log_file: Optional[TextIO],
                  working_directory: str,
-                 additional_environment: Dict[str, str]) -> None:
+                 additional_environment: Dict[str, str],
+                 background: bool) -> None:
         super().__init__()
         self.configuration: configuration_support.Step = item
         self.out: Output = out
         self.fail_block: Callable[[str], None] = fail_block
         self.send_tag = send_tag
         self.file: Optional[TextIO] = log_file
         self.working_directory: str = working_directory
 
         self.environment: Dict[str, str] = os.environ.copy()
         self.environment.update(item.environment)
         self.environment.update(additional_environment)
 
         self.cmd: sh.Command
         self.process: sh.RunningCommand
-        self._is_background: bool = False
+        self._is_background = background
         self._postponed_out: List[Tuple[Callable[[str], None], str]] = []
+        self._needs_finalization: bool = True
 
     def prepare_command(self) -> bool:  # FIXME: refactor
         if not self.configuration.command:
             self.out.log("No 'command' found. Nothing to execute")
             return False
         command_name: str = utils.strip_path_start(self.configuration.command[0])
         try:
@@ -197,19 +199,19 @@
                 command_name = os.path.abspath(os.path.join(self.working_directory, command_name))
                 self.cmd = make_command(command_name)
         except CiException as ex:
             self.fail_block(str(ex))
             raise StepException() from ex
         return True
 
-    def start(self, is_background: bool) -> None:
+    def start(self) -> None:
         if not self.prepare_command():
+            self._needs_finalization = False
             return
 
-        self._is_background = is_background
         self._postponed_out = []
         self.process = self.cmd(*self.configuration.command[1:],
                                 _iter=True,
                                 _bg_exc=False,
                                 _cwd=self.working_directory,
                                 _env=self.environment,
                                 _bg=self._is_background,
@@ -217,15 +219,15 @@
                                 _err=self.handle_stderr)
 
         log_cmd = utils.trim_and_convert_to_unicode(self.process.ran)
         self.out.log_external_command(log_cmd)
         if self.file:
             self.file.write("$ " + log_cmd + "\n")
 
-    def handle_stdout(self, line: str = u"") -> None:
+    def handle_stdout(self, line: str = "") -> None:
         line = utils.trim_and_convert_to_unicode(line)
 
         if self.file:
             self.file.write(line + "\n")
         elif self._is_background:
             self._postponed_out.append((self.out.log_shell_output, line))
         else:
@@ -247,14 +249,19 @@
         request: Response = self.send_tag(tag)
         if request.status_code != 200:
             self.out.log_stderr(request.text)
         else:
             self.out.log("Tag '" + tag + "' added to build.")
 
     def finalize(self) -> None:
+        if not self._needs_finalization:
+            if self._is_background:
+                self._is_background = False
+                self.out.log("Nothing was executed: this background step had no command")
+            return
         try:
             text = ""
             try:
                 self.process.wait()
             except Exception as e:
                 if isinstance(e, sh.ErrorReturnCode):
                     text = f"Module sh got exit code {e.exit_code}\n"
@@ -347,15 +354,15 @@
         config_path = utils.parse_path(self.config_path, self.settings.project_root)
         configuration_support.set_project_root(self.settings.project_root)
         config_globals: Dict[str, configuration_support.Configuration] = {}
         sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
         sys.path.append(os.path.join(os.path.dirname(config_path)))
 
         try:
-            with open(config_path) as config_file:
+            with open(config_path, encoding="utf-8") as config_file:
                 exec(config_file.read(), config_globals)  # pylint: disable=exec-used
             self.source_project_configs = config_globals["configs"]
             dump_file: TextIO = self.artifacts.create_text_file("CONFIGS_DUMP.txt")
             dump_file.write(self.source_project_configs.dump())
             dump_file.close()
             config = self.source_project_configs.filter(check_if_env_set)
             self.project_config = config.filter(
@@ -395,15 +402,15 @@
         log_file: Optional[TextIO] = None
         if self.output == "file":
             log_file = self.artifacts.create_text_file(item.name + "_log.txt")
             self.out.log("Execution log is redirected to file")
 
         additional_environment = self.api_support.get_environment_settings()
         return RunningStep(item, self.out, fail_block, self.server.add_build_tag,
-                    log_file, working_directory, additional_environment)
+                    log_file, working_directory, additional_environment, item.background)
 
     def launch_custom_configs(self, custom_configs: configuration_support.Configuration) -> None:
         self.structure.execute_step_structure(custom_configs, self.create_process)
 
     @make_block("Executing build steps")
     def launch_project(self) -> None:
         self.reporter.add_block_to_report(self.structure.get_current_block())
```

### Comparing `Universum-0.19.8/universum/modules/output/teamcity_output.py` & `Universum-0.19.9/universum/modules/output/teamcity_output.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 
 def escape(message):
     return message.replace('\r', '').replace('|', '||').replace('\'', '|\'').replace('[', '|[').replace(']', '|]')
 
 
 class TeamcityOutput(BaseOutput):
     def open_block(self, num_str, name):
-        print(u"##teamcity[blockOpened name='{} {}']".format(num_str, escape(name)))
+        print(f"##teamcity[blockOpened name='{num_str} {escape(name)}']")
 
     def close_block(self, num_str, name, status):
-        print(u"##teamcity[blockClosed name='{} {}']".format(num_str, escape(name)))
+        print(f"##teamcity[blockClosed name='{num_str} {escape(name)}']")
 
     def report_error(self, description):
-        print(u"##teamcity[buildProblem description='<{}>']".format(escape(description)))
+        print(f"##teamcity[buildProblem description='<{escape(description)}>']")
 
     def report_skipped(self, message):
         lines = message.split("\n")
         for single_line in lines:
-            print(u"##teamcity[message text='{}' status='WARNING']".format(escape(single_line)))
+            print(f"##teamcity[message text='{escape(single_line)}' status='WARNING']")
 
     def change_status(self, message):
-        print(u"##teamcity[buildStatus text='{}']".format(escape(message)))
+        print(f"##teamcity[buildStatus text='{escape(message)}']")
 
     def log_exception(self, line):
         lines = line.split("\n")
         for single_line in lines:
-            print(u"##teamcity[message text='{}' status='ERROR']".format(escape(single_line)))
+            print(f"##teamcity[message text='{escape(single_line)}' status='ERROR']")
 
     def log_stderr(self, line):
         lines = line.split("\n")
         for single_line in lines:
-            print(u"##teamcity[message text='{}' status='WARNING']".format(escape(single_line)))
+            print(f"##teamcity[message text='{escape(single_line)}' status='WARNING']")
 
     def log(self, line):
-        print(u"==>", line)
+        print("==>", line)
 
     def log_external_command(self, command):
-        print(u"$", command)
+        print("$", command)
 
     def log_shell_output(self, line):
         print(line)
```

### Comparing `Universum-0.19.8/universum/modules/output/terminal_based_output.py` & `Universum-0.19.9/universum/modules/output/terminal_based_output.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/modules/project_directory.py` & `Universum-0.19.9/universum/modules/project_directory.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/modules/reporter.py` & `Universum-0.19.9/universum/modules/reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from collections import defaultdict
+from typing import Dict, List, Optional, TextIO, Tuple
+from typing_extensions import TypedDict
 
-from ..lib.gravity import Module, Dependency
+from ..lib.gravity import Dependency
 from ..lib.utils import make_block
 from . import automation_server
 from .output import HasOutput
 from .structure_handler import HasStructure
 
 __all__ = [
     "ReportObserver",
     "Reporter"
 ]
 
+ReportMessage = TypedDict('ReportMessage', {'message': str, 'line': int})
+
 
 class ReportObserver:
     """
     Abstract base class for reporting modules
     """
 
     def get_review_link(self):
@@ -22,15 +26,15 @@
 
     def report_start(self, report_text):
         raise NotImplementedError
 
     def report_result(self, result, report_text=None, no_vote=False):
         raise NotImplementedError
 
-    def code_report_to_review(self, report):
+    def code_report_to_review(self, report: Dict[str, List[ReportMessage]]) -> None:
         raise NotImplementedError
 
 
 class Reporter(HasOutput, HasStructure):
     automation_server_factory = Dependency(automation_server.AutomationServerForHostingBuild)
 
     @staticmethod
@@ -49,15 +53,15 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.observers = []
         self.report_initialized = False
         self.blocks_to_report = []
         self.artifacts_to_report = []
-        self.code_report_comments = defaultdict(list)
+        self.code_report_comments: Dict[str, List[ReportMessage]] = defaultdict(list)
 
         self.automation_server = self.automation_server_factory()
 
     def subscribe(self, observer):
         self.observers.append(observer)
 
     def report_review_link(self):
@@ -84,15 +88,15 @@
 
     def add_block_to_report(self, block):
         self.blocks_to_report.append(block)
 
     def report_artifacts(self, artifact_list):
         self.artifacts_to_report.extend(artifact_list)
 
-    def code_report(self, path, message):
+    def code_report(self, path: str, message: ReportMessage) -> None:
         self.code_report_comments[path].append(message)
 
     @make_block("Reporting build result", pass_errors=False)
     def report_build_result(self):
         if self.report_initialized is False:
             self.out.log("Not reporting: no build steps executed")
             return
```

### Comparing `Universum-0.19.8/universum/modules/structure_handler.py` & `Universum-0.19.9/universum/modules/structure_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,28 +37,28 @@
     '1.1. Run tests - Success'
     >>> b4.is_successful()
     True
     >>> b2 is b4.parent
     True
     """
 
-    def __init__(self, name: str, parent: Optional['Block'] = None) -> None:
+    def __init__(self, name: str, parent: Optional["Block"] = None) -> None:
         self.name: str = name
         self.status: str = "Success"
         self.children: List[Block] = []
 
         self.parent: Optional[Block] = parent
         self.number: str = ''
         if parent:
             parent.children.append(self)
-            self.number = '{}{}.'.format(parent.number, len(parent.children))
+            self.number = f"{parent.number}{len(parent.children)}."
 
     def __str__(self) -> str:
         result = self.number + ' ' + self.name
-        return '{} - {}'.format(result, self.status) if not self.children else result
+        return f"{result} - {self.status}" if not self.children else result
 
     def is_successful(self) -> bool:
         return self.status == "Success"
 
 
 class BackgroundStepInfo(TypedDict):
     name: str
@@ -133,21 +133,20 @@
         return result
 
     def execute_one_step(self, configuration: Step,
                          step_executor: Callable, is_critical: bool) -> None:
         # step_executor is [[Step], Step], but referring to Step creates circular dependency
         process = step_executor(configuration)
 
-        background = configuration.background
-        process.start(is_background=background)
-        if not background:
+        process.start()
+        if not configuration.background:
             process.finalize()
             return
 
-        self.out.log("Will continue in background")
+        self.out.log("This step is marked to be executed in background")
         self.active_background_steps.append({'name': configuration.name,
                                              'finalizer': process.finalize,
                                              'is_critical': is_critical})
 
     def finalize_background_step(self, background_step: BackgroundStepInfo):
         try:
             background_step['finalizer']()
@@ -173,25 +172,21 @@
             try:
                 item: Step = parent + copy.deepcopy(obj_a)
 
                 if obj_a.children:
                     # Here pass_errors=True, because any exception outside executing build step
                     # is not step-related and should stop script executing
 
-                    numbering = " [ {:{length}}+{:{length}} ] ".format("", "", length=step_num_len)
+                    numbering = f" [ {'':{step_num_len}}+{'':{step_num_len}} ] "
                     step_name = numbering + item.name
                     self.run_in_block(self.execute_steps_recursively, step_name, True,
                                       item, obj_a.children, step_executor, skipped)
                 else:
                     self.configs_current_number += 1
-                    numbering = " [ {:>{}}/{} ] ".format(
-                        self.configs_current_number,
-                        step_num_len,
-                        self.configs_total_count
-                    )
+                    numbering = f" [ {self.configs_current_number:>{step_num_len}}/{self.configs_total_count} ] "
                     step_name = numbering + item.name
                     if skipped:
                         self.report_skipped_block(step_name)
                         continue
 
                     if item.finish_background and self.active_background_steps:
                         self.out.log("All ongoing background steps should be finished before next step execution")
```

### Comparing `Universum-0.19.8/universum/modules/vcs/base_vcs.py` & `Universum-0.19.9/universum/modules/vcs/base_vcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class BaseVcs(ProjectDirectory):
     """
     Base class for VCS drivers
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.repo_status = u""
+        self.repo_status = ""
         self.sources_need_cleaning = False
 
     def append_repo_status(self, line):
         self.repo_status += line
 
     def get_repo_status(self):
         return self.repo_status
```

### Comparing `Universum-0.19.8/universum/modules/vcs/gerrit_vcs.py` & `Universum-0.19.9/universum/modules/vcs/gerrit_vcs.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/modules/vcs/git_vcs.py` & `Universum-0.19.9/universum/modules/vcs/git_vcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,30 +241,30 @@
                 full_path = utils.parse_path(record_parameters[-1], self.settings.project_root)
                 modified_files.add(full_path)
 
         for file_path in file_list:
             all_matches = glob.glob(file_path)
             relative_path = os.path.relpath(file_path, self.settings.project_root)
             if not all_matches:
-                self.out.log("Skipping '{}'...".format(relative_path))
+                self.out.log(f"Skipping '{relative_path}'...")
                 continue
 
             for matching_path in all_matches:
                 relative_path = os.path.relpath(matching_path, self.settings.project_root)
                 if os.path.isdir(matching_path):
                     files_in_dir = [os.path.relpath(item, self.settings.project_root)
                                     for item in modified_files if item.startswith(file_path)]
                     if not files_in_dir:
-                        self.out.log("Skipping '{}'...".format(relative_path))
+                        self.out.log(f"Skipping '{relative_path}'...")
                     result.extend(files_in_dir)
                 else:
                     if matching_path in modified_files:
                         result.append(relative_path)
                     else:
-                        self.out.log("Skipping '{}'...".format(relative_path))
+                        self.out.log(f"Skipping '{relative_path}'...")
         return result
 
     def git_commit_locally(self, description, file_list, edit_only=False):
         try:
             self.repo = git.Repo(convert_to_str(self.settings.project_root))
         except git.exc.NoSuchPathError as e:
             raise CriticalCiException("No such directory as '" + self.settings.project_root + "'") from e
```

### Comparing `Universum-0.19.8/universum/modules/vcs/github_vcs.py` & `Universum-0.19.9/universum/modules/vcs/github_vcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         parser.add_argument("--github-app-id", "-gta", dest="integration_id", metavar="GITHUB_APP_ID",
                             help="GitHub application ID to use for check run report. Only GitHub App "
                                  "can report a check run result! If you don't have an App for reporting purposes, "
                                  "please don't use ``--report-to-review`` with GitHub")
         parser.add_argument("--github-private-key", "-gtk", dest="key", metavar="GITHUB_PRIVATE_KEY",
                             help="GitHub App private key for obtaining installation authentication token. "
                                  "Pass raw key data via environment variable or pass a file path to read the key from "
-                                 "by starting the value string with '@'. File path can be either absolute or relative")
+                                 "by starting the value string with '@'. File path can be either absolute or relative. "
+                                 "Please note, that when passing a file, it is expected to be in UTF-8 encoding")
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.check_required_option("integration_id", """
             The GitHub App ID is not specified.
 
             Only GitHub Application owner knows this ID. If you are the App owner, please
@@ -61,14 +62,15 @@
             one GitHub App. Because of that, it is required to specify private key within
             the CI configuration.
 
             As the private key is a multiline string, it is not convenient to pass it
             directly via command line. If you start the parameter with '@', the rest should be
             the path to a file containing the key. The path can be absolute or relative to the 
             project root. You can also store the key in GITHUB_PRIVATE_KEY environment variable.
+            Please note, that when passing a file, it's expected to be in UTF-8 encoding")
             """)
 
         global github
         try:
             github = importlib.import_module("github")
         except ImportError as e:
             text = "Error: using GitHub Handler or VCS type 'github' requires Python package 'pygithub' " \
@@ -167,25 +169,25 @@
             '--github-check-id' ('-ghi') command line parameter or by setting
             GITHUB_CHECK_ID environment variable.
 
             If using 'universum github-handler', the check ID is automatically extracted
             from the webhook payload and passed via GITHUB_CHECK_ID environment variable.
             """)
 
-        self.request = dict()
+        self.request = {}
         self.request["status"] = "in_progress"
         self.request["output"] = {
             "title": self.settings.check_name,
             "summary": ""
         }
 
     def _clone(self, history_depth, destination_directory, clone_url):
         parsed_repo = urllib.parse.urlsplit(clone_url)
         if parsed_repo.scheme == "https" and not parsed_repo.username:
-            new_netloc = "x-access-token:{}@{}".format(self.get_token(), parsed_repo.netloc)
+            new_netloc = f"x-access-token:{self.get_token()}@{parsed_repo.netloc}"
             parsed_repo = (parsed_repo.scheme, new_netloc, parsed_repo.path, parsed_repo.query, parsed_repo.fragment)
         clone_url = urllib.parse.urlunsplit(parsed_repo)
         super()._clone(history_depth, destination_directory, clone_url)
 
     def code_review(self):
         self.reporter = self.reporter_factory()
         self.reporter.subscribe(self)
```

### Comparing `Universum-0.19.8/universum/modules/vcs/local_vcs.py` & `Universum-0.19.9/universum/modules/vcs/local_vcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,11 +48,11 @@
             self.out.log("Moving sources to '" + self.settings.project_root + "'...")
             shutil.copytree(self.source_dir, self.settings.project_root)
             self.append_repo_status("Got sources from: " + self.source_dir + "\n")
         except OSError as e:
             text = f"{e}\nPossible reasons of this error:"
             text += f"\n * Sources path, passed to the script ('{self.settings.source_dir}')," + \
                     " does not lead to actual sources or was processed incorrectly"
-            text += "\n * Directory '{}' already exists in working dir (e.g. due to previous builds)".format(
-                os.path.basename(self.settings.project_root))
+            text += f"\n * Directory '{os.path.basename(self.settings.project_root)}'" + \
+                    " already exists in working dir (e.g. due to previous builds)"
             text += "\n * File reading permissions troubles"
             raise CriticalCiException(text) from e
```

### Comparing `Universum-0.19.8/universum/modules/vcs/perforce_vcs.py` & `Universum-0.19.9/universum/modules/vcs/perforce_vcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,21 +159,23 @@
                 raise P4Exception from e
             return []
 
     def reconcile_one_path(self, file_path, workspace_root, change_id, edit_only):
         # TODO: cover 'not file_path.startswith("/")' case with tests
         if not file_path.startswith("/"):
             file_path = workspace_root + "/" + file_path
+        if not file_path.endswith("/") and os.path.isdir(file_path):
+            file_path += "/"
         if file_path.endswith("/"):
             file_path += "..."
         if edit_only:
             reconcile_result = self.p4reconcile("-c", change_id, "-e", convert_to_str(file_path))
             if not reconcile_result:
                 self.out.log(
-                    "The file was not edited. Skipping '{}'...".format(os.path.relpath(file_path, workspace_root)))
+                    f"The file was not edited. Skipping '{os.path.relpath(file_path, workspace_root)}'...")
         else:
             reconcile_result = self.p4reconcile("-c", change_id, convert_to_str(file_path))
 
         for line in reconcile_result:
             # p4reconcile returns list of dicts AND strings if file is opened in another workspace
             # so we catch TypeError if line is not dict
             try:
@@ -195,29 +197,36 @@
         client = self.p4.fetch_client(self.settings.client)
         workspace_root = client['Root']
 
         change = self.p4.fetch_change()
         change["Files"] = []
         change["Description"] = description
         change_id = self.p4.save_change(change)[0].split()[1]
+        self.out.log(f"Created empty CL {change_id} for reconciling")
 
         try:
             for file_path in file_list:
                 self.reconcile_one_path(file_path, workspace_root, change_id, edit_only)
 
             current_cl = self.p4.fetch_change(change_id)
             # If no changes were reconciled, there will be no file records in CL dictionary
             if "Files" not in current_cl:
                 self.p4.run_change("-d", change_id)
+                self.out.log(f"Deleted empty CL {change_id}")
                 return 0
 
+            text = "The changes in following files are going to be submitted:"
+            for line in current_cl["Files"]:
+                text+= "\n\t" + line
+            self.out.log(text)
             self.p4.run_submit(current_cl, "-f", "revertunchanged")
         except Exception as e:
             self.p4.run_revert("-k", "-c", change_id, "//...")
             self.p4.run_change("-d", change_id)
+            self.out.log(f"Reverted and deleted CL {change_id}")
             raise CriticalCiException(str(e)) from e
 
         return change_id
 
 
 class PerforceWithMappings(PerforceVcs):
 
@@ -417,15 +426,15 @@
                     text = "Error getting latest CL number for '" + depot["path"] + "'"
                     text += "\nPlease check depot path formatting (e.g. '/...' in the end for directories)"
                     raise CriticalCiException(text) from e
                 self.out.log("Latest CL: " + depot["cl"])
 
             line = depot["path"] + '@' + depot["cl"]
             # Set environment variable for each mapping in order of there definition
-            os.environ["SYNC_CL_{}".format(idx)] = depot["cl"]
+            os.environ[f"SYNC_CL_{idx}"] = depot["cl"]
 
             self.out.log("Downloading " + line)
             try:
                 result = self.p4.run_sync("-f", line)
             except P4Exception as e:
                 if "not in client view" not in str(e):
                     raise CriticalCiException(str(e)) from e
@@ -469,18 +478,18 @@
             p4cmd = sh.Command("p4")
             diff_result = p4cmd("-c", self.settings.client, "-u", self.settings.user,
                                 "-P", self.settings.password, "-p", self.settings.port,
                                 "diff", depot)
             result: str = utils.trim_and_convert_to_unicode(diff_result.stdout)
         except sh.ErrorReturnCode as e:
             for line in e.stderr.splitlines():
-                if not (line.startswith("Librarian checkout")
-                        or line.startswith("Error opening librarian file")
-                        or line.startswith("Transfer of librarian file")
-                        or line.endswith(".gz: No such file or directory")):
+                if not (line.startswith(b"Librarian checkout")
+                        or line.startswith(b"Error opening librarian file")
+                        or line.startswith(b"Transfer of librarian file")
+                        or line.endswith(b".gz: No such file or directory")):
                     raise CriticalCiException(utils.trim_and_convert_to_unicode(e.stderr)) from e
             result = utils.trim_and_convert_to_unicode(e.stdout)
         return result
 
     def calculate_file_diff(self) -> Optional[List[Dict[str, str]]]:
         action_list: Dict[str, str] = {}
         for timeout in [0, 5, 10, 20, 40, 80]:
@@ -612,15 +621,15 @@
                         self.out.log(f"CL {item['change']} is empty")
                     else:
                         raise
                 self.p4.run_change("-d", item["change"])
             self.p4.delete_client(self.client_name)
             self.out.log(f"Client '{self.client_name}' deleted")
         except P4Exception as e:
-            if "Client '{}' unknown".format(self.client_name) in e.value:
+            if f"Client '{self.client_name}' unknown" in e.value:
                 self.out.log("No client to delete")
             else:
                 self.structure.fail_current_block(e.value)
 
     def finalize(self):
         with Uninterruptible(self.out.log_exception) as run:
             if self.settings.force_clean:
```

### Comparing `Universum-0.19.8/universum/modules/vcs/swarm.py` & `Universum-0.19.9/universum/modules/vcs/swarm.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,16 +150,16 @@
 
     def is_latest_version(self):
         self.update_review_version()
 
         if self.review_latest_version == self.review_version:
             return True
 
-        text = "Current review version is {0}, while latest review version is already {1}".format(
-            self.review_version, self.review_latest_version)
+        text = f"Current review version is {self.review_version}, " + \
+               f"while latest review version is already {self.review_latest_version}"
         self.out.log(text)
         return False
 
     def post_comment(self, text, filename=None, line=None, version=None, no_notification=False):
         request = {"body": text,
                    "topic": "reviews/" + str(self.settings.review_id)}
         if filename:
@@ -213,20 +213,20 @@
 
         if self.is_latest_version():
             if link is not None:
                 self.out.log("Build status on Swarm will be updated via URL " + link)
                 utils.make_request(link, critical=False)
             else:
                 self.out.log("Build status on Swarm will not be updated because " +
-                             "the '{0}' link has not been provided.".format("PASS" if result else "FAIL"))
+                             f"the '{'PASS' if result else 'FAIL'}' link has not been provided.")
         else:
             text = "Build status on Swarm will not be updated because tested review revision is not latest."
             if not link:
-                text += " Also, even if the review revision was latest, we wouldn't be able to report the status " \
-                        "because the '{0}' link has not been provided.".format("PASS" if result else "FAIL")
+                text += " Also, even if the review revision was latest, we wouldn't be able to report the status " + \
+                        f"because the '{'PASS' if result else 'FAIL'}' link has not been provided."
             self.out.log(text)
 
         # Voting up or down; posting comments if any
         # An addition to "Automated Tests" functionality, requires login to Swarm
         self.update_review_version()
         if not no_vote:
             self.vote_review(result, version=self.review_version)
```

### Comparing `Universum-0.19.8/universum/modules/vcs/vcs.py` & `Universum-0.19.9/universum/modules/vcs/vcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,37 +70,36 @@
                                      "Git ('git'), Gerrit ('gerrit'), GitHub ('github') or a local directory ('none'). "
                                      "Gerrit uses Git parameters. Each VCS type has its own settings.")
 
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
             if not getattr(self.settings, "type", None):
-                self.error("""
+                self.error(f"""
                     The repository (VCS) type is not set.
                      
                     The repository type defines the version control system that is used for
                     performing the requested action. For example, Universum needs to get project
                     source codes for performing Continuous Integration (CI) builds.
 
-                    The following types are supported: {}.
+                    The following types are supported: {', '.join(vcs_types)}.
                     
                     Each of these types requires supplying its own
                     configuration parameters. At the minimum, the following
                     parameters are required:
                       * "git", "github" and "gerrit" - GIT_REPO (-gr) and GIT_REFSPEC (-grs)
                       * "perforce"                   - P4PORT (-p4p), P4USER (-p4u), P4PASSWD (-p4P)
                       * "none"                       - SOURCE_DIR (-fsd)
                       
                     Depending on the requested action, additional type-specific parameters are
                     required. For example, P4CLIENT (-p4c) is required for CI builds with perforce.
                     
                     Please specify the VCS type by using '--vcs-type' ('-vt') command-line option or
                     VCS_TYPE environment variable.
-                    """.
-                           format(", ".join(vcs_types)))
+                    """)
                 return
 
             if self.settings.type == "none":
                 driver_factory = self.local_driver_factory
             elif self.settings.type == "git":
                 driver_factory = self.git_driver_factory
             elif self.settings.type == "gerrit":
```

### Comparing `Universum-0.19.8/universum/nonci.py` & `Universum-0.19.9/universum/nonci.py`

 * *Files identical despite different names*

### Comparing `Universum-0.19.8/universum/poll.py` & `Universum-0.19.9/universum/poll.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,42 +34,42 @@
         if len(self.latest_cls[depot]) == 1:
             self.stored_cls[depot] = self.latest_cls[depot].pop()
             self.out.log("No changes detected")
             return
 
         for change in self.latest_cls[depot]:
             if change == self.stored_cls[depot]:
-                self.out.log("Commit {} is latest known".format(change))
+                self.out.log(f"Commit {change} is latest known")
                 continue
 
             if change in self.triggered_cls:
-                self.out.log("Commit {} already processed".format(change))
+                self.out.log(f"Commit {change} already processed")
                 continue
 
-            self.out.log("Detected commit {}, triggering build".format(change))
+            self.out.log(f"Detected commit {change}, triggering build")
             self.server.trigger_build(change)
             self.triggered_cls.add(change)
             self.stored_cls[depot] = change
 
     @make_block("Enumerating changes")
     def execute(self):
         try:
-            with open(self.settings.db_file) as db_file:
+            with open(self.settings.db_file, encoding="utf-8") as db_file:
                 self.stored_cls = json.load(db_file)
         except IOError as io_error:
             if io_error.errno == 2:
                 pass
             else:
                 raise
 
         try:
             self.latest_cls = self.vcs.driver.get_changes(self.stored_cls, self.settings.max_number)
             for depot in self.latest_cls.keys():
                 self.structure.run_in_block(self.process_single_mapping, "Processing depot " + depot, True, depot)
         except NotImplementedError:
             self.out.log("Polling is skipped because current VCS doesn't support it")
         finally:
-            with open(self.settings.db_file, "w") as db_file:
+            with open(self.settings.db_file, "w", encoding="utf-8") as db_file:
                 json.dump(self.stored_cls, db_file, indent=4, sort_keys=True)
 
     def finalize(self):
         self.vcs.finalize()
```

### Comparing `Universum-0.19.8/universum/submit.py` & `Universum-0.19.9/universum/submit.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,30 +20,34 @@
                                  "instead of actual submitting to repo")
         parser.add_argument("--edit-only", action="store_true", dest="edit_only",
                             help="Only submit existing vcs modifications, no adding or deleting")
 
         parser.add_argument('--commit-message', '-cm', dest='commit_message', metavar="COMMIT_MESSAGE",
                             help="Commit message. Enter in command line directly, store in environment variable "
                                  "or pass a file path to read the message from by starting the value string with "
-                                 "'@'. File path can be either absolute or relative")
+                                 "'@'. File path can be either absolute or relative. "
+                                 "Please note, that when passing a file, it is expected to be in UTF-8 encoding")
         parser.add_argument("--reconcile-list", "-rl", dest="reconcile_list", metavar="RECONCILE_LIST",
                             help="Comma-separated or linebreak-separated list of files or directories "
                                  "to be reconciled for commit (relative paths starting at client root "
                                  "are supported). To use command line directly, add quotes if needed "
                                  "(e.g. ``-rl 'target1, target2'``). To use a file with reconcile list, "
-                                 "start a path to file with '@' (e.g. ``-rl @/path/to/file``)")
+                                 "start a path to file with '@' (e.g. ``-rl @/path/to/file``)."
+                                 "Please note, that when passing a file, it's expected to be in UTF-8 "
+                                 "encoding")
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.commit_message = self.read_and_check_multiline_option("commit_message", """
             Commit message is not specified.
 
             Please use '--commit-message' option to provide it. If you start the parameter with '@', the
             rest should be the path to a file containing the commit message text. The path can be absolute
             or relative to the project root. You can also store the message in COMMIT_MESSAGE environment variable.
+            Please note, that when passing a file, it's expected to be in UTF-8 encoding
             """)
 
         try:
             self.reconcile_list = utils.unify_argument_list(self.read_multiline_option("reconcile_list").splitlines())
         except AttributeError:
             self.reconcile_list = []
```

