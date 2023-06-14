# Comparing `tmp/djangoldp-2.1.8.tar.gz` & `tmp/djangoldp-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp-2.1.8.tar", last modified: Wed Apr 14 13:59:13 2021, max compression
+gzip compressed data, was "dist/djangoldp-2.1.9.tar", last modified: Fri Apr 23 15:12:59 2021, max compression
```

## Comparing `djangoldp-2.1.8.tar` & `djangoldp-2.1.9.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1011 2021-04-14 13:59:13.000000 djangoldp-2.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2277 2021-04-14 13:58:53.000000 djangoldp-2.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       75 2021-04-14 13:58:53.000000 djangoldp-2.1.8/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp_crypto/
--rw-rw-rw-   0 root         (0) root         (0)      902 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp_crypto/models.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp_crypto/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp_crypto/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      685 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp_crypto/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp_crypto/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp_crypto/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp_crypto/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      804 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp_crypto/management/commands/creatersakey.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp_crypto/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp_crypto/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp_crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2021-04-14 13:58:53.000000 djangoldp-2.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/
--rw-rw-rw-   0 root         (0) root         (0)    39434 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)    18319 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/models.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/conf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/conf/package_template/
--rw-rw-rw-   0 root         (0) root         (0)      374 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       17 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/
--rw-rw-rw-   0 root         (0) root         (0)      114 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/apps.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      220 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/models.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      143 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/views.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       60 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/tests.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       33 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/admin.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      262 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      184 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       22 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/app_name/__init__.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       81 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/package_template/setup.py-tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/conf/server_template/
--rwxrwxrwx   0 root         (0) root         (0)      816 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/server_template/manage.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      367 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/server_template/settings.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/conf/server_template/server/
--rw-rw-rw-   0 root         (0) root         (0)      598 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/server_template/server/wsgi.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)     1002 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/server_template/server/urls.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/server_template/server/__init__.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)     4311 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     4839 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/ldpsettings.py
--rw-rw-rw-   0 root         (0) root         (0)        1 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/activities/
--rw-rw-rw-   0 root         (0) root         (0)     5050 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/activities/objects.py
--rw-rw-rw-   0 root         (0) root         (0)    28065 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/activities/services.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/activities/verbs.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/activities/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/activities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8560 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)     3043 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/endpoints/webfinger.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30033 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/views.py
--rw-rw-rw-   0 root         (0) root         (0)     2594 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/related.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     5144 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     2327 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_sources.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)    28591 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_update.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/performance_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     7962 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_guardian.py
--rw-rw-rw-   0 root         (0) root         (0)    18514 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_user_permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/tests/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1753 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/scripts/prod_data_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2153 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/scripts/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1098 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/scripts/test_data_generator.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/tests/dummy/
--rw-rw-rw-   0 root         (0) root         (0)      241 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/dummy/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/dummy/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/dummy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      610 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_delete.py
--rw-rw-rw-   0 root         (0) root         (0)     2940 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_ldp_viewset.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_auto_author.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_performance.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)    11970 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_get.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1528 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_anonymous_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     5796 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_perf_get.py
--rw-rw-rw-   0 root         (0) root         (0)    18691 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_backlinks_service.py
--rw-rw-rw-   0 root         (0) root         (0)    11634 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/settings_default.py
--rw-rw-rw-   0 root         (0) root         (0)    27419 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_inbox.py
--rw-rw-rw-   0 root         (0) root         (0)    36950 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_model_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2821 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/tests_ldp_model.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/tests/djangoldp_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      773 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0007_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0011_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0003_auto_20190911_0931.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0012_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0008_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0010_follower.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0002_auto_20190906_0642.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0005_auto_20200221_1127.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0006_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0004_auto_20200221_1118.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0015_auto_20210125_1847.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0013_auto_20200624_1709.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0014_auto_20200909_2206.py
--rw-rw-rw-   0 root         (0) root         (0)      601 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/0009_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/pagination.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     2474 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/management/commands/federate.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/management/commands/mock_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/management/commands/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/management/commands/configure.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/management/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2933 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2021-04-14 13:58:53.000000 djangoldp-2.1.8/djangoldp/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2021-04-14 13:59:07.000000 djangoldp-2.1.8/djangoldp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      339 2021-04-14 13:59:13.000000 djangoldp-2.1.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      304 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       50 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     4228 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      339 2021-04-14 13:59:13.000000 djangoldp-2.1.8/djangoldp.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2021-04-23 15:12:59.000000 djangoldp-2.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2021-04-23 15:12:39.000000 djangoldp-2.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       75 2021-04-23 15:12:39.000000 djangoldp-2.1.9/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp_crypto/
+-rw-rw-rw-   0 root         (0) root         (0)      902 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp_crypto/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp_crypto/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp_crypto/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/management/commands/creatersakey.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/management/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp_crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2021-04-23 15:12:39.000000 djangoldp-2.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/
+-rw-rw-rw-   0 root         (0) root         (0)    39434 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)    18319 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/package_template/
+-rw-rw-rw-   0 root         (0) root         (0)      374 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       17 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/apps.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      220 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/models.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      143 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/views.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       60 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/tests.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       33 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/admin.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      262 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      184 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       22 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/app_name/__init__.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       81 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/package_template/setup.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/server_template/
+-rwxrwxrwx   0 root         (0) root         (0)      816 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/manage.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      367 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/settings.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/conf/server_template/server/
+-rw-rw-rw-   0 root         (0) root         (0)      598 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/server/wsgi.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/server/urls.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/server_template/server/__init__.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)     4311 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4839 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/ldpsettings.py
+-rw-rw-rw-   0 root         (0) root         (0)        1 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/activities/
+-rw-rw-rw-   0 root         (0) root         (0)     5050 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    28065 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/verbs.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/activities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8560 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/endpoints/webfinger.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30033 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     2594 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/related.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     5144 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2327 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_sources.py
+-rw-rw-rw-   0 root         (0) root         (0)    11559 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    28591 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/performance_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     7962 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_guardian.py
+-rw-rw-rw-   0 root         (0) root         (0)    18514 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_user_permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/tests/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/scripts/prod_data_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2153 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/scripts/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/scripts/test_data_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/tests/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)      241 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/dummy/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/dummy/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/dummy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      610 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     2940 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_ldp_viewset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_auto_author.py
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_performance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    11970 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_anonymous_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5796 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_perf_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    18691 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_backlinks_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    11634 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/settings_default.py
+-rw-rw-rw-   0 root         (0) root         (0)    28823 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_inbox.py
+-rw-rw-rw-   0 root         (0) root         (0)    36950 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_model_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/tests_ldp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/tests/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      773 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0007_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0011_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0003_auto_20190911_0931.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0012_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0008_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0010_follower.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0002_auto_20190906_0642.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0005_auto_20200221_1127.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0006_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0004_auto_20200221_1118.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0015_auto_20210125_1847.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0013_auto_20200624_1709.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0014_auto_20200909_2206.py
+-rw-rw-rw-   0 root         (0) root         (0)      601 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/0009_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/pagination.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)     2474 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/federate.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/mock_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/management/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2933 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2021-04-23 15:12:39.000000 djangoldp-2.1.9/djangoldp/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2021-04-23 15:12:52.000000 djangoldp-2.1.9/djangoldp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      339 2021-04-23 15:12:59.000000 djangoldp-2.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      304 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     4228 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      339 2021-04-23 15:12:59.000000 djangoldp-2.1.9/djangoldp.egg-info/PKG-INFO
```

### Comparing `djangoldp-2.1.8/setup.cfg` & `djangoldp-2.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/README.md` & `djangoldp-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp_crypto/models.py` & `djangoldp-2.1.9/djangoldp_crypto/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp_crypto/migrations/0001_initial.py` & `djangoldp-2.1.9/djangoldp_crypto/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp_crypto/management/commands/creatersakey.py` & `djangoldp-2.1.9/djangoldp_crypto/management/commands/creatersakey.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/serializers.py` & `djangoldp-2.1.9/djangoldp/serializers.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/models.py` & `djangoldp-2.1.9/djangoldp/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/utils.py` & `djangoldp-2.1.9/djangoldp/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/conf/server_template/manage.py-tpl` & `djangoldp-2.1.9/djangoldp/conf/server_template/manage.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/conf/server_template/server/wsgi.py-tpl` & `djangoldp-2.1.9/djangoldp/conf/server_template/server/wsgi.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/conf/server_template/server/urls.py-tpl` & `djangoldp-2.1.9/djangoldp/conf/server_template/server/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/conf/default_settings.py` & `djangoldp-2.1.9/djangoldp/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/conf/ldpsettings.py` & `djangoldp-2.1.9/djangoldp/conf/ldpsettings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/apps.py` & `djangoldp-2.1.9/djangoldp/apps.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/activities/objects.py` & `djangoldp-2.1.9/djangoldp/activities/objects.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/activities/services.py` & `djangoldp-2.1.9/djangoldp/activities/services.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/activities/verbs.py` & `djangoldp-2.1.9/djangoldp/activities/verbs.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/permissions.py` & `djangoldp-2.1.9/djangoldp/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/endpoints/webfinger.py` & `djangoldp-2.1.9/djangoldp/endpoints/webfinger.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/views.py` & `djangoldp-2.1.9/djangoldp/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/related.py` & `djangoldp-2.1.9/djangoldp/related.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/check_integrity.py` & `djangoldp-2.1.9/djangoldp/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/admin.py` & `djangoldp-2.1.9/djangoldp/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_sources.py` & `djangoldp-2.1.9/djangoldp/tests/tests_sources.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/models.py` & `djangoldp-2.1.9/djangoldp/tests/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_update.py` & `djangoldp-2.1.9/djangoldp/tests/tests_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_settings.py` & `djangoldp-2.1.9/djangoldp/tests/tests_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/runner.py` & `djangoldp-2.1.9/djangoldp/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/performance_runner.py` & `djangoldp-2.1.9/djangoldp/tests/performance_runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_guardian.py` & `djangoldp-2.1.9/djangoldp/tests/tests_guardian.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_user_permissions.py` & `djangoldp-2.1.9/djangoldp/tests/tests_user_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/scripts/prod_data_generator.py` & `djangoldp-2.1.9/djangoldp/tests/scripts/prod_data_generator.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/scripts/utils.py` & `djangoldp-2.1.9/djangoldp/tests/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/scripts/test_data_generator.py` & `djangoldp-2.1.9/djangoldp/tests/scripts/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_delete.py` & `djangoldp-2.1.9/djangoldp/tests/tests_delete.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_ldp_viewset.py` & `djangoldp-2.1.9/djangoldp/tests/tests_ldp_viewset.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_auto_author.py` & `djangoldp-2.1.9/djangoldp/tests/tests_auto_author.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_performance.py` & `djangoldp-2.1.9/djangoldp/tests/tests_performance.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/djangoldp_urls.py` & `djangoldp-2.1.9/djangoldp/tests/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_post.py` & `djangoldp-2.1.9/djangoldp/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_get.py` & `djangoldp-2.1.9/djangoldp/tests/tests_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_pagination.py` & `djangoldp-2.1.9/djangoldp/tests/tests_pagination.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_anonymous_permissions.py` & `djangoldp-2.1.9/djangoldp/tests/tests_anonymous_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_perf_get.py` & `djangoldp-2.1.9/djangoldp/tests/tests_perf_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_backlinks_service.py` & `djangoldp-2.1.9/djangoldp/tests/tests_backlinks_service.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_cache.py` & `djangoldp-2.1.9/djangoldp/tests/tests_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/settings_default.py` & `djangoldp-2.1.9/djangoldp/tests/settings_default.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_inbox.py` & `djangoldp-2.1.9/djangoldp/tests/tests_inbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,45 @@
         self.assertEqual(circles[0].owner, self.user)
         self._assert_activity_created(response)
 
         # assert external circle member now following local user
         self.assertEquals(Follower.objects.count(), 1)
         self._assert_follower_created(self.user.urlid, "https://distant.com/circles/1/")
 
+    # tests creation, and tests that consequential creation also happens
+    # i.e. that I pass it an external circle which it doesn't know about, and it creates that too
+    def test_create_activity_circle_member(self):
+        obj = {
+            "@type": "hd:circlemember",
+            "@id": "https://distant.com/circlemembers/1/",
+            "user": {
+                "@type": "foaf:user",
+                "@id": self.user.urlid
+            },
+            "circle": {
+                "@type": "hd:circle",
+                "@id": "https://distant.com/circles/1/"
+            }
+        }
+        payload = self._get_activity_request_template("Create", obj)
+
+        response = self.client.post('/inbox/',
+                                    data=json.dumps(payload), content_type='application/ld+json')
+        self.assertEqual(response.status_code, 201)
+
+        # assert that the circle was created and the user associated as member
+        circles = Circle.objects.all()
+        self.assertEquals(len(circles), 1)
+        self.assertIn("https://distant.com/circles/1/", circles.values_list('urlid', flat=True))
+        self.assertTrue(circles[0].members.filter(user=self.user).exists())
+        self._assert_activity_created(response)
+
+        # assert external circle member now following local user
+        self._assert_follower_created(self.user.urlid, "https://distant.com/circlemembers/1/")
+
     # sender has sent a circle with a local user that doesn't exist
     def test_create_activity_circle_local(self):
         urlid = '{}/{}'.format(settings.SITE_URL, 'someonewhodoesntexist')
         obj = {
             "@type": "hd:circle",
             "@id": "https://distant.com/circles/1/",
             "owner": {
```

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_model_serializer.py` & `djangoldp-2.1.9/djangoldp/tests/tests_model_serializer.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/tests/tests_ldp_model.py` & `djangoldp-2.1.9/djangoldp/tests/tests_ldp_model.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/urls.py` & `djangoldp-2.1.9/djangoldp/urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/cli.py` & `djangoldp-2.1.9/djangoldp/cli.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0007_auto_20200429_1346.py` & `djangoldp-2.1.9/djangoldp/migrations/0007_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0011_auto_20200610_1323.py` & `djangoldp-2.1.9/djangoldp/migrations/0011_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0012_auto_20200617_1817.py` & `djangoldp-2.1.9/djangoldp/migrations/0012_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0008_auto_20200501_1207.py` & `djangoldp-2.1.9/djangoldp/migrations/0008_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0010_follower.py` & `djangoldp-2.1.9/djangoldp/migrations/0010_follower.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0002_auto_20190906_0642.py` & `djangoldp-2.1.9/djangoldp/migrations/0002_auto_20190906_0642.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0006_activity.py` & `djangoldp-2.1.9/djangoldp/migrations/0006_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0015_auto_20210125_1847.py` & `djangoldp-2.1.9/djangoldp/migrations/0015_auto_20210125_1847.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0001_initial.py` & `djangoldp-2.1.9/djangoldp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0013_auto_20200624_1709.py` & `djangoldp-2.1.9/djangoldp/migrations/0013_auto_20200624_1709.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0014_auto_20200909_2206.py` & `djangoldp-2.1.9/djangoldp/migrations/0014_auto_20200909_2206.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/migrations/0009_auto_20200505_1733.py` & `djangoldp-2.1.9/djangoldp/migrations/0009_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/pagination.py` & `djangoldp-2.1.9/djangoldp/pagination.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/management/commands/federate.py` & `djangoldp-2.1.9/djangoldp/management/commands/federate.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/management/commands/check_integrity.py` & `djangoldp-2.1.9/djangoldp/management/commands/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/management/commands/configure.py` & `djangoldp-2.1.9/djangoldp/management/commands/configure.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/filters.py` & `djangoldp-2.1.9/djangoldp/filters.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp/middleware.py` & `djangoldp-2.1.9/djangoldp/middleware.py`

 * *Files identical despite different names*

### Comparing `djangoldp-2.1.8/djangoldp.egg-info/SOURCES.txt` & `djangoldp-2.1.9/djangoldp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

