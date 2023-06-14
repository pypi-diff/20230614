# Comparing `tmp/tutor-15.3.7.tar.gz` & `tmp/tutor-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-15.3.7.tar", last modified: Tue Jun 13 08:44:10 2023, max compression
+gzip compressed data, was "tutor-16.0.0.tar", last modified: Wed Jun 14 21:51:28 2023, max compression
```

## Comparing `tutor-15.3.7.tar` & `tutor-16.0.0.tar`

### file list

```diff
@@ -1,159 +1,163 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-13 08:40:35.000000 tutor-15.3.7/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      121 2023-06-13 08:40:35.000000 tutor-15.3.7/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6664 2023-06-13 08:44:10.000000 tutor-15.3.7/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4745 2023-06-13 08:40:35.000000 tutor-15.3.7/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-13 08:40:35.000000 tutor-15.3.7/pyproject.toml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)       98 2023-06-13 08:40:35.000000 tutor-15.3.7/requirements/base.in
--rw-r--r--   0 ci        (1000) ci        (1000)      341 2023-06-13 08:40:35.000000 tutor-15.3.7/requirements/plugins.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-13 08:44:10.000000 tutor-15.3.7/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     2505 2023-06-13 08:40:35.000000 tutor-15.3.7/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tests/
--rw-r--r--   0 ci        (1000) ci        (1000)     4172 2023-06-13 08:40:35.000000 tutor-15.3.7/tests/test_config.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15899 2023-06-13 08:40:35.000000 tutor-15.3.7/tests/test_env.py
--rw-r--r--   0 ci        (1000) ci        (1000)      472 2023-06-13 08:40:35.000000 tutor-15.3.7/tests/test_images.py
--rw-r--r--   0 ci        (1000) ci        (1000)     3063 2023-06-13 08:40:35.000000 tutor-15.3.7/tests/test_plugin_indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)     8273 2023-06-13 08:40:35.000000 tutor-15.3.7/tests/test_plugins_v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1617 2023-06-13 08:40:35.000000 tutor-15.3.7/tests/test_serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)    10669 2023-06-13 08:40:35.000000 tutor-15.3.7/tests/test_utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/
--rw-r--r--   0 ci        (1000) ci        (1000)     1159 2023-06-13 08:43:23.000000 tutor-15.3.7/tutor/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1843 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/bindmounts.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/commands/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/__init__.py
--rwxr-xr-x   0 ci        (1000) ci        (1000)     4349 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/cli.py
--rw-r--r--   0 ci        (1000) ci        (1000)    17488 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5647 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/config.py
--rw-r--r--   0 ci        (1000) ci        (1000)      794 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/context.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4880 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/dev.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6304 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11445 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/jobs.py
--rw-r--r--   0 ci        (1000) ci        (1000)    21033 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     7466 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/local.py
--rw-r--r--   0 ci        (1000) ci        (1000)    13436 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/plugins.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/commands/upgrade/
--rw-r--r--   0 ci        (1000) ci        (1000)      146 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/upgrade/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1826 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/upgrade/common.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5853 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/upgrade/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5574 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/commands/upgrade/local.py
--rw-r--r--   0 ci        (1000) ci        (1000)     9685 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/core/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/core/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/core/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      451 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/core/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     8085 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/core/hooks/actions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     3376 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/core/hooks/contexts.py
--rw-r--r--   0 ci        (1000) ci        (1000)    12849 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/core/hooks/filters.py
--rw-r--r--   0 ci        (1000) ci        (1000)      638 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/core/hooks/priorities.py
--rw-r--r--   0 ci        (1000) ci        (1000)    17511 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/env.py
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/exceptions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/fmt.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      273 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)    25047 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/hooks/catalog.py
--rw-r--r--   0 ci        (1000) ci        (1000)      657 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5076 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/interactive.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/plugins/
--rw-r--r--   0 ci        (1000) ci        (1000)     3653 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/plugins/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      548 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/plugins/base.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6989 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/plugins/indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15132 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/plugins/v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2324 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/plugins/v1.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/py.typed
--rw-r--r--   0 ci        (1000) ci        (1000)     1536 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1385 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/tasks.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/caddy/
--rw-r--r--   0 ci        (1000) ci        (1000)     1989 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/caddy/Caddyfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/openedx/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/openedx/config/
--rw-r--r--   0 ci        (1000) ci        (1000)     1542 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/config/cms.env.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1787 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/config/lms.env.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/openedx/config/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      673 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/config/partials/auth.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      591 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/cms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)      529 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/cms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/cms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1132 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/lms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1039 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/lms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/lms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)     9859 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/partials/common_all.py
--rw-r--r--   0 ci        (1000) ci        (1000)      924 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/partials/common_cms.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1748 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/partials/common_lms.py
--rw-r--r--   0 ci        (1000) ci        (1000)      105 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/settings/partials/common_test.py
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/openedx/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/apps/redis/
--rw-r--r--   0 ci        (1000) ci        (1000)      854 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/apps/redis/redis.conf
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/
--rw-r--r--   0 ci        (1000) ci        (1000)    10443 2023-06-13 08:43:23.000000 tutor-15.3.7/tutor/templates/build/openedx/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/bin/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/bin/openedx-assets
--rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/bin/reload-uwsgi
--rw-r--r--   0 ci        (1000) ci        (1000)     2329 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/bin/site-configuration
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/locale/
--rw-r--r--   0 ci        (1000) ci        (1000)      438 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/locale/customlocales.md
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)      305 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/requirements/private-sample.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       29 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/revisions.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      317 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/cms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/cms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      306 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/lms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/lms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      441 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/partials/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)      420 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/partials/i18n.py
--rw-r--r--   0 ci        (1000) ci        (1000)      262 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/settings/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/openedx/themes/
--rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/openedx/themes/README
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/build/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/permissions/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      302 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/build/permissions/setowner.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/config/
--rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/config/base.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2627 2023-06-13 08:43:23.000000 tutor-15.3.7/tutor/templates/config/defaults.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/dev/
--rw-r--r--   0 ci        (1000) ci        (1000)      885 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/dev/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1721 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/dev/docker-compose.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)      418 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/jobs/init/cms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1807 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/jobs/init/lms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      756 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/jobs/init/mounted-edx-platform.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1455 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/jobs/init/mysql.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/k8s/
--rw-r--r--   0 ci        (1000) ci        (1000)    13208 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/k8s/deployments.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2090 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/k8s/jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      125 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/k8s/namespace.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/k8s/override.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2416 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/k8s/services.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1428 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/k8s/volumes.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2142 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/kustomization.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor/templates/local/
--rw-r--r--   0 ci        (1000) ci        (1000)     1979 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/local/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      950 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/local/docker-compose.prod.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     6701 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/local/docker-compose.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       19 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/templates/version
--rw-r--r--   0 ci        (1000) ci        (1000)     1327 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/types.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11298 2023-06-13 08:40:35.000000 tutor-15.3.7/tutor/utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6664 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     3998 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      397 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        6 2023-06-13 08:44:10.000000 tutor-15.3.7/tutor.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.019098 tutor-16.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-14 21:50:41.000000 tutor-16.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      121 2023-06-14 21:50:41.000000 tutor-16.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-06-14 21:51:28.019098 tutor-16.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4745 2023-06-14 21:50:41.000000 tutor-16.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 21:50:41.000000 tutor-16.0.0/pyproject.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.985764 tutor-16.0.0/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)       98 2023-06-14 21:50:41.000000 tutor-16.0.0/requirements/base.in
+-rw-r--r--   0 ci        (1000) ci        (1000)      340 2023-06-14 21:50:41.000000 tutor-16.0.0/requirements/plugins.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 21:51:28.022431 tutor-16.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     2506 2023-06-14 21:50:41.000000 tutor-16.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.989098 tutor-16.0.0/tests/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2491 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_bindmount.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4172 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15898 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3063 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_plugin_indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8279 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_plugins_v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2432 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10669 2023-06-14 21:50:41.000000 tutor-16.0.0/tests/test_utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.992431 tutor-16.0.0/tutor/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1159 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2546 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/bindmount.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.995764 tutor-16.0.0/tutor/commands/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/__init__.py
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     4485 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/cli.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    16737 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     7317 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      794 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/context.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2240 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/dev.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11658 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10722 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/jobs.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    21033 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1772 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/local.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4446 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/mounts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      741 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/params.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    13436 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/plugins.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.999098 tutor-16.0.0/tutor/commands/upgrade/
+-rw-r--r--   0 ci        (1000) ci        (1000)      185 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/upgrade/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2082 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/upgrade/common.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6047 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/upgrade/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5685 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/commands/upgrade/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9685 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.999098 tutor-16.0.0/tutor/core/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.999098 tutor-16.0.0/tutor/core/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      292 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5707 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/actions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2929 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/contexts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9006 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/filters.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      638 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/core/hooks/priorities.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    17753 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/exceptions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/fmt.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.002431 tutor-16.0.0/tutor/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      273 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    24524 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/hooks/catalog.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      571 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5076 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/interactive.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.002431 tutor-16.0.0/tutor/plugins/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3802 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      548 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/base.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6989 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15218 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2376 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/plugins/v1.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/py.typed
+-rw-r--r--   0 ci        (1000) ci        (1000)     1947 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1385 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/tasks.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.979097 tutor-16.0.0/tutor/templates/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/caddy/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1989 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/caddy/Caddyfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/openedx/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/openedx/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1542 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/config/cms.env.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1787 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/config/lms.env.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/openedx/config/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      673 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/config/partials/auth.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.979097 tutor-16.0.0/tutor/templates/apps/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.005764 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      591 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      529 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.009098 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1132 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1039 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.009098 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)    10001 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_all.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      924 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_cms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1450 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_lms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      105 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_test.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/openedx/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.009098 tutor-16.0.0/tutor/templates/apps/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      380 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/permissions/setowners.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.009098 tutor-16.0.0/tutor/templates/apps/redis/
+-rw-r--r--   0 ci        (1000) ci        (1000)      854 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/apps/redis/redis.conf
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.982431 tutor-16.0.0/tutor/templates/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/
+-rw-r--r--   0 ci        (1000) ci        (1000)    12605 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/bin/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/bin/openedx-assets
+-rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/bin/reload-uwsgi
+-rw-r--r--   0 ci        (1000) ci        (1000)     2329 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/bin/site-configuration
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/locale/
+-rw-r--r--   0 ci        (1000) ci        (1000)      438 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/locale/customlocales.md
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)      305 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/requirements/private-sample.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/revisions.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      317 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/cms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/cms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      306 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/lms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/lms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      441 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/partials/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      420 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/partials/i18n.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      262 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/settings/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.012431 tutor-16.0.0/tutor/templates/build/openedx/themes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/openedx/themes/README
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.015764 tutor-16.0.0/tutor/templates/build/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/permissions/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      302 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/build/permissions/setowner.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.015764 tutor-16.0.0/tutor/templates/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/config/base.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2610 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/config/defaults.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.015764 tutor-16.0.0/tutor/templates/dev/
+-rw-r--r--   0 ci        (1000) ci        (1000)      885 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/dev/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1395 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/dev/docker-compose.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.982431 tutor-16.0.0/tutor/templates/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.015764 tutor-16.0.0/tutor/templates/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)      418 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/jobs/init/cms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1807 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/jobs/init/lms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      756 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/jobs/init/mounted-edx-platform.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1455 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.019098 tutor-16.0.0/tutor/templates/k8s/
+-rw-r--r--   0 ci        (1000) ci        (1000)    13150 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/deployments.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2090 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      125 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/namespace.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/override.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2358 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/services.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1428 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/k8s/volumes.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2142 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/kustomization.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:28.019098 tutor-16.0.0/tutor/templates/local/
+-rw-r--r--   0 ci        (1000) ci        (1000)     2185 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/local/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      950 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/local/docker-compose.prod.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     6496 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/local/docker-compose.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       19 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/templates/version
+-rw-r--r--   0 ci        (1000) ci        (1000)     1327 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/types.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10935 2023-06-14 21:50:41.000000 tutor-16.0.0/tutor/utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 21:51:27.995764 tutor-16.0.0/tutor.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6665 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4098 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      397 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        6 2023-06-14 21:51:27.000000 tutor-16.0.0/tutor.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tutor-15.3.7/LICENSE.txt` & `tutor-16.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/PKG-INFO` & `tutor-16.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 15.3.7
+Version: 16.0.0
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor
@@ -114,14 +114,14 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
```

### Comparing `tutor-15.3.7/README.rst` & `tutor-16.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/setup.py` & `tutor-16.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,26 +52,26 @@
     author="Overhang.io",
     author_email="contact@overhang.io",
     description="The Docker-based Open edX distribution designed for peace of mind",
     long_description=load_readme(),
     long_description_content_type="text/x-rst",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=load_requirements("base.in"),
     extras_require={
         "full": load_requirements("plugins.txt"),
     },
     entry_points={"console_scripts": ["tutor=tutor.commands.cli:main"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     test_suite="tests",
 )
```

### Comparing `tutor-15.3.7/tests/test_config.py` & `tutor-16.0.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tests/test_env.py` & `tutor-16.0.0/tests/test_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
             with open(
                 os.path.join(env.base_dir(root), env.VERSION_FILENAME),
                 "w",
                 encoding="utf-8",
             ) as f:
                 f.write(__version__)
             self.assertEqual(__version__, env.current_version(root))
-            self.assertEqual("olive", env.get_env_release(root))
+            self.assertEqual("palm", env.get_env_release(root))
             self.assertIsNone(env.should_upgrade_from_release(root))
             self.assertTrue(env.is_up_to_date(root))
 
 
 class PatchRendererTests(unittest.TestCase):
     def setUp(self) -> None:
         self.render = env.PatchRenderer()
```

### Comparing `tutor-15.3.7/tests/test_plugin_indexes.py` & `tutor-16.0.0/tests/test_plugin_indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tests/test_plugins_v0.py` & `tutor-16.0.0/tests/test_plugins_v0.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         )
         plugins.load_all(["plugin1"])
         patches = list(plugins.iter_patches("patch1"))
         self.assertEqual(["Hello {{ ID }}"], patches)
 
     def test_plugin_without_patches(self) -> None:
         plugins_v0.DictPlugin({"name": "plugin1"})
-        plugins.load("plugin1")
+        plugins.load_all(["plugin1"])
         patches = list(plugins.iter_patches("patch1"))
         self.assertEqual([], patches)
 
     def test_configure(self) -> None:
         plugins_v0.DictPlugin(
             {
                 "name": "plugin1",
```

### Comparing `tutor-15.3.7/tests/test_serialize.py` & `tutor-16.0.0/tests/test_serialize.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,7 +37,21 @@
         self.assertEqual(("x", "a=bcd"), serialize.parse_key_value("x=a=bcd"))
         self.assertEqual(
             ("x", {"key1": {"subkey": "value"}, "key2": {"subkey": "value"}}),
             serialize.parse_key_value(
                 "x=key1:\n  subkey: value\nkey2:\n  subkey: value"
             ),
         )
+
+    def test_str_format(self) -> None:
+        self.assertEqual("true", serialize.str_format(True))
+        self.assertEqual("false", serialize.str_format(False))
+        self.assertEqual("null", serialize.str_format(None))
+        self.assertEqual("éü©", serialize.str_format("éü©"))
+        self.assertEqual("""[1, 'abcd']""", serialize.str_format([1, "abcd"]))
+
+    def test_load_str_format(self) -> None:
+        self.assertEqual(True, serialize.load(serialize.str_format(True)))
+        self.assertEqual(False, serialize.load(serialize.str_format(False)))
+        self.assertEqual(None, serialize.load(serialize.str_format(None)))
+        self.assertEqual("éü©", serialize.load(serialize.str_format("éü©")))
+        self.assertEqual([1, "abcd"], serialize.load(serialize.str_format([1, "abcd"])))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tutor-15.3.7/tests/test_utils.py` & `tutor-16.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/__about__.py` & `tutor-16.0.0/tutor/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Increment this version number to trigger a new release. See
 # docs/tutor.html#versioning for information on the versioning scheme.
-__version__ = "15.3.7"
+__version__ = "16.0.0"
 
 # The version suffix will be appended to the actual version, separated by a
 # dash. Use this suffix to differentiate between the actual released version and
 # the versions from other branches. For instance: set the suffix to "nightly" in
 # the nightly branch.
 # The suffix is cleanly separated from the __version__ in this module to avoid
 # conflicts when merging branches.
```

### Comparing `tutor-15.3.7/tutor/commands/cli.py` & `tutor-16.0.0/tutor/commands/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from tutor.__about__ import __app__, __version__
 from tutor.commands.config import config_command
 from tutor.commands.context import Context
 from tutor.commands.dev import dev
 from tutor.commands.images import images_command
 from tutor.commands.k8s import k8s
 from tutor.commands.local import local
+from tutor.commands.mounts import mounts_command
 from tutor.commands.plugins import plugins_command
 
 
 def main() -> None:
     try:
         # Everyone on board
         # Note that this action should not be triggered in the module scope, because it
@@ -125,13 +126,22 @@
 @click.command(help="Print this help", name="help")
 @click.pass_context
 def help_command(context: click.Context) -> None:
     context.invoke(cli, show_help=True)
 
 
 hooks.Filters.CLI_COMMANDS.add_items(
-    [images_command, config_command, local, dev, k8s, help_command, plugins_command]
+    [
+        config_command,
+        dev,
+        help_command,
+        images_command,
+        k8s,
+        local,
+        mounts_command,
+        plugins_command,
+    ]
 )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tutor-15.3.7/tutor/commands/config.py` & `tutor-16.0.0/tutor/commands/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,59 +2,55 @@
 
 import json
 import typing as t
 
 import click
 import click.shell_completion
 
-from .. import config as tutor_config
-from .. import env, exceptions, fmt
-from .. import interactive as interactive_config
-from .. import serialize
-from ..types import Config, ConfigValue
-from .context import Context
+from tutor import config as tutor_config
+from tutor import env, exceptions, fmt
+from tutor import interactive as interactive_config
+from tutor import serialize
+from tutor.commands.context import Context
+from tutor.commands.params import ConfigLoaderParam
+from tutor.types import ConfigValue
 
 
 @click.group(
     name="config",
     short_help="Configure Open edX",
     help="""Configure Open edX and store configuration values in $TUTOR_ROOT/config.yml""",
 )
 def config_command() -> None:
     pass
 
 
-class ConfigKeyParamType(click.ParamType):
+class ConfigKeyParamType(ConfigLoaderParam):
     name = "configkey"
 
     def shell_complete(
         self, ctx: click.Context, param: click.Parameter, incomplete: str
     ) -> list[click.shell_completion.CompletionItem]:
         return [
             click.shell_completion.CompletionItem(key)
-            for key, _value in self._shell_complete_config_items(ctx, incomplete)
+            for key, _value in self._shell_complete_config_items(incomplete)
         ]
 
-    @staticmethod
     def _shell_complete_config_items(
-        ctx: click.Context, incomplete: str
+        self, incomplete: str
     ) -> list[tuple[str, ConfigValue]]:
-        # Here we want to auto-complete the name of the config key. For that we need to
-        # figure out the list of enabled plugins, and for that we need the project root.
-        # The project root would ordinarily be stored in ctx.obj.root, but during
-        # auto-completion we don't have access to our custom Tutor context. So we resort
-        # to a dirty hack, which is to examine the grandparent context.
-        root = getattr(
-            getattr(getattr(ctx, "parent", None), "parent", None), "params", {}
-        ).get("root", "")
-        config = tutor_config.load_full(root)
         return [
-            (key, value) for key, value in config.items() if key.startswith(incomplete)
+            (key, value)
+            for key, value in self._candidate_config_items()
+            if key.startswith(incomplete)
         ]
 
+    def _candidate_config_items(self) -> t.Iterable[tuple[str, ConfigValue]]:
+        yield from self.config.items()
+
 
 class ConfigKeyValParamType(ConfigKeyParamType):
     """
     Parser for <KEY>=<YAML VALUE> command line arguments.
     """
 
     name = "configkeyval"
@@ -72,65 +68,119 @@
         Nice and friendly <KEY>=<VAL> auto-completion.
         """
         if "=" not in incomplete:
             # Auto-complete with '<KEY>='. Note the single quotes which allow users to
             # further auto-complete later.
             return [
                 click.shell_completion.CompletionItem(f"'{key}='")
-                for key, value in self._shell_complete_config_items(ctx, incomplete)
+                for key, value in self._shell_complete_config_items(incomplete)
             ]
         if incomplete.endswith("="):
             # raise ValueError(f"incomplete: <{incomplete}>")
             # Auto-complete with '<KEY>=<VALUE>'
             return [
                 click.shell_completion.CompletionItem(f"{key}={json.dumps(value)}")
-                for key, value in self._shell_complete_config_items(
-                    ctx, incomplete[:-1]
-                )
+                for key, value in self._shell_complete_config_items(incomplete[:-1])
             ]
         # Else, don't bother
         return []
 
 
+class ConfigListKeyValParamType(ConfigKeyValParamType):
+    """
+    Same as the parent class, but for keys of type `list`.
+    """
+
+    def _candidate_config_items(self) -> t.Iterable[tuple[str, ConfigValue]]:
+        for key, val in self.config.items():
+            if isinstance(val, list):
+                yield key, val
+
+
 @click.command(help="Create and save configuration interactively")
 @click.option("-i", "--interactive", is_flag=True, help="Run interactively")
 @click.option(
     "-s",
     "--set",
     "set_vars",
     type=ConfigKeyValParamType(),
     multiple=True,
     metavar="KEY=VAL",
     help="Set a configuration value (can be used multiple times)",
 )
 @click.option(
+    "-a",
+    "--append",
+    "append_vars",
+    type=ConfigListKeyValParamType(),
+    multiple=True,
+    metavar="KEY=VAL",
+    help="Append an item to a configuration value of type list. The value will only be added it it is not already present. (can be used multiple times)",
+)
+@click.option(
+    "-A",
+    "--remove",
+    "remove_vars",
+    type=ConfigListKeyValParamType(),
+    multiple=True,
+    metavar="KEY=VAL",
+    help="Remove an item from a configuration value of type list (can be used multiple times)",
+)
+@click.option(
     "-U",
     "--unset",
     "unset_vars",
     multiple=True,
     type=ConfigKeyParamType(),
     help="Remove a configuration value (can be used multiple times)",
 )
 @click.option(
     "-e", "--env-only", "env_only", is_flag=True, help="Skip updating config.yml"
 )
 @click.pass_obj
 def save(
     context: Context,
     interactive: bool,
-    set_vars: Config,
+    set_vars: list[tuple[str, t.Any]],
+    append_vars: list[tuple[str, t.Any]],
+    remove_vars: list[tuple[str, t.Any]],
     unset_vars: list[str],
     env_only: bool,
 ) -> None:
     config = tutor_config.load_minimal(context.root)
+    config_full = tutor_config.load_full(context.root)
     if interactive:
         interactive_config.ask_questions(config)
     if set_vars:
-        for key, value in dict(set_vars).items():
+        for key, value in set_vars:
             config[key] = env.render_unknown(config, value)
+    if append_vars:
+        for key, value in append_vars:
+            if key not in config:
+                config[key] = config_full.get(key, [])
+            values = config[key]
+            if not isinstance(values, list):
+                raise exceptions.TutorError(
+                    f"Could not append value to '{key}': current setting is of type '{values.__class__.__name__}', expected list."
+                )
+            if not isinstance(value, str):
+                raise exceptions.TutorError(
+                    f"Could not append value to '{key}': appended value is of type '{value.__class__.__name__}', expected str."
+                )
+            if value not in values:
+                values.append(value)
+    if remove_vars:
+        for key, value in remove_vars:
+            values = config.get(key, [])
+            if not isinstance(values, list):
+                raise exceptions.TutorError(
+                    f"Could not remove value from '{key}': current setting is of type '{values.__class__.__name__}', expected list."
+                )
+            while value in values:
+                values.remove(value)
     for key in unset_vars:
         config.pop(key, None)
     if not env_only:
         tutor_config.save_config_file(context.root, config)
 
     # Reload configuration, without version checking
     config = tutor_config.load_full(context.root)
@@ -145,18 +195,18 @@
 
 @click.command(help="Print a configuration value")
 @click.argument("key", type=ConfigKeyParamType())
 @click.pass_obj
 def printvalue(context: Context, key: str) -> None:
     config = tutor_config.load(context.root)
     try:
-        # Note that this will incorrectly print None values
-        fmt.echo(str(config[key]))
+        value = config[key]
     except KeyError as e:
         raise exceptions.TutorError(f"Missing configuration value: {key}") from e
+    fmt.echo(serialize.str_format(value))
 
 
 @click.group(name="patches", help="Commands related to patches in configurations")
 def patches_command() -> None:
     pass
 
 
@@ -167,9 +217,9 @@
     renderer = env.PatchRenderer(config)
     renderer.print_patches_locations()
 
 
 config_command.add_command(save)
 config_command.add_command(printroot)
 config_command.add_command(printvalue)
-config_command.add_command(patches_command)
 patches_command.add_command(patches_list)
+config_command.add_command(patches_command)
```

### Comparing `tutor-15.3.7/tutor/commands/context.py` & `tutor-16.0.0/tutor/commands/context.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/commands/jobs.py` & `tutor-16.0.0/tutor/commands/jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Common jobs that must be added both to local, dev and k8s commands.
 """
 from __future__ import annotations
 
 import functools
+import shlex
 import typing as t
 
 import click
 from typing_extensions import ParamSpec
 
 from tutor import config as tutor_config
-from tutor import env, fmt, hooks, utils
+from tutor import env, fmt, hooks
 from tutor.hooks import priorities
 
 
 class DoGroup(click.Group):
     """
     A Click group that prints subcommands under 'Jobs' instead of 'Commands' when we run
     `.. do --help`. Hackish but it works.
@@ -32,68 +33,49 @@
 def _add_core_init_tasks() -> None:
     """
     Declare core init scripts at runtime.
 
     The context is important, because it allows us to select the init scripts based on
     the --limit argument.
     """
-    with hooks.Contexts.APP("mysql").enter():
+    with hooks.Contexts.app("mysql").enter():
         hooks.Filters.CLI_DO_INIT_TASKS.add_item(
             ("mysql", env.read_core_template_file("jobs", "init", "mysql.sh"))
         )
-    with hooks.Contexts.APP("lms").enter():
+    with hooks.Contexts.app("lms").enter():
         hooks.Filters.CLI_DO_INIT_TASKS.add_item(
             (
                 "lms",
                 env.read_core_template_file("jobs", "init", "mounted-edx-platform.sh"),
             ),
             # If edx-platform is mounted, then we may need to perform some setup
             # before other initialization scripts can be run.
             priority=priorities.HIGH,
         )
         hooks.Filters.CLI_DO_INIT_TASKS.add_item(
             ("lms", env.read_core_template_file("jobs", "init", "lms.sh"))
         )
-    with hooks.Contexts.APP("cms").enter():
+    with hooks.Contexts.app("cms").enter():
         hooks.Filters.CLI_DO_INIT_TASKS.add_item(
             ("cms", env.read_core_template_file("jobs", "init", "cms.sh"))
         )
 
 
 @click.command("init", help="Initialise all applications")
 @click.option("-l", "--limit", help="Limit initialisation to this service or plugin")
 def initialise(limit: t.Optional[str]) -> t.Iterator[tuple[str, str]]:
     fmt.echo_info("Initialising all services...")
-    filter_context = hooks.Contexts.APP(limit).name if limit else None
+    filter_context = hooks.Contexts.app(limit).name if limit else None
 
-    # Deprecated pre-init tasks
-    for service, path in hooks.Filters.COMMANDS_PRE_INIT.iterate_from_context(
-        filter_context
-    ):
-        fmt.echo_alert(
-            f"Running deprecated pre-init task: {'/'.join(path)}. Init tasks should no longer be added to the COMMANDS_PRE_INIT filter. Plugin developers should use the CLI_DO_INIT_TASKS filter instead, with a high priority."
-        )
-        yield service, env.read_template_file(*path)
-
-    # Init tasks
     for service, task in hooks.Filters.CLI_DO_INIT_TASKS.iterate_from_context(
         filter_context
     ):
         fmt.echo_info(f"Running init task in {service}")
         yield service, task
 
-    # Deprecated init tasks
-    for service, path in hooks.Filters.COMMANDS_INIT.iterate_from_context(
-        filter_context
-    ):
-        fmt.echo_alert(
-            f"Running deprecated init task: {'/'.join(path)}. Init tasks should no longer be added to the COMMANDS_INIT filter. Plugin developers should use the CLI_DO_INIT_TASKS filter instead."
-        )
-        yield service, env.read_template_file(*path)
-
     fmt.echo_info("All services initialised.")
 
 
 @click.command(help="Create an Open edX user and interactively set their password")
 @click.option("--superuser", is_flag=True, help="Make superuser")
 @click.option("--staff", is_flag=True, help="Make staff user")
 @click.option(
@@ -143,26 +125,33 @@
     "-r",
     "--repo",
     default="https://github.com/openedx/edx-demo-course",
     show_default=True,
     help="Git repository that contains the course to be imported",
 )
 @click.option(
+    "-d",
+    "--repo-dir",
+    default="",
+    show_default=True,
+    help="Git relative subdirectory to import data from",
+)
+@click.option(
     "-v",
     "--version",
     help="Git branch, tag or sha1 identifier. If unspecified, will default to the value of the OPENEDX_COMMON_VERSION setting.",
 )
 def importdemocourse(
-    repo: str, version: t.Optional[str]
+    repo: str, repo_dir: str, version: t.Optional[str]
 ) -> t.Iterable[tuple[str, str]]:
     version = version or "{{ OPENEDX_COMMON_VERSION }}"
     template = f"""
 # Import demo course
 git clone {repo} --branch {version} --depth 1 /tmp/course
-python ./manage.py cms import ../data /tmp/course
+python ./manage.py cms import ../data /tmp/course/{repo_dir}
 
 # Re-index courses
 ./manage.py cms reindex_course --all --setup"""
     yield ("cms", template)
 
 
 @click.command(
@@ -249,15 +238,15 @@
     Open an SQL shell as root
 
     Extra arguments will be passed to the `mysql` command verbatim. For instance, to
     show tables from the "openedx" database, run `do sqlshell openedx -e 'show tables'`.
     """
     command = "mysql --user={{ MYSQL_ROOT_USERNAME }} --password={{ MYSQL_ROOT_PASSWORD }} --host={{ MYSQL_HOST }} --port={{ MYSQL_PORT }}"
     if args:
-        command += " " + utils._shlex_join(*args)  # pylint: disable=protected-access
+        command += " " + shlex.join(args)  # pylint: disable=protected-access
     yield ("lms", command)
 
 
 def add_job_commands(do_command_group: click.Group) -> None:
     """
     This is meant to be called with the `local/dev/k8s do` group commands, to add the
     different `do` subcommands.
```

### Comparing `tutor-15.3.7/tutor/commands/k8s.py` & `tutor-16.0.0/tutor/commands/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/commands/plugins.py` & `tutor-16.0.0/tutor/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/commands/upgrade/common.py` & `tutor-16.0.0/tutor/commands/upgrade/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,7 +35,15 @@
         tutor_config.save_enabled_plugins(config)
 
 
 def upgrade_from_nutmeg(context: click.Context, config: Config) -> None:
     context.obj.job_runner(config).run_task(
         "lms", "./manage.py lms compute_grades -v1 --all_courses"
     )
+
+
+PALM_RENAME_ORA2_FOLDER_COMMAND = """
+if stat '/openedx/data/ora2/SET-ME-PLEASE (ex. bucket-name)' 2> /dev/null; then
+    echo "Renaming ora2 folder..."
+    mv '/openedx/data/ora2/SET-ME-PLEASE (ex. bucket-name)' /openedx/data/ora2/openedxuploads
+fi
+"""
```

### Comparing `tutor-15.3.7/tutor/commands/upgrade/local.py` & `tutor-16.0.0/tutor/commands/upgrade/compose.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,34 +35,28 @@
         upgrade_from_maple(context, config)
         running_release = "nutmeg"
 
     if running_release == "nutmeg":
         common_upgrade.upgrade_from_nutmeg(context, config)
         running_release = "olive"
 
+    if running_release == "olive":
+        upgrade_from_olive(context, config)
+        running_release = "palm"
+
 
 def upgrade_from_ironwood(context: click.Context, config: Config) -> None:
     click.echo(fmt.title("Upgrading from Ironwood"))
     tutor_env.save(context.obj.root, config)
 
     click.echo(fmt.title("Stopping any existing platform"))
     context.invoke(compose.stop)
 
-    if not config["RUN_MONGODB"]:
-        fmt.echo_info(
-            "You are not running MongoDB (RUN_MONGODB=false). It is your "
-            "responsibility to upgrade your MongoDb instance to v3.6. There is "
-            "nothing left to do to upgrade from Ironwood to Juniper."
-        )
-        return
-
     upgrade_mongodb(context, config, "3.4", "3.4")
-    context.invoke(compose.stop)
     upgrade_mongodb(context, config, "3.6", "3.6")
-    context.invoke(compose.stop)
 
 
 def upgrade_from_juniper(context: click.Context, config: Config) -> None:
     click.echo(fmt.title("Upgrading from Juniper"))
     tutor_env.save(context.obj.root, config)
 
     click.echo(fmt.title("Stopping any existing platform"))
@@ -142,20 +136,39 @@
     )
     context.invoke(
         compose.run,
         args=["cms", "sh", "-e", "-c", "./manage.py cms simulate_publish"],
     )
 
 
+def upgrade_from_olive(context: click.Context, config: Config) -> None:
+    # Note that we need to exec because the ora2 folder is not bind-mounted in the job
+    # services.
+    context.invoke(compose.start, detach=True, services=["lms"])
+    context.invoke(
+        compose.execute,
+        args=["lms", "sh", "-e", "-c", common_upgrade.PALM_RENAME_ORA2_FOLDER_COMMAND],
+    )
+    upgrade_mongodb(context, config, "4.2.17", "4.2")
+    upgrade_mongodb(context, config, "4.4.22", "4.4")
+
+
 def upgrade_mongodb(
     context: click.Context,
     config: Config,
     to_docker_version: str,
     to_compatibility_version: str,
 ) -> None:
+    if not config["RUN_MONGODB"]:
+        fmt.echo_info(
+            f"You are not running MongoDB (RUN_MONGODB=false). It is your "
+            f"responsibility to upgrade your MongoDb instance to {to_docker_version}."
+        )
+        return
+
     click.echo(fmt.title(f"Upgrading MongoDb to v{to_docker_version}"))
     # Note that the DOCKER_IMAGE_MONGODB value is never saved, because we only save the
     # environment, not the configuration.
     config["DOCKER_IMAGE_MONGODB"] = f"mongo:{to_docker_version}"
     tutor_env.save(context.obj.root, config)
     context.invoke(compose.start, detach=True, services=["mongodb"])
     fmt.echo_info("Waiting for mongodb to boot...")
```

### Comparing `tutor-15.3.7/tutor/config.py` & `tutor-16.0.0/tutor/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
 @hooks.Actions.PLUGIN_UNLOADED.add()
 def _remove_plugin_config_overrides_on_unload(
     plugin: str, _root: str, config: Config
 ) -> None:
     # Find the configuration entries that were overridden by the plugin and
     # remove them from the current config
     for key, _value in hooks.Filters.CONFIG_OVERRIDES.iterate_from_context(
-        hooks.Contexts.APP(plugin).name
+        hooks.Contexts.app(plugin).name
     ):
         value = config.pop(key, None)
         value = env.render_unknown(config, value)
         fmt.echo_info(f"    config - removing entry: {key}={value}")
 
 
 @hooks.Actions.PLUGIN_UNLOADED.add(priority=100)
```

### Comparing `tutor-15.3.7/tutor/core/hooks/contexts.py` & `tutor-16.0.0/tutor/core/hooks/contexts.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,30 +39,14 @@
         try:
             Context.CURRENT.append(self.name)
             yield
         finally:
             Context.CURRENT.pop()
 
 
-class ContextTemplate:
-    """
-    Context templates are for filters for which the name needs to be formatted
-    before the filter can be applied.
-    """
-
-    def __init__(self, name: str):
-        self.template = name
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}('{self.template}')"
-
-    def __call__(self, *args: t.Any, **kwargs: t.Any) -> Context:
-        return Context(self.template.format(*args, **kwargs))
-
-
 class Contextualized:
     """
     This is a simple class to store the current context in hooks.
 
     The current context is stored as a static variable.
     """
```

### Comparing `tutor-15.3.7/tutor/core/hooks/filters.py` & `tutor-16.0.0/tutor/core/hooks/filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 # The Tutor plugin system is licensed under the terms of the Apache 2.0 license.
 __license__ = "Apache 2.0"
 
 import sys
 import typing as t
+from weakref import WeakSet
 
 from typing_extensions import Concatenate, ParamSpec
 
 from . import contexts, priorities
 
 #: Filter generic return value, which is also the type of the first callback argument.
 T1 = t.TypeVar("T1")
@@ -39,48 +40,40 @@
     Filter hooks have callbacks that are triggered as a chain.
 
     Several filters are defined across the codebase. Each filters is given a unique
     name. To each filter are associated zero or more callbacks, sorted by priority.
 
     This is the typical filter lifecycle:
 
-    1. Create an action with method :py:meth:`get`.
-    2. Add callbacks with method :py:meth:`add`.
+    1. Create a filter with ``Filter()``.
+    2. Add callbacks with :py:meth:`add`.
     3. Call the filter callbacks with method :py:meth:`apply`.
 
     The result of each callback is passed as the first argument to the next one. Thus,
     the type of the first argument must match the callback return type.
 
-    The `T` and `P` type parameters of the Filter class correspond to the expected
-    signature of the filter callbacks. `T` is the type of the first argument (and thus
-    the return value type as well) and `P` is the signature of the other arguments.
+    The ``T1`` and ``T2`` type parameters of the Filter class correspond to the expected
+    signature of the filter callbacks. ``T1`` is the type of the first argument (and thus
+    the return value type as well) and ``T2`` is the signature of the other arguments.
 
     For instance, `Filter[str, [int]]` means that the filter callbacks are expected to
     take two arguments: one string and one integer. Each callback must then return a
     string.
 
     This strong typing makes it easier for plugin developers to quickly check whether
     they are adding and calling filter callbacks correctly.
     """
 
-    INDEX: dict[str, "Filter[t.Any, t.Any]"] = {}
+    # Keep a weak reference to all created filters. This allows us to clear them when
+    # necessary.
+    INSTANCES: WeakSet[Filter[t.Any, t.Any]] = WeakSet()
 
-    def __init__(self, name: str) -> None:
-        self.name = name
+    def __init__(self) -> None:
         self.callbacks: list[FilterCallback[T1, T2]] = []
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}('{self.name}')"
-
-    @classmethod
-    def get(cls, name: str) -> "Filter[t.Any, t.Any]":
-        """
-        Get an existing action with the given name from the index, or create one.
-        """
-        return cls.INDEX.setdefault(name, cls(name))
+        self.INSTANCES.add(self)
 
     def add(
         self, priority: t.Optional[int] = None
     ) -> t.Callable[[FilterCallbackFunc[T1, T2]], FilterCallbackFunc[T1, T2]]:
         """
         Decorator to add a filter callback.
 
@@ -152,29 +145,37 @@
                     value = callback.apply(
                         value,
                         *args,
                         **kwargs,
                     )
                 except:
                     sys.stderr.write(
-                        f"Error applying filter '{self.name}': func={callback.func} contexts={callback.contexts}'\n"
+                        f"Error applying filter: func={callback.func} contexts={callback.contexts}'\n"
                     )
                     raise
         return value
 
     def clear(self, context: t.Optional[str] = None) -> None:
         """
         Clear any previously defined filter with the given context.
         """
         self.callbacks = [
             callback
             for callback in self.callbacks
             if not callback.is_in_context(context)
         ]
 
+    @classmethod
+    def clear_all(cls, context: t.Optional[str] = None) -> None:
+        """
+        Clear any previously defined filter with the given context.
+        """
+        for filtre in cls.INSTANCES:
+            filtre.clear(context)
+
     # The methods below are specific to filters which take lists as first arguments
     def add_item(
         self: "Filter[list[L], T2]", item: L, priority: t.Optional[int] = None
     ) -> None:
         """
         Convenience decorator to add a single item to a filter that returns a list of items.
 
@@ -201,16 +202,16 @@
         This method is only valid for filters that return list of items.
 
         This is a similar method to :py:data:`Filter.add_item` except that it can be
         used to add multiple items at the same time. If you find yourself calling
         ``add_item`` multiple times on the same filter, then you probably want to use a
         single call to ``add_items`` instead.
 
-        :param name: filter name.
         :param list[object] items: items that will be appended to the resulting list.
+        :param int priority: optional priority.
 
         Usage::
 
             my_filter.add_items(["item1", "item2"])
             my_filter.add_items(["item3", "item4"])
 
             assert ["item1", "item2", "item3", "item4"] == my_filter.apply([])
@@ -221,23 +222,18 @@
             my_filter.add_items(["item1", "item2"])
 
             # Multiple calls to add_item
             my_filter.add_item("item1")
             my_filter.add_item("item2")
         """
 
-        # Unfortunately we have to type-ignore this line. If not, mypy complains with:
-        #
-        #   Argument 1 has incompatible type "Callable[[Arg(List[E], 'values'), **T2], List[E]]"; expected "Callable[[List[E], **T2], List[E]]"
-        #   This is likely because "callback" has named arguments: "values". Consider marking them positional-only
-        #
-        # But we are unable to mark arguments positional-only (by adding / after values arg) in Python 3.7.
-        # Get rid of this statement after Python 3.7 EOL.
-        @self.add(priority=priority)  # type: ignore
-        def callback(values: list[L], *_args: T2.args, **_kwargs: T2.kwargs) -> list[L]:
+        @self.add(priority=priority)
+        def callback(
+            values: list[L], /, *_args: T2.args, **_kwargs: T2.kwargs
+        ) -> list[L]:
             return values + items
 
     def iterate(
         self: "Filter[list[L], T2]", *args: T2.args, **kwargs: T2.kwargs
     ) -> t.Iterator[L]:
         """
         Convenient function to iterate over the results of a filter result list.
@@ -262,118 +258,7 @@
         *args: T2.args,
         **kwargs: T2.kwargs,
     ) -> t.Iterator[L]:
         """
         Same as :py:func:`Filter.iterate` but apply only callbacks from a given context.
         """
         yield from self.apply_from_context(context, [], *args, **kwargs)
-
-
-class FilterTemplate(t.Generic[T1, T2]):
-    """
-    Filter templates are for filters for which the name needs to be formatted
-    before the filter can be applied.
-
-    Similar to :py:class:`tutor.core.hooks.ActionTemplate`, filter templates are used to generate
-    :py:class:`Filter` objects for which the name matches a certain template.
-
-    Templated filters must be formatted with ``(*args)`` before being applied. For example::
-
-        filter_template = FilterTemplate("namespace:{0}")
-        named_filter = filter_template("name")
-
-        @named_filter.add()
-        def my_callback(x: int) -> int:
-            ...
-
-        named_filter.apply(42)
-    """
-
-    def __init__(self, name: str):
-        self.template = name
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}('{self.template}')"
-
-    def __call__(self, *args: t.Any, **kwargs: t.Any) -> Filter[T1, T2]:
-        return get(self.template.format(*args, **kwargs))
-
-
-# Syntactic sugar
-get = Filter.get
-
-
-def get_template(name: str) -> FilterTemplate[t.Any, t.Any]:
-    """
-    Create a filter with a template name.
-    """
-    return FilterTemplate(name)
-
-
-def add(
-    name: str, priority: t.Optional[int] = None
-) -> t.Callable[[FilterCallbackFunc[T1, T2]], FilterCallbackFunc[T1, T2]]:
-    """
-    Decorator for functions that will be applied to a single named filter.
-    """
-    return Filter.get(name).add(priority=priority)
-
-
-def add_item(name: str, item: T1, priority: t.Optional[int] = None) -> None:
-    """
-    Convenience function to add a single item to a filter that returns a list of items.
-    """
-    get(name).add_item(item, priority=priority)
-
-
-def add_items(name: str, items: list[T1], priority: t.Optional[int] = None) -> None:
-    """
-    Convenience decorator to add multiple item to a filter that returns a list of items.
-    """
-    get(name).add_items(items, priority=priority)
-
-
-def iterate(name: str, *args: t.Any, **kwargs: t.Any) -> t.Iterator[T1]:
-    """
-    Convenient function to iterate over the results of a filter result list.
-    """
-    yield from iterate_from_context(None, name, *args, **kwargs)
-
-
-def iterate_from_context(
-    context: t.Optional[str], name: str, *args: t.Any, **kwargs: t.Any
-) -> t.Iterator[T1]:
-    yield from Filter.get(name).iterate_from_context(context, *args, **kwargs)
-
-
-def apply(name: str, value: T1, *args: t.Any, **kwargs: t.Any) -> T1:
-    """
-    Apply all declared filters to a single value, passing along the additional arguments.
-    """
-    return apply_from_context(None, name, value, *args, **kwargs)
-
-
-def apply_from_context(
-    context: t.Optional[str], name: str, value: T1, *args: T2.args, **kwargs: T2.kwargs
-) -> T1:
-    """
-    Same as :py:func:`apply` but only run the callbacks that were created in a given context.
-    """
-    filtre: Filter[T1, T2] = Filter.get(name)
-    return filtre.apply_from_context(context, value, *args, **kwargs)
-
-
-def clear_all(context: t.Optional[str] = None) -> None:
-    """
-    Clear any previously defined filter with the given context.
-    """
-    for name in Filter.INDEX:
-        clear(name, context=context)
-
-
-def clear(name: str, context: t.Optional[str] = None) -> None:
-    """
-    Clear any previously defined filter with the given name and context.
-    """
-    filtre = Filter.INDEX.get(name)
-    if filtre:
-        filtre.clear(context=context)
```

### Comparing `tutor-15.3.7/tutor/core/hooks/priorities.py` & `tutor-16.0.0/tutor/core/hooks/priorities.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/env.py` & `tutor-16.0.0/tutor/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     )
     # Template variables
     hooks.Filters.ENV_TEMPLATE_VARIABLES.add_items(
         [
             ("HOST_USER_ID", utils.get_user_id()),
             ("TUTOR_APP", __app__.replace("-", "_")),
             ("TUTOR_VERSION", __version__),
+            ("is_buildkit_enabled", utils.is_buildkit_enabled),
         ],
     )
 
 
 _prepare_environment()
 
 
@@ -157,23 +158,26 @@
         Render calls to {{ patch("...") }} in environment templates from plugin patches.
         """
         patches = []
         for patch in plugins.iter_patches(name):
             try:
                 patches.append(self.render_str(patch))
             except exceptions.TutorError:
-                fmt.echo_error(f"Error rendering patch '{name}': {patch}")
+                fmt.echo_error(f"Error rendering patch '{name}':\n{patch}")
                 raise
         rendered = separator.join(patches)
         if rendered:
             rendered += suffix
         return rendered
 
     def render_str(self, text: str) -> str:
-        template = self.environment.from_string(text)
+        try:
+            template = self.environment.from_string(text)
+        except jinja2.exceptions.TemplateSyntaxError as e:
+            raise exceptions.TutorError(f"Template syntax error: {e.args[0]}")
         return self.__render(template)
 
     def render_template(self, template_name: str) -> t.Union[str, bytes]:
         """
         Render a template file. Return the corresponding string. If it's a binary file
         (as indicated by its path), return bytes.
 
@@ -446,14 +450,15 @@
         "3": "ironwood",
         "10": "juniper",
         "11": "koa",
         "12": "lilac",
         "13": "maple",
         "14": "nutmeg",
         "15": "olive",
+        "16": "palm",
     }[version.split(".", maxsplit=1)[0]]
 
 
 def current_version(root: str) -> t.Optional[str]:
     """
     Return the current environment version. If the current environment has no version,
     return None.
@@ -517,15 +522,15 @@
 
 @hooks.Actions.PLUGIN_UNLOADED.add()
 def _delete_plugin_templates(plugin: str, root: str, _config: Config) -> None:
     """
     Delete plugin env files on unload.
     """
     targets = hooks.Filters.ENV_TEMPLATE_TARGETS.iterate_from_context(
-        hooks.Contexts.APP(plugin).name
+        hooks.Contexts.app(plugin).name
     )
     for src, dst in targets:
         path = pathjoin(root, dst.replace("/", os.sep), src.replace("/", os.sep))
         if os.path.exists(path):
             fmt.echo_info(f"    env - removing folder: {path}")
             try:
                 shutil.rmtree(path)
```

### Comparing `tutor-15.3.7/tutor/fmt.py` & `tutor-16.0.0/tutor/fmt.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/hooks/catalog.py` & `tutor-16.0.0/tutor/hooks/catalog.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,19 @@
 to generate part of the reference documentation.
 """
 from __future__ import annotations
 
 # The Tutor plugin system is licensed under the terms of the Apache 2.0 license.
 __license__ = "Apache 2.0"
 
-from typing import Any, Callable, Iterable
+from typing import Any, Callable, Iterable, Literal, Union
 
 import click
 
-from tutor.core.hooks import (
-    Action,
-    ActionTemplate,
-    Context,
-    ContextTemplate,
-    Filter,
-    FilterTemplate,
-    actions,
-    filters,
-)
+from tutor.core.hooks import Action, Context, Filter
 from tutor.types import Config
 
 __all__ = ["Actions", "Filters", "Contexts"]
 
 
 class Actions:
     """
@@ -60,76 +51,74 @@
     """
 
     #: Triggered whenever a "docker-compose start", "up" or "restart" command is executed.
     #:
     #: :parameter str root: project root.
     #: :parameter dict config: project configuration.
     #: :parameter str name: docker-compose project name.
-    COMPOSE_PROJECT_STARTED: Action[[str, Config, str]] = actions.get(
-        "compose:project:started"
-    )
+    COMPOSE_PROJECT_STARTED: Action[[str, Config, str]] = Action()
 
     #: Called whenever the core project is ready to run. This action is called as soon
     #: as possible. This is the right time to discover plugins, for instance. In
     #: particular, we auto-discover the following plugins:
     #:
     #: - Python packages that declare a "tutor.plugin.v0" entrypoint.
     #: - Python packages that declare a "tutor.plugin.v1" entrypoint.
     #: - YAML and Python plugins stored in ~/.local/share/tutor-plugins (as indicated by ``tutor plugins printroot``)
     #: - When running the binary version of Tutor, official plugins that ship with the binary are automatically discovered.
     #:
     #: Discovering a plugin is typically done by the Tutor plugin mechanism. Thus, plugin
     #: developers probably don't have to implement this action themselves.
     #:
     #: This action does not have any parameter.
-    CORE_READY: Action[[]] = actions.get("core:ready")
+    CORE_READY: Action[[]] = Action()
 
     #: Called just before triggering the job tasks of any ``... do <job>`` command.
     #:
     #: :parameter str job: job name.
     #: :parameter args: job positional arguments.
     #: :parameter kwargs: job named arguments.
-    DO_JOB: Action[[str, Any]] = actions.get("do:job")
+    DO_JOB: Action[[str, Any]] = Action()
 
     #: Triggered when a single plugin needs to be loaded. Only plugins that have previously been
     #: discovered can be loaded (see :py:data:`CORE_READY`).
     #:
     #: Plugins are typically loaded because they were enabled by the user; the list of
     #: plugins to enable is found in the project root (see
     #: :py:data:`PROJECT_ROOT_READY`).
     #:
     #: Most plugin developers will not have to implement this action themselves, unless
     #: they want to perform a specific action at the moment the plugin is enabled.
     #:
-    #: This action does not have any parameter.
-    PLUGIN_LOADED: ActionTemplate[[]] = actions.get_template("plugins:loaded:{0}")
+    #: :parameter str plugin: plugin name.
+    PLUGIN_LOADED: Action[[str]] = Action()
 
     #: Triggered after all plugins have been loaded. At this point the list of loaded
     #: plugins may be obtained from the :py:data:`Filters.PLUGINS_LOADED` filter.
     #:
     #: This action does not have any parameter.
-    PLUGINS_LOADED: Action[[]] = actions.get("plugins:loaded")
+    PLUGINS_LOADED: Action[[]] = Action()
 
     #: Triggered when a single plugin is unloaded. Only plugins that have previously been
     #: loaded can be unloaded (see :py:data:`PLUGIN_LOADED`).
     #:
     #: Plugins are typically unloaded because they were disabled by the user.
     #:
     #: Most plugin developers will not have to implement this action themselves, unless
     #: they want to perform a specific action at the moment the plugin is disabled.
     #:
     #: :parameter str plugin: plugin name.
     #: :parameter str root: absolute path to the project root.
     #: :parameter config: full project configuration
-    PLUGIN_UNLOADED: Action[str, str, Config] = actions.get("plugins:unloaded")
+    PLUGIN_UNLOADED: Action[str, str, Config] = Action()
 
     #: Called as soon as we have access to the Tutor project root.
     #:
     #: :parameter str root: absolute path to the project root.
-    PROJECT_ROOT_READY: Action[str] = actions.get("project:root:ready")
+    PROJECT_ROOT_READY: Action[str] = Action()
 
 
 class Filters:
     """
     Here are the names of all filters used across Tutor. (see
     :py:class:`tutor.core.hooks.Filter`) Filters are used to modify some data at
     specific points during the Tutor life cycle.
@@ -170,166 +159,124 @@
     The ``echo`` commands will then be run every time the "init" tasks are run, for
     instance during `tutor local launch`.
 
     For more information about how filters work, check out the
     :py:class:`tutor.core.hooks.Filter` API.
     """
 
+    #: Hostnames of user-facing applications.
+    #:
+    #: So far this filter is only used to inform the user of application urls after they have run ``launch``.
+    #:
+    #: :parameter list[str] hostnames: items from this list are templates that will be
+    #:   rendered by the environment.
+    #: :parameter str context_name: either "local" or "dev", depending on the calling context.
+    APP_PUBLIC_HOSTS: Filter[list[str], [Literal["local", "dev"]]] = Filter()
+
     #: List of command line interface (CLI) commands.
     #:
     #: :parameter list commands: commands are instances of ``click.Command``. They will
     #:   all be added as subcommands of the main ``tutor`` command.
-    CLI_COMMANDS: Filter[list[click.Command], []] = filters.get("cli:commands")
+    CLI_COMMANDS: Filter[list[click.Command], []] = Filter()
 
     #: List of `do ...` commands.
     #:
     #: :parameter list commands: see :py:data:`CLI_COMMANDS`. These commands will be
     #:   added as subcommands to the `local/dev/k8s do` commands. They must return a list of
     #:   ("service name", "service command") tuples. Each "service command" will be executed
     #:   in the "service" container, both in local, dev and k8s mode.
     CLI_DO_COMMANDS: Filter[
         list[Callable[[Any], Iterable[tuple[str, str]]]], []
-    ] = filters.get("cli:commands:do")
+    ] = Filter()
 
     #: List of initialization tasks (scripts) to be run in the `init` job. This job
     #: includes all database migrations, setting up, etc. To run some tasks before or
     #: after others, they should be assigned a different priority.
     #:
     #: :parameter list[tuple[str, str]] tasks: list of ``(service, task)`` tuples. Each
     #:   task is essentially a bash script to be run in the "service" container. Scripts
     #:   may contain Jinja markup, similar to templates.
-    CLI_DO_INIT_TASKS: Filter[list[tuple[str, str]], []] = filters.get(
-        "cli:commands:do:init"
-    )
-
-    #: DEPRECATED use :py:data:`CLI_DO_INIT_TASKS` instead.
-    #:
-    #: List of commands to be executed during initialization. These commands typically
-    #: include database migrations, setting feature flags, etc.
-    #:
-    #: :parameter list[tuple[str, tuple[str, ...]]] tasks: list of ``(service, path)`` tasks.
-    #:
-    #:     - ``service`` is the name of the container in which the task will be executed.
-    #:     - ``path`` is a tuple that corresponds to a template relative path.
-    #:       Example: ``("myplugin", "hooks", "myservice", "pre-init")`` (see :py:data:`IMAGES_BUILD`).
-    #:       The command to execute will be read from that template, after it is rendered.
-    COMMANDS_INIT: Filter[list[tuple[str, tuple[str, ...]]], []] = filters.get(
-        "commands:init"
-    )
+    CLI_DO_INIT_TASKS: Filter[list[tuple[str, str]], []] = Filter()
 
-    #: DEPRECATED use :py:data:`CLI_DO_INIT_TASKS` instead with a lower priority score.
-    #:
-    #: List of commands to be executed prior to initialization. These commands are run even
-    #: before the mysql databases are created and the migrations are applied.
+    #: List of folders to bind-mount in docker-compose containers, either in ``tutor local`` or ``tutor dev``.
     #:
-    #: :parameter list[tuple[str, tuple[str, ...]]] tasks: list of ``(service, path)``
-    #:   tasks. (see :py:data:`COMMANDS_INIT`).
-    COMMANDS_PRE_INIT: Filter[list[tuple[str, tuple[str, ...]]], []] = filters.get(
-        "commands:pre-init"
-    )
-
-    #: Same as :py:data:`COMPOSE_LOCAL_JOBS_TMP` but for the development environment.
-    COMPOSE_DEV_JOBS_TMP: Filter[Config, []] = filters.get("compose:dev-jobs:tmp")
-
-    #: Same as :py:data:`COMPOSE_LOCAL_TMP` but for the development environment.
-    COMPOSE_DEV_TMP: Filter[Config, []] = filters.get("compose:dev:tmp")
-
-    #: Same as :py:data:`COMPOSE_LOCAL_TMP` but for jobs
-    COMPOSE_LOCAL_JOBS_TMP: Filter[Config, []] = filters.get("compose:local-jobs:tmp")
-
-    #: Contents of the (local|dev)/docker-compose.tmp.yml files that will be generated at
-    #: runtime. This is used for instance to bind-mount folders from the host (see
-    #: :py:data:`COMPOSE_MOUNTS`)
+    #: This filter is for processing values of the ``MOUNTS`` setting such as::
     #:
-    #: :parameter dict[str, ...] docker_compose_tmp: values which will be serialized to local/docker-compose.tmp.yml.
-    #:   Keys and values will be rendered before saving, such that you may include ``{{ ... }}`` statements.
-    COMPOSE_LOCAL_TMP: Filter[Config, []] = filters.get("compose:local:tmp")
-
-    #: List of folders to bind-mount in docker-compose containers, either in ``tutor local`` or ``tutor dev``.
+    #:     tutor mounts add /path/to/edx-platform
     #:
-    #: Many ``tutor local`` and ``tutor dev`` commands support ``--mounts`` options
-    #: that allow plugins to define custom behaviour at runtime. For instance
-    #: ``--mount=/path/to/edx-platform`` would cause this host folder to be
-    #: bind-mounted in different containers (lms, lms-worker, cms, cms-worker) at the
+    #: In this example, this host folder would be bind-mounted in different containers
+    #: (lms, lms-worker, cms, cms-worker, lms-job, cms-job) at the
     #: /openedx/edx-platform location. Plugin developers may implement this filter to
     #: define custom behaviour when mounting folders that relate to their plugins. For
-    #: instance, the ecommerce plugin may process the ``--mount=/path/to/ecommerce``
-    #: option.
+    #: instance, the ecommerce plugin may process the ``/path/to/ecommerce`` value.
+    #:
+    #: To also bind-mount these folder at build time, implement also the
+    #: :py:data:`IMAGES_BUILD_MOUNTS` filter.
     #:
     #: :parameter list[tuple[str, str]] mounts: each item is a ``(service, path)``
     #:   tuple, where ``service`` is the name of the docker-compose service and ``path`` is
     #:   the location in the container where the folder should be bind-mounted. Note: the
     #:   path must be slash-separated ("/"). Thus, do not use ``os.path.join`` to generate
     #:   the ``path`` because it will fail on Windows.
     #: :parameter str name: basename of the host-mounted folder. In the example above,
     #:   this is "edx-platform". When implementing this filter you should check this name to
-    #:   conditionnally add mounts.
-    COMPOSE_MOUNTS: Filter[list[tuple[str, str]], [str]] = filters.get("compose:mounts")
+    #:   conditionally add mounts.
+    COMPOSE_MOUNTS: Filter[list[tuple[str, str]], [str]] = Filter()
 
     #: Declare new default configuration settings that don't necessarily have to be saved in the user
     #: ``config.yml`` file. Default settings may be overridden with ``tutor config save --set=...``, in which
     #: case they will automatically be added to ``config.yml``.
     #:
     #: :parameter list[tuple[str, ...]] items: list of (name, value) new settings. All
     #:    new entries must be prefixed with the plugin name in all-caps.
-    CONFIG_DEFAULTS: Filter[list[tuple[str, Any]], []] = filters.get("config:defaults")
+    CONFIG_DEFAULTS: Filter[list[tuple[str, Any]], []] = Filter()
 
     #: Modify existing settings, either from Tutor core or from other plugins. Beware not to override any
     #: important setting, such as passwords! Overridden setting values will be printed to stdout when the plugin
     #: is disabled, such that users have a chance to back them up.
     #:
     #: :parameter list[tuple[str, ...]] items: list of (name, value) settings.
-    CONFIG_OVERRIDES: Filter[list[tuple[str, Any]], []] = filters.get(
-        "config:overrides"
-    )
+    CONFIG_OVERRIDES: Filter[list[tuple[str, Any]], []] = Filter()
 
     #: Declare unique configuration settings that must be saved in the user ``config.yml`` file. This is where
     #: you should declare passwords and randomly-generated values that are different from one environment to the next.
     #:
     #: :parameter list[tuple[str, ...]] items: list of (name, value) new settings. All
     #:   names must be prefixed with the plugin name in all-caps.
-    CONFIG_UNIQUE: Filter[list[tuple[str, Any]], []] = filters.get("config:unique")
+    CONFIG_UNIQUE: Filter[list[tuple[str, Any]], []] = Filter()
 
     #: Use this filter to modify the ``docker build`` command. For instance, to replace
     #: the ``build`` subcommand by ``buildx build``.
     #:
     #: :parameter list[str] command: the full build command, including options and
     #:   arguments. Note that these arguments do not include the leading ``docker`` command.
-    DOCKER_BUILD_COMMAND: Filter[list[str], []] = filters.get("docker:build:command")
+    DOCKER_BUILD_COMMAND: Filter[list[str], []] = Filter()
 
-    #: List of patches that should be inserted in a given location of the templates. The
-    #: filter name must be formatted with the patch name.
-    #: This filter is not so convenient and plugin developers will probably
-    #: prefer :py:data:`ENV_PATCHES`.
-    #:
-    #: :parameter list[str] patches: each item is the unrendered patch content.
-    ENV_PATCH: FilterTemplate[list[str], []] = filters.get_template("env:patches:{0}")
-
-    #: List of patches that should be inserted in a given location of the templates. This is very similar to :py:data:`ENV_PATCH`, except that the patch is added as a ``(name, content)`` tuple.
+    #: List of patches that should be inserted in a given location of the templates.
     #:
     #: :parameter list[tuple[str, str]] patches: pairs of (name, content) tuples. Use this
     #:   filter to modify the Tutor templates.
-    ENV_PATCHES: Filter[list[tuple[str, str]], []] = filters.get("env:patches")
+    ENV_PATCHES: Filter[list[tuple[str, str]], []] = Filter()
 
     #: List of template path patterns to be ignored when rendering templates to the project root. By default, we ignore:
     #:
     #: - hidden files (``.*``)
     #: - ``__pycache__`` directories and ``*.pyc`` files
     #: - "partials" directories.
     #:
     #: Ignored patterns are overridden by include patterns; see :py:data:`ENV_PATTERNS_INCLUDE`.
     #:
     #: :parameter list[str] patterns: list of regular expression patterns. E.g: ``r"(.*/)?ignored_file_name(/.*)?"``.
-    ENV_PATTERNS_IGNORE: Filter[list[str], []] = filters.get("env:patterns:ignore")
+    ENV_PATTERNS_IGNORE: Filter[list[str], []] = Filter()
 
     #: List of template path patterns to be included when rendering templates to the project root.
     #: Patterns from this list will take priority over the patterns from :py:data:`ENV_PATTERNS_IGNORE`.
     #:
     #: :parameter list[str] patterns: list of regular expression patterns. See :py:data:`ENV_PATTERNS_IGNORE`.
-    ENV_PATTERNS_INCLUDE: Filter[list[str], []] = filters.get("env:patterns:include")
+    ENV_PATTERNS_INCLUDE: Filter[list[str], []] = Filter()
 
     #: List of `Jinja2 filters <https://jinja.palletsprojects.com/en/latest/templates/#filters>`__ that will be
     #: available in templates. Jinja2 filters are basically functions that can be used
     #: as follows within templates::
     #:
     #:    {{ "somevalue"|my_filter }}
     #:
@@ -352,119 +299,144 @@
     #:
     #:     {% for file in "apps/myplugin"|walk_templates %}
     #:     ...
     #:     {% endfor %}
     #:
     #: :parameter filters: list of (name, function) tuples. The function signature
     #:   should correspond to its usage in templates.
-    ENV_TEMPLATE_FILTERS: Filter[
-        list[tuple[str, Callable[..., Any]]], []
-    ] = filters.get("env:templates:filters")
+    ENV_TEMPLATE_FILTERS: Filter[list[tuple[str, Callable[..., Any]]], []] = Filter()
 
     #: List of all template root folders.
     #:
     #: :parameter list[str] templates_root: absolute paths to folders which contain templates.
     #:   The templates in these folders will then be accessible by the environment
     #:   renderer using paths that are relative to their template root.
-    ENV_TEMPLATE_ROOTS: Filter[list[str], []] = filters.get("env:templates:roots")
+    ENV_TEMPLATE_ROOTS: Filter[list[str], []] = Filter()
 
     #: List of template source/destination targets.
     #:
     #: :parameter list[tuple[str, str]] targets: list of (source, destination) pairs.
     #:   Each source is a path relative to one of the template roots, and each destination
     #:   is a path relative to the environment root. For instance: adding ``("c/d",
     #:   "a/b")`` to the filter will cause all files from "c/d" to be rendered to the ``a/b/c/d``
     #:   subfolder.
-    ENV_TEMPLATE_TARGETS: Filter[list[tuple[str, str]], []] = filters.get(
-        "env:templates:targets"
-    )
+    ENV_TEMPLATE_TARGETS: Filter[list[tuple[str, str]], []] = Filter()
 
     #: List of extra variables to be included in all templates.
     #:
+    #: Out of the box, this filter will include all configuration settings, but also the following:
+    #:
+    #: - `HOST_USER_ID`: the numerical ID of the user on the host.
+    #: - `TUTOR_APP`: the app name ("tutor" by default), used to determine the dev/local project names.
+    #: - `TUTOR_VERSION`: the current version of Tutor.
+    #: - `is_buildkit_enabled`: a boolean function that indicates whether BuildKit is available on the host.
+    #: - `iter_values_named`: a function to iterate on variables that start or end with a given string.
+    #: - `iter_mounts`: a function that yields compose-compatible bind-mounts for any given service.
+    #: - `patch`: a function to incorporate extra content into a template.
+    #:
     #: :parameter filters: list of (name, value) tuples.
-    ENV_TEMPLATE_VARIABLES: Filter[list[tuple[str, Any]], []] = filters.get(
-        "env:templates:variables"
-    )
+    ENV_TEMPLATE_VARIABLES: Filter[list[tuple[str, Any]], []] = Filter()
 
     #: List of images to be built when we run ``tutor images build ...``.
     #:
     #: :parameter list[tuple[str, tuple[str, ...], str, tuple[str, ...]]] tasks: list of ``(name, path, tag, args)`` tuples.
     #:
     #:    - ``name`` is the name of the image, as in ``tutor images build myimage``.
-    #:    - ``path`` is the relative path to the folder that contains the Dockerfile.
+    #:    - ``path`` is the relative path to the folder that contains the Dockerfile. This can be either a string or a tuple of strings.
     #:      For instance ``("myplugin", "build", "myservice")`` indicates that the template will be read from
-    #:      ``myplugin/build/myservice/Dockerfile``
+    #:      ``myplugin/build/myservice/Dockerfile``. This argument value would be equivalent to "myplugin/build/myservice".
     #:    - ``tag`` is the Docker tag that will be applied to the image. It will be
     #:      rendered at runtime with the user configuration. Thus, the image tag could
     #:      be ``"{{ DOCKER_REGISTRY }}/myimage:{{ TUTOR_VERSION }}"``.
     #:    - ``args`` is a list of arguments that will be passed to ``docker build ...``.
     #: :parameter Config config: user configuration.
     IMAGES_BUILD: Filter[
-        list[tuple[str, tuple[str, ...], str, tuple[str, ...]]], [Config]
-    ] = filters.get("images:build")
+        list[tuple[str, Union[str, tuple[str, ...]], str, tuple[str, ...]]], [Config]
+    ] = Filter()
+
+    #: List of image names which must be built prior to launching the platform. These
+    #: images will be built on launch, in "dev" and "local" mode (but not in Kubernetes).
+    #:
+    #: :parameter list[str] names: list of image names.
+    #: :parameter str context_name: either "local" or "dev", depending on the calling context.
+    IMAGES_BUILD_REQUIRED: Filter[list[str], [Literal["local", "dev"]]] = Filter()
+
+    #: List of host directories to be automatically bind-mounted in Docker images at
+    #: build time. For instance, this is useful to build Docker images using a custom
+    #: repository on the host.
+    #:
+    #: This filter works similarly to the :py:data:`COMPOSE_MOUNTS` filter, with a few differences.
+    #:
+    #: :parameter list[tuple[str, str]] mounts: each item is a pair of ``(name, value)``
+    #:   used to generate a build context at build time. See the corresponding `Docker
+    #:   documentation <https://docs.docker.com/engine/reference/commandline/buildx_build/#build-context>`__.
+    #:   The following option will be added to the ``docker buildx build`` command:
+    #:   ``--build-context={name}={value}``. If the Dockerfile contains a "name" stage, then
+    #:   that stage will be replaced by the corresponding directory on the host.
+    #: :parameter str name: full path to the host-mounted folder. As opposed to
+    #:   :py:data:`COMPOSE_MOUNTS`, this is not just the basename, but the full path. When
+    #:   implementing this filter you should check this path (for instance: with
+    #:   ``os.path.basename(path)``) to conditionally add mounts.
+    IMAGES_BUILD_MOUNTS: Filter[list[tuple[str, str]], [str]] = Filter()
 
     #: List of images to be pulled when we run ``tutor images pull ...``.
     #:
     #: :parameter list[tuple[str, str]] tasks: list of ``(name, tag)`` tuples.
     #:
     #:    - ``name`` is the name of the image, as in ``tutor images pull myimage``.
     #:    - ``tag`` is the Docker tag that will be applied to the image. (see :py:data:`IMAGES_BUILD`).
     #: :parameter Config config: user configuration.
-    IMAGES_PULL: Filter[list[tuple[str, str]], [Config]] = filters.get("images:pull")
+    IMAGES_PULL: Filter[list[tuple[str, str]], [Config]] = Filter()
 
     #: List of images to be pushed when we run ``tutor images push ...``.
     #: Parameters are the same as for :py:data:`IMAGES_PULL`.
-    IMAGES_PUSH: Filter[list[tuple[str, str]], [Config]] = filters.get("images:push")
+    IMAGES_PUSH: Filter[list[tuple[str, str]], [Config]] = Filter()
 
     #: List of plugin indexes that are loaded when we run `tutor plugins update`. By
     #: default, the plugin indexes are stored in the user configuration. This filter makes
     #: it possible to extend and modify this list with plugins.
     #:
     #: :parameter list[str] indexes: list of index URLs. Remember that entries further
     #:   in the list have priority.
-    PLUGIN_INDEXES: Filter[list[str], []] = filters.get("plugins:indexes:entries")
+    PLUGIN_INDEXES: Filter[list[str], []] = Filter()
 
     #: Filter to modify the url of a plugin index url. This is convenient to alias
     #: plugin indexes with a simple name, such as "main" or "contrib".
     #:
     #: :parameter str url: value passed to the `index add/remove` commands.
-    PLUGIN_INDEX_URL: Filter[str, []] = filters.get("plugins:indexes:url")
+    PLUGIN_INDEX_URL: Filter[str, []] = Filter()
 
     #: When installing an entry from a plugin index, the plugin data from the index will
     #: go through this filter before it is passed along to `pip install`. Thus, this is a
     #: good place to add custom authentication when you need to install from a private
     #: index.
     #:
     #: :parameter dict[str, str] plugin: the dict entry from the plugin index. It
     #:   includes an additional "index" key which contains the plugin index URL.
-    PLUGIN_INDEX_ENTRY_TO_INSTALL: Filter[dict[str, str], []] = filters.get(
-        "plugins:indexes:entries:install"
-    )
+    PLUGIN_INDEX_ENTRY_TO_INSTALL: Filter[dict[str, str], []] = Filter()
 
     #: Information about each installed plugin, including its version.
     #: Keep this information to a single line for easier parsing by 3rd-party scripts.
     #:
     #: :param list[tuple[str, str]] versions: each pair is a ``(plugin, info)`` tuple.
-    PLUGINS_INFO: Filter[list[tuple[str, str]], []] = filters.get(
-        "plugins:installed:versions"
-    )
+    PLUGINS_INFO: Filter[list[tuple[str, str]], []] = Filter()
 
     #: List of installed plugins. In order to be added to this list, a plugin must first
     #: be discovered (see :py:data:`Actions.CORE_READY`).
     #:
     #: :param list[str] plugins: plugin developers probably don't have to implement this
     #:   filter themselves, but they can apply it to check for the presence of other
     #:   plugins.
-    PLUGINS_INSTALLED: Filter[list[str], []] = filters.get("plugins:installed")
+    PLUGINS_INSTALLED: Filter[list[str], []] = Filter()
 
     #: List of loaded plugins.
     #:
     #: :param list[str] plugins: plugin developers probably don't have to modify this
     #:   filter themselves, but they can apply it to check whether other plugins are enabled.
-    PLUGINS_LOADED: Filter[list[str], []] = filters.get("plugins:loaded")
+    PLUGINS_LOADED: Filter[list[str], []] = Filter()
 
 
 class Contexts:
     """
     Here we list all the :py:class:`contexts <tutor.core.hooks.Context>` that are used across Tutor. It is not expected that
     plugin developers will ever need to use contexts. But if you do, this is how it
     should be done::
@@ -476,18 +448,24 @@
             ...
 
         # Apply only the hook callbacks that were created within SOME_CONTEXT
         hooks.Actions.MY_ACTION.do_from_context(str(hooks.Contexts.SOME_CONTEXT))
         hooks.Filters.MY_FILTER.apply_from_context(hooks.Contexts.SOME_CONTEXT.name)
     """
 
-    #: We enter this context whenever we create hooks for a specific application or :
-    #: plugin. For instance, plugin "myplugin" will be enabled within the "app:myplugin"
-    #: context.
-    APP = ContextTemplate("app:{0}")
+    #: Dictionary of name/contexts. Each value is a context that we enter whenever we
+    #: create hooks for a specific application or : : plugin. For instance, plugin
+    #: "myplugin" will be enabled within the "app:myplugin" : context.
+    APP: dict[str, Context] = {}
+
+    @classmethod
+    def app(cls, name: str) -> Context:
+        if name not in cls.APP:
+            cls.APP[name] = Context(f"app:{name}")
+        return cls.APP[name]
 
     #: Plugins will be installed and enabled within this context.
     PLUGINS = Context("plugins")
 
     #: YAML-formatted v0 plugins will be installed within this context.
     PLUGINS_V0_YAML = Context("plugins:v0:yaml")
```

### Comparing `tutor-15.3.7/tutor/interactive.py` & `tutor-16.0.0/tutor/interactive.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/plugins/__init__.py` & `tutor-16.0.0/tutor/plugins/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,32 @@
 
 from tutor import exceptions, fmt, hooks
 from tutor.types import Config, get_typed
 
 # Import modules to trigger hook creation
 from . import v0, v1
 
+# Cache of plugin patches, for efficiency
+ENV_PATCHES_DICT: dict[str, list[str]] = {}
+
 
 @hooks.Actions.PLUGINS_LOADED.add()
 def _convert_plugin_patches() -> None:
     """
     Some patches are added as (name, content) tuples with the ENV_PATCHES
-    filter. We convert these patches to add them to ENV_PATCH. This makes it
+    filter. We convert these patches to add them to ENV_PATCHES_DICT. This makes it
     easier for end-user to declare patches, and it's more performant.
 
     This action is run after plugins have been loaded.
     """
+    ENV_PATCHES_DICT.clear()
     patches: t.Iterable[tuple[str, str]] = hooks.Filters.ENV_PATCHES.iterate()
     for name, content in patches:
-        hooks.Filters.ENV_PATCH(name).add_item(content)
+        ENV_PATCHES_DICT.setdefault(name, [])
+        ENV_PATCHES_DICT[name].append(content)
 
 
 def is_installed(name: str) -> bool:
     """
     Return true if the plugin is installed.
     """
     return name in iter_installed()
@@ -85,16 +90,16 @@
 
     Loading a plugin is done within a context, such that we can remove all hooks when a
     plugin is disabled, or during unit tests.
     """
     if not is_installed(name):
         raise exceptions.TutorError(f"plugin '{name}' is not installed.")
     with hooks.Contexts.PLUGINS.enter():
-        with hooks.Contexts.APP(name).enter():
-            hooks.Actions.PLUGIN_LOADED(name).do()
+        with hooks.Contexts.app(name).enter():
+            hooks.Actions.PLUGIN_LOADED.do(name)
             hooks.Filters.PLUGINS_LOADED.add_item(name)
 
 
 def iter_loaded() -> t.Iterator[str]:
     """
     Iterate on the list of loaded plugin names, sorted in alphabetical order.
 
@@ -105,20 +110,20 @@
     yield from sorted(set(plugins))
 
 
 def iter_patches(name: str) -> t.Iterator[str]:
     """
     Yields: patch (str)
     """
-    yield from hooks.Filters.ENV_PATCH(name).iterate()
+    yield from ENV_PATCHES_DICT.get(name, [])
 
 
 def unload(plugin: str) -> None:
     """
     Remove all filters and actions associated to a given plugin.
     """
-    hooks.clear_all(context=hooks.Contexts.APP(plugin).name)
+    hooks.clear_all(context=hooks.Contexts.app(plugin).name)
 
 
 @hooks.Actions.PLUGIN_UNLOADED.add(priority=50)
 def _unload_on_disable(plugin: str, _root: str, _config: Config) -> None:
     unload(plugin)
```

### Comparing `tutor-15.3.7/tutor/plugins/base.py` & `tutor-16.0.0/tutor/plugins/base.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/plugins/indexes.py` & `tutor-16.0.0/tutor/plugins/indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/plugins/v0.py` & `tutor-16.0.0/tutor/plugins/v0.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,18 @@
         # Add itself to the list of installed plugins
         hooks.Filters.PLUGINS_INSTALLED.add_item(self.name)
 
         # Add plugin version
         hooks.Filters.PLUGINS_INFO.add_item((self.name, self._version() or ""))
 
         # Create actions and filters on load
-        hooks.Actions.PLUGIN_LOADED(self.name).add()(self.__load)
+        @hooks.Actions.PLUGIN_LOADED.add()
+        def _load_plugin(name: str) -> None:
+            if name == self.name:
+                self.__load()
 
     def __load(self) -> None:
         """
         On loading a plugin, we create all the required actions and filters.
 
         Note that this method is quite costly. Thus it is important that as little is
         done as part of installing the plugin. For instance, we should not import
```

### Comparing `tutor-15.3.7/tutor/plugins/v1.py` & `tutor-16.0.0/tutor/plugins/v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,24 +39,25 @@
     # Add plugin to the list of installed plugins
     hooks.Filters.PLUGINS_INSTALLED.add_item(name)
 
     # Add plugin information
     hooks.Filters.PLUGINS_INFO.add_item((name, path))
 
     # Import module on enable
-    load_plugin_action = hooks.Actions.PLUGIN_LOADED(name)
-
-    @load_plugin_action.add()
-    def load() -> None:
-        # https://docs.python.org/3/library/importlib.html#importing-a-source-file-directly
-        spec = importlib.util.spec_from_file_location("tutor.plugin.v1.{name}", path)
-        if spec is None or spec.loader is None:
-            raise ValueError("Plugin could not be found: {path}")
-        module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(module)
+    @hooks.Actions.PLUGIN_LOADED.add()
+    def load(plugin_name: str) -> None:
+        if name == plugin_name:
+            # https://docs.python.org/3/library/importlib.html#importing-a-source-file-directly
+            spec = importlib.util.spec_from_file_location(
+                "tutor.plugin.v1.{name}", path
+            )
+            if spec is None or spec.loader is None:
+                raise ValueError("Plugin could not be found: {path}")
+            module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(module)
 
 
 def discover_package(entrypoint: pkg_resources.EntryPoint) -> None:
     """
     Install a plugin from a python package.
     """
     name = entrypoint.name
@@ -66,12 +67,11 @@
 
     # Add plugin information
     if entrypoint.dist is None:
         raise ValueError(f"Could not read plugin version: {name}")
     hooks.Filters.PLUGINS_INFO.add_item((name, entrypoint.dist.version))
 
     # Import module on enable
-    load_plugin_action = hooks.Actions.PLUGIN_LOADED(name)
-
-    @load_plugin_action.add()
-    def load() -> None:
-        entrypoint.load()
+    @hooks.Actions.PLUGIN_LOADED.add()
+    def load(plugin_name: str) -> None:
+        if name == plugin_name:
+            entrypoint.load()
```

### Comparing `tutor-15.3.7/tutor/tasks.py` & `tutor-16.0.0/tutor/tasks.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/caddy/Caddyfile` & `tutor-16.0.0/tutor/templates/apps/caddy/Caddyfile`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/config/cms.env.yml` & `tutor-16.0.0/tutor/templates/apps/openedx/config/cms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/config/lms.env.yml` & `tutor-16.0.0/tutor/templates/apps/openedx/config/lms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/config/partials/auth.yml` & `tutor-16.0.0/tutor/templates/apps/openedx/config/partials/auth.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/settings/cms/development.py` & `tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/settings/cms/production.py` & `tutor-16.0.0/tutor/templates/apps/openedx/settings/cms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/settings/lms/development.py` & `tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/settings/lms/production.py` & `tutor-16.0.0/tutor/templates/apps/openedx/settings/lms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/settings/partials/common_all.py` & `tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_all.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,16 +114,18 @@
     "STORAGE_TYPE": "",
     "STORAGE_KWARGS": {
         "base_url": "/media/grades/",
         "location": "/openedx/media/grades",
     },
 }
 
+# ORA2
 ORA2_FILEUPLOAD_BACKEND = "filesystem"
 ORA2_FILEUPLOAD_ROOT = "/openedx/data/ora2"
+FILE_UPLOAD_STORAGE_BUCKET_NAME = "openedxuploads"
 ORA2_FILEUPLOAD_CACHE_NAME = "ora2-storage"
 
 # Change syslog-based loggers which don't work inside docker containers
 LOGGING["handlers"]["local"] = {
     "class": "logging.handlers.WatchedFileHandler",
     "filename": os.path.join(LOG_DIR, "all.log"),
     "formatter": "standard",
@@ -131,26 +133,29 @@
 LOGGING["handlers"]["tracking"] = {
     "level": "DEBUG",
     "class": "logging.handlers.WatchedFileHandler",
     "filename": os.path.join(LOG_DIR, "tracking.log"),
     "formatter": "standard",
 }
 LOGGING["loggers"]["tracking"]["handlers"] = ["console", "local", "tracking"]
+
 # Silence some loggers (note: we must attempt to get rid of these when upgrading from one release to the next)
+LOGGING["loggers"]["blockstore.apps.bundles.storage"] = {"handlers": ["console"], "level": "WARNING"}
 
+# These warnings are visible in simple commands and init tasks
 import warnings
 from django.utils.deprecation import RemovedInDjango40Warning, RemovedInDjango41Warning
 warnings.filterwarnings("ignore", category=RemovedInDjango40Warning)
 warnings.filterwarnings("ignore", category=RemovedInDjango41Warning)
-warnings.filterwarnings("ignore", category=DeprecationWarning, module="lms.djangoapps.course_wiki.plugins.markdownedx.wiki_plugin")
 warnings.filterwarnings("ignore", category=DeprecationWarning, module="wiki.plugins.links.wiki_plugin")
 warnings.filterwarnings("ignore", category=DeprecationWarning, module="boto.plugin")
 warnings.filterwarnings("ignore", category=DeprecationWarning, module="botocore.vendored.requests.packages.urllib3._collections")
-warnings.filterwarnings("ignore", category=DeprecationWarning, module="storages.backends.s3boto")
-warnings.filterwarnings("ignore", category=DeprecationWarning, module="openedx.core.types.admin")
+warnings.filterwarnings("ignore", category=DeprecationWarning, module="pkg_resources")
+warnings.filterwarnings("ignore", category=DeprecationWarning, module="fs")
+warnings.filterwarnings("ignore", category=DeprecationWarning, module="fs.opener")
 SILENCED_SYSTEM_CHECKS = ["2_0.W001", "fields.W903"]
 
 # Email
 EMAIL_USE_SSL = {{ SMTP_USE_SSL }}
 # Forward all emails from edX's Automated Communication Engine (ACE) to django.
 ACE_ENABLED_CHANNELS = ["django_email"]
 ACE_CHANNEL_DEFAULT_EMAIL = "django_email"
```

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/settings/partials/common_cms.py` & `tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_cms.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/apps/openedx/settings/partials/common_lms.py` & `tutor-16.0.0/tutor/templates/apps/openedx/settings/partials/common_lms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% include "apps/openedx/settings/partials/common_all.py" %}
 
 ######## Common LMS settings
 LOGIN_REDIRECT_WHITELIST = ["{{ CMS_HOST }}"]
 
 # Better layout of honor code/tos links during registration
-REGISTRATION_EXTRA_FIELDS["terms_of_service"] = "required"
+REGISTRATION_EXTRA_FIELDS["terms_of_service"] = "hidden"
 REGISTRATION_EXTRA_FIELDS["honor_code"] = "hidden"
 
 # Fix media files paths
 PROFILE_IMAGE_BACKEND["options"]["location"] = os.path.join(
     MEDIA_ROOT, "profile-images/"
 )
 
@@ -32,19 +32,14 @@
 
 # Caching
 CACHES["staticfiles"] = {
     "KEY_PREFIX": "staticfiles_lms",
     "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
     "LOCATION": "staticfiles_lms",
 }
-CACHES["ora2-storage"] = {
-    "KEY_PREFIX": "ora2-storage",
-    "BACKEND": "django_redis.cache.RedisCache",
-    "LOCATION": "redis://{% if REDIS_USERNAME and REDIS_PASSWORD %}{{ REDIS_USERNAME }}:{{ REDIS_PASSWORD }}{% endif %}@{{ REDIS_HOST }}:{{ REDIS_PORT }}/{{ OPENEDX_CACHE_REDIS_DB }}",
-}
 
 # Create folders if necessary
 for folder in [DATA_DIR, LOG_DIR, MEDIA_ROOT, STATIC_ROOT_BASE, ORA2_FILEUPLOAD_ROOT]:
     if not os.path.exists(folder):
         os.makedirs(folder, exist_ok=True)
 
 {{ patch("openedx-lms-common-settings") }}
```

### Comparing `tutor-15.3.7/tutor/templates/apps/redis/redis.conf` & `tutor-16.0.0/tutor/templates/apps/redis/redis.conf`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/build/openedx/bin/openedx-assets` & `tutor-16.0.0/tutor/templates/build/openedx/bin/openedx-assets`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/build/openedx/bin/site-configuration` & `tutor-16.0.0/tutor/templates/build/openedx/bin/site-configuration`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/config/base.yml` & `tutor-16.0.0/tutor/templates/config/base.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/config/defaults.yml` & `tutor-16.0.0/tutor/templates/config/defaults.yml`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 CMS_OAUTH2_KEY_SSO_DEV: "cms-sso-dev"
 CONTACT_EMAIL: "contact@{{ LMS_HOST }}"
 DEV_PROJECT_NAME: "{{ TUTOR_APP }}_dev"
 DOCKER_COMPOSE_VERSION: "3.7"
 DOCKER_REGISTRY: "docker.io/"
 DOCKER_IMAGE_OPENEDX: "{{ DOCKER_REGISTRY }}overhangio/openedx:{{ TUTOR_VERSION }}"
 DOCKER_IMAGE_OPENEDX_DEV: "openedx-dev:{{ TUTOR_VERSION }}"
-DOCKER_IMAGE_CADDY: "docker.io/caddy:2.6.3"
-DOCKER_IMAGE_ELASTICSEARCH: "docker.io/elasticsearch:7.10.1"
-DOCKER_IMAGE_MONGODB: "docker.io/mongo:4.2.24"
-DOCKER_IMAGE_MYSQL: "docker.io/mysql:5.7.35"
+DOCKER_IMAGE_CADDY: "docker.io/caddy:2.6.4"
+DOCKER_IMAGE_ELASTICSEARCH: "docker.io/elasticsearch:7.17.9"
+DOCKER_IMAGE_MONGODB: "docker.io/mongo:4.4.22"
+DOCKER_IMAGE_MYSQL: "docker.io/mysql:8.0.33"
 DOCKER_IMAGE_PERMISSIONS: "{{ DOCKER_REGISTRY }}overhangio/openedx-permissions:{{ TUTOR_VERSION }}"
-DOCKER_IMAGE_REDIS: "docker.io/redis:6.2.6"
-DOCKER_IMAGE_SMTP: "docker.io/devture/exim-relay:4.95-r0-2"
+DOCKER_IMAGE_REDIS: "docker.io/redis:7.0.11"
+DOCKER_IMAGE_SMTP: "docker.io/devture/exim-relay:4.96-r1-0"
 EDX_PLATFORM_REPOSITORY: "https://github.com/openedx/edx-platform.git"
 EDX_PLATFORM_VERSION: "{{ OPENEDX_COMMON_VERSION }}"
 ELASTICSEARCH_HOST: "elasticsearch"
 ELASTICSEARCH_PORT: 9200
 ELASTICSEARCH_SCHEME: "http"
 ELASTICSEARCH_HEAP_SIZE: 1g
 ENABLE_HTTPS: false
@@ -39,38 +39,37 @@
 MONGODB_HOST: "mongodb"
 MONGODB_DATABASE: "openedx"
 MONGODB_PORT: 27017
 MONGODB_USERNAME: ""
 MONGODB_PASSWORD: ""
 MONGODB_REPLICA_SET: ""
 MONGODB_USE_SSL: false
+MOUNTS: []
 OPENEDX_AWS_ACCESS_KEY: ""
 OPENEDX_AWS_SECRET_ACCESS_KEY: ""
 OPENEDX_CACHE_REDIS_DB: 1
 OPENEDX_CELERY_REDIS_DB: 0
 OPENEDX_CMS_UWSGI_WORKERS: 2
 OPENEDX_LMS_UWSGI_WORKERS: 2
 OPENEDX_MYSQL_DATABASE: "openedx"
 OPENEDX_MYSQL_USERNAME: "openedx"
-OPENEDX_COMMON_VERSION: "open-release/olive.4"
+OPENEDX_COMMON_VERSION: "open-release/palm.1"
 OPENEDX_EXTRA_PIP_REQUIREMENTS:
-  - "openedx-scorm-xblock>=15.0.0,<16.0.0"
+  - "openedx-scorm-xblock>=16.0.0,<17.0.0"
 MYSQL_HOST: "mysql"
 MYSQL_PORT: 3306
 MYSQL_ROOT_USERNAME: "root"
 NPM_REGISTRY: "https://registry.npmjs.org/"
 PLATFORM_NAME: "My Open edX"
 PREVIEW_LMS_HOST: "preview.{{ LMS_HOST }}"
 REDIS_HOST: "redis"
 REDIS_PORT: 6379
 REDIS_USERNAME: ""
 REDIS_PASSWORD: ""
-RUN_CMS: true
 RUN_ELASTICSEARCH: true
-RUN_LMS: true
 RUN_MONGODB: true
 RUN_MYSQL: true
 RUN_REDIS: true
 RUN_SMTP: true
 SMTP_HOST: "smtp"
 SMTP_PORT: 8025
 SMTP_USERNAME: ""
```

### Comparing `tutor-15.3.7/tutor/templates/dev/docker-compose.jobs.yml` & `tutor-16.0.0/tutor/templates/dev/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/dev/docker-compose.yml` & `tutor-16.0.0/tutor/templates/dev/docker-compose.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 version: "{{ DOCKER_COMPOSE_VERSION }}"
 
 x-openedx-service:
   &openedx-service
   image: {{ DOCKER_IMAGE_OPENEDX_DEV }}
-  build:
-    context: ../build/openedx/
-    target: development
-    args:
-      # Note that we never build the openedx-dev image with root user ID, as it would simply fail.
-      APP_USER_ID: "{{ HOST_USER_ID or 1000 }}"
   stdin_open: true
   tty: true
   volumes:
     # Settings & config
     - ../apps/openedx/settings/lms:/openedx/edx-platform/lms/envs/tutor:ro
     - ../apps/openedx/settings/cms:/openedx/edx-platform/cms/envs/tutor:ro
     - ../apps/openedx/config:/openedx/config:ro
     # theme files
     - ../build/openedx/themes:/openedx/themes
     # editable requirements
     - ../build/openedx/requirements:/openedx/requirements
 
 services:
-  lms-permissions:
-    command: ["{{ HOST_USER_ID }}", "/openedx/data", "/openedx/media"]
-
-  cms-permissions:
-    command: ["{{ HOST_USER_ID }}", "/openedx/data", "/openedx/media"]
+  permissions:
+    environment:
+      OPENEDX_USER_ID: "{{ HOST_USER_ID }}"
 
   lms:
     <<: *openedx-service
     command: ./manage.py lms runserver 0.0.0.0:8000
     environment:
         DJANGO_SETTINGS_MODULE: lms.envs.tutor.development
     ports:
```

### Comparing `tutor-15.3.7/tutor/templates/jobs/init/lms.sh` & `tutor-16.0.0/tutor/templates/jobs/init/lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/jobs/init/mounted-edx-platform.sh` & `tutor-16.0.0/tutor/templates/jobs/init/mounted-edx-platform.sh`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/jobs/init/mysql.sh` & `tutor-16.0.0/tutor/templates/jobs/init/mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/k8s/deployments.yml` & `tutor-16.0.0/tutor/templates/k8s/deployments.yml`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
           configMap:
             name: caddy-config
         {%- if ENABLE_WEB_PROXY %}
         - name: data
           persistentVolumeClaim:
             claimName: caddy
         {%- endif %}
-{% if RUN_CMS %}
 ---
 apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: cms
   labels:
     app.kubernetes.io/name: cms
@@ -163,16 +162,14 @@
             name: openedx-settings-lms
         - name: settings-cms
           configMap:
             name: openedx-settings-cms
         - name: config
           configMap:
             name: openedx-config
-{% endif %}
-{% if RUN_LMS %}
 ---
 apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: lms
   labels:
     app.kubernetes.io/name: lms
@@ -274,15 +271,14 @@
             name: openedx-settings-lms
         - name: settings-cms
           configMap:
             name: openedx-settings-cms
         - name: config
           configMap:
             name: openedx-config
-{% endif %}
 {% if RUN_ELASTICSEARCH %}
 ---
 apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: elasticsearch
   labels:
```

### Comparing `tutor-15.3.7/tutor/templates/k8s/jobs.yml` & `tutor-16.0.0/tutor/templates/k8s/jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/k8s/services.yml` & `tutor-16.0.0/tutor/templates/k8s/services.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,46 +30,42 @@
   type: ClusterIP
   ports:
     - port: {{ CADDY_HTTP_PORT }}
       name: http
   selector:
     app.kubernetes.io/name: caddy
 {% endif %}
-{% if RUN_CMS %}
 ---
 apiVersion: v1
 kind: Service
 metadata:
   name: cms
   labels:
     app.kubernetes.io/name: cms
 spec:
   type: ClusterIP
   ports:
     - port: 8000
       protocol: TCP
   selector:
     app.kubernetes.io/name: cms
-{% endif %}
-{% if RUN_LMS %}
 ---
 apiVersion: v1
 kind: Service
 metadata:
   name: lms
   labels:
     app.kubernetes.io/name: lms
 spec:
   type: ClusterIP
   ports:
     - port: 8000
       protocol: TCP
   selector:
     app.kubernetes.io/name: lms
-{% endif %}
 {% if RUN_ELASTICSEARCH %}
 ---
 apiVersion: v1
 kind: Service
 metadata:
   name: elasticsearch
   labels:
```

### Comparing `tutor-15.3.7/tutor/templates/k8s/volumes.yml` & `tutor-16.0.0/tutor/templates/k8s/volumes.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/kustomization.yml` & `tutor-16.0.0/tutor/templates/kustomization.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/local/docker-compose.jobs.yml` & `tutor-16.0.0/tutor/templates/local/docker-compose.jobs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -23,21 +23,27 @@
       environment:
         SERVICE_VARIANT: lms
         DJANGO_SETTINGS_MODULE: lms.envs.tutor.production
       volumes:
         - ../apps/openedx/settings/lms:/openedx/edx-platform/lms/envs/tutor:ro
         - ../apps/openedx/settings/cms:/openedx/edx-platform/cms/envs/tutor:ro
         - ../apps/openedx/config:/openedx/config:ro
+        {%- for mount in iter_mounts(MOUNTS, "lms-job") %}
+        - {{ mount }}
+        {%- endfor %}
       depends_on: {{ [("mysql", RUN_MYSQL), ("mongodb", RUN_MONGODB)]|list_if }}
 
     cms-job:
       image: {{ DOCKER_IMAGE_OPENEDX }}
       environment:
         SERVICE_VARIANT: cms
         DJANGO_SETTINGS_MODULE: cms.envs.tutor.production
       volumes:
         - ../apps/openedx/settings/lms:/openedx/edx-platform/lms/envs/tutor:ro
         - ../apps/openedx/settings/cms:/openedx/edx-platform/cms/envs/tutor:ro
         - ../apps/openedx/config:/openedx/config:ro
+        {%- for mount in iter_mounts(MOUNTS, "cms-job") %}
+        - {{ mount }}
+        {%- endfor %}
       depends_on: {{ [("mysql", RUN_MYSQL), ("mongodb", RUN_MONGODB), ("elasticsearch", RUN_ELASTICSEARCH), ("redis", RUN_REDIS)]|list_if }}
 
     {{ patch("local-docker-compose-jobs-services")|indent(4) }}
```

### Comparing `tutor-15.3.7/tutor/templates/local/docker-compose.prod.yml` & `tutor-16.0.0/tutor/templates/local/docker-compose.prod.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/templates/local/docker-compose.yml` & `tutor-16.0.0/tutor/templates/local/docker-compose.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 version: "{{ DOCKER_COMPOSE_VERSION }}"
 services:
 
+  # Set bind-mounted folder ownership
+  permissions:
+    image: {{ DOCKER_IMAGE_PERMISSIONS }}
+    restart: on-failure
+    entrypoint: []
+    command: ["sh", "/usr/local/bin/setowners.sh"]
+    environment:
+      OPENEDX_USER_ID: "1000"
+    volumes:
+      # Command script
+      - ../apps/permissions/setowners.sh:/usr/local/bin/setowners.sh:ro
+      # Bind-mounted volumes to set ownership
+      - ../../data/lms:/mounts/lms
+      - ../../data/cms:/mounts/cms
+      - ../../data/openedx-media:/mounts/openedx
+      {% if RUN_MONGODB %}- ../../data/mongodb:/mounts/mongodb{% endif %}
+      {% if RUN_MYSQL %}- ../../data/mysql:/mounts/mysql{% endif %}
+      {% if RUN_ELASTICSEARCH %}- ../../data/elasticsearch:/mounts/elasticsearch{% endif %}
+      {% if RUN_REDIS %}- ../../data/redis:/mounts/redis{% endif %}
+      {{ patch("local-docker-compose-permissions-volumes")|indent(6) }}
+
   ############# External services
 
-  {% if RUN_MONGODB %}
+  {% if RUN_MONGODB -%}
   mongodb:
     image: {{ DOCKER_IMAGE_MONGODB }}
     # Use WiredTiger in all environments, just like at edx.org
     command: mongod --nojournal --storageEngine wiredTiger
     restart: unless-stopped
     user: "999:999"
-    privileged: false
     volumes:
       - ../../data/mongodb:/data/db
     depends_on:
-      - mongodb-permissions
-  mongodb-permissions:
-    image: {{ DOCKER_IMAGE_PERMISSIONS }}
-    command: ["999", "/data/db"]
-    restart: on-failure
-    volumes:
-      - ../../data/mongodb:/data/db
-  {% endif %}
+      - permissions
+  {%- endif %}
 
-  {% if RUN_MYSQL %}
+  {% if RUN_MYSQL -%}
   mysql:
     image: {{ DOCKER_IMAGE_MYSQL }}
     command: mysqld --character-set-server=utf8 --collation-server=utf8_general_ci
     restart: unless-stopped
     user: "999:999"
-    privileged: false
     volumes:
       - ../../data/mysql:/var/lib/mysql
     environment:
       MYSQL_ROOT_PASSWORD: "{{ MYSQL_ROOT_PASSWORD }}"
-  mysql-permissions:
-    image: {{ DOCKER_IMAGE_PERMISSIONS }}
-    command: ["999", "/var/lib/mysql"]
-    restart: on-failure
-    volumes:
-      - ../../data/mysql:/var/lib/mysql
-  {% endif %}
+  {%- endif %}
 
-  {% if RUN_ELASTICSEARCH %}
+  {% if RUN_ELASTICSEARCH -%}
   elasticsearch:
     image: {{ DOCKER_IMAGE_ELASTICSEARCH }}
     environment:
       - cluster.name=openedx
       - bootstrap.memory_lock=true
       - discovery.type=single-node
       - "ES_JAVA_OPTS=-Xms{{ ELASTICSEARCH_HEAP_SIZE }} -Xmx{{ ELASTICSEARCH_HEAP_SIZE }}"
@@ -55,151 +62,129 @@
         soft: -1
         hard: -1
     restart: unless-stopped
     user: "1000:1000"
     volumes:
       - ../../data/elasticsearch:/usr/share/elasticsearch/data
     depends_on:
-      - elasticsearch-permissions
-  elasticsearch-permissions:
-    image: {{ DOCKER_IMAGE_PERMISSIONS }}
-    command: ["1000", "/usr/share/elasticsearch/data"]
-    restart: on-failure
-    volumes:
-      - ../../data/elasticsearch:/usr/share/elasticsearch/data
-  {% endif %}
+      - permissions
+  {%- endif %}
 
-  {% if RUN_REDIS %}
+  {% if RUN_REDIS -%}
   redis:
     image: {{ DOCKER_IMAGE_REDIS }}
     working_dir: /openedx/redis/data
     user: "1000:1000"
     volumes:
       - ../apps/redis/redis.conf:/openedx/redis/config/redis.conf:ro
       - ../../data/redis:/openedx/redis/data
     command: redis-server /openedx/redis/config/redis.conf
     restart: unless-stopped
     depends_on:
-      - redis-permissions
-  redis-permissions:
-    image: {{ DOCKER_IMAGE_PERMISSIONS }}
-    command: ["1000", "/openedx/redis/data"]
-    restart: on-failure
-    volumes:
-      - ../../data/redis:/openedx/redis/data
-  {% endif %}
+      - permissions
+  {%- endif %}
 
-  {% if RUN_SMTP %}
+  {% if RUN_SMTP -%}
   smtp:
     image: {{ DOCKER_IMAGE_SMTP }}
     restart: unless-stopped
     user: "100:101"
     environment:
       HOSTNAME: "{{ LMS_HOST }}"
-  {% endif %}
+  {%- endif %}
 
   ############# LMS and CMS
 
-  {% if RUN_LMS %}
   lms:
     image: {{ DOCKER_IMAGE_OPENEDX }}
     environment:
       SERVICE_VARIANT: lms
       DJANGO_SETTINGS_MODULE: lms.envs.tutor.production
       UWSGI_WORKERS: {{ OPENEDX_LMS_UWSGI_WORKERS }}
     restart: unless-stopped
     volumes:
       - ../apps/openedx/settings/lms:/openedx/edx-platform/lms/envs/tutor:ro
       - ../apps/openedx/settings/cms:/openedx/edx-platform/cms/envs/tutor:ro
       - ../apps/openedx/config:/openedx/config:ro
       - ../apps/openedx/uwsgi.ini:/openedx/edx-platform/uwsgi.ini:ro
       - ../../data/lms:/openedx/data
       - ../../data/openedx-media:/openedx/media
+      {%- for mount in iter_mounts(MOUNTS, "lms") %}
+      - {{ mount }}
+      {%- endfor %}
     depends_on:
-      - lms-permissions
+      - permissions
       {% if RUN_MYSQL %}- mysql{% endif %}
       {% if RUN_ELASTICSEARCH %}- elasticsearch{% endif %}
       {% if RUN_MONGODB %}- mongodb{% endif %}
       {% if RUN_REDIS %}- redis{% endif %}
       {% if RUN_SMTP %}- smtp{% endif %}
       {{ patch("local-docker-compose-lms-dependencies")|indent(6) }}
-  lms-permissions:
-    image: {{ DOCKER_IMAGE_PERMISSIONS }}
-    command: ["1000", "/openedx/data", "/openedx/media"]
-    restart: on-failure
-    volumes:
-      - ../../data/lms:/openedx/data
-      - ../../data/openedx-media:/openedx/media
-  {% endif %}
 
-  {% if RUN_CMS %}
   cms:
     image: {{ DOCKER_IMAGE_OPENEDX }}
     environment:
       SERVICE_VARIANT: cms
       DJANGO_SETTINGS_MODULE: cms.envs.tutor.production
       UWSGI_WORKERS: {{ OPENEDX_CMS_UWSGI_WORKERS }}
     restart: unless-stopped
     volumes:
       - ../apps/openedx/settings/lms:/openedx/edx-platform/lms/envs/tutor:ro
       - ../apps/openedx/settings/cms:/openedx/edx-platform/cms/envs/tutor:ro
       - ../apps/openedx/config:/openedx/config:ro
       - ../apps/openedx/uwsgi.ini:/openedx/edx-platform/uwsgi.ini:ro
       - ../../data/cms:/openedx/data
       - ../../data/openedx-media:/openedx/media
+      {%- for mount in iter_mounts(MOUNTS, "cms") %}
+      - {{ mount }}
+      {%- endfor %}
     depends_on:
-      - cms-permissions
+      - permissions
+      - lms
       {% if RUN_MYSQL %}- mysql{% endif %}
       {% if RUN_ELASTICSEARCH %}- elasticsearch{% endif %}
       {% if RUN_MONGODB %}- mongodb{% endif %}
       {% if RUN_REDIS %}- redis{% endif %}
       {% if RUN_SMTP %}- smtp{% endif %}
-      {% if RUN_LMS %}- lms{% endif %}
       {{ patch("local-docker-compose-cms-dependencies")|indent(6) }}
-  cms-permissions:
-    image: {{ DOCKER_IMAGE_PERMISSIONS }}
-    command: ["1000", "/openedx/data", "/openedx/media"]
-    restart: on-failure
-    volumes:
-      - ../../data/cms:/openedx/data
-      - ../../data/openedx-media:/openedx/media
-  {% endif %}
 
   ############# LMS and CMS workers
 
-  {% if RUN_LMS %}
   lms-worker:
     image: {{ DOCKER_IMAGE_OPENEDX }}
     environment:
       SERVICE_VARIANT: lms
       DJANGO_SETTINGS_MODULE: lms.envs.tutor.production
     command: celery --app=lms.celery worker --loglevel=info --hostname=edx.lms.core.default.%%h --max-tasks-per-child=100 --exclude-queues=edx.cms.core.default
     restart: unless-stopped
     volumes:
       - ../apps/openedx/settings/lms:/openedx/edx-platform/lms/envs/tutor:ro
       - ../apps/openedx/settings/cms:/openedx/edx-platform/cms/envs/tutor:ro
       - ../apps/openedx/config:/openedx/config:ro
       - ../../data/lms:/openedx/data
       - ../../data/openedx-media:/openedx/media
+      {%- for mount in iter_mounts(MOUNTS, "lms-worker") %}
+      - {{ mount }}
+      {%- endfor %}
     depends_on:
       - lms
-  {% endif %}
 
-  {% if RUN_CMS %}
   cms-worker:
     image: {{ DOCKER_IMAGE_OPENEDX }}
     environment:
       SERVICE_VARIANT: cms
       DJANGO_SETTINGS_MODULE: cms.envs.tutor.production
     command: celery --app=cms.celery worker --loglevel=info --hostname=edx.cms.core.default.%%h --max-tasks-per-child 100 --exclude-queues=edx.lms.core.default
     restart: unless-stopped
     volumes:
       - ../apps/openedx/settings/lms:/openedx/edx-platform/lms/envs/tutor:ro
       - ../apps/openedx/settings/cms:/openedx/edx-platform/cms/envs/tutor:ro
       - ../apps/openedx/config:/openedx/config:ro
       - ../../data/cms:/openedx/data
       - ../../data/openedx-media:/openedx/media
+      {%- for mount in iter_mounts(MOUNTS, "cms-worker") %}
+      - {{ mount }}
+      {%- endfor %}
     depends_on:
       - cms
-  {% endif %}
 
   {{ patch("local-docker-compose-services")|indent(2) }}
```

### Comparing `tutor-15.3.7/tutor/types.py` & `tutor-16.0.0/tutor/types.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.7/tutor/utils.py` & `tutor-16.0.0/tutor/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,37 +170,34 @@
         raise exceptions.TutorError(
             "docker is not installed. Please follow instructions from https://docs.docker.com/install/"
         )
     return execute("docker", *command)
 
 
 @lru_cache(maxsize=None)
-def _docker_compose_command() -> Tuple[str, ...]:
+def is_buildkit_enabled() -> bool:
     """
-    A helper function to determine which program to call when running docker compose
+    A helper function to determine whether we can run `docker buildx` with BuildKit.
     """
-    if os.environ.get("TUTOR_USE_COMPOSE_SUBCOMMAND") is not None:
-        return ("docker", "compose")
-    if shutil.which("docker-compose") is not None:
-        return ("docker-compose",)
-    if shutil.which("docker") is not None:
-        if (
-            subprocess.run(
-                ["docker", "compose"], capture_output=True, check=False
-            ).returncode
-            == 0
-        ):
-            return ("docker", "compose")
-    raise exceptions.TutorError(
-        "docker-compose is not installed. Please follow instructions from https://docs.docker.com/compose/install/"
-    )
+    # First, we respect the DOCKER_BUILDKIT environment variable
+    enabled_by_env = {
+        "1": True,
+        "0": False,
+    }.get(os.environ.get("DOCKER_BUILDKIT", ""))
+    if enabled_by_env is not None:
+        return enabled_by_env
+    try:
+        subprocess.run(["docker", "buildx", "version"], capture_output=True, check=True)
+        return True
+    except subprocess.CalledProcessError:
+        return False
 
 
 def docker_compose(*command: str) -> int:
-    return execute(*_docker_compose_command(), *command)
+    return execute("docker", "compose", *command)
 
 
 def kubectl(*command: str) -> int:
     if shutil.which("kubectl") is None:
         raise exceptions.TutorError(
             "kubectl is not installed. Please follow instructions from https://kubernetes.io/docs/tasks/tools/install-kubectl/"
         )
@@ -212,15 +209,15 @@
     Return True if stdin is able to allocate a tty. Tty allocation sometimes cannot be
     enabled, for instance in cron jobs
     """
     return sys.stdin.isatty()
 
 
 def execute(*command: str) -> int:
-    click.echo(fmt.command(_shlex_join(*command)))
+    click.echo(fmt.command(shlex.join(command)))
     return execute_silent(*command)
 
 
 def execute_silent(*command: str) -> int:
     with subprocess.Popen(command) as p:
         try:
             result = p.wait(timeout=None)
@@ -235,36 +232,37 @@
         if result > 0:
             raise exceptions.TutorError(
                 f"Command failed with status {result}: {' '.join(command)}"
             )
     return result
 
 
-def _shlex_join(*split_command: str) -> str:
-    """
-    Return a shell-escaped string from *split_command.
-
-    TODO: REMOVE THIS FUNCTION AFTER 2023-06-27.
-      This function is a shim for the ``shlex.join`` standard library function,
-      which becomes available in Python 3.8  The end-of-life date for Python 3.7
-      is in Jan 2023 (https://endoflife.date/python). After that point, it
-      would be good to delete this function and just use Py3.8's ``shlex.join``.
-    """
-    return " ".join(shlex.quote(arg) for arg in split_command)
-
-
 def check_output(*command: str) -> bytes:
-    literal_command = _shlex_join(*command)
+    literal_command = shlex.join(command)
     click.echo(fmt.command(literal_command))
     try:
         return subprocess.check_output(command)
     except Exception as e:
         raise exceptions.TutorError(f"Command failed: {literal_command}") from e
 
 
+def warn_macos_docker_memory() -> None:
+    try:
+        check_macos_docker_memory()
+    except exceptions.TutorError as e:
+        fmt.echo_alert(
+            f"""Could not verify sufficient RAM allocation in Docker:
+
+    {e}
+
+Tutor may not work if Docker is configured with < 4 GB RAM. Please follow instructions from:
+    https://docs.tutor.overhang.io/install.html"""
+        )
+
+
 def check_macos_docker_memory() -> None:
     """
     Try to check that the RAM allocated to the Docker VM on macOS is at least 4 GB.
 
     Parse macOS Docker settings file from user directory and return the max
     allocated memory. Will raise TutorError in case of parsing/loading error.
     """
```

### Comparing `tutor-15.3.7/tutor.egg-info/PKG-INFO` & `tutor-16.0.0/tutor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 15.3.7
+Version: 16.0.0
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor
@@ -114,14 +114,14 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: full
```

### Comparing `tutor-15.3.7/tutor.egg-info/SOURCES.txt` & `tutor-16.0.0/tutor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
 requirements/base.in
 requirements/plugins.txt
+tests/test_bindmount.py
 tests/test_config.py
 tests/test_env.py
-tests/test_images.py
 tests/test_plugin_indexes.py
 tests/test_plugins_v0.py
 tests/test_serialize.py
 tests/test_utils.py
 tutor/__about__.py
 tutor/__init__.py
-tutor/bindmounts.py
+tutor/bindmount.py
 tutor/config.py
 tutor/env.py
 tutor/exceptions.py
 tutor/fmt.py
 tutor/images.py
 tutor/interactive.py
 tutor/py.typed
@@ -38,19 +38,21 @@
 tutor/commands/config.py
 tutor/commands/context.py
 tutor/commands/dev.py
 tutor/commands/images.py
 tutor/commands/jobs.py
 tutor/commands/k8s.py
 tutor/commands/local.py
+tutor/commands/mounts.py
+tutor/commands/params.py
 tutor/commands/plugins.py
 tutor/commands/upgrade/__init__.py
 tutor/commands/upgrade/common.py
+tutor/commands/upgrade/compose.py
 tutor/commands/upgrade/k8s.py
-tutor/commands/upgrade/local.py
 tutor/core/__init__.py
 tutor/core/hooks/__init__.py
 tutor/core/hooks/actions.py
 tutor/core/hooks/contexts.py
 tutor/core/hooks/filters.py
 tutor/core/hooks/priorities.py
 tutor/hooks/__init__.py
@@ -75,14 +77,15 @@
 tutor/templates/apps/openedx/settings/lms/development.py
 tutor/templates/apps/openedx/settings/lms/production.py
 tutor/templates/apps/openedx/settings/lms/test.py
 tutor/templates/apps/openedx/settings/partials/common_all.py
 tutor/templates/apps/openedx/settings/partials/common_cms.py
 tutor/templates/apps/openedx/settings/partials/common_lms.py
 tutor/templates/apps/openedx/settings/partials/common_test.py
+tutor/templates/apps/permissions/setowners.sh
 tutor/templates/apps/redis/redis.conf
 tutor/templates/build/openedx/Dockerfile
 tutor/templates/build/openedx/revisions.yml
 tutor/templates/build/openedx/bin/openedx-assets
 tutor/templates/build/openedx/bin/reload-uwsgi
 tutor/templates/build/openedx/bin/site-configuration
 tutor/templates/build/openedx/locale/customlocales.md
```

