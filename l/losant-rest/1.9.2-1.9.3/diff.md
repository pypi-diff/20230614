# Comparing `tmp/losant-rest-1.9.2.tar.gz` & `tmp/losant-rest-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/losant-rest-1.9.2.tar", last modified: Fri Jan 10 16:17:44 2020, max compression
+gzip compressed data, was "dist/losant-rest-1.9.3.tar", last modified: Wed Feb 19 23:24:57 2020, max compression
```

## Comparing `losant-rest-1.9.2.tar` & `losant-rest-1.9.3.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 mkuehl     (501) staff       (20)        0 2020-01-10 16:17:44.000000 losant-rest-1.9.2/
--rw-r--r--   0 mkuehl     (501) staff       (20)    17691 2020-01-10 16:17:44.000000 losant-rest-1.9.2/PKG-INFO
-drwxr-xr-x   0 mkuehl     (501) staff       (20)        0 2020-01-10 16:17:43.000000 losant-rest-1.9.2/losant_rest.egg-info/
--rw-r--r--   0 mkuehl     (501) staff       (20)    17691 2020-01-10 16:17:43.000000 losant-rest-1.9.2/losant_rest.egg-info/PKG-INFO
--rw-r--r--   0 mkuehl     (501) staff       (20)     1893 2020-01-10 16:17:43.000000 losant-rest-1.9.2/losant_rest.egg-info/SOURCES.txt
--rw-r--r--   0 mkuehl     (501) staff       (20)       15 2020-01-10 16:17:43.000000 losant-rest-1.9.2/losant_rest.egg-info/requires.txt
--rw-r--r--   0 mkuehl     (501) staff       (20)       11 2020-01-10 16:17:43.000000 losant-rest-1.9.2/losant_rest.egg-info/top_level.txt
--rw-r--r--   0 mkuehl     (501) staff       (20)        1 2020-01-10 16:17:43.000000 losant-rest-1.9.2/losant_rest.egg-info/dependency_links.txt
--rw-r--r--   0 mkuehl     (501) staff       (20)     1083 2020-01-10 16:12:55.000000 losant-rest-1.9.2/LICENSE
--rw-r--r--   0 mkuehl     (501) staff       (20)       34 2016-06-14 21:43:43.000000 losant-rest-1.9.2/MANIFEST.in
--rw-r--r--   0 mkuehl     (501) staff       (20)    14961 2019-02-27 14:11:20.000000 losant-rest-1.9.2/README.md
--rw-r--r--   0 mkuehl     (501) staff       (20)     1380 2020-01-10 16:12:51.000000 losant-rest-1.9.2/setup.py
--rw-r--r--   0 mkuehl     (501) staff       (20)       38 2020-01-10 16:17:44.000000 losant-rest-1.9.2/setup.cfg
-drwxr-xr-x   0 mkuehl     (501) staff       (20)        0 2020-01-10 16:17:44.000000 losant-rest-1.9.2/losantrest/
--rw-r--r--   0 mkuehl     (501) staff       (20)    11595 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/flow_version.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     8291 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_version.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6600 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application_keys.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6628 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/auth.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6986 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/files.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     8757 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application_certificate_authority.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    10825 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_view.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7559 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/event.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    22541 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/org.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    26135 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/me.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7269 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_users.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7942 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application_key.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6389 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application_api_tokens.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7649 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/webhook.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    30126 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/device.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6511 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/dashboards.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    16689 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/events.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6507 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/data_tables.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     8295 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/client.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7088 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/applications.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6799 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application_certificates.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     1465 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/losant_error.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6577 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/orgs.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7078 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     1157 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/__init__.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    19057 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/flow.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7991 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_slug.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     5484 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_domains.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7836 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/integration.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    27663 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    11112 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/dashboard.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6673 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_versions.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7803 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application_api_token.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    10105 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/file.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7991 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_user.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    10412 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_endpoints.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6627 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_groups.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     4912 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/org_invites.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     8037 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_group.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     8307 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/data_table_row.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6955 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application_certificate_authorities.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7615 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/flow_versions.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    10362 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/device_recipe.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    13616 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/flows.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    11061 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_endpoint.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    12288 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/data_table.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    11443 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/edge_deployments.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6459 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/webhooks.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6567 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/device_recipes.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    14875 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/notebook.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6479 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/notebooks.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     4423 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/audit_logs.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     8083 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_domain.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    13815 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/devices.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     8323 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/application_certificate.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6573 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/integrations.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     6992 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_views.py
--rw-r--r--   0 mkuehl     (501) staff       (20)    16805 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/data_table_rows.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     3346 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/audit_log.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     5444 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/experience_slugs.py
--rw-r--r--   0 mkuehl     (501) staff       (20)     7822 2020-01-10 16:13:24.000000 losant-rest-1.9.2/losantrest/data.py
+drwxr-xr-x   0 erinthompson   (501) staff       (20)        0 2020-02-19 23:24:57.000000 losant-rest-1.9.3/
+-rw-r--r--   0 erinthompson   (501) staff       (20)    17691 2020-02-19 23:24:57.000000 losant-rest-1.9.3/PKG-INFO
+drwxr-xr-x   0 erinthompson   (501) staff       (20)        0 2020-02-19 23:24:57.000000 losant-rest-1.9.3/losant_rest.egg-info/
+-rw-r--r--   0 erinthompson   (501) staff       (20)    17691 2020-02-19 23:24:57.000000 losant-rest-1.9.3/losant_rest.egg-info/PKG-INFO
+-rw-r--r--   0 erinthompson   (501) staff       (20)     1929 2020-02-19 23:24:57.000000 losant-rest-1.9.3/losant_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 erinthompson   (501) staff       (20)       15 2020-02-19 23:24:57.000000 losant-rest-1.9.3/losant_rest.egg-info/requires.txt
+-rw-r--r--   0 erinthompson   (501) staff       (20)       11 2020-02-19 23:24:57.000000 losant-rest-1.9.3/losant_rest.egg-info/top_level.txt
+-rw-r--r--   0 erinthompson   (501) staff       (20)        1 2020-02-19 23:24:57.000000 losant-rest-1.9.3/losant_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 erinthompson   (501) staff       (20)     1083 2020-02-19 22:51:46.000000 losant-rest-1.9.3/LICENSE
+-rw-r--r--   0 erinthompson   (501) staff       (20)       34 2020-02-19 22:51:46.000000 losant-rest-1.9.3/MANIFEST.in
+-rw-r--r--   0 erinthompson   (501) staff       (20)    14961 2020-02-19 22:51:46.000000 losant-rest-1.9.3/README.md
+-rw-r--r--   0 erinthompson   (501) staff       (20)     1380 2020-02-19 23:04:55.000000 losant-rest-1.9.3/setup.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)       38 2020-02-19 23:24:57.000000 losant-rest-1.9.3/setup.cfg
+drwxr-xr-x   0 erinthompson   (501) staff       (20)        0 2020-02-19 23:24:57.000000 losant-rest-1.9.3/losantrest/
+-rw-r--r--   0 erinthompson   (501) staff       (20)    11595 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/flow_version.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     8291 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_version.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6600 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_keys.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    10032 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/auth.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6986 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/files.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     8757 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_certificate_authority.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    10825 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_view.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7559 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/event.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    22541 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/org.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    26135 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/me.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7269 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_users.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7942 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_key.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6389 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_api_tokens.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7649 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/webhook.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    30126 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/device.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6511 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/dashboards.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    16689 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/events.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6507 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/data_tables.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     8415 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/client.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7088 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/applications.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6799 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_certificates.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     1465 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/losant_error.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6577 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/orgs.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     4171 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_templates.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7078 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     1157 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/__init__.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    19057 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/flow.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7991 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_slug.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     5484 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_domains.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7836 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/integration.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    31703 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    11112 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/dashboard.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6673 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_versions.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7803 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_api_token.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    10105 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/file.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7991 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_user.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    10412 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_endpoints.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6627 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_groups.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     4912 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/org_invites.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     8037 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_group.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     8307 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/data_table_row.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6955 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_certificate_authorities.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7615 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/flow_versions.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    10362 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/device_recipe.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    13616 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/flows.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    11061 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_endpoint.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    12288 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/data_table.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    11443 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/edge_deployments.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6459 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/webhooks.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6567 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/device_recipes.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    14875 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/notebook.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6479 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/notebooks.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     4423 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/audit_logs.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     8083 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_domain.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    14109 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/devices.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     8323 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/application_certificate.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6573 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/integrations.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     6992 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_views.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)    16805 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/data_table_rows.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     3346 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/audit_log.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     5444 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/experience_slugs.py
+-rw-r--r--   0 erinthompson   (501) staff       (20)     7822 2020-02-19 22:54:04.000000 losant-rest-1.9.3/losantrest/data.py
```

### Comparing `losant-rest-1.9.2/PKG-INFO` & `losant-rest-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losant-rest
-Version: 1.9.2
+Version: 1.9.3
 Summary: A REST client for the Losant API
 Home-page: https://github.com/Losant/losant-rest-python
 Author: Losant
 Author-email: hello@losant.com
 License: MIT
 Description: # Losant Python REST API Client
         
@@ -234,15 +234,15 @@
         * [webhooks](docs/webhooks.md)  
           Contains all the actions that can be performed against the collection of [Webhooks](https://docs.losant.com/applications/webhooks/) belonging to an Application - such as listing the webhooks or creating a new webhook.
         
         <br/>
         
         *****
         
-        Copyright (c) 2019 Losant IoT, Inc
+        Copyright (c) 2020 Losant IoT, Inc
         
         <https://www.losant.com>
         
 Keywords: REST,Losant,IoT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `losant-rest-1.9.2/losant_rest.egg-info/PKG-INFO` & `losant-rest-1.9.3/losant_rest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losant-rest
-Version: 1.9.2
+Version: 1.9.3
 Summary: A REST client for the Losant API
 Home-page: https://github.com/Losant/losant-rest-python
 Author: Losant
 Author-email: hello@losant.com
 License: MIT
 Description: # Losant Python REST API Client
         
@@ -234,15 +234,15 @@
         * [webhooks](docs/webhooks.md)  
           Contains all the actions that can be performed against the collection of [Webhooks](https://docs.losant.com/applications/webhooks/) belonging to an Application - such as listing the webhooks or creating a new webhook.
         
         <br/>
         
         *****
         
-        Copyright (c) 2019 Losant IoT, Inc
+        Copyright (c) 2020 Losant IoT, Inc
         
         <https://www.losant.com>
         
 Keywords: REST,Losant,IoT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `losant-rest-1.9.2/losant_rest.egg-info/SOURCES.txt` & `losant-rest-1.9.3/losant_rest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 losantrest/application_api_tokens.py
 losantrest/application_certificate.py
 losantrest/application_certificate_authorities.py
 losantrest/application_certificate_authority.py
 losantrest/application_certificates.py
 losantrest/application_key.py
 losantrest/application_keys.py
+losantrest/application_templates.py
 losantrest/applications.py
 losantrest/audit_log.py
 losantrest/audit_logs.py
 losantrest/auth.py
 losantrest/client.py
 losantrest/dashboard.py
 losantrest/dashboards.py
```

### Comparing `losant-rest-1.9.2/LICENSE` & `losant-rest-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/README.md` & `losant-rest-1.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -226,10 +226,10 @@
 * [webhooks](docs/webhooks.md)  
   Contains all the actions that can be performed against the collection of [Webhooks](https://docs.losant.com/applications/webhooks/) belonging to an Application - such as listing the webhooks or creating a new webhook.
 
 <br/>
 
 *****
 
-Copyright (c) 2019 Losant IoT, Inc
+Copyright (c) 2020 Losant IoT, Inc
 
 <https://www.losant.com>
```

### Comparing `losant-rest-1.9.2/setup.py` & `losant-rest-1.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='losant-rest',
-    version='1.9.2',
+    version='1.9.3',
     description='A REST client for the Losant API',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/Losant/losant-rest-python',
     author='Losant',
     author_email='hello@losant.com',
     license='MIT',
```

### Comparing `losant-rest-1.9.2/losantrest/flow_version.py` & `losant-rest-1.9.3/losantrest/flow_version.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_version.py` & `losant-rest-1.9.3/losantrest/experience_version.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/application_keys.py` & `losant-rest-1.9.3/losantrest/application_keys.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/auth.py` & `losant-rest-1.9.3/losantrest/org_invites.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,142 +21,105 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 
 import json
 
-""" Module for Losant API Auth wrapper class """
+""" Module for Losant API OrgInvites wrapper class """
 # pylint: disable=C0301
 
-class Auth(object):
-    """ Class containing all the actions for the Auth Resource """
+class OrgInvites(object):
+    """ Class containing all the actions for the Org Invites Resource """
 
     def __init__(self, client):
         self.client = client
 
-    def authenticate_device(self, **kwargs):
+    def get(self, **kwargs):
         """
-        Authenticates a device using the provided credentials.
+        Gets information about an invite
 
         Authentication:
         No api access token is required to call this action.
 
         Parameters:
-        *  {hash} credentials - Device authentication credentials (https://api.losant.com/#/definitions/deviceCredentials)
+        *  {string} token - The token associated with the invite
+        *  {string} email - The email associated with the invite
         *  {string} losantdomain - Domain scope of request (rarely needed)
         *  {boolean} _actions - Return resource actions in response
         *  {boolean} _links - Return resource link in response
         *  {boolean} _embedded - Return embedded resources in response
 
         Responses:
-        *  200 - Successful authentication. The included api access token by default has the scope 'all.Device'. (https://api.losant.com/#/definitions/authedDevice)
+        *  200 - Information about invite (https://api.losant.com/#/definitions/orgInviteInfo)
 
         Errors:
         *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
-        *  401 - Unauthorized error if authentication fails (https://api.losant.com/#/definitions/error)
+        *  404 - Error if invite not found (https://api.losant.com/#/definitions/error)
+        *  410 - Error if invite has expired (https://api.losant.com/#/definitions/error)
         """
 
         query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
         path_params = {}
         headers = {}
         body = None
 
-        if "credentials" in kwargs:
-            body = kwargs["credentials"]
+        if "token" in kwargs:
+            query_params["token"] = kwargs["token"]
+        if "email" in kwargs:
+            query_params["email"] = kwargs["email"]
         if "losantdomain" in kwargs:
             headers["losantdomain"] = kwargs["losantdomain"]
         if "_actions" in kwargs:
             query_params["_actions"] = kwargs["_actions"]
         if "_links" in kwargs:
             query_params["_links"] = kwargs["_links"]
         if "_embedded" in kwargs:
             query_params["_embedded"] = kwargs["_embedded"]
 
-        path = "/auth/device".format(**path_params)
+        path = "/invites".format(**path_params)
 
-        return self.client.request("POST", path, params=query_params, headers=headers, body=body)
-
-    def authenticate_user(self, **kwargs):
-        """
-        Authenticates a user using the provided credentials.
-
-        Authentication:
-        No api access token is required to call this action.
-
-        Parameters:
-        *  {hash} credentials - User authentication credentials (https://api.losant.com/#/definitions/userCredentials)
-        *  {string} losantdomain - Domain scope of request (rarely needed)
-        *  {boolean} _actions - Return resource actions in response
-        *  {boolean} _links - Return resource link in response
-        *  {boolean} _embedded - Return embedded resources in response
-
-        Responses:
-        *  200 - Successful authentication. The included api access token has the scope 'all.User'. (https://api.losant.com/#/definitions/authedUser)
-
-        Errors:
-        *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
-        *  401 - Unauthorized error if authentication fails (https://api.losant.com/#/definitions/error)
-        """
-
-        query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
-        path_params = {}
-        headers = {}
-        body = None
-
-        if "credentials" in kwargs:
-            body = kwargs["credentials"]
-        if "losantdomain" in kwargs:
-            headers["losantdomain"] = kwargs["losantdomain"]
-        if "_actions" in kwargs:
-            query_params["_actions"] = kwargs["_actions"]
-        if "_links" in kwargs:
-            query_params["_links"] = kwargs["_links"]
-        if "_embedded" in kwargs:
-            query_params["_embedded"] = kwargs["_embedded"]
-
-        path = "/auth/user".format(**path_params)
-
-        return self.client.request("POST", path, params=query_params, headers=headers, body=body)
+        return self.client.request("GET", path, params=query_params, headers=headers, body=body)
 
-    def authenticate_user_github(self, **kwargs):
+    def post(self, **kwargs):
         """
-        Authenticates a user via GitHub OAuth.
+        Accepts/Rejects an invite
 
         Authentication:
         No api access token is required to call this action.
 
         Parameters:
-        *  {hash} oauth - User authentication credentials (access token) (https://api.losant.com/#/definitions/githubLogin)
+        *  {hash} invite - Invite info and acceptance (https://api.losant.com/#/definitions/orgInviteAction)
         *  {string} losantdomain - Domain scope of request (rarely needed)
         *  {boolean} _actions - Return resource actions in response
         *  {boolean} _links - Return resource link in response
         *  {boolean} _embedded - Return embedded resources in response
 
         Responses:
-        *  200 - Successful authentication. The included api access token has the scope 'all.User'. (https://api.losant.com/#/definitions/authedUser)
+        *  200 - Acceptance/Rejection of invite (https://api.losant.com/#/definitions/orgInviteResult)
 
         Errors:
         *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
-        *  401 - Unauthorized error if authentication fails (https://api.losant.com/#/definitions/error)
+        *  404 - Error if invite not found (https://api.losant.com/#/definitions/error)
+        *  410 - Error if invite has expired (https://api.losant.com/#/definitions/error)
         """
 
         query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
         path_params = {}
         headers = {}
         body = None
 
-        if "oauth" in kwargs:
-            body = kwargs["oauth"]
+        if "invite" in kwargs:
+            body = kwargs["invite"]
         if "losantdomain" in kwargs:
             headers["losantdomain"] = kwargs["losantdomain"]
         if "_actions" in kwargs:
             query_params["_actions"] = kwargs["_actions"]
         if "_links" in kwargs:
             query_params["_links"] = kwargs["_links"]
         if "_embedded" in kwargs:
             query_params["_embedded"] = kwargs["_embedded"]
 
-        path = "/auth/user/github".format(**path_params)
+        path = "/invites".format(**path_params)
 
         return self.client.request("POST", path, params=query_params, headers=headers, body=body)
```

### Comparing `losant-rest-1.9.2/losantrest/files.py` & `losant-rest-1.9.3/losantrest/files.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/application_certificate_authority.py` & `losant-rest-1.9.3/losantrest/application_certificate_authority.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_view.py` & `losant-rest-1.9.3/losantrest/experience_view.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/event.py` & `losant-rest-1.9.3/losantrest/event.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/org.py` & `losant-rest-1.9.3/losantrest/org.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/me.py` & `losant-rest-1.9.3/losantrest/me.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_users.py` & `losant-rest-1.9.3/losantrest/experience_users.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/application_key.py` & `losant-rest-1.9.3/losantrest/application_key.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/application_api_tokens.py` & `losant-rest-1.9.3/losantrest/application_api_tokens.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/webhook.py` & `losant-rest-1.9.3/losantrest/webhook.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/device.py` & `losant-rest-1.9.3/losantrest/device.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/dashboards.py` & `losant-rest-1.9.3/losantrest/dashboards.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/events.py` & `losant-rest-1.9.3/losantrest/events.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/data_tables.py` & `losant-rest-1.9.3/losantrest/data_tables.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/client.py` & `losant-rest-1.9.3/losantrest/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from .application_api_tokens import ApplicationApiTokens
 from .application_certificate import ApplicationCertificate
 from .application_certificate_authorities import ApplicationCertificateAuthorities
 from .application_certificate_authority import ApplicationCertificateAuthority
 from .application_certificates import ApplicationCertificates
 from .application_key import ApplicationKey
 from .application_keys import ApplicationKeys
+from .application_templates import ApplicationTemplates
 from .applications import Applications
 from .audit_log import AuditLog
 from .audit_logs import AuditLogs
 from .auth import Auth
 from .dashboard import Dashboard
 from .dashboards import Dashboards
 from .data import Data
@@ -93,29 +94,30 @@
 
 class Client(object):
     """
     Losant API
 
     User API for accessing Losant data
 
-    Built For Version 1.16.2
+    Built For Version 1.16.4
     """
 
     def __init__(self, auth_token=None, url="https://api.losant.com"):
         self.url = url
         self.auth_token = auth_token
         self.application = Application(self)
         self.application_api_token = ApplicationApiToken(self)
         self.application_api_tokens = ApplicationApiTokens(self)
         self.application_certificate = ApplicationCertificate(self)
         self.application_certificate_authorities = ApplicationCertificateAuthorities(self)
         self.application_certificate_authority = ApplicationCertificateAuthority(self)
         self.application_certificates = ApplicationCertificates(self)
         self.application_key = ApplicationKey(self)
         self.application_keys = ApplicationKeys(self)
+        self.application_templates = ApplicationTemplates(self)
         self.applications = Applications(self)
         self.audit_log = AuditLog(self)
         self.audit_logs = AuditLogs(self)
         self.auth = Auth(self)
         self.dashboard = Dashboard(self)
         self.dashboards = Dashboards(self)
         self.data = Data(self)
@@ -166,15 +168,15 @@
         """ Base method for making a Losant API request """
         if not headers:
             headers = {}
         if not params:
             params = {}
 
         headers["Accept"] = "application/json"
-        headers["Accept-Version"] = "^1.16.2"
+        headers["Accept-Version"] = "^1.16.4"
         if self.auth_token:
             headers["Authorization"] = "Bearer {0}".format(self.auth_token)
 
         path = self.url + path
         params = self.flatten_params(params)
         response = requests.request(method, path, params=params, headers=headers, json=body)
```

### Comparing `losant-rest-1.9.2/losantrest/applications.py` & `losant-rest-1.9.3/losantrest/applications.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/application_certificates.py` & `losant-rest-1.9.3/losantrest/application_certificates.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/losant_error.py` & `losant-rest-1.9.3/losantrest/losant_error.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/orgs.py` & `losant-rest-1.9.3/losantrest/orgs.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience.py` & `losant-rest-1.9.3/losantrest/experience.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/__init__.py` & `losant-rest-1.9.3/losantrest/__init__.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/flow.py` & `losant-rest-1.9.3/losantrest/flow.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_slug.py` & `losant-rest-1.9.3/losantrest/experience_slug.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_domains.py` & `losant-rest-1.9.3/losantrest/experience_domains.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/integration.py` & `losant-rest-1.9.3/losantrest/integration.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/application.py` & `losant-rest-1.9.3/losantrest/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
         path = "/applications/{applicationId}/archiveData".format(**path_params)
 
         return self.client.request("GET", path, params=query_params, headers=headers, body=body)
 
     def backfill_archive_data(self, **kwargs):
         """
-        Returns success when a job has been enqueued to backfill all current data to it's archive
+        Returns success when a job has been enqueued to backfill all current data to its archive
 
         Authentication:
         The client must be configured with a valid api
         access token to call this action. The token
         must include at least one of the following scopes:
         all.Application, all.Organization, all.User, application.*, or application.backfillArchiveData.
 
@@ -221,15 +221,15 @@
 
         path = "/applications/{applicationId}".format(**path_params)
 
         return self.client.request("DELETE", path, params=query_params, headers=headers, body=body)
 
     def export(self, **kwargs):
         """
-        Export an application and all of it's resources
+        Export an application and all of its resources
 
         Authentication:
         The client must be configured with a valid api
         access token to call this action. The token
         must include at least one of the following scopes:
         all.Application, all.Organization, all.User, application.*, or application.export.
 
@@ -562,14 +562,107 @@
         if "_embedded" in kwargs:
             query_params["_embedded"] = kwargs["_embedded"]
 
         path = "/applications/{applicationId}/payloadCounts".format(**path_params)
 
         return self.client.request("GET", path, params=query_params, headers=headers, body=body)
 
+    def readme(self, **kwargs):
+        """
+        Get the current application readme information
+
+        Authentication:
+        The client must be configured with a valid api
+        access token to call this action. The token
+        must include at least one of the following scopes:
+        all.Application, all.Application.read, all.Organization, all.Organization.read, all.User, all.User.read, application.*, or application.get.
+
+        Parameters:
+        *  {string} applicationId - ID of the associated application
+        *  {string} losantdomain - Domain scope of request (rarely needed)
+        *  {boolean} _actions - Return resource actions in response
+        *  {boolean} _links - Return resource link in response
+        *  {boolean} _embedded - Return embedded resources in response
+
+        Responses:
+        *  200 - The application readme information (https://api.losant.com/#/definitions/applicationReadme)
+
+        Errors:
+        *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
+        *  404 - Error if application was not found (https://api.losant.com/#/definitions/error)
+        """
+
+        query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
+        path_params = {}
+        headers = {}
+        body = None
+
+        if "applicationId" in kwargs:
+            path_params["applicationId"] = kwargs["applicationId"]
+        if "losantdomain" in kwargs:
+            headers["losantdomain"] = kwargs["losantdomain"]
+        if "_actions" in kwargs:
+            query_params["_actions"] = kwargs["_actions"]
+        if "_links" in kwargs:
+            query_params["_links"] = kwargs["_links"]
+        if "_embedded" in kwargs:
+            query_params["_embedded"] = kwargs["_embedded"]
+
+        path = "/applications/{applicationId}/readme".format(**path_params)
+
+        return self.client.request("GET", path, params=query_params, headers=headers, body=body)
+
+    def readme_patch(self, **kwargs):
+        """
+        Update the current application readme information
+
+        Authentication:
+        The client must be configured with a valid api
+        access token to call this action. The token
+        must include at least one of the following scopes:
+        all.Application, all.Organization, all.User, application.*, or application.patch.
+
+        Parameters:
+        *  {string} applicationId - ID of the associated application
+        *  {hash} readme - Object containing new readme information (https://api.losant.com/#/definitions/applicationReadmePatch)
+        *  {string} losantdomain - Domain scope of request (rarely needed)
+        *  {boolean} _actions - Return resource actions in response
+        *  {boolean} _links - Return resource link in response
+        *  {boolean} _embedded - Return embedded resources in response
+
+        Responses:
+        *  200 - Updated readme information (https://api.losant.com/#/definitions/applicationReadme)
+
+        Errors:
+        *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
+        *  404 - Error if application was not found (https://api.losant.com/#/definitions/error)
+        """
+
+        query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
+        path_params = {}
+        headers = {}
+        body = None
+
+        if "applicationId" in kwargs:
+            path_params["applicationId"] = kwargs["applicationId"]
+        if "readme" in kwargs:
+            body = kwargs["readme"]
+        if "losantdomain" in kwargs:
+            headers["losantdomain"] = kwargs["losantdomain"]
+        if "_actions" in kwargs:
+            query_params["_actions"] = kwargs["_actions"]
+        if "_links" in kwargs:
+            query_params["_links"] = kwargs["_links"]
+        if "_embedded" in kwargs:
+            query_params["_embedded"] = kwargs["_embedded"]
+
+        path = "/applications/{applicationId}/readme".format(**path_params)
+
+        return self.client.request("PATCH", path, params=query_params, headers=headers, body=body)
+
     def search(self, **kwargs):
         """
         Search across an application's resources by target identifier
 
         Authentication:
         The client must be configured with a valid api
         access token to call this action. The token
```

### Comparing `losant-rest-1.9.2/losantrest/dashboard.py` & `losant-rest-1.9.3/losantrest/dashboard.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_versions.py` & `losant-rest-1.9.3/losantrest/experience_versions.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/application_api_token.py` & `losant-rest-1.9.3/losantrest/application_api_token.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/file.py` & `losant-rest-1.9.3/losantrest/file.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_user.py` & `losant-rest-1.9.3/losantrest/experience_user.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_endpoints.py` & `losant-rest-1.9.3/losantrest/experience_endpoints.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_groups.py` & `losant-rest-1.9.3/losantrest/experience_groups.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/org_invites.py` & `losant-rest-1.9.3/losantrest/experience_slugs.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,105 +21,109 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 
 import json
 
-""" Module for Losant API OrgInvites wrapper class """
+""" Module for Losant API ExperienceSlugs wrapper class """
 # pylint: disable=C0301
 
-class OrgInvites(object):
-    """ Class containing all the actions for the Org Invites Resource """
+class ExperienceSlugs(object):
+    """ Class containing all the actions for the Experience Slugs Resource """
 
     def __init__(self, client):
         self.client = client
 
     def get(self, **kwargs):
         """
-        Gets information about an invite
+        Returns the experience slugs for an application
 
         Authentication:
-        No api access token is required to call this action.
+        The client must be configured with a valid api
+        access token to call this action. The token
+        must include at least one of the following scopes:
+        all.Application, all.Application.read, all.Organization, all.Organization.read, all.User, all.User.read, experienceSlugs.*, or experienceSlugs.get.
 
         Parameters:
-        *  {string} token - The token associated with the invite
-        *  {string} email - The email associated with the invite
+        *  {string} applicationId - ID associated with the application
         *  {string} losantdomain - Domain scope of request (rarely needed)
         *  {boolean} _actions - Return resource actions in response
         *  {boolean} _links - Return resource link in response
         *  {boolean} _embedded - Return embedded resources in response
 
         Responses:
-        *  200 - Information about invite (https://api.losant.com/#/definitions/orgInviteInfo)
+        *  200 - Collection of experience slugs (https://api.losant.com/#/definitions/experienceSlugs)
 
         Errors:
         *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
-        *  404 - Error if invite not found (https://api.losant.com/#/definitions/error)
-        *  410 - Error if invite has expired (https://api.losant.com/#/definitions/error)
+        *  404 - Error if application was not found (https://api.losant.com/#/definitions/error)
         """
 
         query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
         path_params = {}
         headers = {}
         body = None
 
-        if "token" in kwargs:
-            query_params["token"] = kwargs["token"]
-        if "email" in kwargs:
-            query_params["email"] = kwargs["email"]
+        if "applicationId" in kwargs:
+            path_params["applicationId"] = kwargs["applicationId"]
         if "losantdomain" in kwargs:
             headers["losantdomain"] = kwargs["losantdomain"]
         if "_actions" in kwargs:
             query_params["_actions"] = kwargs["_actions"]
         if "_links" in kwargs:
             query_params["_links"] = kwargs["_links"]
         if "_embedded" in kwargs:
             query_params["_embedded"] = kwargs["_embedded"]
 
-        path = "/invites".format(**path_params)
+        path = "/applications/{applicationId}/experience/slugs".format(**path_params)
 
         return self.client.request("GET", path, params=query_params, headers=headers, body=body)
 
     def post(self, **kwargs):
         """
-        Accepts/Rejects an invite
+        Create a new experience slug for an application
 
         Authentication:
-        No api access token is required to call this action.
+        The client must be configured with a valid api
+        access token to call this action. The token
+        must include at least one of the following scopes:
+        all.Application, all.Organization, all.User, experienceSlugs.*, or experienceSlugs.post.
 
         Parameters:
-        *  {hash} invite - Invite info and acceptance (https://api.losant.com/#/definitions/orgInviteAction)
+        *  {string} applicationId - ID associated with the application
+        *  {hash} experienceSlug - New experience slug information (https://api.losant.com/#/definitions/experienceSlugPost)
         *  {string} losantdomain - Domain scope of request (rarely needed)
         *  {boolean} _actions - Return resource actions in response
         *  {boolean} _links - Return resource link in response
         *  {boolean} _embedded - Return embedded resources in response
 
         Responses:
-        *  200 - Acceptance/Rejection of invite (https://api.losant.com/#/definitions/orgInviteResult)
+        *  201 - Successfully created experience slug (https://api.losant.com/#/definitions/experienceSlug)
 
         Errors:
         *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
-        *  404 - Error if invite not found (https://api.losant.com/#/definitions/error)
-        *  410 - Error if invite has expired (https://api.losant.com/#/definitions/error)
+        *  404 - Error if application was not found (https://api.losant.com/#/definitions/error)
         """
 
         query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
         path_params = {}
         headers = {}
         body = None
 
-        if "invite" in kwargs:
-            body = kwargs["invite"]
+        if "applicationId" in kwargs:
+            path_params["applicationId"] = kwargs["applicationId"]
+        if "experienceSlug" in kwargs:
+            body = kwargs["experienceSlug"]
         if "losantdomain" in kwargs:
             headers["losantdomain"] = kwargs["losantdomain"]
         if "_actions" in kwargs:
             query_params["_actions"] = kwargs["_actions"]
         if "_links" in kwargs:
             query_params["_links"] = kwargs["_links"]
         if "_embedded" in kwargs:
             query_params["_embedded"] = kwargs["_embedded"]
 
-        path = "/invites".format(**path_params)
+        path = "/applications/{applicationId}/experience/slugs".format(**path_params)
 
         return self.client.request("POST", path, params=query_params, headers=headers, body=body)
```

### Comparing `losant-rest-1.9.2/losantrest/experience_group.py` & `losant-rest-1.9.3/losantrest/experience_group.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/data_table_row.py` & `losant-rest-1.9.3/losantrest/data_table_row.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/application_certificate_authorities.py` & `losant-rest-1.9.3/losantrest/application_certificate_authorities.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/flow_versions.py` & `losant-rest-1.9.3/losantrest/flow_versions.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/device_recipe.py` & `losant-rest-1.9.3/losantrest/device_recipe.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/flows.py` & `losant-rest-1.9.3/losantrest/flows.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_endpoint.py` & `losant-rest-1.9.3/losantrest/experience_endpoint.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/data_table.py` & `losant-rest-1.9.3/losantrest/data_table.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/edge_deployments.py` & `losant-rest-1.9.3/losantrest/edge_deployments.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/webhooks.py` & `losant-rest-1.9.3/losantrest/webhooks.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/device_recipes.py` & `losant-rest-1.9.3/losantrest/device_recipes.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/notebook.py` & `losant-rest-1.9.3/losantrest/notebook.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/notebooks.py` & `losant-rest-1.9.3/losantrest/notebooks.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/audit_logs.py` & `losant-rest-1.9.3/losantrest/audit_logs.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_domain.py` & `losant-rest-1.9.3/losantrest/experience_domain.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/devices.py` & `losant-rest-1.9.3/losantrest/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
         *  {string} perPage - How many items to return per page
         *  {string} filterField - Field to filter the results by. Blank or not provided means no filtering. Accepted values are: name
         *  {string} filter - Filter to apply against the filtered field. Supports globbing. Blank or not provided means no filtering.
         *  {hash} deviceClass - Filter the devices by the given device class or classes (https://api.losant.com/#/definitions/deviceClassFilter)
         *  {hash} tagFilter - Array of tag pairs to filter by (https://api.losant.com/#/definitions/deviceTagFilter)
         *  {string} excludeConnectionInfo - If set, do not return connection info
         *  {string} parentId - Filter devices as children of a given system id
+        *  {hash} query - Device filter JSON object which overides the filterField, filter, deviceClass, tagFilter, and parentId parameters. (https://api.losant.com/#/definitions/advancedDeviceQuery)
         *  {string} losantdomain - Domain scope of request (rarely needed)
         *  {boolean} _actions - Return resource actions in response
         *  {boolean} _links - Return resource link in response
         *  {boolean} _embedded - Return embedded resources in response
 
         Responses:
         *  200 - Collection of devices (https://api.losant.com/#/definitions/devices)
@@ -143,14 +144,16 @@
             query_params["deviceClass"] = kwargs["deviceClass"]
         if "tagFilter" in kwargs:
             query_params["tagFilter"] = kwargs["tagFilter"]
         if "excludeConnectionInfo" in kwargs:
             query_params["excludeConnectionInfo"] = kwargs["excludeConnectionInfo"]
         if "parentId" in kwargs:
             query_params["parentId"] = kwargs["parentId"]
+        if "query" in kwargs:
+            query_params["query"] = json.dumps(kwargs["query"])
         if "losantdomain" in kwargs:
             headers["losantdomain"] = kwargs["losantdomain"]
         if "_actions" in kwargs:
             query_params["_actions"] = kwargs["_actions"]
         if "_links" in kwargs:
             query_params["_links"] = kwargs["_links"]
         if "_embedded" in kwargs:
```

### Comparing `losant-rest-1.9.2/losantrest/application_certificate.py` & `losant-rest-1.9.3/losantrest/application_certificate.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/integrations.py` & `losant-rest-1.9.3/losantrest/integrations.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_views.py` & `losant-rest-1.9.3/losantrest/experience_views.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/data_table_rows.py` & `losant-rest-1.9.3/losantrest/data_table_rows.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/audit_log.py` & `losant-rest-1.9.3/losantrest/audit_log.py`

 * *Files identical despite different names*

### Comparing `losant-rest-1.9.2/losantrest/experience_slugs.py` & `losant-rest-1.9.3/losantrest/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,109 +21,160 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 
 import json
 
-""" Module for Losant API ExperienceSlugs wrapper class """
+""" Module for Losant API Data wrapper class """
 # pylint: disable=C0301
 
-class ExperienceSlugs(object):
-    """ Class containing all the actions for the Experience Slugs Resource """
+class Data(object):
+    """ Class containing all the actions for the Data Resource """
 
     def __init__(self, client):
         self.client = client
 
-    def get(self, **kwargs):
+    def export(self, **kwargs):
         """
-        Returns the experience slugs for an application
+        Creates a csv file from a query of devices and attributes over a time range.
 
         Authentication:
         The client must be configured with a valid api
         access token to call this action. The token
         must include at least one of the following scopes:
-        all.Application, all.Application.read, all.Organization, all.Organization.read, all.User, all.User.read, experienceSlugs.*, or experienceSlugs.get.
+        all.Application, all.Application.read, all.Device, all.Device.read, all.Organization, all.Organization.read, all.User, all.User.read, data.*, or data.export.
 
         Parameters:
         *  {string} applicationId - ID associated with the application
+        *  {hash} query - The query parameters (https://api.losant.com/#/definitions/dataExport)
         *  {string} losantdomain - Domain scope of request (rarely needed)
         *  {boolean} _actions - Return resource actions in response
         *  {boolean} _links - Return resource link in response
         *  {boolean} _embedded - Return embedded resources in response
 
         Responses:
-        *  200 - Collection of experience slugs (https://api.losant.com/#/definitions/experienceSlugs)
+        *  200 - If command was successfully sent (https://api.losant.com/#/definitions/success)
 
         Errors:
         *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
         *  404 - Error if application was not found (https://api.losant.com/#/definitions/error)
         """
 
         query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
         path_params = {}
         headers = {}
         body = None
 
         if "applicationId" in kwargs:
             path_params["applicationId"] = kwargs["applicationId"]
+        if "query" in kwargs:
+            body = kwargs["query"]
         if "losantdomain" in kwargs:
             headers["losantdomain"] = kwargs["losantdomain"]
         if "_actions" in kwargs:
             query_params["_actions"] = kwargs["_actions"]
         if "_links" in kwargs:
             query_params["_links"] = kwargs["_links"]
         if "_embedded" in kwargs:
             query_params["_embedded"] = kwargs["_embedded"]
 
-        path = "/applications/{applicationId}/experience/slugs".format(**path_params)
+        path = "/applications/{applicationId}/data/export".format(**path_params)
 
-        return self.client.request("GET", path, params=query_params, headers=headers, body=body)
+        return self.client.request("POST", path, params=query_params, headers=headers, body=body)
+
+    def last_value_query(self, **kwargs):
+        """
+        Returns the last known data for the given attribute
+
+        Authentication:
+        The client must be configured with a valid api
+        access token to call this action. The token
+        must include at least one of the following scopes:
+        all.Application, all.Application.read, all.Device, all.Device.read, all.Organization, all.Organization.read, all.User, all.User.read, data.*, or data.lastValueQuery.
+
+        Parameters:
+        *  {string} applicationId - ID associated with the application
+        *  {hash} query - The query parameters (https://api.losant.com/#/definitions/lastValueQuery)
+        *  {string} losantdomain - Domain scope of request (rarely needed)
+        *  {boolean} _actions - Return resource actions in response
+        *  {boolean} _links - Return resource link in response
+        *  {boolean} _embedded - Return embedded resources in response
+
+        Responses:
+        *  200 - Last known data for the requested attribute (https://api.losant.com/#/definitions/lastValueData)
+
+        Errors:
+        *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
+        *  404 - Error if application was not found (https://api.losant.com/#/definitions/error)
+        """
+
+        query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
+        path_params = {}
+        headers = {}
+        body = None
+
+        if "applicationId" in kwargs:
+            path_params["applicationId"] = kwargs["applicationId"]
+        if "query" in kwargs:
+            body = kwargs["query"]
+        if "losantdomain" in kwargs:
+            headers["losantdomain"] = kwargs["losantdomain"]
+        if "_actions" in kwargs:
+            query_params["_actions"] = kwargs["_actions"]
+        if "_links" in kwargs:
+            query_params["_links"] = kwargs["_links"]
+        if "_embedded" in kwargs:
+            query_params["_embedded"] = kwargs["_embedded"]
+
+        path = "/applications/{applicationId}/data/last-value-query".format(**path_params)
+
+        return self.client.request("POST", path, params=query_params, headers=headers, body=body)
 
-    def post(self, **kwargs):
+    def time_series_query(self, **kwargs):
         """
-        Create a new experience slug for an application
+        Returns the data for the given query
 
         Authentication:
         The client must be configured with a valid api
         access token to call this action. The token
         must include at least one of the following scopes:
-        all.Application, all.Organization, all.User, experienceSlugs.*, or experienceSlugs.post.
+        all.Application, all.Application.read, all.Device, all.Device.read, all.Organization, all.Organization.read, all.User, all.User.read, data.*, or data.timeSeriesQuery.
 
         Parameters:
         *  {string} applicationId - ID associated with the application
-        *  {hash} experienceSlug - New experience slug information (https://api.losant.com/#/definitions/experienceSlugPost)
+        *  {hash} query - The query parameters (https://api.losant.com/#/definitions/timeSeriesQuery)
         *  {string} losantdomain - Domain scope of request (rarely needed)
         *  {boolean} _actions - Return resource actions in response
         *  {boolean} _links - Return resource link in response
         *  {boolean} _embedded - Return embedded resources in response
 
         Responses:
-        *  201 - Successfully created experience slug (https://api.losant.com/#/definitions/experienceSlug)
+        *  200 - Data for requested time range (https://api.losant.com/#/definitions/timeSeriesData)
 
         Errors:
         *  400 - Error if malformed request (https://api.losant.com/#/definitions/error)
         *  404 - Error if application was not found (https://api.losant.com/#/definitions/error)
         """
 
         query_params = {"_actions": "false", "_links": "true", "_embedded": "true"}
         path_params = {}
         headers = {}
         body = None
 
         if "applicationId" in kwargs:
             path_params["applicationId"] = kwargs["applicationId"]
-        if "experienceSlug" in kwargs:
-            body = kwargs["experienceSlug"]
+        if "query" in kwargs:
+            body = kwargs["query"]
         if "losantdomain" in kwargs:
             headers["losantdomain"] = kwargs["losantdomain"]
         if "_actions" in kwargs:
             query_params["_actions"] = kwargs["_actions"]
         if "_links" in kwargs:
             query_params["_links"] = kwargs["_links"]
         if "_embedded" in kwargs:
             query_params["_embedded"] = kwargs["_embedded"]
 
-        path = "/applications/{applicationId}/experience/slugs".format(**path_params)
+        path = "/applications/{applicationId}/data/time-series-query".format(**path_params)
 
         return self.client.request("POST", path, params=query_params, headers=headers, body=body)
```

