# Comparing `tmp/tap-zendesk-2.0.1.tar.gz` & `tmp/tap-zendesk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-zendesk-2.0.1.tar", last modified: Mon Jun  5 09:01:55 2023, max compression
+gzip compressed data, was "dist/tap-zendesk-2.1.0.tar", last modified: Wed Jun 14 10:17:40 2023, max compression
```

## Comparing `tap-zendesk-2.0.1.tar` & `tap-zendesk-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/MANIFEST.in
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8122 2023-06-05 09:01:37.000000 tap-zendesk-2.0.1/tap_zendesk/http.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4101 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/metrics.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4434 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_metrics.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6744 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/tickets.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/group_memberships.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/sla_policies.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1058 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      607 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/groups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/tags.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/shared/attachments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/shared/metadata.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2340 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/shared/via.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18549 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_audits.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1744 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/macros.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1583 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_forms.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6263 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      842 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/satisfaction_ratings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3004 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_fields.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1619 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/schemas/organizations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24869 2023-05-31 06:52:44.000000 tap-zendesk-2.0.1/tap_zendesk/streams.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8280 2023-06-05 09:01:37.000000 tap-zendesk-2.0.1/tap_zendesk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2473 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/tap_zendesk/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1307 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/tap_zendesk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8646 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_all_streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3865 2023-05-31 06:52:44.000000 tap-zendesk-2.0.1/test/test_all_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_minimal_selection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2102 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_custom_fields_discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6986 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10384 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_standard_bookmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3283 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10085 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_start_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6792 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/test/test_bookmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-06-05 09:01:55.000000 tap-zendesk-2.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-06-05 09:01:37.000000 tap-zendesk-2.0.1/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1553 2023-05-30 04:15:54.000000 tap-zendesk-2.0.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-14 10:17:40.000000 tap-zendesk-2.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       93 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-14 10:17:40.000000 tap-zendesk-2.1.0/tap_zendesk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8122 2023-06-13 03:09:32.000000 tap-zendesk-2.1.0/tap_zendesk/http.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4101 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/metrics.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-14 10:17:40.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4434 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_metrics.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6744 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/tickets.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/group_memberships.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2375 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/sla_policies.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1058 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      607 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/tags.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1821 2023-06-14 10:17:08.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_metric_events.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-14 10:17:40.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/shared/attachments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2493 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/shared/metadata.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2340 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/shared/via.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18549 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_audits.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1744 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/macros.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1583 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_forms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3075 2023-06-14 10:17:08.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/talk_phone_numbers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6263 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/users.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      842 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/satisfaction_ratings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3004 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_fields.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1619 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/schemas/organizations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26635 2023-06-14 10:17:08.000000 tap-zendesk-2.1.0/tap_zendesk/streams.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8280 2023-06-13 03:09:32.000000 tap-zendesk-2.1.0/tap_zendesk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2473 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/tap_zendesk/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-14 10:17:40.000000 tap-zendesk-2.1.0/tap_zendesk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      125 2023-06-14 10:17:39.000000 tap-zendesk-2.1.0/tap_zendesk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-14 10:17:39.000000 tap-zendesk-2.1.0/tap_zendesk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-14 10:17:39.000000 tap-zendesk-2.1.0/tap_zendesk.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-06-14 10:17:39.000000 tap-zendesk-2.1.0/tap_zendesk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1397 2023-06-14 10:17:39.000000 tap-zendesk-2.1.0/tap_zendesk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-06-14 10:17:39.000000 tap-zendesk-2.1.0/tap_zendesk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-14 10:17:40.000000 tap-zendesk-2.1.0/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3201 2023-06-14 10:17:08.000000 tap-zendesk-2.1.0/test/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8646 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/test/test_all_streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4013 2023-06-14 10:17:08.000000 tap-zendesk-2.1.0/test/test_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2706 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/test/test_minimal_selection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2102 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/test/test_custom_fields_discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6986 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/test/test_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10408 2023-06-14 10:17:08.000000 tap-zendesk-2.1.0/test/test_standard_bookmark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3334 2023-06-14 10:17:08.000000 tap-zendesk-2.1.0/test/test_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10085 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/test/test_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6792 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/test/test_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-06-14 10:17:40.000000 tap-zendesk-2.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2023-06-14 10:17:40.000000 tap-zendesk-2.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-06-14 10:17:08.000000 tap-zendesk-2.1.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1553 2023-05-30 04:15:54.000000 tap-zendesk-2.1.0/README.md
```

### Comparing `tap-zendesk-2.0.1/tap_zendesk/http.py` & `tap-zendesk-2.1.0/tap_zendesk/http.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/metrics.py` & `tap-zendesk-2.1.0/tap_zendesk/metrics.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_metrics.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_metrics.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/tickets.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/tickets.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/group_memberships.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/group_memberships.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/sla_policies.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/sla_policies.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_comments.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_comments.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/groups.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/shared/attachments.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/shared/attachments.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/shared/metadata.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/shared/metadata.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/shared/via.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/shared/via.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_audits.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_audits.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/macros.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/macros.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_forms.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_forms.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/users.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/users.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/satisfaction_ratings.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/satisfaction_ratings.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/ticket_fields.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/ticket_fields.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/schemas/organizations.json` & `tap-zendesk-2.1.0/tap_zendesk/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/streams.py` & `tap-zendesk-2.1.0/tap_zendesk/streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -402,14 +402,42 @@
         HEADERS['Authorization'] = 'Bearer {}'.format(self.config["access_token"])
         try:
             http.call_api(url, self.request_timeout, params={'per_page': 1}, headers=HEADERS)
         except http.ZendeskNotFoundError:
             #Skip 404 ZendeskNotFoundError error as goal is just to check whether TicketComments have read permission or not
             pass
 
+class TicketMetricEvents(Stream):
+    name = "ticket_metric_events"
+    replication_method = "INCREMENTAL"
+    replication_key = "time"
+    count = 0
+
+    def sync(self, state):
+        bookmark = self.get_bookmark(state)
+        start = bookmark - datetime.timedelta(seconds=1)
+
+        epoch_start = int(start.strftime('%s'))
+        parsed_start = singer.strftime(start, "%Y-%m-%dT%H:%M:%SZ")
+        ticket_metric_events = self.client.tickets.metrics_incremental(start_time=epoch_start)
+        for event in ticket_metric_events:
+            self.count += 1
+            if bookmark < utils.strptime_with_tz(event.time):
+                self.update_bookmark(state, event.time)
+            if parsed_start <= event.time:
+                yield (self.stream, event)
+
+    def check_access(self):
+        try:
+            epoch_start = int(utils.now().strftime('%s'))
+            self.client.tickets.metrics_incremental(start_time=epoch_start)
+        except http.ZendeskNotFoundError:
+            #Skip 404 ZendeskNotFoundError error as goal is just to check whether TicketComments have read permission or not
+            pass
+
 class TicketComments(Stream):
     name = "ticket_comments"
     replication_method = "INCREMENTAL"
     count = 0
     endpoint = "https://{}.zendesk.com/api/v2/tickets/{}/comments.json"
     item_key='comments'
 
@@ -436,14 +464,29 @@
         HEADERS['Authorization'] = 'Bearer {}'.format(self.config["access_token"])
         try:
             http.call_api(url, self.request_timeout, params={'per_page': 1}, headers=HEADERS)
         except http.ZendeskNotFoundError:
             #Skip 404 ZendeskNotFoundError error as goal is to just check to whether TicketComments have read permission or not
             pass
 
+class TalkPhoneNumbers(Stream):
+    name = 'talk_phone_numbers'
+    replication_method = "FULL_TABLE"
+
+    def sync(self, state): # pylint: disable=unused-argument
+        for phone_number in self.client.talk.phone_numbers():
+            yield (self.stream, phone_number)
+
+    def check_access(self):
+        try:
+            self.client.talk.phone_numbers()
+        except http.ZendeskNotFoundError:
+            #Skip 404 ZendeskNotFoundError error as goal is to just check to whether TicketComments have read permission or not
+            pass
+
 class SatisfactionRatings(CursorBasedStream):
     name = "satisfaction_ratings"
     replication_method = "INCREMENTAL"
     replication_key = "updated_at"
     endpoint = 'https://{}.zendesk.com/api/v2/satisfaction_ratings'
     item_key = 'satisfaction_ratings'
 
@@ -604,9 +647,11 @@
     "ticket_fields": TicketFields,
     "ticket_forms": TicketForms,
     "group_memberships": GroupMemberships,
     "macros": Macros,
     "satisfaction_ratings": SatisfactionRatings,
     "tags": Tags,
     "ticket_metrics": TicketMetrics,
+    "ticket_metric_events": TicketMetricEvents,
     "sla_policies": SLAPolicies,
+    "talk_phone_numbers": TalkPhoneNumbers,
 }
```

### Comparing `tap-zendesk-2.0.1/tap_zendesk/__init__.py` & `tap-zendesk-2.1.0/tap_zendesk/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/sync.py` & `tap-zendesk-2.1.0/tap_zendesk/sync.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk/discover.py` & `tap-zendesk-2.1.0/tap_zendesk/discover.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/tap_zendesk.egg-info/SOURCES.txt` & `tap-zendesk-2.1.0/tap_zendesk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 tap_zendesk/schemas/group_memberships.json
 tap_zendesk/schemas/groups.json
 tap_zendesk/schemas/macros.json
 tap_zendesk/schemas/organizations.json
 tap_zendesk/schemas/satisfaction_ratings.json
 tap_zendesk/schemas/sla_policies.json
 tap_zendesk/schemas/tags.json
+tap_zendesk/schemas/talk_phone_numbers.json
 tap_zendesk/schemas/ticket_audits.json
 tap_zendesk/schemas/ticket_comments.json
 tap_zendesk/schemas/ticket_fields.json
 tap_zendesk/schemas/ticket_forms.json
+tap_zendesk/schemas/ticket_metric_events.json
 tap_zendesk/schemas/ticket_metrics.json
 tap_zendesk/schemas/tickets.json
 tap_zendesk/schemas/users.json
 tap_zendesk/schemas/shared/attachments.json
 tap_zendesk/schemas/shared/metadata.json
 tap_zendesk/schemas/shared/via.json
 test/test_all_fields.py
```

### Comparing `tap-zendesk-2.0.1/test/test_pagination.py` & `tap-zendesk-2.1.0/test/test_pagination.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         """
         
         # Streams to verify all fields tests
         expected_streams = self.expected_check_streams()
         expected_streams = expected_streams - {
             "satisfaction_ratings", # skip as only end user of tickets can create data
             "tags", #  Test Stability Issue: TDL-17980
+            "talk_phone_numbers"
         }
 
         conn_id = connections.ensure_connection(self)
 
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # table and field selection
```

### Comparing `tap-zendesk-2.0.1/test/test_all_streams.py` & `tap-zendesk-2.1.0/test/test_all_streams.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/test/test_all_fields.py` & `tap-zendesk-2.1.0/test/test_all_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         • Verify no unexpected streams were replicated
         • Verify that more than just the automatic fields are replicated for each stream. 
         • verify all fields for each stream are replicated
         """
         
         
         # Streams to verify all fields tests
-        expected_streams = self.expected_check_streams()
+        expected_streams = self.expected_check_streams() - {"talk_phone_numbers"}
         
         expected_automatic_fields = self.expected_automatic_fields()
         conn_id = connections.ensure_connection(self)
 
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # table and field selection
@@ -74,10 +74,12 @@
                 # As we can't generate following fields by zendesk APIs now so expected.
                 if stream == "ticket_fields":
                     expected_all_keys = expected_all_keys - {'system_field_options', 'sub_type_id'}
                 elif stream == "users":
                     expected_all_keys = expected_all_keys - {'chat_only'}
                 elif stream == "ticket_metrics":
                     expected_all_keys = expected_all_keys - {'status', 'instance_id', 'metric', 'type', 'time'}
+                elif stream == "talk_phone_numbers":
+                    expected_all_keys = expected_all_keys - {'token'}
                             
                 # verify all fields for each stream are replicated
                 self.assertSetEqual(expected_all_keys, actual_all_keys)
```

### Comparing `tap-zendesk-2.0.1/test/test_minimal_selection.py` & `tap-zendesk-2.1.0/test/test_minimal_selection.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/test/test_custom_fields_discover.py` & `tap-zendesk-2.1.0/test/test_custom_fields_discover.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/test/test_discovery.py` & `tap-zendesk-2.1.0/test/test_discovery.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/test/test_standard_bookmark.py` & `tap-zendesk-2.1.0/test/test_standard_bookmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,12 +182,12 @@
                         "INVALID EXPECTATIONS\t\tSTREAM: {} REPLICATION_METHOD: {}".format(
                             stream, expected_replication_method)
                     )
 
                 # Verify at least 1 record was replicated in the second sync
                 # 'tags' stream (FULL_TABLE) data appears to have aged out 11/18/2022. Since we do not have CRUD
                 # we will allow this stream to pass with a warning about decreased coverage
-                if stream == 'tags' and second_sync_count == 0 and first_sync_count == 0:
+                if stream in {'tags', 'talk_phone_numbers'} and second_sync_count == 0 and first_sync_count == 0:
                     print(f"FULL_TABLE stream 'tags' replicated 0 records, stream not fully tested")
                     continue
                 self.assertGreater(
                     second_sync_count, 0, msg="We are not fully testing bookmarking for {}".format(stream))
```

### Comparing `tap-zendesk-2.0.1/test/test_automatic_fields.py` & `tap-zendesk-2.1.0/test/test_automatic_fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def test_run(self):
         """
         Verify we can deselect all fields except when inclusion=automatic, which is handled by base.py methods
         Verify that only the automatic fields are sent to the target.
         Verify that all replicated records have unique primary key values.
         """
 
-        streams_to_test = self.expected_check_streams()
+        streams_to_test = self.expected_check_streams() - {"talk_phone_numbers"}
 
         conn_id = connections.ensure_connection(self)
 
         found_catalogs = self.run_and_verify_check_mode(conn_id)
 
         # table and field selection
         test_catalogs_automatic_fields = [catalog for catalog in found_catalogs
@@ -60,12 +60,12 @@
                     msg="The number of records is not over the stream min limit")
 
                 # Verify that only the automatic fields are sent to the target
                 for actual_keys in record_messages_keys:
                     self.assertSetEqual(expected_keys, actual_keys)
 
                 # Verify that all replicated records have unique primary key values.
-                if stream == 'organizations': # BUG_TDL-19428
+                if stream in {'organizations', 'ticket_metric_events'}: # BUG_TDL-19428
                     continue # skipping
                 self.assertEqual(len(primary_keys_list),
                                  len(unique_primary_keys_list),
                                  msg="Replicated record does not have unique primary key values.")
```

### Comparing `tap-zendesk-2.0.1/test/test_start_date.py` & `tap-zendesk-2.1.0/test/test_start_date.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/test/test_bookmarks.py` & `tap-zendesk-2.1.0/test/test_bookmarks.py`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/setup.py` & `tap-zendesk-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-zendesk',
-      version='2.0.1',
+      version='2.1.0',
       description='Singer.io tap for extracting data from the Zendesk API',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_zendesk'],
       install_requires=[
           'singer-python==5.12.2',
```

### Comparing `tap-zendesk-2.0.1/LICENSE` & `tap-zendesk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-zendesk-2.0.1/README.md` & `tap-zendesk-2.1.0/README.md`

 * *Files identical despite different names*

