# Comparing `tmp/alertlogic-sdk-definitions-0.1.98.tar.gz` & `tmp/alertlogic-sdk-definitions-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertlogic-sdk-definitions-0.1.98.tar", last modified: Sat Nov 12 12:06:51 2022, max compression
+gzip compressed data, was "alertlogic-sdk-definitions-0.1.99.tar", last modified: Sun Nov 13 12:03:19 2022, max compression
```

## Comparing `alertlogic-sdk-definitions-0.1.98.tar` & `alertlogic-sdk-definitions-0.1.99.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.944395 alertlogic-sdk-definitions-0.1.98/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/.github/workflows/stage1_merge_automatic_prs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/.github/workflows/stage2_create_automatic_rel_tag.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/.github/workflows/stage3_release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/.github/workflows/stage4_release_gh_release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/.github/workflows/test_all.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/.travis.yml.defunct
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-12 12:06:51.000000 alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3074 2022-11-12 12:06:51.000000 alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 12:06:51.000000 alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 12:06:51.000000 alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-12 12:06:51.000000 alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-12 12:06:51.000000 alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/
--rw-r--r--   0 runner    (1001) docker     (121)    11533 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.944395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aecontent/
--rw-r--r--   0 runner    (1001) docker     (121)    28841 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aecontent/aecontent.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aefr/
--rw-r--r--   0 runner    (1001) docker     (121)    48923 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aefr/aefr.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aemanual/
--rw-r--r--   0 runner    (1001) docker     (121)     4895 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aemanual/aemanual.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aepublish/
--rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aepublish/aepublish.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aerta/
--rw-r--r--   0 runner    (1001) docker     (121)    30906 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aerta/aerta.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aetag/
--rw-r--r--   0 runner    (1001) docker     (121)    56728 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aetag/aetag.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aetuner/
--rw-r--r--   0 runner    (1001) docker     (121)    25770 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aetuner/aetuner.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aims/
--rw-r--r--   0 runner    (1001) docker     (121)   130603 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aims/aims.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.948395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/api/
--rw-r--r--   0 runner    (1001) docker     (121)  1022224 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/api/assets_manager.v1.html
--rw-r--r--   0 runner    (1001) docker     (121)    18539 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/assets_manager.v1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/examples.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/parameters.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/responses.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/schemas.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/
--rw-r--r--   0 runner    (1001) docker     (121)   152742 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/assets_query.v1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   181596 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/examples.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19738 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/parameters.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    49173 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/remediations.v1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8237 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/responses.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    37050 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/schemas.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/
--rw-r--r--   0 runner    (1001) docker     (121)    73342 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/assets_write.v1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    10818 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/examples.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/parameters.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     7287 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/responses.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    21045 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/schemas.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/cargo/
--rw-r--r--   0 runner    (1001) docker     (121)    11102 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/cargo/cargo.v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/connectors/
--rw-r--r--   0 runner    (1001) docker     (121)    53463 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/connectors/connectors.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/credentials/
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/credentials/credentials.v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/deployments/
--rw-r--r--   0 runner    (1001) docker     (121)    12932 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/deployments/deployments.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/endpoints/
--rw-r--r--   0 runner    (1001) docker     (121)     7183 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/endpoints/endpoints.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/herald/
--rw-r--r--   0 runner    (1001) docker     (121)    41343 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/herald/herald.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/ingest/
--rw-r--r--   0 runner    (1001) docker     (121)    27297 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/ingest/ingest.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/iris/
--rw-r--r--   0 runner    (1001) docker     (121)    58387 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/iris/iris.v3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/kalm/
--rw-r--r--   0 runner    (1001) docker     (121)     9081 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/kalm/kalm.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/notify/
--rw-r--r--   0 runner    (1001) docker     (121)    11888 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/notify/notify.v3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/otis/
--rw-r--r--   0 runner    (1001) docker     (121)    69312 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/otis/otis.v3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/policies/
--rw-r--r--   0 runner    (1001) docker     (121)     6066 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/policies/policies.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/
--rw-r--r--   0 runner    (1001) docker     (121)   153762 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/assets_query.v1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   183568 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/examples.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    19743 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/parameters.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    49173 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/remediations.v1.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8237 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/responses.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    37432 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/schemas.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/responder/
--rw-r--r--   0 runner    (1001) docker     (121)   169821 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/responder/responder.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/scan_scheduler/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.952395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/scan_scheduler/api/
--rw-r--r--   0 runner    (1001) docker     (121)  1124133 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/scan_scheduler/api/scheduler.v2.html
--rw-r--r--   0 runner    (1001) docker     (121)    49211 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/scan_scheduler/scheduler.v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/search/
--rw-r--r--   0 runner    (1001) docker     (121)    43825 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/search/search.v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (121)    15116 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/subscriptions/subscriptions.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/themis/
--rw-r--r--   0 runner    (1001) docker     (121)     9080 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/themis/themis.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/vulnerabilities/
--rw-r--r--   0 runner    (1001) docker     (121)    15496 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/vulnerabilities/vulnerabilities.v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/alsdkdefs/schema/
--rw-r--r--   0 runner    (1001) docker     (121)    26001 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/schema/openapi_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-12 12:06:51.000000 alertlogic-sdk-definitions-0.1.98/alsdkdefs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/doc/CI.puml
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/doc/automatic_releases.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/doc/images/
--rw-r--r--   0 runner    (1001) docker     (121)    35803 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/doc/images/CI.png
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1787 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/scripts/automerge.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     6421 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/scripts/create_release.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2212 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/scripts/validate_my_definition.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      798 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/scripts/validate_my_definition.sh
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 12:06:51.956395 alertlogic-sdk-definitions-0.1.98/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/tests/test_apis_validate.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-11-12 12:06:42.000000 alertlogic-sdk-definitions-0.1.98/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.147661 alertlogic-sdk-definitions-0.1.99/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1844 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/.github/workflows/stage1_merge_automatic_prs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/.github/workflows/stage2_create_automatic_rel_tag.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/.github/workflows/stage3_release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/.github/workflows/stage4_release_gh_release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/.github/workflows/test_all.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/.travis.yml.defunct
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-11-13 12:03:19.000000 alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3074 2022-11-13 12:03:19.000000 alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 12:03:19.000000 alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 12:03:19.000000 alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-13 12:03:19.000000 alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-13 12:03:19.000000 alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/
+-rw-r--r--   0 runner    (1001) docker     (121)    11533 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.151661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aecontent/
+-rw-r--r--   0 runner    (1001) docker     (121)    28841 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aecontent/aecontent.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aefr/
+-rw-r--r--   0 runner    (1001) docker     (121)    48923 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aefr/aefr.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aemanual/
+-rw-r--r--   0 runner    (1001) docker     (121)     4895 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aemanual/aemanual.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aepublish/
+-rw-r--r--   0 runner    (1001) docker     (121)     4331 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aepublish/aepublish.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aerta/
+-rw-r--r--   0 runner    (1001) docker     (121)    30906 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aerta/aerta.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aetag/
+-rw-r--r--   0 runner    (1001) docker     (121)    56728 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aetag/aetag.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aetuner/
+-rw-r--r--   0 runner    (1001) docker     (121)    25770 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aetuner/aetuner.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.155661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aims/
+-rw-r--r--   0 runner    (1001) docker     (121)   130603 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aims/aims.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.159661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.159661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (121)  1022224 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/api/assets_manager.v1.html
+-rw-r--r--   0 runner    (1001) docker     (121)    18539 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/assets_manager.v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2188 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/parameters.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/schemas.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.159661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/
+-rw-r--r--   0 runner    (1001) docker     (121)   153762 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/assets_query.v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   183568 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    19743 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/parameters.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    49173 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/remediations.v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8237 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    37432 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/schemas.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.159661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/
+-rw-r--r--   0 runner    (1001) docker     (121)    73342 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/assets_write.v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10818 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/parameters.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     7287 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    21045 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/schemas.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.159661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/cargo/
+-rw-r--r--   0 runner    (1001) docker     (121)    11102 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/cargo/cargo.v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.159661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/connectors/
+-rw-r--r--   0 runner    (1001) docker     (121)    53463 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/connectors/connectors.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/credentials/
+-rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/credentials/credentials.v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/deployments/
+-rw-r--r--   0 runner    (1001) docker     (121)    12932 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/deployments/deployments.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (121)     7183 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/endpoints/endpoints.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/herald/
+-rw-r--r--   0 runner    (1001) docker     (121)    41343 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/herald/herald.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/ingest/
+-rw-r--r--   0 runner    (1001) docker     (121)    27297 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/ingest/ingest.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/iris/
+-rw-r--r--   0 runner    (1001) docker     (121)    58387 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/iris/iris.v3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/kalm/
+-rw-r--r--   0 runner    (1001) docker     (121)     9081 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/kalm/kalm.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/notify/
+-rw-r--r--   0 runner    (1001) docker     (121)    11888 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/notify/notify.v3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/otis/
+-rw-r--r--   0 runner    (1001) docker     (121)    69312 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/otis/otis.v3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/policies/
+-rw-r--r--   0 runner    (1001) docker     (121)     6066 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/policies/policies.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/
+-rw-r--r--   0 runner    (1001) docker     (121)   153762 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/assets_query.v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   183568 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    19743 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/parameters.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    49173 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/remediations.v1.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8237 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    37432 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/schemas.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/responder/
+-rw-r--r--   0 runner    (1001) docker     (121)   169821 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/responder/responder.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/scan_scheduler/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.163661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/scan_scheduler/api/
+-rw-r--r--   0 runner    (1001) docker     (121)  1124133 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/scan_scheduler/api/scheduler.v2.html
+-rw-r--r--   0 runner    (1001) docker     (121)    49211 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/scan_scheduler/scheduler.v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/search/
+-rw-r--r--   0 runner    (1001) docker     (121)    43825 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/search/search.v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (121)    15116 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/subscriptions/subscriptions.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/themis/
+-rw-r--r--   0 runner    (1001) docker     (121)     9080 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/themis/themis.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/vulnerabilities/
+-rw-r--r--   0 runner    (1001) docker     (121)    15496 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/vulnerabilities/vulnerabilities.v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/alsdkdefs/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)    26001 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/schema/openapi_schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-13 12:03:18.000000 alertlogic-sdk-definitions-0.1.99/alsdkdefs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/doc/CI.puml
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/doc/automatic_releases.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    35803 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/doc/images/CI.png
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1787 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/scripts/automerge.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6421 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/scripts/create_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2212 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/scripts/validate_my_definition.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      798 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/scripts/validate_my_definition.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 12:03:19.167661 alertlogic-sdk-definitions-0.1.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/tests/test_apis_validate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2022-11-13 12:03:07.000000 alertlogic-sdk-definitions-0.1.99/tox.ini
```

### Comparing `alertlogic-sdk-definitions-0.1.98/.github/workflows/stage1_merge_automatic_prs.yml` & `alertlogic-sdk-definitions-0.1.99/.github/workflows/stage1_merge_automatic_prs.yml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/.github/workflows/stage2_create_automatic_rel_tag.yml` & `alertlogic-sdk-definitions-0.1.99/.github/workflows/stage2_create_automatic_rel_tag.yml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/.github/workflows/stage3_release_pypi.yml` & `alertlogic-sdk-definitions-0.1.99/.github/workflows/stage3_release_pypi.yml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/.github/workflows/stage4_release_gh_release.yml` & `alertlogic-sdk-definitions-0.1.99/.github/workflows/stage4_release_gh_release.yml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/.github/workflows/test_all.yml` & `alertlogic-sdk-definitions-0.1.99/.github/workflows/test_all.yml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/.gitignore` & `alertlogic-sdk-definitions-0.1.99/.gitignore`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/.travis.yml.defunct` & `alertlogic-sdk-definitions-0.1.99/.travis.yml.defunct`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/LICENSE` & `alertlogic-sdk-definitions-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/PKG-INFO` & `alertlogic-sdk-definitions-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertlogic-sdk-definitions
-Version: 0.1.98
+Version: 0.1.99
 Summary: The Alert Logic API definitions.
 Home-page: https://github.com/alertlogic/alertlogic-sdk-definitions
 Author: Alert Logic Inc.
 Author-email: devsupport@alertlogic.com
 License: MIT license
 Keywords: alcli,almdr,alsdkdefs,alertlogic,alertlogic-cli
 Platform: any
```

### Comparing `alertlogic-sdk-definitions-0.1.98/README.md` & `alertlogic-sdk-definitions-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/PKG-INFO` & `alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertlogic-sdk-definitions
-Version: 0.1.98
+Version: 0.1.99
 Summary: The Alert Logic API definitions.
 Home-page: https://github.com/alertlogic/alertlogic-sdk-definitions
 Author: Alert Logic Inc.
 Author-email: devsupport@alertlogic.com
 License: MIT license
 Keywords: alcli,almdr,alsdkdefs,alertlogic,alertlogic-cli
 Platform: any
```

### Comparing `alertlogic-sdk-definitions-0.1.98/alertlogic_sdk_definitions.egg-info/SOURCES.txt` & `alertlogic-sdk-definitions-0.1.99/alertlogic_sdk_definitions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/__init__.py` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/__init__.py`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aecontent/aecontent.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aecontent/aecontent.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aefr/aefr.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aefr/aefr.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aemanual/aemanual.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aemanual/aemanual.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aepublish/aepublish.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aepublish/aepublish.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aerta/aerta.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aerta/aerta.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aetag/aetag.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aetag/aetag.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aetuner/aetuner.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aetuner/aetuner.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/aims/aims.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/aims/aims.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/api/assets_manager.v1.html` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/api/assets_manager.v1.html`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/assets_manager.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/assets_manager.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/examples.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/examples.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/parameters.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/parameters.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_manager/schemas.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_manager/schemas.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/assets_query.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/assets_query.v1.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -424,14 +424,16 @@
       - $ref: 'parameters.yaml#/ParamQFields'
       - $ref: 'parameters.yaml#/ParamFilter'
       - $ref: 'parameters.yaml#/ParamFilterRelationship'
       - $ref: 'parameters.yaml#/ParamRelatedProperties'
       - $ref: 'parameters.yaml#/ParamTopoChain'
       - $ref: 'parameters.yaml#/ParamScopeBoolean'
       - $ref: 'parameters.yaml#/ParamIncludeAlertlogicSecurity'
+      - $ref: 'parameters.yaml#/ParamContinue'
+      - $ref: 'parameters.yaml#/ParamPageSize'
     get:
       operationId: query_assets
       summary: Query Assets for Account
       description: Return a list of related assets.
       tags:
         - Queries
       x-codeSamples:
@@ -466,14 +468,24 @@
             curl "https://api.cloudinsight.alertlogic.com/assets_query/v1/12345678/assets?asset_types=r:region&r..vpc=false" \
                  -H "x-aims-auth-token: $TOKEN" -H "accept: application/json"
         - lang: Shell
           label: Get account hosts that private IP address match given CIDR block
           source: |-
             curl "https://api.cloudinsight.alertlogic.com/assets_query/v1/12345678/assets?asset_types=h:host&h.private_ip_addresses=:cidr_match:192.168.0.0/16" \
                  -H "x-aims-auth-token: $TOKEN" -H "accept: application/json"
+        - lang: Shell
+          label: Get all assets for an account ID with pagination
+          source: |-
+            curl "https://api.cloudinsight.alertlogic.com/assets_query/v1/12345678/assets?page_size=10" \
+                 -H "x-aims-auth-token: $TOKEN" -H "accept: application/json"
+        - lang: Shell
+          label: Get all assets for an account ID with pagination (continue)
+          source: |-
+            curl "https://api.cloudinsight.alertlogic.com/assets_query/v1/12345678/assets?continue=EEBBD0DF-B927-411B-B771-247D4C96F9AC" \
+                 -H "x-aims-auth-token: $TOKEN" -H "accept: application/json"
       responses:
         "200":
           description: OK
           content:
             application/json:
               schema:
                 $ref: 'schemas.yaml#/QueryAssetsResponse'
@@ -492,14 +504,18 @@
                   $ref: 'examples.yaml#/QueryAssetsAssetTypesVPCSubnetHostInRegionExample'
                 asset_types=region & not related to a vpc:
                   $ref: 'examples.yaml#/QueryAssetsAssetTypesRegionNotRelatedToAVpcExample'
                 asset_types=host & ip_addresses match CIDR 192.168.0.0/16:
                   $ref: 'examples.yaml#/QueryAssetsAssetTypesHostCIDRMatchExample'
                 topo_chain=false:
                   $ref: 'examples.yaml#/QueryAssetsTopoChainFalseExample'
+                asset_types=any & page_size=5:
+                  $ref: 'examples.yaml#/QueryAssetsAssetTypesAnyWithPagination'
+                asset_types=any & continue=EEBBD0DF-B927-411B-B771-247D4C96F9AC:
+                  $ref: 'examples.yaml#/QueryAssetsAssetTypesAnyWithPaginationContinue'
         "400":
           $ref: 'responses.yaml#/QueryAssetsBadRequestError'
         "401":
           $ref: 'responses.yaml#/Unauthorized'
         "403":
           $ref: 'responses.yaml#/Forbidden'
         "404":
```

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/examples.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/examples.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,66 @@
           key: /aws/us-east-1/image/ami-abcdef01
           account_id: "12345678"
       - - deployment_id: CD7C26C3-FAA1-4AD1-86CB-9628ED1B3327
           type: subnet
           key: /aws/us-east-1/subnet/subnet-01020304
           account_id: "12345678"
     rows: 7
+QueryAssetsAssetTypesAnyWithPagination:
+  value:
+    assets:
+      - - deployment_id: 1C0EFEC8-7DBE-480D-A025-ECC13DE30AD5
+          type: host
+          key: /aws/us-east-1/host/i-1234abcd1234abcd
+          account_id: "12345678"
+      - - deployment_id: 9E4B8AAB-5E07-4B46-8E07-AA16D3CA1D03
+          type: subnet
+          key: /aws/us-east-1/subnet/subnet-abcd1234
+          account_id: "12345678"
+      - - deployment_id: CD7C26C3-FAA1-4AD1-86CB-9628ED1B3327
+          type: sg
+          key: /aws/us-east-1/sg/sg-1234abcd
+          account_id: "12345678"
+      - - deployment_id: 1C0EFEC8-7DBE-480D-A025-ECC13DE30AD5
+          type: image
+          key: /aws/us-east-1/image/ami-abcdef01
+          account_id: "12345678"
+      - - deployment_id: CD7C26C3-FAA1-4AD1-86CB-9628ED1B3327
+          type: subnet
+          key: /aws/us-east-1/subnet/subnet-01020304
+          account_id: "12345678"
+    rows: 5
+    continue: EEBBD0DF-B927-411B-B771-247D4C96F9AC
+    total_assets: 14
+QueryAssetsAssetTypesAnyWithPaginationContinue:
+  value:
+    assets:
+      - - deployment_id: 1C0EFEC8-7DBE-480D-A025-ECC13DE30AD5
+          type: host
+          key: /aws/us-east-1/host/i-1234abcd1234abcd
+          account_id: "12345678"
+      - - deployment_id: 9E4B8AAB-5E07-4B46-8E07-AA16D3CA1D03
+          type: subnet
+          key: /aws/us-east-1/subnet/subnet-abcd1234
+          account_id: "12345678"
+      - - deployment_id: CD7C26C3-FAA1-4AD1-86CB-9628ED1B3327
+          type: sg
+          key: /aws/us-east-1/sg/sg-1234abcd
+          account_id: "12345678"
+      - - deployment_id: 1C0EFEC8-7DBE-480D-A025-ECC13DE30AD5
+          type: image
+          key: /aws/us-east-1/image/ami-abcdef01
+          account_id: "12345678"
+      - - deployment_id: CD7C26C3-FAA1-4AD1-86CB-9628ED1B3327
+          type: subnet
+          key: /aws/us-east-1/subnet/subnet-01020304
+          account_id: "12345678"
+    rows: 5
+    continue: C446F70F-3E5F-465D-B743-69C28D06EF90
+    total_assets: 14
 FindAssetAgentByUuidExample:
   value:
     type: agent
     key: /agent/CD7C26C3-FAA1-4AD1-86CB-9628ED1B3327
     deployment_id: D155C4AA-3292-4C6A-8958-DE5CF318BEC9
     host_key: /aws/us-east-1/i-c764bf1fc87783f33
 FindAssetCollectorByUuidExample:
```

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/parameters.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/parameters.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -555,9 +555,9 @@
     returned.
 ParamPageSize:
   schema:
     type: integer
   in: query
   name: page_size
   description: |-
-    The number of results to be returned, default is 50. page_size is only valid
+    The number of results to be returned, maximum is 10000. `page_size` is only valid
     on initial calls to GET assets and will have no effect on subsequent calls.
```

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/remediations.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/remediations.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/responses.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/responses.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_query/schemas.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_query/schemas.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,24 @@
         type: array
         title: column
         items:
           $ref: '#/Asset'
     rows:
       type: integer
       title: the number of rows in the query response
+    continue:
+      type: string
+      title: |-
+        A UUID to be used for subsequent GET assets calls to get the next set of results. 
+        Only present when there are more rows to paginate through.
+    total_assets:
+      type: integer
+      title: |-
+        The total number of rows in the assets list. 
+        Only present when there are more rows to paginate through.
   required:
     - assets
     - rows
   x-examples:
     basic example:
       assets:
         - - deployment_id: 1C0EFEC8-7DBE-480D-A025-ECC13DE30AD5
```

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/assets_write.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/assets_write.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/examples.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/examples.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/parameters.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/parameters.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/responses.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/responses.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/assets_write/schemas.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/assets_write/schemas.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/cargo/cargo.v2.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/cargo/cargo.v2.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/connectors/connectors.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/connectors/connectors.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/credentials/credentials.v2.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/credentials/credentials.v2.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/deployments/deployments.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/deployments/deployments.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/endpoints/endpoints.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/endpoints/endpoints.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/herald/herald.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/herald/herald.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/ingest/ingest.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/ingest/ingest.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/iris/iris.v3.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/iris/iris.v3.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/kalm/kalm.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/kalm/kalm.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/notify/notify.v3.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/notify/notify.v3.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/otis/otis.v3.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/otis/otis.v3.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/policies/policies.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/policies/policies.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/assets_query.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/assets_query.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/examples.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/examples.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/parameters.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/parameters.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/remediations.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/remediations.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/responses.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/responses.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/remediations/schemas.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/remediations/schemas.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/responder/responder.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/responder/responder.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/scan_scheduler/api/scheduler.v2.html` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/scan_scheduler/api/scheduler.v2.html`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/scan_scheduler/scheduler.v2.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/scan_scheduler/scheduler.v2.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/search/search.v2.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/search/search.v2.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/subscriptions/subscriptions.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/subscriptions/subscriptions.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/themis/themis.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/themis/themis.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/apis/vulnerabilities/vulnerabilities.v1.yaml` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/apis/vulnerabilities/vulnerabilities.v1.yaml`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/alsdkdefs/schema/openapi_schema.json` & `alertlogic-sdk-definitions-0.1.99/alsdkdefs/schema/openapi_schema.json`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/doc/automatic_releases.md` & `alertlogic-sdk-definitions-0.1.99/doc/automatic_releases.md`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/doc/images/CI.png` & `alertlogic-sdk-definitions-0.1.99/doc/images/CI.png`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/scripts/automerge.sh` & `alertlogic-sdk-definitions-0.1.99/scripts/automerge.sh`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/scripts/create_release.py` & `alertlogic-sdk-definitions-0.1.99/scripts/create_release.py`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/scripts/validate_my_definition.py` & `alertlogic-sdk-definitions-0.1.99/scripts/validate_my_definition.py`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/scripts/validate_my_definition.sh` & `alertlogic-sdk-definitions-0.1.99/scripts/validate_my_definition.sh`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/setup.py` & `alertlogic-sdk-definitions-0.1.99/setup.py`

 * *Files identical despite different names*

### Comparing `alertlogic-sdk-definitions-0.1.98/tests/test_apis_validate.py` & `alertlogic-sdk-definitions-0.1.99/tests/test_apis_validate.py`

 * *Files identical despite different names*

