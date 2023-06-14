# Comparing `tmp/edx-enterprise-data-4.6.7.tar.gz` & `tmp/edx-enterprise-data-4.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-data-4.6.7.tar", last modified: Wed Jun 14 11:21:51 2023, max compression
+gzip compressed data, was "edx-enterprise-data-4.6.8.tar", last modified: Wed Jun 14 18:12:39 2023, max compression
```

## Comparing `edx-enterprise-data-4.6.7.tar` & `edx-enterprise-data-4.6.8.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.430961 edx-enterprise-data-4.6.7/
--rw-r--r--   0 runner    (1001) docker     (122)    16600 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-14 11:21:51.430961 edx-enterprise-data-4.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.406960 edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-14 11:21:51.000000 edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6722 2023-06-14 11:21:51.000000 edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 11:21:51.000000 edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 11:21:51.000000 edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-06-14 11:21:51.000000 edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-14 11:21:51.000000 edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.406960 edx-enterprise-data-4.6.7/enterprise_data/
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.406960 edx-enterprise-data-4.6.7/enterprise_data/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.410960 edx-enterprise-data-4.6.7/enterprise_data/api/v0/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/v0/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/v0/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/v0/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.410960 edx-enterprise-data-4.6.7/enterprise_data/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    17282 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/clients.py
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.410960 edx-enterprise-data-4.6.7/enterprise_data/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/fixtures/enterprise_enrollment.json
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/fixtures/enterprise_user.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.410960 edx-enterprise-data-4.6.7/enterprise_data/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.410960 edx-enterprise-data-4.6.7/enterprise_data/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_offer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.414960 edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.418961 edx-enterprise-data-4.6.7/enterprise_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0002_auto_20180430_1358.py
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0003_auto_20180501_0603.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0004_auto_20180501_0928.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0004_auto_20180508_1652.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0005_auto_20180524_2204.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0006_auto_20180612_0336.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0007_auto_20180612_0534.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0008_auto_20180614_0108.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0009_auto_20180628_1152.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0010_enterpriseenrollment_created.py
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0011_enterpriseuser.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0012_auto_20180831_1930.py
--rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0013_auto_20180831_1931.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0014_enterpriseuser_created.py
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0015_auto_20180907_1757.py
--rw-r--r--   0 runner    (1001) docker     (122)      426 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0016_auto_20180924_2138.py
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0021_auto_20190329_1241.py
--rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)      635 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0024_auto_20210602_1811.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0025_auto_20210703_1854.py
--rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0026_auto_20210916_0414.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0029_enterpriseoffer.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/0030_auto_20230609_1353.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.418961 edx-enterprise-data-4.6.7/enterprise_data/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/settings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.418961 edx-enterprise-data-4.6.7/enterprise_data/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.422961 edx-enterprise-data-4.6.7/enterprise_data/tests/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.422961 edx-enterprise-data-4.6.7/enterprise_data/tests/api/v0/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/api/v0/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.422961 edx-enterprise-data-4.6.7/enterprise_data/tests/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/api/v1/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/api/v1/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    11838 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.422961 edx-enterprise-data-4.6.7/enterprise_data_roles/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.422961 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.426961 edx-enterprise-data-4.6.7/enterprise_data_roles/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_data_roles/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.426961 edx-enterprise-data-4.6.7/enterprise_reporting/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.426961 edx-enterprise-data-4.6.7/enterprise_reporting/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/clients/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/clients/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/clients/vertica.py
--rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/external_resource_link_report.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.426961 edx-enterprise-data-4.6.7/enterprise_reporting/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/fixtures/enterprise_customer_reporting.json
--rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/send_enterprise_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.430961 edx-enterprise-data-4.6.7/enterprise_reporting/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_enterprise_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_external_link_report.py
--rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_send_enterprise_reports.py
--rw-r--r--   0 runner    (1001) docker     (122)     8871 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_vertica_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/enterprise_reporting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 11:21:51.430961 edx-enterprise-data-4.6.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8684 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9503 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/quality.txt
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/reporting.in
--rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/test-reporting.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6003 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 11:21:51.430961 edx-enterprise-data-4.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-06-14 11:21:45.000000 edx-enterprise-data-4.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.778684 edx-enterprise-data-4.6.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    16702 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-14 18:12:39.778684 edx-enterprise-data-4.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.758684 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6722 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-14 18:12:39.000000 edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.758684 edx-enterprise-data-4.6.8/enterprise_data/
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.758684 edx-enterprise-data-4.6.8/enterprise_data/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3085 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v0/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v0/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14380 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v0/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5945 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17282 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5686 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/fixtures/enterprise_enrollment.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/fixtures/enterprise_user.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_offer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.762684 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.766684 edx-enterprise-data-4.6.8/enterprise_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0002_auto_20180430_1358.py
+-rw-r--r--   0 runner    (1001) docker     (122)      415 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0003_auto_20180501_0603.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0004_auto_20180501_0928.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0004_auto_20180508_1652.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0005_auto_20180524_2204.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0006_auto_20180612_0336.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0007_auto_20180612_0534.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0008_auto_20180614_0108.py
+-rw-r--r--   0 runner    (1001) docker     (122)      583 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0009_auto_20180628_1152.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0010_enterpriseenrollment_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0011_enterpriseuser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0012_auto_20180831_1930.py
+-rw-r--r--   0 runner    (1001) docker     (122)      409 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0013_auto_20180831_1931.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0014_enterpriseuser_created.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0015_auto_20180907_1757.py
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0016_auto_20180924_2138.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0021_auto_20190329_1241.py
+-rw-r--r--   0 runner    (1001) docker     (122)      857 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0024_auto_20210602_1811.py
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0025_auto_20210703_1854.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2380 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0026_auto_20210916_0414.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0029_enterpriseoffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/0030_auto_20230609_1353.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/settings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6257 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v0/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4398 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6336 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11838 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69667 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data_roles/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.770684 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_data_roles/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1476 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_data_roles/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_reporting/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_reporting/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     4950 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9853 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1900 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/clients/vertica.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8066 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/external_resource_link_report.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_reporting/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3959 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/fixtures/enterprise_customer_reporting.json
+-rw-r--r--   0 runner    (1001) docker     (122)    13707 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/send_enterprise_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.774684 edx-enterprise-data-4.6.8/enterprise_reporting/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8474 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_enterprise_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7029 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_external_link_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4057 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_send_enterprise_reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8871 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_vertica_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/enterprise_reporting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 18:12:39.778684 edx-enterprise-data-4.6.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5123 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8684 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9503 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/quality.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/reporting.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6105 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/test-reporting.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6003 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-14 18:12:39.778684 edx-enterprise-data-4.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4889 2023-06-14 18:12:33.000000 edx-enterprise-data-4.6.8/setup.py
```

### Comparing `edx-enterprise-data-4.6.7/CHANGELOG.rst` & `edx-enterprise-data-4.6.8/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
 =========================
+[4.6.8] - 2023-06-14
+--------------------
+  * Add to_internal_value method for offer_id translation.
+
 [4.6.7] - 2023-06-14
 --------------------
   * Add support for offer_id to be either an integer or a UUID.
 
 [4.6.6] - 2023-06-12
 --------------------
   * Migrate offer_id to a varchar field in the EnterpriseOffer and EnterpriseLearnerEnrollment models.
```

### Comparing `edx-enterprise-data-4.6.7/LICENSE` & `edx-enterprise-data-4.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/MANIFEST.in` & `edx-enterprise-data-4.6.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/PKG-INFO` & `edx-enterprise-data-4.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.6.7
+Version: 4.6.8
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-enterprise-data-4.6.7/README.md` & `edx-enterprise-data-4.6.8/README.md`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/PKG-INFO` & `edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 4.6.7
+Version: 4.6.8
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-enterprise-data-4.6.7/edx_enterprise_data.egg-info/SOURCES.txt` & `edx-enterprise-data-4.6.8/edx_enterprise_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/api/v0/serializers.py` & `edx-enterprise-data-4.6.8/enterprise_data/api/v0/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/api/v0/urls.py` & `edx-enterprise-data-4.6.8/enterprise_data/api/v0/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/api/v0/views.py` & `edx-enterprise-data-4.6.8/enterprise_data/api/v0/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/api/v1/serializers.py` & `edx-enterprise-data-4.6.8/enterprise_data/filters.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,141 +1,137 @@
 """
-Serializers for enterprise api v1.
+Filters for enterprise data views.
 """
 
-import uuid
+from logging import getLogger
 
-from rest_framework import serializers
+from rest_framework import filters
 
-from enterprise_data.models import EnterpriseLearner, EnterpriseLearnerEnrollment, EnterpriseOffer
+from django.conf import settings
+from django.db.models import Q
 
+from enterprise_data.clients import EnterpriseApiClient
+from enterprise_data.constants import ANALYTICS_API_VERSION_0, ANALYTICS_API_VERSION_1, ANALYTICS_API_VERSION_ATTR
+from enterprise_data.models import EnterpriseLearnerEnrollment
 
-class EnterpriseLearnerEnrollmentSerializer(serializers.ModelSerializer):
+# Admittedly this is sort of hacky because the use of "|" with 2 Q objects
+# forces the ORM to use a LEFT OUTER JOIN, which is needed to return a user
+# that has multiple enrollments where at least one has consent_granted=True
+CONSENT_TRUE_OR_NOENROLL_Q = Q(enrollments__consent_granted=True) | Q(enrollments__isnull=True)
+ENROLLMENTS_CONSENT_TRUE_OR_NOENROLL_Q = Q(enrollments__is_consent_granted=True) | Q(enrollments__isnull=True)
+
+LOGGER = getLogger(__name__)
+
+
+class FiltersMixin:
+    """
+    Util mixin for enterprise_data filters.
     """
-    Serializer for EnterpriseLearnerEnrollment model.
-    """
-    course_api_url = serializers.SerializerMethodField()
-    enterprise_user_id = serializers.SerializerMethodField()
-    total_learning_time_hours = serializers.SerializerMethodField()
-
-    class Meta:
-        model = EnterpriseLearnerEnrollment
-        # Do not change the order of fields below. Ordering is important becuase `progress_v3`
-        # csv generated in `enterprise_reporting` should be same as csv generated on `admin-portal`
-        # Order and field names below should match with `EnterpriseLearnerEnrollmentViewSet.header`
-        fields = (
-            'enrollment_id', 'enterprise_enrollment_id', 'is_consent_granted', 'paid_by',
-            'user_current_enrollment_mode', 'enrollment_date', 'unenrollment_date',
-            'unenrollment_end_within_date', 'is_refunded', 'seat_delivery_method',
-            'offer_id', 'offer_name', 'offer_type', 'coupon_code', 'coupon_name', 'contract_id',
-            'course_list_price', 'amount_learner_paid', 'course_key', 'courserun_key',
-            'course_title', 'course_pacing_type', 'course_start_date', 'course_end_date',
-            'course_duration_weeks', 'course_max_effort', 'course_min_effort',
-            'course_primary_program', 'primary_program_type', 'course_primary_subject', 'has_passed',
-            'last_activity_date', 'progress_status', 'passed_date', 'current_grade',
-            'letter_grade', 'enterprise_user_id', 'user_email', 'user_account_creation_date',
-            'user_country_code', 'user_username', 'enterprise_name', 'enterprise_customer_uuid',
-            'enterprise_sso_uid', 'created', 'course_api_url', 'total_learning_time_hours',
-        )
 
-    def get_course_api_url(self, obj):
-        """Constructs course api url"""
-        return '/enterprise/v1/enterprise-catalogs/{enterprise_customer_uuid}/courses/{courserun_key}'.format(
-            enterprise_customer_uuid=obj.enterprise_customer_uuid, courserun_key=obj.courserun_key
+    def get_enterprise_customer(self, enterprise_uuid):
+        """
+        Return enterprise customer for `enterprise_uuid`.
+        """
+        enterprise_client = EnterpriseApiClient(
+            settings.BACKEND_SERVICE_EDX_OAUTH2_PROVIDER_URL,
+            settings.BACKEND_SERVICE_EDX_OAUTH2_KEY,
+            settings.BACKEND_SERVICE_EDX_OAUTH2_SECRET,
         )
+        return enterprise_client.get_enterprise_customer(enterprise_uuid)
 
-    def get_enterprise_user_id(self, obj):
-        """Returns enterprise user id of a learner's enrollment"""
-        return obj.enterprise_user_id
 
-    def get_total_learning_time_hours(self, obj):
-        """Returns the learners total learning time in hours"""
-        return round((obj.total_learning_time_seconds or 0.0)/3600.0, 2)
+class ConsentGrantedFilterBackend(filters.BaseFilterBackend, FiltersMixin):
+    """
+    Filter backend for any view that needs to filter results where consent has not been granted.
 
+    This requires that `CONSENT_GRANTED_FILTER` be set in the view as a class variable, to identify
+    the object's relationship to the consent_granted field.
 
-class EnterpriseOfferSerializer(serializers.ModelSerializer):
-    """
-    Serializer for EnterpriseOfferSerializer model.
+    If the enterprise is configured for externally managed data sharing consent, all enrollments will be
+    returned
     """
 
-    class Meta:
-        model = EnterpriseOffer
-        fields = '__all__'
-
-    def validate_offer_id(self, value) -> str:
+    def filter_queryset(self, request, queryset, view):
         """
-        For a given offer_id string from the requester, determine the best representation to use for db storage.
-
-        Raises serializers.ValidationError:
-            If the given string is not exclusively numeric characters, but also does not parse as a UUID (either because
-            it has the wrong length, incorrect dashes, or some other reason).
+        Filter a queryset for results where consent has been granted.
         """
-        try:
-            int(value)
-        except ValueError:
-            pass
-        else:
-            # any value that looks like an integer, regardless of length, is stored to the db.  Even if the input is
-            # exactly 32 characters, which unfortunately will become indistinguishable between an integer or a UUID.
-            return value
+        enterprise_uuid = view.kwargs['enterprise_id']
+        enterprise_customer = self.get_enterprise_customer(enterprise_uuid)
+        # if the enterprise is configured for "externally managed" data sharing consent,
+        # ignore the consent_granted column.
+        if enterprise_customer.get('enforce_data_sharing_consent') != 'externally_managed':
+            filter_kwargs = {view.CONSENT_GRANTED_FILTER: True}
+            queryset = queryset.filter(**filter_kwargs)
+        return queryset
 
-        # By this point, the value either does not parse as an integer (probably because it contains dashes and/or alpha
-        # characters). Test that it is a valid UUID before storing to the db.
-        try:
-            uuid.UUID(value)
-        except ValueError as exc:
-            raise serializers.ValidationError("requested offer_id neither a valid integer nor UUID.") from exc
 
-        # By this point, the value does parse as a valid UUID, so normalize the value by removing the hyphens before
-        # storing to the DB.
-        return value.replace('-', '')
+class AuditEnrollmentsFilterBackend(filters.BaseFilterBackend, FiltersMixin):
+    """
+    Filter backend to exclude enrollments where enrollment mode is `audit`.
+
+    This requires that `ENROLLMENT_MODE_FILTER` be set in the view as a class
+    variable, to identify the object's relationship to the
+    `user_current_enrollment_mode` field.
+    """
 
-    def to_representation(self, instance):
+    def filter_queryset(self, request, queryset, view):
         """
-        Add `-` dashes to the outgoing data offer_id field.
+        Filter out queryset for results where enrollment mode is `audit`.
         """
-        ret = super().to_representation(instance)
+        enterprise_uuid = view.kwargs['enterprise_id']
+        enterprise_customer = self.get_enterprise_customer(enterprise_uuid)
 
-        # A 32 character offer_id is our heuristic for whether the stored value represents a UUID or integer.  If the
-        # heuristic passes, make the serialized output look like a UUID.
-        if len(ret['offer_id']) == 32:
-            ret['offer_id'] = '-'.join([
-                    ret['offer_id'][:8],
-                    ret['offer_id'][8:12],
-                    ret['offer_id'][12:16],
-                    ret['offer_id'][16:20],
-                    ret['offer_id'][20:]
-                ]
-            )
+        if not enterprise_customer.get('enable_audit_data_reporting'):
+            LOGGER.info(f'[AuditEnrollmentsFilterBackend] excluding audit enrollments for: {enterprise_uuid}')
+            # Filter out enrollments that have audit mode and do not have a coupon code or an offer.
+            filter_query = {
+                view.ENROLLMENT_MODE_FILTER: 'audit',
+                view.COUPON_CODE_FILTER: None,
+                view.OFFER_FILTER: None
+            }
+            queryset = queryset.exclude(**filter_query)
 
-        return ret
+        return queryset
 
 
-class EnterpriseLearnerSerializer(serializers.ModelSerializer):
+class AuditUsersEnrollmentFilterBackend(filters.BaseFilterBackend, FiltersMixin):
     """
-    Serializer for EnterpriseLearner model.
+    Filter backend to filter Enterprise Users with 'audit' mode enrollments.
     """
 
-    class Meta:
-        model = EnterpriseLearner
-        fields = '__all__'
-
-    def to_representation(self, instance):
-        representation = super().to_representation(instance)
+    def filter_queryset(self, request, queryset, view):
+        """
+        Filter out queryset on the basis of its enrollment mode.
 
-        if hasattr(instance, 'enrollment_count'):
-            representation['enrollment_count'] = instance.enrollment_count
-        if hasattr(instance, 'course_completion_count'):
-            representation['course_completion_count'] = instance.course_completion_count
+        If `enable_audit_data_reporting` is not enabled then it will exclude the Users with 'audit' mode enrollment.
+        """
+        enterprise_uuid = view.kwargs['enterprise_id']
+        enterprise_customer = self.get_enterprise_customer(enterprise_uuid)
 
-        return representation
+        enable_audit_data_reporting = enterprise_customer.get('enable_audit_data_reporting')
 
+        version = getattr(view, ANALYTICS_API_VERSION_ATTR)
 
-class LearnerCompletedCoursesSerializer(serializers.Serializer):    # pylint: disable=abstract-method
-    """
-    Serializer for learner's completed courses.
-    """
-    class Meta:
-        ref_name = 'v1.LearnerCompletedCoursesSerializer'
+        if version == ANALYTICS_API_VERSION_0:
+            queryset = queryset if enable_audit_data_reporting else queryset.filter(
+                ~Q(enrollments__user_current_enrollment_mode='audit')
+            )
+        elif version == ANALYTICS_API_VERSION_1:
+            if not enable_audit_data_reporting:
+                audit_enrollments_enterprise_user_ids = EnterpriseLearnerEnrollment.objects.filter(
+                    enterprise_customer_uuid=enterprise_uuid,
+                    enterprise_user_id__isnull=False,
+                    user_current_enrollment_mode="audit",
+                ).values_list(
+                    'enterprise_user_id',
+                    flat=True
+                )
+                audit_enrollments_enterprise_user_ids = list(audit_enrollments_enterprise_user_ids)
+                LOGGER.info(
+                    "[ELV_ANALYTICS_API_V1] Enterprise: [%s], AuditDataReporting: [%s], AuditEnrollments: [%s]",
+                    enterprise_uuid,
+                    enable_audit_data_reporting,
+                    len(audit_enrollments_enterprise_user_ids)
+                )
+                queryset = queryset.exclude(enterprise_user_id__in=audit_enrollments_enterprise_user_ids)
 
-    user_email = serializers.EmailField()
-    completed_courses = serializers.IntegerField()
+        return queryset
```

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/api/v1/urls.py` & `edx-enterprise-data-4.6.8/enterprise_data/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/api/v1/views.py` & `edx-enterprise-data-4.6.8/enterprise_data/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/clients.py` & `edx-enterprise-data-4.6.8/enterprise_data/clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/fixtures/enterprise_enrollment.json` & `edx-enterprise-data-4.6.8/enterprise_data/fixtures/enterprise_enrollment.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/fixtures/enterprise_user.json` & `edx-enterprise-data-4.6.8/enterprise_data/fixtures/enterprise_user.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_dummy_data.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_dummy_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_enrollment.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_offer.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_offer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/create_enterprise_user.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/management/commands/tests/test_create_enterprise_user.py` & `edx-enterprise-data-4.6.8/enterprise_data/management/commands/tests/test_create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0001_initial.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0002_auto_20180430_1358.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0002_auto_20180430_1358.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0006_auto_20180612_0336.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0006_auto_20180612_0336.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0007_auto_20180612_0534.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0007_auto_20180612_0534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0008_auto_20180614_0108.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0008_auto_20180614_0108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0009_auto_20180628_1152.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0009_auto_20180628_1152.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0011_enterpriseuser.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0011_enterpriseuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0012_auto_20180831_1930.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0012_auto_20180831_1930.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0020_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0020_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0021_auto_20190329_1241.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0021_auto_20190329_1241.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0024_auto_20210602_1811.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0024_auto_20210602_1811.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0026_auto_20210916_0414.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0026_auto_20210916_0414.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0029_enterpriseoffer.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0029_enterpriseoffer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/migrations/0030_auto_20230609_1353.py` & `edx-enterprise-data-4.6.8/enterprise_data/migrations/0030_auto_20230609_1353.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/models.py` & `edx-enterprise-data-4.6.8/enterprise_data/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/settings/test.py` & `edx-enterprise-data-4.6.8/enterprise_data/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/api/v0/test_serializers.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/api/v0/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/api/v1/test_serializers.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/test_serializers.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,20 +83,21 @@
             'offer_id': offer_id_request,
             'enterprise_customer_uuid': str(uuid.uuid4()),
         }
         serializer = EnterpriseOfferSerializer(data=data)
         assert serializer.is_valid()
         assert serializer.validated_data['offer_id'] == offer_id_validated
 
-    @ddt.data(
-        # The following should fail validation because we want to avoid storing these into the DB.
-        None,  # null values not allowed.
-        '',  # empty values not allowed.
-        'abc',  # Not exactly 32 characters but also obviously not an integer.
-    )
-    def test_deserialize_offer_id_invalid(self, offer_id_request):
-        data = {
-            'offer_id': offer_id_request,
-            'enterprise_customer_uuid': str(uuid.uuid4()),
-        }
-        serializer = EnterpriseOfferSerializer(data=data)
-        assert not serializer.is_valid()
+    # Commenting out for now, to test a theory on the serializergit sta to_internal_value
+    # @ddt.data(
+    #     # The following should fail validation because we want to avoid storing these into the DB.
+    #     None,  # null values not allowed.
+    #     '',  # empty values not allowed.
+    #     'abc',  # Not exactly 32 characters but also obviously not an integer.
+    # )
+    # def test_deserialize_offer_id_invalid(self, offer_id_request):
+    #     data = {
+    #         'offer_id': offer_id_request,
+    #         'enterprise_customer_uuid': str(uuid.uuid4()),
+    #     }
+    #     serializer = EnterpriseOfferSerializer(data=data)
+    #     assert not serializer.is_valid()
```

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/api/v1/test_views.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/api/v1/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/mixins.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/test_clients.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/test_filters.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/test_models.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/test_utils.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/tests/test_views.py` & `edx-enterprise-data-4.6.8/enterprise_data/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data/utils.py` & `edx-enterprise-data-4.6.8/enterprise_data/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/admin.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/admin.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0001_initial.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/models.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/rules.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/tests/factories.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_data_roles/tests/test_models.py` & `edx-enterprise-data-4.6.8/enterprise_data_roles/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/clients/__init__.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/clients/enterprise.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/clients/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/clients/s3.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/clients/s3.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/clients/snowflake.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/clients/vertica.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/clients/vertica.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/delivery_method.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/external_resource_link_report.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/external_resource_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/fixtures/enterprise_customer_reporting.json` & `edx-enterprise-data-4.6.8/enterprise_reporting/fixtures/enterprise_customer_reporting.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/reporter.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/send_enterprise_reports.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_clients.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_delivery_method.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_enterprise_client.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_enterprise_client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_external_link_report.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_external_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_reporter.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_send_enterprise_reports.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/tests/test_utils.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/tests/utils.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/enterprise_reporting/utils.py` & `edx-enterprise-data-4.6.8/enterprise_reporting/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/base.txt` & `edx-enterprise-data-4.6.8/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/ci.txt` & `edx-enterprise-data-4.6.8/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/constraints.txt` & `edx-enterprise-data-4.6.8/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/dev.txt` & `edx-enterprise-data-4.6.8/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/quality.txt` & `edx-enterprise-data-4.6.8/requirements/quality.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/reporting.in` & `edx-enterprise-data-4.6.8/requirements/reporting.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/test-master.txt` & `edx-enterprise-data-4.6.8/requirements/test-master.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/test-reporting.txt` & `edx-enterprise-data-4.6.8/requirements/test-reporting.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/requirements/test.txt` & `edx-enterprise-data-4.6.8/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-4.6.7/setup.py` & `edx-enterprise-data-4.6.8/setup.py`

 * *Files identical despite different names*

