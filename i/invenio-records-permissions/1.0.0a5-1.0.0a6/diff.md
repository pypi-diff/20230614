# Comparing `tmp/invenio-records-permissions-1.0.0a5.tar.gz` & `tmp/invenio-records-permissions-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-records-permissions-1.0.0a5.tar", last modified: Wed Dec 11 09:52:22 2019, max compression
+gzip compressed data, was "dist/invenio-records-permissions-1.0.0a6.tar", last modified: Wed Dec 18 20:46:55 2019, max compression
```

## Comparing `invenio-records-permissions-1.0.0a5.tar` & `invenio-records-permissions-1.0.0a6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      238 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/changes.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      841 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     7493 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      285 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/api.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/license.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/examplesapp.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      298 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/configuration.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     7023 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)    10297 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3919 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1184 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/examples/app.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      203 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/examples/app-teardown.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      158 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/examples/app-fixtures.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)      173 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/examples/app-setup.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      852 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/.editorconfig
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/INSTALL.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      537 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/babel.ini
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/.tx/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/.tx/config
--rw-rw-r--   0 travis    (2000) travis    (2000)      751 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3163 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/tests/test_generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2499 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/tests/test_permissions_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3279 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/tests/test_permissions_records.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2138 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      963 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/tests/test_invenio_records_permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      963 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3389 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/requirements-devel.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      325 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/CHANGES.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)      499 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/run-tests.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/.dockerignore
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-12-11 09:52:21.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-11 09:52:21.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      851 2019-12-11 09:52:21.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3389 2019-12-11 09:52:21.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-11 09:52:21.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2019-12-11 09:52:21.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1836 2019-12-11 09:52:21.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/policies/
--rw-rw-r--   0 travis    (2000) travis    (2000)      484 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/policies/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1045 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/policies/deposits.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2485 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/policies/records.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3831 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/policies/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1265 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      482 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5505 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      503 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/factories/
--rw-rw-r--   0 travis    (2000) travis    (2000)      508 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/factories/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1131 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/factories/deposits.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1696 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/factories/records.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/translations/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/translations/en/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-11 09:52:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/translations/en/LC_MESSAGES/
--rw-rw-r--   0 travis    (2000) travis    (2000)      474 2019-12-11 09:52:21.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/translations/en/LC_MESSAGES/messages.mo
--rw-rw-r--   0 travis    (2000) travis    (2000)      714 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/translations/en/LC_MESSAGES/messages.po
--rw-rw-r--   0 travis    (2000) travis    (2000)      667 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/translations/messages.pot
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      366 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/invenio_records_permissions/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3613 2019-12-11 09:50:22.000000 invenio-records-permissions-1.0.0a5/CONTRIBUTING.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      238 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/changes.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      841 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7493 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)      285 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/api.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/license.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/authors.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       17 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      335 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/examplesapp.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      298 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/configuration.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      262 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/usage.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7023 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/make.bat
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10297 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3974 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1184 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/examples/app.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      203 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/examples/app-teardown.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      158 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/examples/app-fixtures.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      173 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/examples/app-setup.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      255 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1062 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      852 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/.editorconfig
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/INSTALL.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      537 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/babel.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/.tx/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/.tx/config
+-rw-rw-r--   0 travis    (2000) travis    (2000)      751 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4673 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/tests/test_factories_records.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4689 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/tests/test_generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2499 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/tests/test_permissions_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3029 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      963 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/tests/test_invenio_records_permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      963 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3389 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/requirements-devel.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/pytest.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)      325 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/CHANGES.rst
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      499 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/run-tests.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      124 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/.dockerignore
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1133 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3389 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1834 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/policies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      484 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/policies/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      886 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/policies/deposits.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3017 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/policies/records.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3971 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/policies/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1317 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1343 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      482 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7458 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      503 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/factories/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      547 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/factories/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1131 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/factories/deposits.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2968 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/factories/records.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/translations/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/translations/en/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/translations/en/LC_MESSAGES/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      474 2019-12-18 20:46:55.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/translations/en/LC_MESSAGES/messages.mo
+-rw-rw-r--   0 travis    (2000) travis    (2000)      714 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/translations/en/LC_MESSAGES/messages.po
+-rw-rw-r--   0 travis    (2000) travis    (2000)      667 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/translations/messages.pot
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      366 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/invenio_records_permissions/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3613 2019-12-18 20:45:14.000000 invenio-records-permissions-1.0.0a6/CONTRIBUTING.rst
```

### Comparing `invenio-records-permissions-1.0.0a5/docs/index.rst` & `invenio-records-permissions-1.0.0a6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/docs/Makefile` & `invenio-records-permissions-1.0.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/docs/make.bat` & `invenio-records-permissions-1.0.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/docs/conf.py` & `invenio-records-permissions-1.0.0a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/README.rst` & `invenio-records-permissions-1.0.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/setup.py` & `invenio-records-permissions-1.0.0a6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     'isort>=4.3.3',
     'pydocstyle>=2.0.0',
     'pytest-cov>=2.5.1',
     'pytest-mock>=1.6.0',
     'pytest-pep8>=1.0.6',
     'pytest-invenio>=1.0.5',
     'invenio-accounts>=1.1.1,<1.2.0',
+    'invenio_app>=1.2.3,<1.3.0',
     sphinx_require,
 ]
 
 # Should follow inveniosoftware/invenio versions
 invenio_db_version = '>=1.0.4,<1.1.0'
 invenio_search_version = '>=1.2.0,<1.3.0'
 
@@ -73,15 +74,16 @@
 install_requires = [
     'Flask-BabelEx>=0.9.3',
     'Flask-Principal>=0.4.0,<0.5.0',
     # Because of versioning policy that may admit minor incompatible (!)
     # backward change we also place an upper limit
     # https://invenio.readthedocs.io/en/latest/releases/maintenance-policy.html
     'invenio-access>=1.3.0,<1.4.0',
-    'invenio-records-files>=1.2.0,<1.3.0'
+    'invenio-records-files>=1.2.0,<1.3.0',
+    'bidict>=0.18.3'
 ]
 
 packages = find_packages()
 
 
 # Get the version string. Cannot be done with import!
 g = {}
```

### Comparing `invenio-records-permissions-1.0.0a5/examples/app.py` & `invenio-records-permissions-1.0.0a6/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/LICENSE` & `invenio-records-permissions-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/.editorconfig` & `invenio-records-permissions-1.0.0a6/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/babel.ini` & `invenio-records-permissions-1.0.0a6/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/.tx/config` & `invenio-records-permissions-1.0.0a6/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/setup.cfg` & `invenio-records-permissions-1.0.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/tests/test_permissions_base.py` & `invenio-records-permissions-1.0.0a6/tests/test_permissions_base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/tests/test_invenio_records_permissions.py` & `invenio-records-permissions-1.0.0a6/tests/test_invenio_records_permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/MANIFEST.in` & `invenio-records-permissions-1.0.0a6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/PKG-INFO` & `invenio-records-permissions-1.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-permissions
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Permission policies for Invenio records.
 Home-page: https://github.com/inveniosoftware/invenio-records-permissions
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019 CERN.
@@ -75,15 +75,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Development Status :: 3 - Alpha
-Provides-Extra: elasticsearch6
-Provides-Extra: postgresql
 Provides-Extra: docs
-Provides-Extra: sqlite
-Provides-Extra: all
 Provides-Extra: elasticsearch7
-Provides-Extra: mysql
 Provides-Extra: tests
+Provides-Extra: mysql
+Provides-Extra: sqlite
+Provides-Extra: elasticsearch6
+Provides-Extra: postgresql
+Provides-Extra: all
```

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/requires.txt` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 Flask-BabelEx>=0.9.3
 Flask-Principal<0.5.0,>=0.4.0
 invenio-access<1.4.0,>=1.3.0
 invenio-records-files<1.3.0,>=1.2.0
+bidict>=0.18.3
 
 [all]
 Sphinx>=1.5.1
+check-manifest>=0.25
+coverage>=4.0
+isort>=4.3.3
+pydocstyle>=2.0.0
+pytest-cov>=2.5.1
+pytest-mock>=1.6.0
+pytest-pep8>=1.0.6
+pytest-invenio>=1.0.5
+invenio-accounts<1.2.0,>=1.1.1
+invenio_app<1.3.0,>=1.2.3
+Sphinx>=1.5.1
 Sphinx>=1.5.1
 check-manifest>=0.25
 coverage>=4.0
 isort>=4.3.3
 pydocstyle>=2.0.0
 pytest-cov>=2.5.1
 pytest-mock>=1.6.0
 pytest-pep8>=1.0.6
 pytest-invenio>=1.0.5
 invenio-accounts<1.2.0,>=1.1.1
+invenio_app<1.3.0,>=1.2.3
 Sphinx>=1.5.1
 
 [docs]
 Sphinx>=1.5.1
 
 [elasticsearch6]
 invenio-search[elasticsearch6]<1.3.0,>=>=1.2.0
@@ -41,8 +54,9 @@
 isort>=4.3.3
 pydocstyle>=2.0.0
 pytest-cov>=2.5.1
 pytest-mock>=1.6.0
 pytest-pep8>=1.0.6
 pytest-invenio>=1.0.5
 invenio-accounts<1.2.0,>=1.1.1
+invenio_app<1.3.0,>=1.2.3
 Sphinx>=1.5.1
```

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/PKG-INFO` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-permissions
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Permission policies for Invenio records.
 Home-page: https://github.com/inveniosoftware/invenio-records-permissions
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019 CERN.
@@ -75,15 +75,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Development Status :: 3 - Alpha
-Provides-Extra: elasticsearch6
-Provides-Extra: postgresql
 Provides-Extra: docs
-Provides-Extra: sqlite
-Provides-Extra: all
 Provides-Extra: elasticsearch7
-Provides-Extra: mysql
 Provides-Extra: tests
+Provides-Extra: mysql
+Provides-Extra: sqlite
+Provides-Extra: elasticsearch6
+Provides-Extra: postgresql
+Provides-Extra: all
```

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions.egg-info/SOURCES.txt` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,11 +53,11 @@
 invenio_records_permissions/policies/base.py
 invenio_records_permissions/policies/deposits.py
 invenio_records_permissions/policies/records.py
 invenio_records_permissions/translations/messages.pot
 invenio_records_permissions/translations/en/LC_MESSAGES/messages.mo
 invenio_records_permissions/translations/en/LC_MESSAGES/messages.po
 tests/conftest.py
+tests/test_factories_records.py
 tests/test_generators.py
 tests/test_invenio_records_permissions.py
-tests/test_permissions_base.py
-tests/test_permissions_records.py
+tests/test_permissions_base.py
```

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/policies/deposits.py` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/policies/deposits.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 - Create action given to any authenticated user.
 - Read access given to deposit owners.
 - Update access given to deposit owners.
 - Delete access given to admins only.
 - Use same "get_permission_policy" pattern as records.py
 """
 
-from ..generators import AnyUser, GlobalCurators, LocalCurators, RecordOwners
+from ..generators import AnyUser, RecordOwners
 from .base import BasePermissionPolicy
 
 
 class DepositPermissionPolicy(BasePermissionPolicy):
     """Access control configuration for deposits."""
 
-    can_list = [RecordOwners(), LocalCurators()]
-    # FIXME: What is the purpose of Action('deposit-create')?
+    can_list = [RecordOwners()]
     can_create = [AnyUser()]
     can_read = [RecordOwners()]
-    can_update = [GlobalCurators(), LocalCurators()]
-    can_delete = [GlobalCurators()]
+    can_update = []
+    can_delete = []
```

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/policies/records.py` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/policies/records.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Invenio-Records-Permissions is free software; you can redistribute it
 # and/or modify it under the terms of the MIT License; see LICENSE file for
 # more details.
 
 """Access controls for records."""
 
 import six
+from bidict import bidict
 from flask import current_app
 from werkzeug.utils import import_string
 
 from ..errors import UnknownGeneratorError
 from ..generators import Admin, AnyUser, AnyUserIfPublic, Disable, RecordOwners
 from .base import BasePermissionPolicy
 
@@ -44,26 +45,41 @@
 class RecordPermissionPolicy(BasePermissionPolicy):
     """Access control configuration for records.
 
     Note that even if the array is empty, the invenio_access Permission class
     always adds the ``superuser-access``, so admins will always be allowed.
     """
 
+    NEED_LABEL_TO_ACTION = bidict({
+        'bucket-update': 'update_files',
+        'object-read': 'read_files',
+    })
+
     # Read access given to everyone.
     can_list = [AnyUser()]
     # Create action given to no one (Not even superusers) bc Deposits should
     # be used.
     can_create = [Disable()]
     # Read access given to everyone if public record/files and owners always.
     can_read = [AnyUserIfPublic(), RecordOwners()]
-    # can_read_files = [AnyUserIfPublicFiles(), RecordOwners()]
     # Update access given to record owners.
     can_update = [RecordOwners()]
     # Delete access given to admins only.
     can_delete = [Admin()]
+    # Associated files permissions (which are really bucket permissions)
+    can_read_files = [AnyUserIfPublic(), RecordOwners()]
+    can_update_files = [RecordOwners()]
+
+    def __init__(self, action, **over):
+        """Constructor."""
+        self.original_action = action
+        action = RecordPermissionPolicy.NEED_LABEL_TO_ACTION.get(
+            action, action
+        )
+        super(RecordPermissionPolicy, self).__init__(action, **over)
 
 
 def get_record_permission_policy():
     """Return RecordPermissionPolicy.
 
     Relies on ``RECORDS_PERMISSIONS_RECORD_POLICY`` to
     automatically configure functionality. This way the hoster doesn't need to
```

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/policies/base.py` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/policies/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,13 +104,17 @@
         ]
         self.explicit_excludes |= set(chain.from_iterable(excludes))
         self._load_permissions()  # self.explicit_excludes is used here
         return self._permissions.excludes
 
     @property
     def query_filters(self):
-        """List of ElasticSearch query filters."""
+        """List of ElasticSearch query filters.
+
+        These filters consist of additive queries mapping to what the current
+        user should be able to retrieve via search.
+        """
         filters = [
             generator.query_filter(**self.over)
             for generator in self.generators
         ]
         return [f for f in filters if f]
```

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/api.py` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/__init__.py` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 """Permission policies for Invenio records."""
 
 from __future__ import absolute_import, print_function
 
 from .ext import InvenioRecordsPermissions
 from .factories import record_create_permission_factory, \
-    record_delete_permission_factory, record_list_permission_factory, \
-    record_read_permission_factory, record_update_permission_factory
+    record_delete_permission_factory, record_files_permission_factory, \
+    record_list_permission_factory, record_read_permission_factory, \
+    record_update_permission_factory
 from .policies import BasePermissionPolicy, DepositPermissionPolicy, \
     RecordPermissionPolicy
 from .version import __version__
 
 __all__ = (
     '__version__',
     'BasePermissionPolicy',
@@ -26,11 +27,12 @@
     'InvenioRecordsPermissions',
     'RecordPermissionPolicy',
     # TODO: Hide behind invenio_records_permissions.factories
     # if isort PR is merged:
     # https://github.com/inveniosoftware/cookiecutter-invenio-module/pull/129
     'record_create_permission_factory',
     'record_delete_permission_factory',
+    'record_files_permission_factory',
     'record_list_permission_factory',
     'record_read_permission_factory',
     'record_update_permission_factory',
 )
```

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/factories/deposits.py` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/factories/deposits.py`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/translations/en/LC_MESSAGES/messages.po` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/translations/messages.pot` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/invenio_records_permissions/ext.py` & `invenio-records-permissions-1.0.0a6/invenio_records_permissions/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-records-permissions-1.0.0a5/CONTRIBUTING.rst` & `invenio-records-permissions-1.0.0a6/CONTRIBUTING.rst`

 * *Files identical despite different names*

