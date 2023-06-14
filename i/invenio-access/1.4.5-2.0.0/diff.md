# Comparing `tmp/invenio-access-1.4.5.tar.gz` & `tmp/invenio-access-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-access-1.4.5.tar", last modified: Fri Nov 18 09:11:12 2022, max compression
+gzip compressed data, was "invenio-access-2.0.0.tar", last modified: Wed Jun 14 15:28:24 2023, max compression
```

## Comparing `invenio-access-1.4.5.tar` & `invenio-access-2.0.0.tar`

### file list

```diff
@@ -1,205 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-11-18 09:11:03.000000 invenio-access-1.4.5/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-11-18 09:11:03.000000 invenio-access-1.4.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-18 09:11:03.000000 invenio-access-1.4.5/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1910 2022-11-18 09:11:03.000000 invenio-access-1.4.5/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2004 2022-11-18 09:11:03.000000 invenio-access-1.4.5/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-11-18 09:11:03.000000 invenio-access-1.4.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-11-18 09:11:03.000000 invenio-access-1.4.5/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/.tx/
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-11-18 09:11:03.000000 invenio-access-1.4.5/.tx/config
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-18 09:11:03.000000 invenio-access-1.4.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-11-18 09:11:03.000000 invenio-access-1.4.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3725 2022-11-18 09:11:03.000000 invenio-access-1.4.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-11-18 09:11:03.000000 invenio-access-1.4.5/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-11-18 09:11:03.000000 invenio-access-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-11-18 09:11:03.000000 invenio-access-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-11-18 09:11:12.264786 invenio-access-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-11-18 09:11:03.000000 invenio-access-1.4.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-11-18 09:11:03.000000 invenio-access-1.4.5/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.256786 invenio-access-1.4.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7441 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10328 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6997 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-11-18 09:11:03.000000 invenio-access-1.4.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.256786 invenio-access-1.4.5/invenio_access/
--rw-r--r--   0 runner    (1001) docker     (121)    14339 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3802 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.256786 invenio-access-1.4.5/invenio_access/alembic/
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/alembic/04480be1593e_add_actionsystemroles.py
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/alembic/2069a982633b_add_on_delete_cascade_constraint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/alembic/2f63be7b7572_create_access_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/alembic/67ba0de65fbb_create_access_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/alembic/dbe499bfda43_prevent_null_in_actionusers_for_.py
--rw-r--r--   0 runner    (1001) docker     (121)     7584 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     6078 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     8368 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7578 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.256786 invenio-access-1.4.5/invenio_access/translations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.256786 invenio-access-1.4.5/invenio_access/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1577 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.248785 invenio-access-1.4.5/invenio_access/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.260786 invenio-access-1.4.5/invenio_access/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1498 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.252786 invenio-access-1.4.5/invenio_access/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/invenio_access/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-11-18 09:11:11.000000 invenio-access-1.4.5/invenio_access/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-11-18 09:11:03.000000 invenio-access-1.4.5/invenio_access/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.256786 invenio-access-1.4.5/invenio_access.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5207 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-18 09:11:12.000000 invenio-access-1.4.5/invenio_access.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-18 09:11:03.000000 invenio-access-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-11-18 09:11:03.000000 invenio-access-1.4.5/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      769 2022-11-18 09:11:03.000000 invenio-access-1.4.5/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-11-18 09:11:12.268787 invenio-access-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-11-18 09:11:03.000000 invenio-access-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 09:11:12.264786 invenio-access-1.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3901 2022-11-18 09:11:03.000000 invenio-access-1.4.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-11-18 09:11:03.000000 invenio-access-1.4.5/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     8008 2022-11-18 09:11:03.000000 invenio-access-1.4.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3996 2022-11-18 09:11:03.000000 invenio-access-1.4.5/tests/test_invenio_access.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-11-18 09:11:03.000000 invenio-access-1.4.5/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)    14655 2022-11-18 09:11:03.000000 invenio-access-1.4.5/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)    39083 2022-11-18 09:11:03.000000 invenio-access-1.4.5/tests/test_permissions_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.435430 invenio-access-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-14 15:28:13.000000 invenio-access-2.0.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-06-14 15:28:13.000000 invenio-access-2.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-14 15:28:13.000000 invenio-access-2.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.423429 invenio-access-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1910 2023-06-14 15:28:13.000000 invenio-access-2.0.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2004 2023-06-14 15:28:13.000000 invenio-access-2.0.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-06-14 15:28:13.000000 invenio-access-2.0.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-14 15:28:13.000000 invenio-access-2.0.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.423429 invenio-access-2.0.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-14 15:28:13.000000 invenio-access-2.0.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-06-14 15:28:13.000000 invenio-access-2.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-14 15:28:13.000000 invenio-access-2.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-06-14 15:28:13.000000 invenio-access-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-06-14 15:28:13.000000 invenio-access-2.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-14 15:28:13.000000 invenio-access-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-06-14 15:28:13.000000 invenio-access-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4504 2023-06-14 15:28:24.435430 invenio-access-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1474 2023-06-14 15:28:13.000000 invenio-access-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-14 15:28:13.000000 invenio-access-2.0.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.423429 invenio-access-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10328 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)     3694 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-14 15:28:13.000000 invenio-access-2.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.423429 invenio-access-2.0.0/invenio_access/
+-rw-r--r--   0 runner    (1001) docker     (122)    14413 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/alembic/04480be1593e_add_actionsystemroles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2477 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/alembic/2069a982633b_add_on_delete_cascade_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/alembic/2f63be7b7572_create_access_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/alembic/67ba0de65fbb_create_access_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/alembic/842a62b56e60_change_fk_accountsrole_to_string_downgrade.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/alembic/dbe499bfda43_prevent_null_in_actionusers_for_.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/alembic/f9843093f686_change_fk_accountsrole_to_string_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7584 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8369 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7578 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1864 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1577 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.411429 invenio-access-2.0.0/invenio_access/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1377 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.415429 invenio-access-2.0.0/invenio_access/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.415429 invenio-access-2.0.0/invenio_access/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.415429 invenio-access-2.0.0/invenio_access/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.415429 invenio-access-2.0.0/invenio_access/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.415429 invenio-access-2.0.0/invenio_access/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.415429 invenio-access-2.0.0/invenio_access/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1566 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.415429 invenio-access-2.0.0/invenio_access/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.415429 invenio-access-2.0.0/invenio_access/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1610 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.431430 invenio-access-2.0.0/invenio_access/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.435430 invenio-access-2.0.0/invenio_access/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1584 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.435430 invenio-access-2.0.0/invenio_access/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.419429 invenio-access-2.0.0/invenio_access/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.435430 invenio-access-2.0.0/invenio_access/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-06-14 15:28:13.000000 invenio-access-2.0.0/invenio_access/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.427430 invenio-access-2.0.0/invenio_access.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4504 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-06-14 15:28:24.000000 invenio-access-2.0.0/invenio_access.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-06-14 15:28:24.000000 invenio-access-2.0.0/invenio_access.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 15:28:23.000000 invenio-access-2.0.0/invenio_access.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-14 15:28:24.000000 invenio-access-2.0.0/invenio_access.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-14 15:28:24.000000 invenio-access-2.0.0/invenio_access.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-14 15:28:13.000000 invenio-access-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-06-14 15:28:13.000000 invenio-access-2.0.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1465 2023-06-14 15:28:13.000000 invenio-access-2.0.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2728 2023-06-14 15:28:24.435430 invenio-access-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-06-14 15:28:13.000000 invenio-access-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 15:28:24.435430 invenio-access-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3911 2023-06-14 15:28:13.000000 invenio-access-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      911 2023-06-14 15:28:13.000000 invenio-access-2.0.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-06-14 15:28:13.000000 invenio-access-2.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3996 2023-06-14 15:28:13.000000 invenio-access-2.0.0/tests/test_invenio_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2516 2023-06-14 15:28:13.000000 invenio-access-2.0.0/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14664 2023-06-14 15:28:13.000000 invenio-access-2.0.0/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35663 2023-06-14 15:28:13.000000 invenio-access-2.0.0/tests/test_permissions_cache.py
```

### Comparing `invenio-access-1.4.5/.editorconfig` & `invenio-access-2.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/.github/workflows/i18n-pull.yml` & `invenio-access-2.0.0/.github/workflows/i18n-pull.yml`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/.github/workflows/i18n-push.yml` & `invenio-access-2.0.0/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/.github/workflows/pypi-publish.yml` & `invenio-access-2.0.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/.github/workflows/tests.yml` & `invenio-access-2.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/.tx/config` & `invenio-access-2.0.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/AUTHORS.rst` & `invenio-access-2.0.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/CHANGES.rst` & `invenio-access-2.0.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.0.0 (released 2022-06-14)
+
+- upgrade invenio-accounts dependency
+- models: change role_id FK of ActionRoles to string
+
 Version 1.4.4 (released 2022-04-01)
 
 - fix compat issue with Werkzeug 2.1
 
 Version 1.4.3 (released 2022-03-30)
 
 - add support for Flask 2.1, Werkzeug 2.1 and Click 8.1
```

### Comparing `invenio-access-1.4.5/CONTRIBUTING.rst` & `invenio-access-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/LICENSE` & `invenio-access-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/MANIFEST.in` & `invenio-access-2.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/PKG-INFO` & `invenio-access-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-access
-Version: 1.4.5
+Version: 2.0.0
 Summary: Invenio module for common role based access control.
 Home-page: https://github.com/inveniosoftware/invenio-access
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -57,14 +57,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.0.0 (released 2022-06-14)
+        
+        - upgrade invenio-accounts dependency
+        - models: change role_id FK of ActionRoles to string
+        
         Version 1.4.4 (released 2022-04-01)
         
         - fix compat issue with Werkzeug 2.1
         
         Version 1.4.3 (released 2022-03-30)
         
         - add support for Flask 2.1, Werkzeug 2.1 and Click 8.1
```

### Comparing `invenio-access-1.4.5/README.rst` & `invenio-access-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/docs/Makefile` & `invenio-access-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/docs/api.rst` & `invenio-access-2.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/docs/conf.py` & `invenio-access-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/docs/index.rst` & `invenio-access-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/docs/make.bat` & `invenio-access-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/docs/overview.rst` & `invenio-access-2.0.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/__init__.py` & `invenio-access-2.0.0/invenio_access/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,20 @@
 
 Initialize Invenio-Access dependencies, which are Invenio-DB and
 Invenio-Accounts, and then Invenio-Access itself:
 
 >>> from invenio_db import InvenioDB
 >>> from invenio_accounts import InvenioAccounts
 >>> from invenio_access import InvenioAccess
+>>> from invenio_i18n import InvenioI18N
+
 >>> ext_db = InvenioDB(app)
 >>> ext_accounts = InvenioAccounts(app)
 >>> ext_access = InvenioAccess(app)
+>>> ext_i18n = InvenioI18N(app)
 
 The following examples needs to run in a Flask application context, so
 let's push one:
 
 >>> app.app_context().push()
 
 Also, for the examples to work we need to create the database and tables (note,
@@ -431,15 +434,15 @@
     SystemRoleNeed,
     any_user,
     authenticated_user,
     superuser_access,
 )
 from .proxies import current_access
 
-__version__ = "1.4.5"
+__version__ = "2.0.0"
 
 __all__ = (
     "__version__",
     "any_user",
     "authenticated_user",
     "action_factory",
     "current_access",
```

### Comparing `invenio-access-1.4.5/invenio_access/admin.py` & `invenio-access-2.0.0/invenio_access/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/alembic/04480be1593e_add_actionsystemroles.py` & `invenio-access-2.0.0/invenio_access/alembic/04480be1593e_add_actionsystemroles.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/alembic/2069a982633b_add_on_delete_cascade_constraint.py` & `invenio-access-2.0.0/invenio_access/alembic/2069a982633b_add_on_delete_cascade_constraint.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/alembic/2f63be7b7572_create_access_tables.py` & `invenio-access-2.0.0/invenio_access/alembic/2f63be7b7572_create_access_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/alembic/67ba0de65fbb_create_access_branch.py` & `invenio-access-2.0.0/invenio_access/alembic/67ba0de65fbb_create_access_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/alembic/dbe499bfda43_prevent_null_in_actionusers_for_.py` & `invenio-access-2.0.0/invenio_access/alembic/dbe499bfda43_prevent_null_in_actionusers_for_.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/cli.py` & `invenio-access-2.0.0/invenio_access/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/config.py` & `invenio-access-2.0.0/invenio_access/config.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/ext.py` & `invenio-access-2.0.0/invenio_access/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/factory.py` & `invenio-access-2.0.0/invenio_access/factory.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/loaders.py` & `invenio-access-2.0.0/invenio_access/loaders.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/models.py` & `invenio-access-2.0.0/invenio_access/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2015-2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Database models for access module."""
 
 from flask_principal import RoleNeed, UserNeed
@@ -152,15 +152,15 @@
             "argument",
             "role_id",
             name="access_actionsroles_unique",
         ),
     )
 
     role_id = db.Column(
-        db.Integer(),
+        db.String(80),
         db.ForeignKey(Role.id, ondelete="CASCADE"),
         nullable=False,
         index=True,
     )
 
     role = db.relationship(
         "Role", backref=db.backref("actionusers", cascade="all, delete-orphan")
```

### Comparing `invenio-access-1.4.5/invenio_access/permissions.py` & `invenio-access-2.0.0/invenio_access/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/af/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/af/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-access 1.4.4*

 * *Files 2% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 00000180: 7261 6c3d 286e 2021 3d20 3129 3b0a 4d49  ral=(n != 1);.MI
 00000190: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
 000001a0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 000001b0: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
 000001c0: 743d 7574 662d 380a 436f 6e74 656e 742d  t=utf-8.Content-
 000001d0: 5472 616e 7366 6572 2d45 6e63 6f64 696e  Transfer-Encodin
 000001e0: 673a 2038 6269 740a 4765 6e65 7261 7465  g: 8bit.Generate
-000001f0: 642d 4279 3a20 4261 6265 6c20 322e 3131  d-By: Babel 2.11
-00000200: 2e30 0a00                                .0..
+000001f0: 642d 4279 3a20 4261 6265 6c20 322e 3132  d-By: Babel 2.12
+00000200: 2e31 0a00                                .1..
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/af/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/ar/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/ar/LC_MESSAGES/messages.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Arabic (https://www.transifex.com/inveniosoftware/teams/23537/"
 "ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Access: Roles"
 msgstr "الولوج: الأدوار"
 
 msgid "Access: System Roles"
 msgstr "الولوج: أدوار النظام"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/ar/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/bg/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/bg/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,14 +8,14 @@
 "Language: bg\n"
 "Language-Team: Bulgarian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/bg/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "E-mail"
 
 msgid "User ID"
 msgstr "ID на потребителя"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/bg/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/ca/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: ca\n"
 "Language-Team: Catalan (https://www.transifex.com/inveniosoftware/"
 "teams/23537/ca/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Adreça electrònica"
 
 msgid "Role Name"
 msgstr "Rol"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/ca/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/cs/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Czech (https://www.transifex.com/inveniosoftware/teams/23537/"
 "cs/)\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Role Name"
 msgstr "Název role"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/cs/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/da/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/da/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: da\n"
 "Language-Team: Danish (https://www.transifex.com/inveniosoftware/teams/23537/"
 "da/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Role Name"
 msgstr "Rolle"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/da/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/de/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/de/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: de\n"
 "Language-Team: German (https://www.transifex.com/inveniosoftware/teams/23537/"
 "de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Access: Roles"
 msgstr "Zugang: Rollen"
 
 msgid "Access: System Roles"
 msgstr "Zugang: Systemrollen"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/de/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/el/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/gl/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,27 +0,0 @@
-msgid ""
-msgstr ""
-"Project-Id-Version: invenio-access 1.4.4\n"
-"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
-"POT-Creation-Date: 2022-10-12 09:03+0000\n"
-"PO-Revision-Date: 2016-08-18 12:08+0000\n"
-"Last-Translator: Theodoros Theodoropoulos, 2016\n"
-"Language: el\n"
-"Language-Team: Greek (https://www.transifex.com/inveniosoftware/teams/23537/"
-"el/)\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
-
-msgid "Email"
-msgstr "Email"
-
-msgid "Role Name"
-msgstr "Όνομα Ρόλου"
-
-msgid "User ID"
-msgstr "ID Χρήστη"
-
-msgid "User Management"
-msgstr "Διαχείριση Χρήστη"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/el/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/es/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/es/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Spanish (https://www.transifex.com/inveniosoftware/"
 "teams/23537/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Access: Roles"
 msgstr "Acceso: Roles"
 
 msgid "Access: System Roles"
 msgstr "Acceso: Roles del Sistema"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/es/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/et/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/et/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: et\n"
 "Language-Team: Estonian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/et/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Access: Roles"
 msgstr "Juurdepääs: Rollid"
 
 msgid "Access: System Roles"
 msgstr "Juurdepääs: Süsteemi Rollid"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/et/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-access 1.4.4*

 * *Files 2% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 00000190: 616c 3d28 6e20 213d 2031 293b 0a4d 494d  al=(n != 1);.MIM
 000001a0: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
 000001b0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
 000001c0: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
 000001d0: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
 000001e0: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
 000001f0: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
-00000200: 2d42 793a 2042 6162 656c 2032 2e31 312e  -By: Babel 2.11.
-00000210: 300a 00                                  0..
+00000200: 2d42 793a 2042 6162 656c 2032 2e31 322e  -By: Babel 2.12.
+00000210: 310a 00                                  1..
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/fa/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,14 +8,14 @@
 "Language: fa\n"
 "Language-Team: Persian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/fa/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "ایمیل"
 
 msgid "User ID"
 msgstr "هویت کاربر"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/fa/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/fr/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: French (https://www.transifex.com/inveniosoftware/teams/23537/"
 "fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Role Name"
 msgstr "Nom du Rôle"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/fr/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/gl/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/rw/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-access 1.4.4*

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
-00000020: 2c00 0000 d501 0000 2d00 0000 0050 726f  ,.......-....Pro
+00000020: 2c00 0000 d801 0000 2d00 0000 0050 726f  ,.......-....Pro
 00000030: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
 00000040: 2069 6e76 656e 696f 2d61 6363 6573 7320   invenio-access 
 00000050: 312e 342e 340a 5265 706f 7274 2d4d 7367  1.4.4.Report-Msg
 00000060: 6964 2d42 7567 732d 546f 3a20 696e 666f  id-Bugs-To: info
 00000070: 4069 6e76 656e 696f 736f 6674 7761 7265  @inveniosoftware
 00000080: 2e6f 7267 0a50 4f54 2d43 7265 6174 696f  .org.POT-Creatio
 00000090: 6e2d 4461 7465 3a20 3230 3232 2d31 302d  n-Date: 2022-10-
 000000a0: 3132 2030 393a 3033 2b30 3030 300a 504f  12 09:03+0000.PO
 000000b0: 2d52 6576 6973 696f 6e2d 4461 7465 3a20  -Revision-Date: 
 000000c0: 3230 3136 2d30 382d 3138 2031 323a 3038  2016-08-18 12:08
 000000d0: 2b30 3030 300a 4c61 7374 2d54 7261 6e73  +0000.Last-Trans
 000000e0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
 000000f0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
-00000100: 0a4c 616e 6775 6167 653a 2067 6c0a 4c61  .Language: gl.La
-00000110: 6e67 7561 6765 2d54 6561 6d3a 2047 616c  nguage-Team: Gal
-00000120: 6963 6961 6e20 2868 7474 7073 3a2f 2f77  ician (https://w
-00000130: 7777 2e74 7261 6e73 6966 6578 2e63 6f6d  ww.transifex.com
-00000140: 2f69 6e76 656e 696f 736f 6674 7761 7265  /inveniosoftware
-00000150: 2f74 6561 6d73 2f32 3335 3337 2f67 6c2f  /teams/23537/gl/
-00000160: 290a 506c 7572 616c 2d46 6f72 6d73 3a20  ).Plural-Forms: 
-00000170: 6e70 6c75 7261 6c73 3d32 3b20 706c 7572  nplurals=2; plur
-00000180: 616c 3d28 6e20 213d 2031 293b 0a4d 494d  al=(n != 1);.MIM
-00000190: 452d 5665 7273 696f 6e3a 2031 2e30 0a43  E-Version: 1.0.C
-000001a0: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
-000001b0: 742f 706c 6169 6e3b 2063 6861 7273 6574  t/plain; charset
-000001c0: 3d75 7466 2d38 0a43 6f6e 7465 6e74 2d54  =utf-8.Content-T
-000001d0: 7261 6e73 6665 722d 456e 636f 6469 6e67  ransfer-Encoding
-000001e0: 3a20 3862 6974 0a47 656e 6572 6174 6564  : 8bit.Generated
-000001f0: 2d42 793a 2042 6162 656c 2032 2e31 312e  -By: Babel 2.11.
-00000200: 300a 00                                  0..
+00000100: 0a4c 616e 6775 6167 653a 2072 770a 4c61  .Language: rw.La
+00000110: 6e67 7561 6765 2d54 6561 6d3a 204b 696e  nguage-Team: Kin
+00000120: 7961 7277 616e 6461 2028 6874 7470 733a  yarwanda (https:
+00000130: 2f2f 7777 772e 7472 616e 7369 6665 782e  //www.transifex.
+00000140: 636f 6d2f 696e 7665 6e69 6f73 6f66 7477  com/inveniosoftw
+00000150: 6172 652f 7465 616d 732f 3233 3533 372f  are/teams/23537/
+00000160: 7277 2f29 0a50 6c75 7261 6c2d 466f 726d  rw/).Plural-Form
+00000170: 733a 206e 706c 7572 616c 733d 323b 2070  s: nplurals=2; p
+00000180: 6c75 7261 6c3d 286e 2021 3d20 3129 3b0a  lural=(n != 1);.
+00000190: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
+000001a0: 300a 436f 6e74 656e 742d 5479 7065 3a20  0.Content-Type: 
+000001b0: 7465 7874 2f70 6c61 696e 3b20 6368 6172  text/plain; char
+000001c0: 7365 743d 7574 662d 380a 436f 6e74 656e  set=utf-8.Conten
+000001d0: 742d 5472 616e 7366 6572 2d45 6e63 6f64  t-Transfer-Encod
+000001e0: 696e 673a 2038 6269 740a 4765 6e65 7261  ing: 8bit.Genera
+000001f0: 7465 642d 4279 3a20 4261 6265 6c20 322e  ted-By: Babel 2.
+00000200: 3132 2e31 0a00                           12.1..
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/gl/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/hr/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/hr/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,14 +9,14 @@
 "Language-Team: Croatian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/hr/)\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "User ID"
 msgstr "Korisničko ime"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/hr/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/hu/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: hu\n"
 "Language-Team: Hungarian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/hu/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Access: Roles"
 msgstr "Hozzáférés: Szerepkörök"
 
 msgid "Access: System Roles"
 msgstr "Hozzáférés: Rendszer szerepkörök"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/hu/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/it/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/it/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Italian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/it/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Role Name"
 msgstr "Nome di Ruolo"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/it/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/ja/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,14 +8,14 @@
 "Language: ja\n"
 "Language-Team: Japanese (https://www.transifex.com/inveniosoftware/"
 "teams/23537/ja/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Ｅメイル"
 
 msgid "User ID"
 msgstr "ユーザＩＤ"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/ja/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/ka/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/ka/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,14 +8,14 @@
 "Language: ka\n"
 "Language-Team: Georgian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/ka/)\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "ელფოსტა"
 
 msgid "User ID"
 msgstr "მომხმარებლის საიდენტიფიკაციო"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/ka/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/lt/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/lt/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -10,14 +10,14 @@
 "teams/23537/lt/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
 "1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Elektroninis paštas"
 
 msgid "User ID"
 msgstr "Vartotojo ID"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/lt/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/messages.pot` & `invenio-access-2.0.0/invenio_access/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/no/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/no/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,14 +8,14 @@
 "Language: no\n"
 "Language-Team: Norwegian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/no/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "E-post"
 
 msgid "User ID"
 msgstr "Bruker-ID"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/no/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/pl/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -10,14 +10,14 @@
 "pl/)\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
 "n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "User ID"
 msgstr "ID użytkownika"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/pl/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/pt/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,11 +9,11 @@
 "Language-Team: Portuguese (https://www.transifex.com/inveniosoftware/"
 "teams/23537/pt/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "User ID"
 msgstr "ID de Utilizador"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/pt/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/ro/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/ro/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,14 +9,14 @@
 "Language-Team: Romanian (https://www.transifex.com/inveniosoftware/"
 "teams/23537/ro/)\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "E-mail"
 
 msgid "User ID"
 msgstr "ID Utilizator"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/ro/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/ru/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -10,14 +10,14 @@
 "teams/23537/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "Электронная почта"
 
 msgid "User ID"
 msgstr "Идентификатор (ID) пользователя"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/ru/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/rw/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -0,0 +1,21 @@
+msgid ""
+msgstr ""
+"Project-Id-Version: invenio-access 1.4.4\n"
+"Report-Msgid-Bugs-To: info@inveniosoftware.org\n"
+"POT-Creation-Date: 2022-10-12 09:03+0000\n"
+"PO-Revision-Date: 2016-08-18 12:08+0000\n"
+"Last-Translator: Tibor Simko <tibor.simko@cern.ch>, 2016\n"
+"Language: zh_TW\n"
+"Language-Team: Chinese (Taiwan) (https://www.transifex.com/inveniosoftware/"
+"teams/23537/zh_TW/)\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=utf-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Generated-By: Babel 2.12.1\n"
+
+msgid "Email"
+msgstr "電郵"
+
+msgid "User ID"
+msgstr "用戶ID"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/rw/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/sk/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/sk/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language-Team: Slovak (https://www.transifex.com/inveniosoftware/teams/23537/"
 "sk/)\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "E-mail"
 
 msgid "Role Name"
 msgstr "Názov role"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/sk/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/sv/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: sv\n"
 "Language-Team: Swedish (https://www.transifex.com/inveniosoftware/"
 "teams/23537/sv/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Access: Roles"
 msgstr "Tillgång: Roller"
 
 msgid "Access: System Roles"
 msgstr "Tillgång: Systemroller"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/sv/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/tr/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,15 +9,15 @@
 "Language: tr\n"
 "Language-Team: Turkish (https://www.transifex.com/inveniosoftware/"
 "teams/23537/tr/)\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Email"
 msgstr "E-posta"
 
 msgid "Role Name"
 msgstr "Rol Adı"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/tr/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/uk/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/uk/LC_MESSAGES/messages.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: invenio-access 1.4.4*

 * *Files 2% similar despite different names*

```diff
@@ -39,9 +39,9 @@
 00000260: 2929 203f 2032 3a20 3329 3b0a 4d49 4d45  )) ? 2: 3);.MIME
 00000270: 2d56 6572 7369 6f6e 3a20 312e 300a 436f  -Version: 1.0.Co
 00000280: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
 00000290: 2f70 6c61 696e 3b20 6368 6172 7365 743d  /plain; charset=
 000002a0: 7574 662d 380a 436f 6e74 656e 742d 5472  utf-8.Content-Tr
 000002b0: 616e 7366 6572 2d45 6e63 6f64 696e 673a  ansfer-Encoding:
 000002c0: 2038 6269 740a 4765 6e65 7261 7465 642d   8bit.Generated-
-000002d0: 4279 3a20 4261 6265 6c20 322e 3131 2e30  By: Babel 2.11.0
+000002d0: 4279 3a20 4261 6265 6c20 322e 3132 2e31  By: Babel 2.12.1
 000002e0: 0a00                                     ..
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/uk/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-access-2.0.0/invenio_access/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: zh_CN\n"
 "Language-Team: Chinese (China) (https://www.transifex.com/inveniosoftware/"
 "teams/23537/zh_CN/)\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.11.0\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "Access: Roles"
 msgstr "访问：角色"
 
 msgid "Access: System Roles"
 msgstr "访问：系统角色"
```

### Comparing `invenio-access-1.4.5/invenio_access/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-access-2.0.0/invenio_access/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access/utils.py` & `invenio-access-2.0.0/invenio_access/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/invenio_access.egg-info/PKG-INFO` & `invenio-access-2.0.0/invenio_access.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-access
-Version: 1.4.5
+Version: 2.0.0
 Summary: Invenio module for common role based access control.
 Home-page: https://github.com/inveniosoftware/invenio-access
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -57,14 +57,19 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.0.0 (released 2022-06-14)
+        
+        - upgrade invenio-accounts dependency
+        - models: change role_id FK of ActionRoles to string
+        
         Version 1.4.4 (released 2022-04-01)
         
         - fix compat issue with Werkzeug 2.1
         
         Version 1.4.3 (released 2022-03-30)
         
         - add support for Flask 2.1, Werkzeug 2.1 and Click 8.1
```

### Comparing `invenio-access-1.4.5/invenio_access.egg-info/SOURCES.txt` & `invenio-access-2.0.0/invenio_access.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,17 @@
 invenio_access.egg-info/not-zip-safe
 invenio_access.egg-info/requires.txt
 invenio_access.egg-info/top_level.txt
 invenio_access/alembic/04480be1593e_add_actionsystemroles.py
 invenio_access/alembic/2069a982633b_add_on_delete_cascade_constraint.py
 invenio_access/alembic/2f63be7b7572_create_access_tables.py
 invenio_access/alembic/67ba0de65fbb_create_access_branch.py
+invenio_access/alembic/842a62b56e60_change_fk_accountsrole_to_string_downgrade.py
 invenio_access/alembic/dbe499bfda43_prevent_null_in_actionusers_for_.py
+invenio_access/alembic/f9843093f686_change_fk_accountsrole_to_string_upgrade.py
 invenio_access/translations/messages.pot
 invenio_access/translations/af/LC_MESSAGES/messages.mo
 invenio_access/translations/af/LC_MESSAGES/messages.po
 invenio_access/translations/ar/LC_MESSAGES/messages.mo
 invenio_access/translations/ar/LC_MESSAGES/messages.po
 invenio_access/translations/bg/LC_MESSAGES/messages.mo
 invenio_access/translations/bg/LC_MESSAGES/messages.po
```

### Comparing `invenio-access-1.4.5/invenio_access.egg-info/entry_points.txt` & `invenio-access-2.0.0/invenio_access.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/setup.cfg` & `invenio-access-2.0.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 [options]
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	invenio-admin>=1.2.0
-	invenio-accounts>=1.4.13
+	invenio-accounts>=3.0.0
 	invenio-base>=1.2.11
-	invenio-i18n>=1.3.2
+	invenio-i18n>=2.0.0
 
 [options.extras_require]
 tests = 
 	pytest-black>=0.3.0,<0.3.10
 	cachelib>=0.1
 	pytest-invenio>=1.4.1
-	invenio-db[mysql, postgresql]>=1.0.14
+	invenio-db[mysql, postgresql]>=1.1.2
 	redis>=2.10.5
 	sphinx>=4.5
 postgresql = 
 mysql = 
 sqlite = 
 
 [options.entry_points]
```

### Comparing `invenio-access-1.4.5/tests/conftest.py` & `invenio-access-2.0.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 import os
 import warnings
 
 import pytest
 from flask import Flask
 from flask.cli import ScriptInfo
-from flask_babelex import Babel
 from flask_mail import Mail
 from flask_principal import ActionNeed, identity_loaded
 from invenio_accounts import InvenioAccounts
 from invenio_db import InvenioDB, db
+from invenio_i18n import InvenioI18N
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.schema import DropConstraint, DropSequence, DropTable
 
 from invenio_access import InvenioAccess
 from invenio_access.loaders import load_permissions_on_identity_loaded
 from invenio_access.permissions import ParameterizedActionNeed, Permission
 
@@ -52,29 +52,28 @@
         SECURITY_PASSWORD_SALT="CHANGE_ME_ALSO",
         SQLALCHEMY_DATABASE_URI=os.environ.get(
             "SQLALCHEMY_DATABASE_URI", "sqlite:///test.db"
         ),
         SQLALCHEMY_TRACK_MODIFICATIONS=False,
         TESTING=True,
     )
-    Babel(app_)
     Mail(app_)
     InvenioDB(app_)
+    InvenioI18N(app_)
     InvenioAccounts(app_)
     return app_
 
 
 @pytest.fixture()
 def app(base_app, request):
     """Flask application fixture."""
     with base_app.app_context():
         db.create_all()
 
     def teardown():
-
         with base_app.app_context():
             db.drop_all()
             identity_loaded.disconnect(load_permissions_on_identity_loaded)
 
     request.addfinalizer(teardown)
     return base_app
```

### Comparing `invenio-access-1.4.5/tests/test_admin.py` & `invenio-access-2.0.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/tests/test_cli.py` & `invenio-access-2.0.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,14 @@
     def role_args(roles):
         """Generate role arguments."""
         for role in roles:
             yield "role"
             yield role
 
     for action, roles in action_roles.items():
-
         result = runner.invoke(
             access,
             ["allow", action] + list(role_args(roles)),
         )
         assert result.exit_code == 0
 
     result = runner.invoke(
@@ -247,15 +246,14 @@
     assert "role:editor:edit::allow\n" == result.output
     assert result.exit_code == 0
 
     #
     # Remove all permissions.
     #
     for action, roles in action_roles.items():
-
         result = runner.invoke(
             access,
             ["remove", action] + list(role_args(roles)),
         )
         assert result.exit_code == 0
 
     result = runner.invoke(
```

### Comparing `invenio-access-1.4.5/tests/test_invenio_access.py` & `invenio-access-2.0.0/tests/test_invenio_access.py`

 * *Files identical despite different names*

### Comparing `invenio-access-1.4.5/tests/test_loaders.py` & `invenio-access-2.0.0/tests/test_loaders.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2017-2018 CERN.
+# Copyright (C) 2017-2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Test Indentity loaders."""
 
 from flask import current_app, g
@@ -22,55 +22,51 @@
 from invenio_access.loaders import load_permissions_on_identity_loaded
 from invenio_access.permissions import any_user, authenticated_user
 
 
 def test_load_permissions_on_request_loaded(app):
     """Checks that the needs are loaded during request in the user Identity."""
     InvenioAccess(app)
-    with app.test_request_context():
-        with app.test_client() as client:
-            client.get("/")
-            assert g.identity.provides == {any_user}
+    with app.test_client() as client:
+        client.get("/")
+        assert g.identity.provides == {any_user}
 
 
 def test_load_permissions_on_identity_loaded(app):
     """Check that the needs are loaded properly in the user Identity."""
     InvenioAccess(app)
 
-    with app.test_request_context():
-        identity_changed.send(
-            current_app._get_current_object(), identity=AnonymousIdentity()
-        )
-        assert g.identity.provides == {any_user}
-
-    with app.test_request_context():
-        user = testutils.create_test_user("test@example.org")
-        login_user(user)
-        assert g.identity.provides == {any_user, authenticated_user, UserNeed(user.id)}
-        logout_user()
-        # FIXME: The user is still authenticatd when the identity loader
-        # is called during logout. We could filter on AnonymousIdentity, but
-        # This would be inconsistent as the UserNeed(user.id) is still there.
-        # This will pass even if it is unexpected:
-        # assert g.identity.provides == {
-        #     any_user, authenticated_user, UserNeed(user.id)
-        # }
-        # Forcing the identity to reload again cleans the mess. In practice
-        # this won't be needed as the identity is reloaded between requests.
-        identity_changed.send(
-            current_app._get_current_object(), identity=AnonymousIdentity()
-        )
-        assert g.identity.provides == {any_user}
+    identity_changed.send(
+        current_app._get_current_object(), identity=AnonymousIdentity()
+    )
+    assert g.identity.provides == {any_user}
+
+    user = testutils.create_test_user("test@example.org")
+    login_user(user)
+    assert g.identity.provides == {any_user, authenticated_user, UserNeed(user.id)}
+    logout_user()
+    # FIXME: The user is still authenticatd when the identity loader
+    # is called during logout. We could filter on AnonymousIdentity, but
+    # This would be inconsistent as the UserNeed(user.id) is still there.
+    # This will pass even if it is unexpected:
+    # assert g.identity.provides == {
+    #     any_user, authenticated_user, UserNeed(user.id)
+    # }
+    # Forcing the identity to reload again cleans the mess. In practice
+    # this won't be needed as the identity is reloaded between requests.
+    identity_changed.send(
+        current_app._get_current_object(), identity=AnonymousIdentity()
+    )
+    assert g.identity.provides == {any_user}
 
 
 def test_disabled_loader(app):
     """Check that system role loading function can be disabled."""
     app.config.update(ACCESS_LOAD_SYSTEM_ROLE_NEEDS=False)
     InvenioAccess(app)
 
     assert load_permissions_on_identity_loaded not in identity_loaded.receivers.values()
 
-    with app.test_request_context():
-        identity_changed.send(
-            current_app._get_current_object(), identity=AnonymousIdentity()
-        )
-        assert g.identity.provides == set()
+    identity_changed.send(
+        current_app._get_current_object(), identity=AnonymousIdentity()
+    )
+    assert g.identity.provides == set()
```

### Comparing `invenio-access-1.4.5/tests/test_permissions.py` & `invenio-access-2.0.0/tests/test_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2019 CERN.
+# Copyright (C) 2015-2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Tests for Permission class."""
 
 import pytest
@@ -80,15 +80,15 @@
     return [WithUserIdentity(user) for user in users]
 
 
 def create_roles(*names):
     """Helper to create roles."""
     roles = []
     for name in names:
-        role = Role(name=name)
+        role = Role(id=name, name=name)
         db.session.add(role)
         roles.append(role)
     db.session.commit()
     return roles
 
 
 def assign_roles(users_roles):
```

### Comparing `invenio-access-1.4.5/tests/test_permissions_cache.py` & `invenio-access-2.0.0/tests/test_permissions_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2015-2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Module tests."""
 
 import time
@@ -27,941 +27,932 @@
         self.provides = provides
 
 
 def test_invenio_access_permission_cache(app, dynamic_permission):
     """Caching the user using memory caching."""
     cache = SimpleCache()
     InvenioAccess(app, cache=cache)
-    with app.test_request_context():
-        user_can_all = User(email="all@inveniosoftware.org")
-        user_can_open = User(email="open@inveniosoftware.org")
-        user_can_open_1 = User(email="open1@inveniosoftware.org")
-
-        db.session.add(user_can_all)
-        db.session.add(user_can_open)
-        db.session.add(user_can_open_1)
-
-        db.session.add(ActionUsers(action="open", user=user_can_all))
-
-        db.session.flush()
-
-        permission_open = dynamic_permission(ActionNeed("open"))
-
-        identity_open = FakeIdentity(UserNeed(user_can_open.id))
-
-        assert not permission_open.allows(identity_open)
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1)]),
-            set([]),
-        )
-
-        db.session.add(ActionUsers(action="open", user=user_can_open))
-        db.session.flush()
-
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_open)
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
-        )
-
-        db.session.add(ActionUsers(action="open", argument=1, user=user_can_open_1))
-        db.session.flush()
-
-        identity_open_1 = FakeIdentity(UserNeed(user_can_open_1.id))
-        permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
-        assert not permission_open.allows(identity_open_1)
-        assert permission_open_1.allows(identity_open_1)
-        assert current_access.get_action_cache("open::1") == (
-            set(
-                [
-                    Need(method="id", value=1),
-                    Need(method="id", value=2),
-                    Need(method="id", value=3),
-                ]
-            ),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
-        )
+    user_can_all = User(email="all@inveniosoftware.org")
+    user_can_open = User(email="open@inveniosoftware.org")
+    user_can_open_1 = User(email="open1@inveniosoftware.org")
+
+    db.session.add(user_can_all)
+    db.session.add(user_can_open)
+    db.session.add(user_can_open_1)
+
+    db.session.add(ActionUsers(action="open", user=user_can_all))
+
+    db.session.flush()
+
+    permission_open = dynamic_permission(ActionNeed("open"))
+
+    identity_open = FakeIdentity(UserNeed(user_can_open.id))
+
+    assert not permission_open.allows(identity_open)
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1)]),
+        set([]),
+    )
+
+    db.session.add(ActionUsers(action="open", user=user_can_open))
+    db.session.flush()
+
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_open)
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
+
+    db.session.add(ActionUsers(action="open", argument=1, user=user_can_open_1))
+    db.session.flush()
+
+    identity_open_1 = FakeIdentity(UserNeed(user_can_open_1.id))
+    permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
+    assert not permission_open.allows(identity_open_1)
+    assert permission_open_1.allows(identity_open_1)
+    assert current_access.get_action_cache("open::1") == (
+        set(
+            [
+                Need(method="id", value=1),
+                Need(method="id", value=2),
+                Need(method="id", value=3),
+            ]
+        ),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
 
 
 def test_invenio_access_permission_cache_redis(app, dynamic_permission):
     """Caching the user using redis."""
     cache = RedisCache()
     InvenioAccess(app, cache=cache)
-    with app.test_request_context():
-        user_can_all = User(email="all@inveniosoftware.org")
-        user_can_open = User(email="open@inveniosoftware.org")
-        user_can_open_1 = User(email="open1@inveniosoftware.org")
-
-        db.session.add(user_can_all)
-        db.session.add(user_can_open)
-        db.session.add(user_can_open_1)
+    user_can_all = User(email="all@inveniosoftware.org")
+    user_can_open = User(email="open@inveniosoftware.org")
+    user_can_open_1 = User(email="open1@inveniosoftware.org")
+
+    db.session.add(user_can_all)
+    db.session.add(user_can_open)
+    db.session.add(user_can_open_1)
+
+    db.session.add(ActionUsers(action="open", user=user_can_all))
+
+    db.session.flush()
+
+    identity_open = FakeIdentity(UserNeed(user_can_open.id))
+
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert not permission_open.allows(identity_open)
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1)]),
+        set([]),
+    )
+
+    db.session.add(ActionUsers(action="open", user=user_can_open))
+    db.session.flush()
+
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_open)
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
+
+    db.session.add(ActionUsers(action="open", argument=1, user=user_can_open_1))
+
+    db.session.flush()
+
+    identity_open_1 = FakeIdentity(UserNeed(user_can_open_1.id))
+    permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
+    assert not permission_open.allows(identity_open_1)
+    assert permission_open_1.allows(identity_open_1)
+    assert current_access.get_action_cache("open::1") == (
+        set(
+            [
+                Need(method="id", value=1),
+                Need(method="id", value=2),
+                Need(method="id", value=3),
+            ]
+        ),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
 
-        db.session.add(ActionUsers(action="open", user=user_can_all))
 
-        db.session.flush()
+def test_invenio_access_cache_performance(app, dynamic_permission):
+    """Performance test simulating 1000 users."""
+    InvenioAccess(app, cache=None)
+    # CDS has (2015-11-19) 74 actions with 414 possible arguments with
+    # 49259 users and 307 roles. In this test we are going to divide
+    # into 50 and use the next prime number.
+    users_number = 991
+    actions_users_number = 11
+    actions_roles_number = 7
 
-        identity_open = FakeIdentity(UserNeed(user_can_open.id))
+    roles = []
+    actions = []
+    for i in range(actions_roles_number):
+        role = Role(id=str(i), name="role{0}".format(i))
+        roles.append(role)
+        db.session.add(role)
+        db.session.flush()
 
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert not permission_open.allows(identity_open)
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1)]),
-            set([]),
+        action_role = ActionRoles(
+            action="action{0}".format(str(i % actions_roles_number)), role=role
         )
-
-        db.session.add(ActionUsers(action="open", user=user_can_open))
+        actions.append(action_role)
+        db.session.add(action_role)
         db.session.flush()
 
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_open)
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
+    users = []
+    for i in range(users_number):
+        user = User(
+            email="invenio{0}@inveniosoftware.org".format(str(i)),
+            roles=[roles[i % actions_roles_number]],
         )
-
-        db.session.add(ActionUsers(action="open", argument=1, user=user_can_open_1))
-
+        users.append(user)
+        db.session.add(user)
         db.session.flush()
 
-        identity_open_1 = FakeIdentity(UserNeed(user_can_open_1.id))
-        permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
-        assert not permission_open.allows(identity_open_1)
-        assert permission_open_1.allows(identity_open_1)
-        assert current_access.get_action_cache("open::1") == (
-            set(
-                [
-                    Need(method="id", value=1),
-                    Need(method="id", value=2),
-                    Need(method="id", value=3),
-                ]
+        action_user = ActionUsers(
+            action="action{0}".format(
+                str((i % actions_users_number) + actions_roles_number)
             ),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
+            user=user,
         )
+        actions.append(action_user)
+        db.session.add(action_user)
+        db.session.flush()
 
-
-def test_intenio_access_cache_performance(app, dynamic_permission):
-    """Performance test simulating 1000 users."""
-    InvenioAccess(app, cache=None)
-    with app.test_request_context():
-        # CDS has (2015-11-19) 74 actions with 414 possible arguments with
-        # 49259 users and 307 roles. In this test we are going to divide
-        # into 50 and use the next prime number.
-        users_number = 991
-        actions_users_number = 11
-        actions_roles_number = 7
-
-        roles = []
-        actions = []
-        for i in range(actions_roles_number):
-            role = Role(name="role{0}".format(i))
-            roles.append(role)
-            db.session.add(role)
-            db.session.flush()
-
-            action_role = ActionRoles(
-                action="action{0}".format(str(i % actions_roles_number)), role=role
-            )
-            actions.append(action_role)
-            db.session.add(action_role)
-            db.session.flush()
-
-        users = []
+    def test_permissions():
+        """Iterates over all users checking its permissions."""
         for i in range(users_number):
-            user = User(
-                email="invenio{0}@inveniosoftware.org".format(str(i)),
-                roles=[roles[i % actions_roles_number]],
-            )
-            users.append(user)
-            db.session.add(user)
-            db.session.flush()
-
-            action_user = ActionUsers(
-                action="action{0}".format(
-                    str((i % actions_users_number) + actions_roles_number)
+            identity = FakeIdentity(UserNeed(users[i].id))
+
+            # Allowed permission
+            permission_allowed_both = dynamic_permission(
+                ActionNeed(
+                    "action{0}".format(
+                        (i % actions_users_number) + actions_roles_number
+                    )
                 ),
-                user=user,
+                ActionNeed("action{0}".format(i % actions_roles_number)),
             )
-            actions.append(action_user)
-            db.session.add(action_user)
-            db.session.flush()
-
-        def test_permissions():
-            """Iterates over all users checking its permissions."""
-            for i in range(users_number):
-                identity = FakeIdentity(UserNeed(users[i].id))
-
-                # Allowed permission
-                permission_allowed_both = dynamic_permission(
-                    ActionNeed(
-                        "action{0}".format(
-                            (i % actions_users_number) + actions_roles_number
-                        )
-                    ),
-                    ActionNeed("action{0}".format(i % actions_roles_number)),
-                )
-                assert permission_allowed_both.allows(identity)
+            assert permission_allowed_both.allows(identity)
 
-                # Not allowed action user
-                permission_not_allowed_user = dynamic_permission(
-                    ActionNeed(
-                        "action{0}".format(
-                            (i + 1) % actions_users_number + actions_roles_number
-                        )
+            # Not allowed action user
+            permission_not_allowed_user = dynamic_permission(
+                ActionNeed(
+                    "action{0}".format(
+                        (i + 1) % actions_users_number + actions_roles_number
                     )
                 )
-                assert not permission_not_allowed_user.allows(identity)
+            )
+            assert not permission_not_allowed_user.allows(identity)
 
-                # Not allowed action role
-                permission_not_allowed_role = dynamic_permission(
-                    ActionNeed("action{0}".format((i + 1) % actions_roles_number))
-                )
-                assert not permission_not_allowed_role.allows(identity)
+            # Not allowed action role
+            permission_not_allowed_role = dynamic_permission(
+                ActionNeed("action{0}".format((i + 1) % actions_roles_number))
+            )
+            assert not permission_not_allowed_role.allows(identity)
 
-        app.extensions["invenio-access"].cache = None
-        start_time_wo_cache = time.time()
-        test_permissions()
-        end_time_wo_cache = time.time()
-        time_wo_cache = end_time_wo_cache - start_time_wo_cache
-
-        app.extensions["invenio-access"].cache = SimpleCache()
-        start_time_w_cache = time.time()
-        test_permissions()
-        end_time_w_cache = time.time()
-        time_w_cache = end_time_w_cache - start_time_w_cache
+    app.extensions["invenio-access"].cache = None
+    start_time_wo_cache = time.time()
+    test_permissions()
+    end_time_wo_cache = time.time()
+    time_wo_cache = end_time_wo_cache - start_time_wo_cache
+
+    app.extensions["invenio-access"].cache = SimpleCache()
+    start_time_w_cache = time.time()
+    test_permissions()
+    end_time_w_cache = time.time()
+    time_w_cache = end_time_w_cache - start_time_w_cache
 
-        assert time_wo_cache / time_w_cache > 10
+    assert time_wo_cache / time_w_cache > 10
 
 
 def test_invenio_access_permission_cache_users_updates(app, dynamic_permission):
     """Testing ActionUsers cache with inserts/updates/deletes."""
     cache = SimpleCache()
     InvenioAccess(app, cache=cache)
-    with app.test_request_context():
-        # Creation of some data to test.
-        user_1 = User(email="user_1@inveniosoftware.org")
-        user_2 = User(email="user_2@inveniosoftware.org")
-        user_3 = User(email="user_3@inveniosoftware.org")
-        user_4 = User(email="user_4@inveniosoftware.org")
-        user_5 = User(email="user_5@inveniosoftware.org")
-        user_6 = User(email="user_6@inveniosoftware.org")
-
-        db.session.add(user_1)
-        db.session.add(user_2)
-        db.session.add(user_3)
-        db.session.add(user_4)
-        db.session.add(user_5)
-        db.session.add(user_6)
-
-        db.session.add(ActionUsers(action="open", user=user_1))
-        db.session.add(ActionUsers(action="write", user=user_4))
-
-        db.session.flush()
-
-        # Creation identities to test.
-        identity_user_1 = FakeIdentity(UserNeed(user_1.id))
-        identity_user_2 = FakeIdentity(UserNeed(user_2.id))
-        identity_user_3 = FakeIdentity(UserNeed(user_3.id))
-        identity_user_4 = FakeIdentity(UserNeed(user_4.id))
-        identity_user_5 = FakeIdentity(UserNeed(user_5.id))
-        identity_user_6 = FakeIdentity(UserNeed(user_6.id))
-
-        # Test if user 1 can open. In this case, the cache should store only
-        # this object.
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_user_1)
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1)]),
-            set([]),
-        )
-
-        # Test if user 4 can write. In this case, the cache should have this
-        # new object and the previous one (Open is allowed to user_1)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_user_4)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="id", value=4)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1)]),
-            set([]),
-        )
-
-        # If we add a new user to the action open, the open action in cache
-        # should be removed but it should still containing the write entry.
-        db.session.add(ActionUsers(action="open", user=user_2))
-        db.session.flush()
-        assert current_access.get_action_cache("open") is None
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_user_2)
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="id", value=4)]),
-            set([]),
-        )
-
-        # Test if the new user is added to the action 'open'
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_user_4)
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="id", value=4)]),
-            set([]),
-        )
-
-        # If we update an action swapping a user, the cache containing the
-        # action, should be removed.
-        user_4_action_write = ActionUsers.query.filter(
-            ActionUsers.action == "write" and ActionUsers.user == user_4
-        ).first()
-        user_4_action_write.user = user_3
-        db.session.flush()
-        assert current_access.get_action_cache("write") is None
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
-        )
-
-        # Test if the user_3 can now write.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_user_4)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_user_3)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="id", value=3)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
-        )
-
-        # If we remove a user from an action, the cache should clear the
-        # action item.
-        user_3_action_write = ActionUsers.query.filter(
-            ActionUsers.action == "write" and ActionUsers.user == user_3
-        ).first()
-        db.session.delete(user_3_action_write)
-        db.session.flush()
-        assert current_access.get_action_cache("write") is None
-        # If no one is allowed to perform an action then everybody is allowed.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_user_3)
-        assert current_access.get_action_cache("write") == (set([]), set([]))
-        db.session.add(ActionUsers(action="write", user=user_5))
-        db.session.flush()
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_user_5)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_user_3)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="id", value=5)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
-        )
-
-        # If you update the name of an existing action, the previous action
-        # and the new action should be remove from cache.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_user_5)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="id", value=5)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="id", value=1), Need(method="id", value=2)]),
-            set([]),
-        )
-        user_5_action_write = ActionUsers.query.filter(
-            ActionUsers.action == "write" and ActionUsers.user == user_5
-        ).first()
-        user_5_action_write.action = "open"
-        db.session.flush()
-        assert current_access.get_action_cache("write") is None
-        assert current_access.get_action_cache("open") is None
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_user_1)
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="id", value=1),
-                    Need(method="id", value=2),
-                    Need(method="id", value=5),
-                ]
-            ),
-            set([]),
-        )
-        db.session.add(ActionUsers(action="write", user=user_4))
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_user_5)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="id", value=4)]),
-            set([]),
-        )
-
-        db.session.add(ActionUsers(action="open", argument="1", user=user_6))
-        db.session.flush()
-        permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
-        assert not permission_open.allows(identity_user_6)
-        assert permission_open_1.allows(identity_user_6)
-        assert current_access.get_action_cache("open::1") == (
-            set(
-                [
-                    Need(method="id", value=1),
-                    Need(method="id", value=2),
-                    Need(method="id", value=5),
-                    Need(method="id", value=6),
-                ]
-            ),
-            set([]),
-        )
-        user_6_action_open_1 = ActionUsers.query.filter_by(
-            action="open", argument="1", user_id=user_6.id
-        ).first()
-        user_6_action_open_1.argument = "2"
-        db.session.flush()
-        assert current_access.get_action_cache("open::1") is None
-        assert current_access.get_action_cache("open::2") is None
-        permission_open_2 = dynamic_permission(ParameterizedActionNeed("open", "2"))
-        assert permission_open_2.allows(identity_user_6)
-        assert current_access.get_action_cache("open::2") == (
-            set(
-                [
-                    Need(method="id", value=1),
-                    Need(method="id", value=2),
-                    Need(method="id", value=5),
-                    Need(method="id", value=6),
-                ]
-            ),
-            set([]),
-        )
-        # open action cache should remain as before
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="id", value=1),
-                    Need(method="id", value=2),
-                    Need(method="id", value=5),
-                ]
-            ),
-            set([]),
-        )
+    # Creation of some data to test.
+    user_1 = User(email="user_1@inveniosoftware.org")
+    user_2 = User(email="user_2@inveniosoftware.org")
+    user_3 = User(email="user_3@inveniosoftware.org")
+    user_4 = User(email="user_4@inveniosoftware.org")
+    user_5 = User(email="user_5@inveniosoftware.org")
+    user_6 = User(email="user_6@inveniosoftware.org")
+
+    db.session.add(user_1)
+    db.session.add(user_2)
+    db.session.add(user_3)
+    db.session.add(user_4)
+    db.session.add(user_5)
+    db.session.add(user_6)
+
+    db.session.add(ActionUsers(action="open", user=user_1))
+    db.session.add(ActionUsers(action="write", user=user_4))
+
+    db.session.flush()
+
+    # Creation identities to test.
+    identity_user_1 = FakeIdentity(UserNeed(user_1.id))
+    identity_user_2 = FakeIdentity(UserNeed(user_2.id))
+    identity_user_3 = FakeIdentity(UserNeed(user_3.id))
+    identity_user_4 = FakeIdentity(UserNeed(user_4.id))
+    identity_user_5 = FakeIdentity(UserNeed(user_5.id))
+    identity_user_6 = FakeIdentity(UserNeed(user_6.id))
+
+    # Test if user 1 can open. In this case, the cache should store only
+    # this object.
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_user_1)
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1)]),
+        set([]),
+    )
+
+    # Test if user 4 can write. In this case, the cache should have this
+    # new object and the previous one (Open is allowed to user_1)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_user_4)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="id", value=4)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1)]),
+        set([]),
+    )
+
+    # If we add a new user to the action open, the open action in cache
+    # should be removed but it should still containing the write entry.
+    db.session.add(ActionUsers(action="open", user=user_2))
+    db.session.flush()
+    assert current_access.get_action_cache("open") is None
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_user_2)
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="id", value=4)]),
+        set([]),
+    )
+
+    # Test if the new user is added to the action 'open'
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_user_4)
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="id", value=4)]),
+        set([]),
+    )
+
+    # If we update an action swapping a user, the cache containing the
+    # action, should be removed.
+    user_4_action_write = ActionUsers.query.filter(
+        ActionUsers.action == "write" and ActionUsers.user == user_4
+    ).first()
+    user_4_action_write.user = user_3
+    db.session.flush()
+    assert current_access.get_action_cache("write") is None
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
+
+    # Test if the user_3 can now write.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_user_4)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_user_3)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="id", value=3)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
+
+    # If we remove a user from an action, the cache should clear the
+    # action item.
+    user_3_action_write = ActionUsers.query.filter(
+        ActionUsers.action == "write" and ActionUsers.user == user_3
+    ).first()
+    db.session.delete(user_3_action_write)
+    db.session.flush()
+    assert current_access.get_action_cache("write") is None
+    # If no one is allowed to perform an action then everybody is allowed.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_user_3)
+    assert current_access.get_action_cache("write") == (set([]), set([]))
+    db.session.add(ActionUsers(action="write", user=user_5))
+    db.session.flush()
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_user_5)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_user_3)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="id", value=5)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
+
+    # If you update the name of an existing action, the previous action
+    # and the new action should be remove from cache.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_user_5)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="id", value=5)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="id", value=1), Need(method="id", value=2)]),
+        set([]),
+    )
+    user_5_action_write = ActionUsers.query.filter(
+        ActionUsers.action == "write" and ActionUsers.user == user_5
+    ).first()
+    user_5_action_write.action = "open"
+    db.session.flush()
+    assert current_access.get_action_cache("write") is None
+    assert current_access.get_action_cache("open") is None
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_user_1)
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="id", value=1),
+                Need(method="id", value=2),
+                Need(method="id", value=5),
+            ]
+        ),
+        set([]),
+    )
+    db.session.add(ActionUsers(action="write", user=user_4))
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_user_5)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="id", value=4)]),
+        set([]),
+    )
+
+    db.session.add(ActionUsers(action="open", argument="1", user=user_6))
+    db.session.flush()
+    permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
+    assert not permission_open.allows(identity_user_6)
+    assert permission_open_1.allows(identity_user_6)
+    assert current_access.get_action_cache("open::1") == (
+        set(
+            [
+                Need(method="id", value=1),
+                Need(method="id", value=2),
+                Need(method="id", value=5),
+                Need(method="id", value=6),
+            ]
+        ),
+        set([]),
+    )
+    user_6_action_open_1 = ActionUsers.query.filter_by(
+        action="open", argument="1", user_id=user_6.id
+    ).first()
+    user_6_action_open_1.argument = "2"
+    db.session.flush()
+    assert current_access.get_action_cache("open::1") is None
+    assert current_access.get_action_cache("open::2") is None
+    permission_open_2 = dynamic_permission(ParameterizedActionNeed("open", "2"))
+    assert permission_open_2.allows(identity_user_6)
+    assert current_access.get_action_cache("open::2") == (
+        set(
+            [
+                Need(method="id", value=1),
+                Need(method="id", value=2),
+                Need(method="id", value=5),
+                Need(method="id", value=6),
+            ]
+        ),
+        set([]),
+    )
+    # open action cache should remain as before
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="id", value=1),
+                Need(method="id", value=2),
+                Need(method="id", value=5),
+            ]
+        ),
+        set([]),
+    )
 
 
 def test_invenio_access_permission_cache_roles_updates(app, dynamic_permission):
     """Testing ActionRoles cache with inserts/updates/deletes."""
     # This test case is doing the same of user test case but using roles.
     cache = SimpleCache()
     InvenioAccess(app, cache=cache)
-    with app.test_request_context():
-        # Creation of some data to test.
-        role_1 = Role(name="role_1")
-        role_2 = Role(name="role_2")
-        role_3 = Role(name="role_3")
-        role_4 = Role(name="role_4")
-        role_5 = Role(name="role_5")
-        role_6 = Role(name="role_6")
-
-        db.session.add(role_1)
-        db.session.add(role_2)
-        db.session.add(role_3)
-        db.session.add(role_4)
-        db.session.add(role_5)
-        db.session.add(role_6)
-
-        db.session.add(ActionRoles(action="open", role=role_1))
-        db.session.add(ActionRoles(action="write", role=role_4))
-
-        db.session.flush()
-
-        # Creation of identities to test.
-        identity_fake_role_1 = FakeIdentity(RoleNeed(role_1.name))
-        identity_fake_role_2 = FakeIdentity(RoleNeed(role_2.name))
-        identity_fake_role_3 = FakeIdentity(RoleNeed(role_3.name))
-        identity_fake_role_4 = FakeIdentity(RoleNeed(role_4.name))
-        identity_fake_role_5 = FakeIdentity(RoleNeed(role_5.name))
-        identity_fake_role_6 = FakeIdentity(RoleNeed(role_6.name))
-
-        # Test if role 1 can open. In this case, the cache should store only
-        # this object.
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_fake_role_1)
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="role", value=role_1.name)]),
-            set([]),
-        )
-
-        # Test if role 4 can write. In this case, the cache should have this
-        # new object and the previous one (Open is allowed to role_1)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_role_4)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="role", value=role_4.name)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([Need(method="role", value=role_1.name)]),
-            set([]),
-        )
-
-        # If we add a new role to the action open, the open action in cache
-        # should be removed but it should still containing the write entry.
-        db.session.add(ActionRoles(action="open", role=role_2))
-        db.session.flush()
-        assert current_access.get_action_cache("open") is None
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_fake_role_2)
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                ]
-            ),
-            set([]),
-        )
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="role", value=role_4.name)]),
-            set([]),
-        )
-
-        # Test if the new role is added to the action 'open'
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_role_4)
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                ]
-            ),
-            set([]),
-        )
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="role", value=role_4.name)]),
-            set([]),
-        )
-
-        # If we update an action swapping a role, the cache containing the
-        # action, should be removed.
-        role_4_action_write = ActionRoles.query.filter(
-            ActionRoles.action == "write" and ActionRoles.role == role_4
-        ).first()
-        role_4_action_write.role = role_3
-        db.session.flush()
-
-        assert current_access.get_action_cache("write") is None
-        assert current_access.get_action_cache("open") is not None
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                ]
-            ),
-            set([]),
-        )
-
-        # Test if the role_3 can write now.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_fake_role_4)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_role_3)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="role", value=role_3.name)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                ]
-            ),
-            set([]),
-        )
-
-        # If we remove a role from an action, the cache should clear the
-        # action item.
-        role_3_action_write = ActionRoles.query.filter(
-            ActionRoles.action == "write" and ActionRoles.role == role_3
-        ).first()
-        db.session.delete(role_3_action_write)
-        db.session.flush()
-        assert current_access.get_action_cache("write") is None
-        # If no one is allowed to perform an action then everybody is allowed.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_role_3)
-        assert current_access.get_action_cache("write") == (set([]), set([]))
-        db.session.add(ActionRoles(action="write", role=role_5))
-        db.session.flush()
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_role_5)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_fake_role_3)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="role", value=role_5.name)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                ]
-            ),
-            set([]),
-        )
-
-        # If you update the name of an existing action, the previous action
-        # and the new action should be remove from cache.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_role_5)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="role", value=role_5.name)]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                ]
-            ),
-            set([]),
-        )
-        role_5_action_write = ActionRoles.query.filter(
-            ActionRoles.action == "write" and ActionRoles.role == role_5
-        ).first()
-        role_5_action_write.action = "open"
-        db.session.flush()
-        assert current_access.get_action_cache("write") is None
-        assert current_access.get_action_cache("open") is None
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_fake_role_1)
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                    Need(method="role", value=role_5.name),
-                ]
-            ),
-            set([]),
-        )
-        db.session.add(ActionRoles(action="write", role=role_4))
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_fake_role_5)
-        assert current_access.get_action_cache("write") == (
-            set([Need(method="role", value=role_4.name)]),
-            set([]),
-        )
-
-        db.session.add(ActionRoles(action="open", argument="1", role=role_6))
-        db.session.flush()
-        permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
-        assert not permission_open.allows(identity_fake_role_6)
-        assert permission_open_1.allows(identity_fake_role_6)
-        assert current_access.get_action_cache("open::1") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                    Need(method="role", value=role_5.name),
-                    Need(method="role", value=role_6.name),
-                ]
-            ),
-            set([]),
-        )
-        user_6_action_open_1 = ActionRoles.query.filter_by(
-            action="open", argument="1", role_id=role_6.id
-        ).first()
-        user_6_action_open_1.argument = "2"
-        db.session.flush()
-        assert current_access.get_action_cache("open::1") is None
-        assert current_access.get_action_cache("open::2") is None
-        permission_open_2 = dynamic_permission(ParameterizedActionNeed("open", "2"))
-        assert permission_open_2.allows(identity_fake_role_6)
-        assert current_access.get_action_cache("open::2") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                    Need(method="role", value=role_5.name),
-                    Need(method="role", value=role_6.name),
-                ]
-            ),
-            set([]),
-        )
-        # open action cache should remain as before
-        assert current_access.get_action_cache("open") == (
-            set(
-                [
-                    Need(method="role", value=role_1.name),
-                    Need(method="role", value=role_2.name),
-                    Need(method="role", value=role_5.name),
-                ]
-            ),
-            set([]),
-        )
+    # Creation of some data to test.
+    role_1 = Role(id="role_1", name="role_1")
+    role_2 = Role(id="role_2", name="role_2")
+    role_3 = Role(id="role_3", name="role_3")
+    role_4 = Role(id="role_4", name="role_4")
+    role_5 = Role(id="role_5", name="role_5")
+    role_6 = Role(id="role_6", name="role_6")
+
+    db.session.add(role_1)
+    db.session.add(role_2)
+    db.session.add(role_3)
+    db.session.add(role_4)
+    db.session.add(role_5)
+    db.session.add(role_6)
+
+    db.session.add(ActionRoles(action="open", role=role_1))
+    db.session.add(ActionRoles(action="write", role=role_4))
+
+    db.session.flush()
+
+    # Creation of identities to test.
+    identity_fake_role_1 = FakeIdentity(RoleNeed(role_1.name))
+    identity_fake_role_2 = FakeIdentity(RoleNeed(role_2.name))
+    identity_fake_role_3 = FakeIdentity(RoleNeed(role_3.name))
+    identity_fake_role_4 = FakeIdentity(RoleNeed(role_4.name))
+    identity_fake_role_5 = FakeIdentity(RoleNeed(role_5.name))
+    identity_fake_role_6 = FakeIdentity(RoleNeed(role_6.name))
+
+    # Test if role 1 can open. In this case, the cache should store only
+    # this object.
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_fake_role_1)
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="role", value=role_1.name)]),
+        set([]),
+    )
+
+    # Test if role 4 can write. In this case, the cache should have this
+    # new object and the previous one (Open is allowed to role_1)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_role_4)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="role", value=role_4.name)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([Need(method="role", value=role_1.name)]),
+        set([]),
+    )
+
+    # If we add a new role to the action open, the open action in cache
+    # should be removed but it should still containing the write entry.
+    db.session.add(ActionRoles(action="open", role=role_2))
+    db.session.flush()
+    assert current_access.get_action_cache("open") is None
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_fake_role_2)
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+            ]
+        ),
+        set([]),
+    )
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="role", value=role_4.name)]),
+        set([]),
+    )
+
+    # Test if the new role is added to the action 'open'
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_role_4)
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+            ]
+        ),
+        set([]),
+    )
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="role", value=role_4.name)]),
+        set([]),
+    )
+
+    # If we update an action swapping a role, the cache containing the
+    # action, should be removed.
+    role_4_action_write = ActionRoles.query.filter(
+        ActionRoles.action == "write" and ActionRoles.role == role_4
+    ).first()
+    role_4_action_write.role = role_3
+    db.session.flush()
+
+    assert current_access.get_action_cache("write") is None
+    assert current_access.get_action_cache("open") is not None
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+            ]
+        ),
+        set([]),
+    )
+
+    # Test if the role_3 can write now.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_fake_role_4)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_role_3)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="role", value=role_3.name)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+            ]
+        ),
+        set([]),
+    )
+
+    # If we remove a role from an action, the cache should clear the
+    # action item.
+    role_3_action_write = ActionRoles.query.filter(
+        ActionRoles.action == "write" and ActionRoles.role == role_3
+    ).first()
+    db.session.delete(role_3_action_write)
+    db.session.flush()
+    assert current_access.get_action_cache("write") is None
+    # If no one is allowed to perform an action then everybody is allowed.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_role_3)
+    assert current_access.get_action_cache("write") == (set([]), set([]))
+    db.session.add(ActionRoles(action="write", role=role_5))
+    db.session.flush()
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_role_5)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_fake_role_3)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="role", value=role_5.name)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+            ]
+        ),
+        set([]),
+    )
+
+    # If you update the name of an existing action, the previous action
+    # and the new action should be remove from cache.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_role_5)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="role", value=role_5.name)]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+            ]
+        ),
+        set([]),
+    )
+    role_5_action_write = ActionRoles.query.filter(
+        ActionRoles.action == "write" and ActionRoles.role == role_5
+    ).first()
+    role_5_action_write.action = "open"
+    db.session.flush()
+    assert current_access.get_action_cache("write") is None
+    assert current_access.get_action_cache("open") is None
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_fake_role_1)
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+                Need(method="role", value=role_5.name),
+            ]
+        ),
+        set([]),
+    )
+    db.session.add(ActionRoles(action="write", role=role_4))
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_fake_role_5)
+    assert current_access.get_action_cache("write") == (
+        set([Need(method="role", value=role_4.name)]),
+        set([]),
+    )
+
+    db.session.add(ActionRoles(action="open", argument="1", role=role_6))
+    db.session.flush()
+    permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
+    assert not permission_open.allows(identity_fake_role_6)
+    assert permission_open_1.allows(identity_fake_role_6)
+    assert current_access.get_action_cache("open::1") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+                Need(method="role", value=role_5.name),
+                Need(method="role", value=role_6.name),
+            ]
+        ),
+        set([]),
+    )
+    user_6_action_open_1 = ActionRoles.query.filter_by(
+        action="open", argument="1", role_id=role_6.id
+    ).first()
+    user_6_action_open_1.argument = "2"
+    db.session.flush()
+    assert current_access.get_action_cache("open::1") is None
+    assert current_access.get_action_cache("open::2") is None
+    permission_open_2 = dynamic_permission(ParameterizedActionNeed("open", "2"))
+    assert permission_open_2.allows(identity_fake_role_6)
+    assert current_access.get_action_cache("open::2") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+                Need(method="role", value=role_5.name),
+                Need(method="role", value=role_6.name),
+            ]
+        ),
+        set([]),
+    )
+    # open action cache should remain as before
+    assert current_access.get_action_cache("open") == (
+        set(
+            [
+                Need(method="role", value=role_1.name),
+                Need(method="role", value=role_2.name),
+                Need(method="role", value=role_5.name),
+            ]
+        ),
+        set([]),
+    )
 
 
 def test_invenio_access_permission_cache_system_roles_updates(app, dynamic_permission):
     """Testing ActionSystemRoles cache with inserts/updates/deletes."""
     # This test case is doing the same of user test case but using
     # system roles.
     cache = SimpleCache()
     InvenioAccess(app, cache=cache)
-    with app.test_request_context():
-        system_role_1 = SystemRoleNeed("system_role_1")
-        system_role_2 = SystemRoleNeed("system_role_2")
-        system_role_3 = SystemRoleNeed("system_role_3")
-        system_role_4 = SystemRoleNeed("system_role_4")
-        system_role_5 = SystemRoleNeed("system_role_5")
-        system_role_6 = SystemRoleNeed("system_role_6")
-        current_access.system_roles = {
-            "system_role_1": system_role_1,
-            "system_role_2": system_role_2,
-            "system_role_3": system_role_3,
-            "system_role_4": system_role_4,
-            "system_role_5": system_role_5,
-            "system_role_6": system_role_6,
-        }
-
-        # Creation of some data to test.
-        db.session.add(ActionSystemRoles(action="open", role_name=system_role_1.value))
-        db.session.add(ActionSystemRoles(action="write", role_name=system_role_4.value))
-
-        db.session.flush()
-
-        # Creation of identities to test.
-        identity_fake_1 = FakeIdentity(system_role_1)
-        identity_fake_2 = FakeIdentity(system_role_2)
-        identity_fake_3 = FakeIdentity(system_role_3)
-        identity_fake_4 = FakeIdentity(system_role_4)
-        identity_fake_5 = FakeIdentity(system_role_5)
-        identity_fake_6 = FakeIdentity(system_role_6)
-
-        # Test if system_role_1 can open. In this case, the cache should store
-        # only this object.
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_fake_1)
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1]),
-            set([]),
-        )
-
-        # Test if system_role_2 can write. In this case, the cache should
-        # have this new object and the previous one (Open is allowed to
-        # system_role_1)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_4)
-        assert current_access.get_action_cache("write") == (
-            set([system_role_4]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1]),
-            set([]),
-        )
-
-        # If we add a new system role to the action open, the open action in
-        # cache should be removed but it should still containing the write
-        # entry.
-        db.session.add(ActionSystemRoles(action="open", role_name=system_role_2.value))
-        db.session.flush()
-        assert current_access.get_action_cache("open") is None
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_fake_2)
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1, system_role_2]),
-            set([]),
-        )
-        assert current_access.get_action_cache("write") == (
-            set([system_role_4]),
-            set([]),
-        )
-
-        # Test if the new role is added to the action 'open'
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_4)
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1, system_role_2]),
-            set([]),
-        )
-        assert current_access.get_action_cache("write") == (
-            set([system_role_4]),
-            set([]),
-        )
-
-        # If we update an action swapping a role, the cache containing the
-        # action, should be removed.
-        role_4_action_write = ActionSystemRoles.query.filter(
-            ActionSystemRoles.action == "write"
-            and ActionSystemRoles.role_name == system_role_4.value
-        ).first()
-        role_4_action_write.role_name = system_role_3.value
-        db.session.flush()
-
-        assert current_access.get_action_cache("write") is None
-        assert current_access.get_action_cache("open") is not None
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1, system_role_2]),
-            set([]),
-        )
-
-        # Test if the system_role_3 can write now.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_fake_4)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_3)
-        assert current_access.get_action_cache("write") == (
-            set([system_role_3]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1, system_role_2]),
-            set([]),
-        )
-
-        # If we remove a role from an action, the cache should clear the
-        # action item.
-        cust_action_write = ActionSystemRoles.query.filter(
-            ActionSystemRoles.action == "write"
-            and ActionSystemRoles.role_name == system_role_3
-        ).first()
-        db.session.delete(cust_action_write)
-        db.session.flush()
-        assert current_access.get_action_cache("write") is None
-        # If no one is allowed to perform an action then everybody is allowed.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_3)
-        assert current_access.get_action_cache("write") == (set([]), set([]))
-        db.session.add(ActionSystemRoles(action="write", role_name=system_role_5.value))
-        db.session.flush()
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_5)
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_fake_3)
-        assert current_access.get_action_cache("write") == (
-            set([system_role_5]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1, system_role_2]),
-            set([]),
-        )
-
-        # If you update the name of an existing action, the previous action
-        # and the new action should be remove from cache.
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert permission_write.allows(identity_fake_5)
-        assert current_access.get_action_cache("write") == (
-            set([system_role_5]),
-            set([]),
-        )
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1, system_role_2]),
-            set([]),
-        )
-        role_5_action_write = ActionSystemRoles.query.filter(
-            ActionSystemRoles.action == "write"
-            and ActionSystemRoles.role_name == system_role_5.value
-        ).first()
-        role_5_action_write.action = "open"
-        db.session.flush()
-        assert current_access.get_action_cache("write") is None
-        assert current_access.get_action_cache("open") is None
-        permission_open = dynamic_permission(ActionNeed("open"))
-        assert permission_open.allows(identity_fake_1)
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1, system_role_2, system_role_5]),
-            set([]),
-        )
-        db.session.add(ActionSystemRoles(action="write", role_name=system_role_4.value))
-        permission_write = dynamic_permission(ActionNeed("write"))
-        assert not permission_write.allows(identity_fake_5)
-        assert current_access.get_action_cache("write") == (
-            set([system_role_4]),
-            set([]),
-        )
-
-        db.session.add(
-            ActionSystemRoles(
-                action="open", argument="1", role_name=system_role_6.value
-            )
-        )
-        db.session.flush()
-        permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
-        assert not permission_open.allows(identity_fake_6)
-        assert permission_open_1.allows(identity_fake_6)
-        assert current_access.get_action_cache("open::1") == (
-            set([system_role_1, system_role_2, system_role_5, system_role_6]),
-            set([]),
-        )
-        user_6_action_open_1 = ActionSystemRoles.query.filter_by(
-            action="open", argument="1", role_name=system_role_6.value
-        ).first()
-        user_6_action_open_1.argument = "2"
-        db.session.flush()
-        assert current_access.get_action_cache("open::1") is None
-        assert current_access.get_action_cache("open::2") is None
-        permission_open_2 = dynamic_permission(ParameterizedActionNeed("open", "2"))
-        assert permission_open_2.allows(identity_fake_6)
-        assert current_access.get_action_cache("open::2") == (
-            set([system_role_1, system_role_2, system_role_5, system_role_6]),
-            set([]),
-        )
-        # open action cache should remain as before
-        assert current_access.get_action_cache("open") == (
-            set([system_role_1, system_role_2, system_role_5]),
-            set([]),
-        )
+    system_role_1 = SystemRoleNeed("system_role_1")
+    system_role_2 = SystemRoleNeed("system_role_2")
+    system_role_3 = SystemRoleNeed("system_role_3")
+    system_role_4 = SystemRoleNeed("system_role_4")
+    system_role_5 = SystemRoleNeed("system_role_5")
+    system_role_6 = SystemRoleNeed("system_role_6")
+    current_access.system_roles = {
+        "system_role_1": system_role_1,
+        "system_role_2": system_role_2,
+        "system_role_3": system_role_3,
+        "system_role_4": system_role_4,
+        "system_role_5": system_role_5,
+        "system_role_6": system_role_6,
+    }
+
+    # Creation of some data to test.
+    db.session.add(ActionSystemRoles(action="open", role_name=system_role_1.value))
+    db.session.add(ActionSystemRoles(action="write", role_name=system_role_4.value))
+
+    db.session.flush()
+
+    # Creation of identities to test.
+    identity_fake_1 = FakeIdentity(system_role_1)
+    identity_fake_2 = FakeIdentity(system_role_2)
+    identity_fake_3 = FakeIdentity(system_role_3)
+    identity_fake_4 = FakeIdentity(system_role_4)
+    identity_fake_5 = FakeIdentity(system_role_5)
+    identity_fake_6 = FakeIdentity(system_role_6)
+
+    # Test if system_role_1 can open. In this case, the cache should store
+    # only this object.
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_fake_1)
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1]),
+        set([]),
+    )
+
+    # Test if system_role_2 can write. In this case, the cache should
+    # have this new object and the previous one (Open is allowed to
+    # system_role_1)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_4)
+    assert current_access.get_action_cache("write") == (
+        set([system_role_4]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1]),
+        set([]),
+    )
+
+    # If we add a new system role to the action open, the open action in
+    # cache should be removed but it should still containing the write
+    # entry.
+    db.session.add(ActionSystemRoles(action="open", role_name=system_role_2.value))
+    db.session.flush()
+    assert current_access.get_action_cache("open") is None
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_fake_2)
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1, system_role_2]),
+        set([]),
+    )
+    assert current_access.get_action_cache("write") == (
+        set([system_role_4]),
+        set([]),
+    )
+
+    # Test if the new role is added to the action 'open'
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_4)
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1, system_role_2]),
+        set([]),
+    )
+    assert current_access.get_action_cache("write") == (
+        set([system_role_4]),
+        set([]),
+    )
+
+    # If we update an action swapping a role, the cache containing the
+    # action, should be removed.
+    role_4_action_write = ActionSystemRoles.query.filter(
+        ActionSystemRoles.action == "write"
+        and ActionSystemRoles.role_name == system_role_4.value
+    ).first()
+    role_4_action_write.role_name = system_role_3.value
+    db.session.flush()
+
+    assert current_access.get_action_cache("write") is None
+    assert current_access.get_action_cache("open") is not None
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1, system_role_2]),
+        set([]),
+    )
+
+    # Test if the system_role_3 can write now.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_fake_4)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_3)
+    assert current_access.get_action_cache("write") == (
+        set([system_role_3]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1, system_role_2]),
+        set([]),
+    )
+
+    # If we remove a role from an action, the cache should clear the
+    # action item.
+    cust_action_write = ActionSystemRoles.query.filter(
+        ActionSystemRoles.action == "write"
+        and ActionSystemRoles.role_name == system_role_3
+    ).first()
+    db.session.delete(cust_action_write)
+    db.session.flush()
+    assert current_access.get_action_cache("write") is None
+    # If no one is allowed to perform an action then everybody is allowed.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_3)
+    assert current_access.get_action_cache("write") == (set([]), set([]))
+    db.session.add(ActionSystemRoles(action="write", role_name=system_role_5.value))
+    db.session.flush()
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_5)
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_fake_3)
+    assert current_access.get_action_cache("write") == (
+        set([system_role_5]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1, system_role_2]),
+        set([]),
+    )
+
+    # If you update the name of an existing action, the previous action
+    # and the new action should be remove from cache.
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert permission_write.allows(identity_fake_5)
+    assert current_access.get_action_cache("write") == (
+        set([system_role_5]),
+        set([]),
+    )
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1, system_role_2]),
+        set([]),
+    )
+    role_5_action_write = ActionSystemRoles.query.filter(
+        ActionSystemRoles.action == "write"
+        and ActionSystemRoles.role_name == system_role_5.value
+    ).first()
+    role_5_action_write.action = "open"
+    db.session.flush()
+    assert current_access.get_action_cache("write") is None
+    assert current_access.get_action_cache("open") is None
+    permission_open = dynamic_permission(ActionNeed("open"))
+    assert permission_open.allows(identity_fake_1)
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1, system_role_2, system_role_5]),
+        set([]),
+    )
+    db.session.add(ActionSystemRoles(action="write", role_name=system_role_4.value))
+    permission_write = dynamic_permission(ActionNeed("write"))
+    assert not permission_write.allows(identity_fake_5)
+    assert current_access.get_action_cache("write") == (
+        set([system_role_4]),
+        set([]),
+    )
+
+    db.session.add(
+        ActionSystemRoles(action="open", argument="1", role_name=system_role_6.value)
+    )
+    db.session.flush()
+    permission_open_1 = dynamic_permission(ParameterizedActionNeed("open", "1"))
+    assert not permission_open.allows(identity_fake_6)
+    assert permission_open_1.allows(identity_fake_6)
+    assert current_access.get_action_cache("open::1") == (
+        set([system_role_1, system_role_2, system_role_5, system_role_6]),
+        set([]),
+    )
+    user_6_action_open_1 = ActionSystemRoles.query.filter_by(
+        action="open", argument="1", role_name=system_role_6.value
+    ).first()
+    user_6_action_open_1.argument = "2"
+    db.session.flush()
+    assert current_access.get_action_cache("open::1") is None
+    assert current_access.get_action_cache("open::2") is None
+    permission_open_2 = dynamic_permission(ParameterizedActionNeed("open", "2"))
+    assert permission_open_2.allows(identity_fake_6)
+    assert current_access.get_action_cache("open::2") == (
+        set([system_role_1, system_role_2, system_role_5, system_role_6]),
+        set([]),
+    )
+    # open action cache should remain as before
+    assert current_access.get_action_cache("open") == (
+        set([system_role_1, system_role_2, system_role_5]),
+        set([]),
+    )
 
 
 def test_dynamic_permission_needs_cache_invalidation(app, dynamic_permission):
     """Testing DynamicPermission refreshes needs.
 
     This is important when protecting a view with
     @permission.require(http_exception=403)
     If cache does not get invalidated, the needs will only be refreshed when
     the Python process restarts.
     """
     cache = SimpleCache()
     InvenioAccess(app, cache=cache)
-    with app.test_request_context():
-        user_can_all = User(email="all@inveniosoftware.org")
-        user_can_open = User(email="open@inveniosoftware.org")
-        db.session.add(user_can_all)
-        db.session.add(user_can_open)
+    user_can_all = User(email="all@inveniosoftware.org")
+    user_can_open = User(email="open@inveniosoftware.org")
+    db.session.add(user_can_all)
+    db.session.add(user_can_open)
 
-        db.session.add(ActionUsers(action="open", user=user_can_all))
-        db.session.flush()
+    db.session.add(ActionUsers(action="open", user=user_can_all))
+    db.session.flush()
 
-        permission_open = dynamic_permission(ActionNeed("open"))
+    permission_open = dynamic_permission(ActionNeed("open"))
 
-        assert permission_open.needs == set([Need(method="id", value=1)])
+    assert permission_open.needs == set([Need(method="id", value=1)])
 
-        db.session.add(ActionUsers(action="open", user=user_can_open))
-        db.session.flush()
+    db.session.add(ActionUsers(action="open", user=user_can_open))
+    db.session.flush()
 
-        assert permission_open.needs == set(
-            [Need(method="id", value=1), Need(method="id", value=2)]
-        )
+    assert permission_open.needs == set(
+        [Need(method="id", value=1), Need(method="id", value=2)]
+    )
```

