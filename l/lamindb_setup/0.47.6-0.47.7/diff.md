# Comparing `tmp/lamindb_setup-0.47.6.tar.gz` & `tmp/lamindb_setup-0.47.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.47.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.47.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.47.6.tar` & `lamindb_setup-0.47.7.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.6/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.6/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.6/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.6/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.6/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.6/README.md
--rw-r--r--   0        0        0    54530 2023-06-12 20:35:01.136062 lamindb_setup-0.47.6/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.6/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.6/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.6/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.6/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.6/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.6/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.6/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.47.6/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.6/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.6/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.6/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.6/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.6/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.6/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.6/lamin-project.yaml
--rw-r--r--   0        0        0     2715 2023-06-12 20:34:39.904011 lamindb_setup-0.47.6/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.6/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.6/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.47.6/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.6/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.6/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.6/lamindb_setup/_info.py
--rw-r--r--   0        0        0     6835 2023-06-11 19:14:24.008674 lamindb_setup-0.47.6/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     5670 2023-06-11 19:14:24.008895 lamindb_setup-0.47.6/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0      322 2023-06-04 10:03:32.191280 lamindb_setup-0.47.6/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.6/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.6/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.6/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.6/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.6/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.6/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.6/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.6/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.6/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.6/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.47.6/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.6/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     9986 2023-06-12 20:33:20.803923 lamindb_setup-0.47.6/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.6/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     9331 2023-06-11 19:14:24.009365 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.6/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2370 2023-06-12 19:19:26.360494 lamindb_setup-0.47.6/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.6/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.47.6/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2670 2023-06-08 17:51:53.349359 lamindb_setup-0.47.6/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      815 2023-06-12 10:24:01.838397 lamindb_setup-0.47.6/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.6/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.47.6/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.6/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.6/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    27342 2023-06-12 19:29:46.148924 lamindb_setup-0.47.6/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.6/lnschema-core/LICENSE
--rw-r--r--   0        0        0      308 2023-06-12 10:24:01.839064 lamindb_setup-0.47.6/lnschema-core/README.md
--rw-r--r--   0        0        0      608 2023-06-12 19:29:46.149107 lamindb_setup-0.47.6/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.6/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.47.6/lnschema-core/lnschema_core/_queryset.py
--rw-r--r--   0        0        0     1644 2023-06-12 19:29:46.149255 lamindb_setup-0.47.6/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    12754 2023-06-12 19:29:46.149559 lamindb_setup-0.47.6/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.6/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    20627 2023-06-12 19:29:46.149767 lamindb_setup-0.47.6/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      591 2023-06-12 10:24:01.840710 lamindb_setup-0.47.6/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.47.6/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      184 2023-06-12 10:24:01.840993 lamindb_setup-0.47.6/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.6/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.6/noxfile.py
--rw-r--r--   0        0        0     1337 2023-06-11 19:14:24.010612 lamindb_setup-0.47.6/pyproject.toml
--rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.6/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.6/tests/test_init_instance.py
--rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.47.6/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.6/tests/test_login.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.6/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.6/tests/test_signup.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.6/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.7/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.7/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.7/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.7/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.7/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.7/README.md
+-rw-r--r--   0        0        0    54530 2023-06-14 08:21:46.101997 lamindb_setup-0.47.7/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.7/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.7/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.7/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.7/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.7/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.7/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.7/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.47.7/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.7/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.7/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.7/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.7/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.7/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.7/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.7/lamin-project.yaml
+-rw-r--r--   0        0        0     2715 2023-06-14 08:21:40.696674 lamindb_setup-0.47.7/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.7/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.7/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.47.7/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.7/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.7/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.7/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6662 2023-06-14 07:51:53.730520 lamindb_setup-0.47.7/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     5670 2023-06-11 19:14:24.008895 lamindb_setup-0.47.7/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0      322 2023-06-04 10:03:32.191280 lamindb_setup-0.47.7/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.7/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.7/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.7/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.7/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.7/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.7/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.7/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.7/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.7/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.7/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.47.7/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.7/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0     9986 2023-06-12 20:33:20.803923 lamindb_setup-0.47.7/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.7/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     9359 2023-06-14 07:52:21.048065 lamindb_setup-0.47.7/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.7/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.7/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.7/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.7/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2370 2023-06-12 19:19:26.360494 lamindb_setup-0.47.7/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.7/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.47.7/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.47.7/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      815 2023-06-12 10:24:01.838397 lamindb_setup-0.47.7/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.7/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.47.7/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.7/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.7/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    27342 2023-06-12 19:29:46.148924 lamindb_setup-0.47.7/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.7/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      308 2023-06-12 10:24:01.839064 lamindb_setup-0.47.7/lnschema-core/README.md
+-rw-r--r--   0        0        0      608 2023-06-12 19:29:46.149107 lamindb_setup-0.47.7/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.7/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.47.7/lnschema-core/lnschema_core/_queryset.py
+-rw-r--r--   0        0        0     1644 2023-06-12 19:29:46.149255 lamindb_setup-0.47.7/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    12754 2023-06-12 19:29:46.149559 lamindb_setup-0.47.7/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.7/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    20627 2023-06-12 19:29:46.149767 lamindb_setup-0.47.7/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      591 2023-06-12 10:24:01.840710 lamindb_setup-0.47.7/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.47.7/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      184 2023-06-12 10:24:01.840993 lamindb_setup-0.47.7/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.7/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.7/noxfile.py
+-rw-r--r--   0        0        0     1337 2023-06-11 19:14:24.010612 lamindb_setup-0.47.7/pyproject.toml
+-rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.7/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.7/tests/test_init_instance.py
+-rw-r--r--   0        0        0      655 2023-06-01 11:33:10.508620 lamindb_setup-0.47.7/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.7/tests/test_login.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.7/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.7/tests/test_signup.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.7/PKG-INFO
```

### Comparing `lamindb_setup-0.47.6/.github/workflows/build.yml` & `lamindb_setup-0.47.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.7/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/.gitignore` & `lamindb_setup-0.47.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/.pre-commit-config.yaml` & `lamindb_setup-0.47.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/LICENSE` & `lamindb_setup-0.47.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/docs/changelog.md` & `lamindb_setup-0.47.7/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-♻️ Different migr strategy | [417](https://github.com/laminlabs/lamindb-setup/pull/417) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.6
+♻️ Different migr strategy | [417](https://github.com/laminlabs/lamindb-setup/pull/417) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.7
 🍱 Added migration script from legacy instances | [416](https://github.com/laminlabs/lamindb-setup/pull/416) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.5
 🔥 Adapt locker to lock entire lamindb session | [415](https://github.com/laminlabs/lamindb-setup/pull/415) | [Koncopd](https://github.com/Koncopd) | 2023-06-11 |
 🚑 Only delete bionty sources when bionty is installed | [414](https://github.com/laminlabs/lamindb-setup/pull/414) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.4
 🚚 Rename source_key to source | [413](https://github.com/laminlabs/lamindb-setup/pull/413) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.3
 ⬆️ Rename bionty variables | [412](https://github.com/laminlabs/lamindb-setup/pull/412) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.2
 🚑 Removed `LAMINDB_INSTANCE_LOADED` env variable | [411](https://github.com/laminlabs/lamindb-setup/pull/411) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 | 0.47.1
 ⬆️ Adapt to bionty naming in 0.18.0 | [410](https://github.com/laminlabs/lamindb-setup/pull/410) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-09 |
```

### Comparing `lamindb_setup-0.47.6/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.47.7/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.47.7/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.47.7/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.47.7/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.47.7/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.47.7/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.47.7/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/docs/guide/setup-user.md` & `lamindb_setup-0.47.7/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/__init__.py` & `lamindb_setup-0.47.7/lamindb_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.47.6"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.47.7"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.47.6/lamindb_setup/__main__.py` & `lamindb_setup-0.47.7/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.47.7/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_close.py` & `lamindb_setup-0.47.7/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_delete.py` & `lamindb_setup-0.47.7/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_docstrings.py` & `lamindb_setup-0.47.7/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_init_instance.py` & `lamindb_setup-0.47.7/lamindb_setup/_init_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,18 +173,14 @@
         raise RuntimeError(
             "Your instance DB is already set up but couldn't be loaded, something"
             " is off"
         )
     load_from_isettings(isettings, init=True)
     if isettings._is_cloud_sqlite:
         logger.hint("To push changes to the cloud SQLite file, call: lamin close")
-        # @Sergei, this is currently not yet enabled
-        # logger.hint(
-        #     f"In the meantime, {isettings._sqlite_file} is locked for other users"
-        # )
     if not isettings.is_remote:
         logger.hint(
             "Did not register local instance on hub (if you want to, call `lamin"
             " register`)"
         )
     return None
```

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_load_instance.py` & `lamindb_setup-0.47.7/lamindb_setup/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_notebook.py` & `lamindb_setup-0.47.7/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_register_instance.py` & `lamindb_setup-0.47.7/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_schema.py` & `lamindb_setup-0.47.7/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_set.py` & `lamindb_setup-0.47.7/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_settings.py` & `lamindb_setup-0.47.7/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_setup_user.py` & `lamindb_setup-0.47.7/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.47.7/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_django.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_settings_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
             os.utime(cache_file, times=(cloud_mtime, cloud_mtime))
             self._cloud_sqlite_locker.unlock()
 
     def _update_local_sqlite_file(self) -> None:
         """Download the cloud sqlite file if it is newer than local."""
         if self._is_cloud_sqlite:
             logger.info(
-                "Synching cloud SQLite to local (synch back to cloud via: lamin close)"
+                "Updating local SQLite & locking cloud SQLite (sync back & unlock:"
+                " lamin close)"
             )
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.synchronize(cache_file)  # type: ignore
             self._cloud_sqlite_locker.lock()
 
     @property
```

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lamindb_setup/dev/upath.py` & `lamindb_setup-0.47.7/lamindb_setup/dev/upath.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,7 +89,8 @@
     return mtime.astimezone().replace(tzinfo=None)
 
 
 UPath.download_to = _download_to
 UPath.upload_from = _upload_from
 UPath.synchronize = _synchronize
 UPath.modified = property(_modified)
+UPath.__doc__ = "Universal path."
```

### Comparing `lamindb_setup-0.47.6/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.47.7/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.7/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/.gitignore` & `lamindb_setup-0.47.7/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.47.7/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.47.7/lnschema-core/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/LICENSE` & `lamindb_setup-0.47.7/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.47.7/lnschema-core/lnschema_core/__init__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/lnschema_core/_lookup.py` & `lamindb_setup-0.47.7/lnschema-core/lnschema_core/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/lnschema_core/_queryset.py` & `lamindb_setup-0.47.7/lnschema-core/lnschema_core/_queryset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.47.7/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.47.7/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.47.7/lnschema-core/lnschema_core/models.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.47.7/lnschema-core/lnschema_core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/lnschema-core/pyproject.toml` & `lamindb_setup-0.47.7/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/noxfile.py` & `lamindb_setup-0.47.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/pyproject.toml` & `lamindb_setup-0.47.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/tests/test_bionty.py` & `lamindb_setup-0.47.7/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/tests/test_init_instance.py` & `lamindb_setup-0.47.7/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/tests/test_load_instance.py` & `lamindb_setup-0.47.7/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.6/PKG-INFO` & `lamindb_setup-0.47.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.47.6
+Version: 0.47.7
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.10
 Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
```

