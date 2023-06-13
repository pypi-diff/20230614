# Comparing `tmp/navi pro-7.1.8.tar.gz` & `tmp/navi pro-7.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/navi pro-7.1.8.tar", last modified: Mon Oct 17 17:51:14 2022, max compression
+gzip compressed data, was "dist/navi pro-7.1.9.tar", last modified: Mon Oct 17 18:16:44 2022, max compression
```

## Comparing `navi pro-7.1.8.tar` & `navi pro-7.1.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 17:51:14.000000 navi pro-7.1.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 17:51:14.000000 navi pro-7.1.8/navi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 17:51:14.000000 navi pro-7.1.8/navi/plugins/
--rw-r--r--   0 root         (0) root         (0)     1415 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5783 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/access.py
--rw-r--r--   0 root         (0) root         (0)     2035 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/add.py
--rw-r--r--   0 root         (0) root         (0)     1250 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/add_by_file.py
--rw-r--r--   0 root         (0) root         (0)     1760 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/agent_export.py
--rw-r--r--   0 root         (0) root         (0)     2278 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/agent_group_export.py
--rw-r--r--   0 root         (0) root         (0)     7500 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/agents.py
--rw-r--r--   0 root         (0) root         (0)      701 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/api.py
--rw-r--r--   0 root         (0) root         (0)     5881 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/api_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     1410 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/attribute.py
--rw-r--r--   0 root         (0) root         (0)      700 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/cancel.py
--rw-r--r--   0 root         (0) root         (0)     2364 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/compliance_export_csv.py
--rw-r--r--   0 root         (0) root         (0)     2176 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/cve_compare.py
--rw-r--r--   0 root         (0) root         (0)     6899 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/database.py
--rw-r--r--   0 root         (0) root         (0)     7015 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/dbconfig.py
--rw-r--r--   0 root         (0) root         (0)     2879 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/delete.py
--rw-r--r--   0 root         (0) root         (0)      535 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/deploy.py
--rw-r--r--   0 root         (0) root         (0)    29240 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/display.py
--rw-r--r--   0 root         (0) root         (0)      175 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/error_msg.py
--rw-r--r--   0 root         (0) root         (0)     6293 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/export.py
--rw-r--r--   0 root         (0) root         (0)    13223 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/find.py
--rw-r--r--   0 root         (0) root         (0)     8385 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/fixed_export.py
--rw-r--r--   0 root         (0) root         (0)    23454 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/ip.py
--rw-r--r--   0 root         (0) root         (0)     1382 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/keys.py
--rw-r--r--   0 root         (0) root         (0)      268 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/licensed_count.py
--rw-r--r--   0 root         (0) root         (0)     2568 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/lumin.py
--rw-r--r--   0 root         (0) root         (0)     2584 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/migrate.py
--rw-r--r--   0 root         (0) root         (0)     5481 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/network.py
--rw-r--r--   0 root         (0) root         (0)     1131 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/query_export.py
--rw-r--r--   0 root         (0) root         (0)     1615 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/rules.py
--rw-r--r--   0 root         (0) root         (0)    20757 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/scan.py
--rw-r--r--   0 root         (0) root         (0)    11770 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/scan_efficentcy.py
--rw-r--r--   0 root         (0) root         (0)    15489 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/scan_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/sla.py
--rw-r--r--   0 root         (0) root         (0)    24879 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/tag.py
--rw-r--r--   0 root         (0) root         (0)     2615 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/tag_helper.py
--rw-r--r--   0 root         (0) root         (0)     6826 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/target_group.py
--rw-r--r--   0 root         (0) root         (0)     9131 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/th_asset_export.py
--rw-r--r--   0 root         (0) root         (0)     8152 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/th_compliance_export.py
--rw-r--r--   0 root         (0) root         (0)    13373 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/th_vuln_export.py
--rw-r--r--   0 root         (0) root         (0)     4565 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/update.py
--rw-r--r--   0 root         (0) root         (0)     4088 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/user.py
--rw-r--r--   0 root         (0) root         (0)     1165 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/user_export.py
--rw-r--r--   0 root         (0) root         (0)     2247 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/plugins/usergroup.py
--rw-r--r--   0 root         (0) root         (0)       27 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      219 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 17:51:14.000000 navi pro-7.1.8/navi_pro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3531 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi_pro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1377 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi_pro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi_pro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi_pro.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      136 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi_pro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-10-17 17:51:13.000000 navi pro-7.1.8/navi_pro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2529 2022-10-17 17:51:12.000000 navi pro-7.1.8/README.md
--rwxr-xr-x   0 root         (0) root         (0)     1329 2022-10-17 17:51:13.000000 navi pro-7.1.8/setup.py
--rw-r--r--   0 root         (0) root         (0)     3531 2022-10-17 17:51:14.000000 navi pro-7.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-17 17:51:14.000000 navi pro-7.1.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 18:16:44.000000 navi pro-7.1.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/
+-rw-r--r--   0 root         (0) root         (0)     1415 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/access.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/add.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/add_by_file.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/agent_export.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/agent_group_export.py
+-rw-r--r--   0 root         (0) root         (0)     7500 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/agents.py
+-rw-r--r--   0 root         (0) root         (0)      701 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/api.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/api_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/attribute.py
+-rw-r--r--   0 root         (0) root         (0)      700 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/cancel.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/compliance_export_csv.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/cve_compare.py
+-rw-r--r--   0 root         (0) root         (0)     6899 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/database.py
+-rw-r--r--   0 root         (0) root         (0)     7015 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/dbconfig.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/delete.py
+-rw-r--r--   0 root         (0) root         (0)      535 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    29240 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/display.py
+-rw-r--r--   0 root         (0) root         (0)      175 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/error_msg.py
+-rw-r--r--   0 root         (0) root         (0)     6293 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/export.py
+-rw-r--r--   0 root         (0) root         (0)    13223 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/find.py
+-rw-r--r--   0 root         (0) root         (0)     8385 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/fixed_export.py
+-rw-r--r--   0 root         (0) root         (0)    23454 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/ip.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/keys.py
+-rw-r--r--   0 root         (0) root         (0)      268 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/licensed_count.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/lumin.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/migrate.py
+-rw-r--r--   0 root         (0) root         (0)     5481 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/network.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/query_export.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/rules.py
+-rw-r--r--   0 root         (0) root         (0)    20757 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/scan.py
+-rw-r--r--   0 root         (0) root         (0)    11774 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/scan_efficentcy.py
+-rw-r--r--   0 root         (0) root         (0)    15489 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/scan_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/sla.py
+-rw-r--r--   0 root         (0) root         (0)    24879 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/tag.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/tag_helper.py
+-rw-r--r--   0 root         (0) root         (0)     6826 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/target_group.py
+-rw-r--r--   0 root         (0) root         (0)     9131 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/th_asset_export.py
+-rw-r--r--   0 root         (0) root         (0)     8152 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/th_compliance_export.py
+-rw-r--r--   0 root         (0) root         (0)    13373 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/th_vuln_export.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/update.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/user.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/user_export.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/plugins/usergroup.py
+-rw-r--r--   0 root         (0) root         (0)       27 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      219 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi_pro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3531 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi_pro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1377 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi_pro.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi_pro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2022-10-17 18:16:44.000000 navi pro-7.1.9/navi_pro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2529 2022-10-17 18:16:43.000000 navi pro-7.1.9/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     1329 2022-10-17 18:16:44.000000 navi pro-7.1.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2022-10-17 18:16:44.000000 navi pro-7.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-17 18:16:44.000000 navi pro-7.1.9/setup.cfg
```

### Comparing `navi pro-7.1.8/navi/plugins/__init__.py` & `navi pro-7.1.9/navi/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/access.py` & `navi pro-7.1.9/navi/plugins/access.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/add.py` & `navi pro-7.1.9/navi/plugins/add.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/add_by_file.py` & `navi pro-7.1.9/navi/plugins/add_by_file.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/agent_export.py` & `navi pro-7.1.9/navi/plugins/agent_export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/agent_group_export.py` & `navi pro-7.1.9/navi/plugins/agent_group_export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/agents.py` & `navi pro-7.1.9/navi/plugins/agents.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/api.py` & `navi pro-7.1.9/navi/plugins/api.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/api_wrapper.py` & `navi pro-7.1.9/navi/plugins/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/attribute.py` & `navi pro-7.1.9/navi/plugins/attribute.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/cancel.py` & `navi pro-7.1.9/navi/plugins/cancel.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/compliance_export_csv.py` & `navi pro-7.1.9/navi/plugins/compliance_export_csv.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/cve_compare.py` & `navi pro-7.1.9/navi/plugins/cve_compare.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/database.py` & `navi pro-7.1.9/navi/plugins/database.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/dbconfig.py` & `navi pro-7.1.9/navi/plugins/dbconfig.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/delete.py` & `navi pro-7.1.9/navi/plugins/delete.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/deploy.py` & `navi pro-7.1.9/navi/plugins/deploy.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/display.py` & `navi pro-7.1.9/navi/plugins/display.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/export.py` & `navi pro-7.1.9/navi/plugins/export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/find.py` & `navi pro-7.1.9/navi/plugins/find.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/fixed_export.py` & `navi pro-7.1.9/navi/plugins/fixed_export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/ip.py` & `navi pro-7.1.9/navi/plugins/ip.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/keys.py` & `navi pro-7.1.9/navi/plugins/keys.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/lumin.py` & `navi pro-7.1.9/navi/plugins/lumin.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/migrate.py` & `navi pro-7.1.9/navi/plugins/migrate.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/network.py` & `navi pro-7.1.9/navi/plugins/network.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/query_export.py` & `navi pro-7.1.9/navi/plugins/query_export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/rules.py` & `navi pro-7.1.9/navi/plugins/rules.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/scan.py` & `navi pro-7.1.9/navi/plugins/scan.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/scan_efficentcy.py` & `navi pro-7.1.9/navi/plugins/scan_efficentcy.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         header = ["Scan URl", "Scan Start", "Last Asset Scanned", "Scan Policy", "Scanner IP", "Scan Name",
                   "Total Assets",
                   "Average Scan Duration", "Reported Time", "Indexing Time", "Scan Duration", "Shortest Asset time",
                   "Shortest Scanned Asset", "Longest Asset time", "longest Scanned Asset"]
         trend_writer.writerow(header)
 
         for hist in tio.scans.history(scanid):  # scan_hist['history']:
-            if hist['is_archived']:
+            if not hist['is_archived']:
                 if hist['status'] == 'completed':
                     # Lets get the Reported Scan Duration
                     reported_scan_start = hist['time_start']
                     reported_scan_end = hist['time_end']
                     total_reported_scan_duration = reported_scan_end - reported_scan_start
 
                     # Simple Delta from Tenable.io reported Scan times
```

### Comparing `navi pro-7.1.8/navi/plugins/scan_evaluation.py` & `navi pro-7.1.9/navi/plugins/scan_evaluation.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/sla.py` & `navi pro-7.1.9/navi/plugins/sla.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/tag.py` & `navi pro-7.1.9/navi/plugins/tag.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/tag_helper.py` & `navi pro-7.1.9/navi/plugins/tag_helper.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/target_group.py` & `navi pro-7.1.9/navi/plugins/target_group.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/th_asset_export.py` & `navi pro-7.1.9/navi/plugins/th_asset_export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/th_compliance_export.py` & `navi pro-7.1.9/navi/plugins/th_compliance_export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/th_vuln_export.py` & `navi pro-7.1.9/navi/plugins/th_vuln_export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/update.py` & `navi pro-7.1.9/navi/plugins/update.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/user.py` & `navi pro-7.1.9/navi/plugins/user.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/user_export.py` & `navi pro-7.1.9/navi/plugins/user_export.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi/plugins/usergroup.py` & `navi pro-7.1.9/navi/plugins/usergroup.py`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/navi_pro.egg-info/PKG-INFO` & `navi pro-7.1.9/navi_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navi-pro
-Version: 7.1.8
+Version: 7.1.9
 Summary: A command-line interface to Tenable.io
 Home-page: https://github.com/packetchaos/Navi
 Author: Casey Reid
 Author-email: itprofguru@gmail.com
 License: GNUv3
 Description: # Navi - The Tenable.io Swiss Army Knife
         A command-line tool which leverages the Tenable.io API to automate common tasks
```

### Comparing `navi pro-7.1.8/navi_pro.egg-info/SOURCES.txt` & `navi pro-7.1.9/navi_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/README.md` & `navi pro-7.1.9/README.md`

 * *Files identical despite different names*

### Comparing `navi pro-7.1.8/setup.py` & `navi pro-7.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='navi pro',
-    version='7.1.8',
+    version='7.1.9',
     description="A command-line interface to Tenable.io",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Casey Reid",
     author_email="itprofguru@gmail.com",
     url="https://github.com/packetchaos/Navi",
     license="GNUv3",
```

### Comparing `navi pro-7.1.8/PKG-INFO` & `navi pro-7.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navi pro
-Version: 7.1.8
+Version: 7.1.9
 Summary: A command-line interface to Tenable.io
 Home-page: https://github.com/packetchaos/Navi
 Author: Casey Reid
 Author-email: itprofguru@gmail.com
 License: GNUv3
 Description: # Navi - The Tenable.io Swiss Army Knife
         A command-line tool which leverages the Tenable.io API to automate common tasks
```

