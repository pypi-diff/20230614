# Comparing `tmp/invenio-oauthclient-2.3.0.tar.gz` & `tmp/invenio-oauthclient-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-oauthclient-2.3.0.tar", last modified: Mon Mar 13 15:26:25 2023, max compression
+gzip compressed data, was "dist/invenio-oauthclient-3.0.0.tar", last modified: Wed Jun 14 16:15:06 2023, max compression
```

## Comparing `invenio-oauthclient-2.3.0.tar` & `invenio-oauthclient-3.0.0.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10206 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      594 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/examplesapp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7007 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (122)      169 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/app-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)       85 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/app-teardown.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/github_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/github_app_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/globus_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/globus_app_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/orcid_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/examples/orcid_app_rest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      848 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/_compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py
--rw-r--r--   0 runner    (1001) docker     (122)    12222 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17979 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/cern.py
--rw-r--r--   0 runner    (1001) docker     (122)    15246 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/cern_openid.py
--rw-r--r--   0 runner    (1001) docker     (122)    11557 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/github.py
--rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/globus.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/
--rw-r--r--   0 runner    (1001) docker     (122)     3919 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3570 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)    10486 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/openaire_aai.py
--rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/orcid.py
--rw-r--r--   0 runner    (1001) docker     (122)     4210 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     7465 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7777 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8780 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6403 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     9562 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/postmessage.html
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/rejected.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/rejected.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      987 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     3312 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)    11257 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/views/
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8519 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/views/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/invenio_oauthclient/views/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      939 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      346 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/run-i18n-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1303 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    17883 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-13 15:26:25.000000 invenio-oauthclient-2.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/data/cern_openid_response_content.json
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/data/keycloak_realm_info.json
--rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/data/keycloak_token_response.json
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/data/keycloak_userinfo_response.json
--rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/data/oauth_response_content.json
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/data/orcid_bio.json
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4177 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_base_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_contrib_cern_openid.py
--rw-r--r--   0 runner    (1001) docker     (122)    11031 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_contrib_cern_openid_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)    13036 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_contrib_github.py
--rw-r--r--   0 runner    (1001) docker     (122)    14224 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_contrib_github_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)    10374 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_contrib_globus.py
--rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_contrib_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (122)     9540 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_contrib_orcid.py
--rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_contrib_orcid_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_examples_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_handlers_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4803 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_handlers_ui.py
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    10261 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    17496 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    15887 2023-03-13 15:26:21.000000 invenio-oauthclient-2.3.0/tests/test_views_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7612 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10206 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      594 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/examplesapp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7007 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)     4306 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      169 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/app-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)       85 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/app-teardown.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/github_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/github_app_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/globus_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4123 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/globus_app_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/orcid_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/examples/orcid_app_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      848 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2870 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12518 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17979 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/cern.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15246 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/cern_openid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11557 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11134 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/globus.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/
+-rw-r--r--   0 runner    (1001) docker     (122)     3919 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3570 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10486 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/openaire_aai.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10133 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4502 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3104 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7962 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10212 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8780 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6403 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9562 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7862 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/postmessage.html
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/rejected.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/rejected.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      987 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2843 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2621 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2168 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     4724 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     2622 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3312 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)    11257 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8519 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/views/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/invenio_oauthclient/views/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7612 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      939 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-14 16:15:05.000000 invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      346 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1303 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3138 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    17922 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 16:15:06.000000 invenio-oauthclient-3.0.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/data/cern_openid_response_content.json
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/data/keycloak_realm_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/data/keycloak_token_response.json
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/data/keycloak_userinfo_response.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2753 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/data/oauth_response_content.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/data/orcid_bio.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_base_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6890 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_contrib_cern_openid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11031 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_contrib_cern_openid_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13036 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_contrib_github.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14224 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_contrib_github_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10374 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_contrib_globus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14371 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_contrib_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9540 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_contrib_orcid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9849 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_contrib_orcid_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_examples_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9560 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_handlers_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5072 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_handlers_ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10261 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17496 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15887 2023-06-14 16:14:54.000000 invenio-oauthclient-3.0.0/tests/test_views_rest.py
```

### Comparing `invenio-oauthclient-2.3.0/.editorconfig` & `invenio-oauthclient-3.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/.tx/config` & `invenio-oauthclient-3.0.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/AUTHORS.rst` & `invenio-oauthclient-3.0.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/CHANGES.rst` & `invenio-oauthclient-3.0.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 3.0.0 (released 2023-06-14)
+
+- base client: add group handler
+
 Version 2.3.0 (released 2023-03-13)
 
 - OpenAIRE AAI sandbox remote moved to Keycloak.
 - Keycloak settings helper accept configurable scopes for token request.
 
 Version 2.2.0 (released 2023-03-02)
```

### Comparing `invenio-oauthclient-2.3.0/CONTRIBUTING.rst` & `invenio-oauthclient-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/LICENSE` & `invenio-oauthclient-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/MANIFEST.in` & `invenio-oauthclient-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/PKG-INFO` & `invenio-oauthclient-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauthclient
-Version: 2.3.0
+Version: 3.0.0
 Summary: "Invenio module that provides OAuth web authorization support."
 Home-page: https://github.com/inveniosoftware/invenio-oauthclient
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -56,14 +56,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.0.0 (released 2023-06-14)
+        
+        - base client: add group handler
+        
         Version 2.3.0 (released 2023-03-13)
         
         - OpenAIRE AAI sandbox remote moved to Keycloak.
         - Keycloak settings helper accept configurable scopes for token request.
         
         Version 2.2.0 (released 2023-03-02)
```

### Comparing `invenio-oauthclient-2.3.0/README.rst` & `invenio-oauthclient-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/docs/Makefile` & `invenio-oauthclient-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/docs/api.rst` & `invenio-oauthclient-3.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/docs/conf.py` & `invenio-oauthclient-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/docs/examplesapp.rst` & `invenio-oauthclient-3.0.0/docs/examplesapp.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/docs/index.rst` & `invenio-oauthclient-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/docs/make.bat` & `invenio-oauthclient-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/docs/overview.rst` & `invenio-oauthclient-3.0.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/docs/usage.rst` & `invenio-oauthclient-3.0.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/examples/app.py` & `invenio-oauthclient-3.0.0/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/examples/github_app.py` & `invenio-oauthclient-3.0.0/examples/github_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/examples/github_app_rest.py` & `invenio-oauthclient-3.0.0/examples/github_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/examples/globus_app.py` & `invenio-oauthclient-3.0.0/examples/globus_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/examples/globus_app_rest.py` & `invenio-oauthclient-3.0.0/examples/globus_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/examples/orcid_app.py` & `invenio-oauthclient-3.0.0/examples/orcid_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/examples/orcid_app_rest.py` & `invenio-oauthclient-3.0.0/examples/orcid_app_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/_compat.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/_compat.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/admin.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/44ab9963e8cf_create_oauthclient_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/97bbc733896c_create_oauthclient_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/aaa265b0afa6_move_useridentity_to_acconuts.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/alembic/bff1f190b9bd_add_timestamp_oauthclient.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/config.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,16 @@
             icon='...',
             authorized_handler="...",
             disconnect_handler="...",
             signup_handler=dict(
                 info="...",
                 setup="...",
                 view="...",
+                groups="...",
+                groups_serializer="...",
             ),
             precedence_mask=dict(
                 email=True
             ),
             signup_options=dict(
                 auto_confirm=True,
                 send_register_msg=False,
@@ -174,14 +176,16 @@
             authorized_handler="...",
             disconnect_handler="...",
             signup_handler=dict(
                 info="...",
                 info_serializer="...",
                 setup="...",
                 view="...",
+                groups="...",
+                groups_serializer="...",
             ),
             response_handler=("..."),
             authorized_redirect_url="...",
             disconnect_redirect_url="...",
             signup_redirect_url="...",
             error_redirect_url="...",
             precedence_mask=dict(...),
@@ -271,14 +275,16 @@
                        ":disconnect_handler",
             )
             signup_handler=dict(
                 info="invenio_oauthclient.contrib.orcid:account_info",
                 info_serializer="invenio_oauthclient.contrib.orcid:account_info_serializer",
                 setup="invenio_oauthclient.contrib.orcid:account_setup",
                 view="invenio_oauthclient.handlers:signup_handler",
+                groups="invenio_oauthclient.handlers:signup_handler",
+                groups_serializer="invenio_oauthclient.handlers:groups_serializer",
             ),
             # ...
         )
     )
 
 Custom remote application
 ^^^^^^^^^^^^^^^^^^^^^^^^^
```

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/cern.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/cern.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/cern_openid.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/cern_openid.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/github.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/github.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/globus.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/globus.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/__init__.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/handlers.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/helpers.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/keycloak/settings.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/keycloak/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/openaire_aai.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/openaire_aai.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/orcid.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/orcid.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/contrib/settings.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/contrib/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -75,14 +75,16 @@
         It should return a dict in this format:
         dict(
             authorized_handler='path_to_method_authorized_signup_handler',
             disconnect_handler='path_to_method_authorized_disconnect_handler',
         signup_handler=dict(
             info='path_to_method_account_info',
             info_serializer='path_to_method_account_info_serializer',
+            groups="path_to_method_account_groups_handler",
+            groups_serializer="path_to_method_account_groups_serializer_handler",
             setup='path_to_method_account_setup',
             view='path_to_method_signup_form_handler',
         )
         """
         raise NotImplementedError
 
     @cached_property
@@ -100,14 +102,16 @@
             authorized_handler='path_to_method_authorized_signup_handler',
             disconnect_handler='path_to_method_disconnect_rest_handler',
             signup_handler=dict(
                 info='path_to_method_account_info',
                 info_serializer='path_to_method_account_info_serializer',
                 setup='path_to_method_account_setup',
                 view='path_to_method_signup_form_handler',
+                groups="path_to_method_account_groups_handler",
+                groups_serializer="path_to_method_account_groups_serializer_handler",
             ),
             response_handler=(
                 'path_to_method_response_handler'
             ),
             authorized_redirect_url='/',
             disconnect_redirect_url='/',
             signup_redirect_url='/',
```

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/errors.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/ext.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/ext.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,24 +108,34 @@
                 signup_handler.get("info", dummy_handler), remote, with_response=False
             )
             account_info_serializer_handler = handlers.make_handler(
                 signup_handler.get("info_serializer", dummy_handler),
                 remote,
                 with_response=False,
             )
+            account_groups_handler = handlers.make_handler(
+                signup_handler.get("groups", dummy_handler), remote, with_response=False
+            )
+            account_groups_serializer_handler = handlers.make_handler(
+                signup_handler.get("groups_serializer", dummy_handler),
+                remote,
+                with_response=False,
+            )
             account_setup_handler = handlers.make_handler(
                 signup_handler.get("setup", dummy_handler), remote, with_response=False
             )
             account_view_handler = handlers.make_handler(
                 signup_handler.get("view", dummy_handler), remote, with_response=False
             )
 
             self.signup_handlers[remote_app] = dict(
                 info=account_info_handler,
                 info_serializer=account_info_serializer_handler,
+                groups=account_groups_handler,
+                groups_serializer=account_groups_serializer_handler,
                 setup=account_setup_handler,
                 view=account_view_handler,
             )
 
         if "cern" in self.oauth.remote_apps:
             warnings.warn(
                 "CERN Remote app is deprecated, use CERN OpenID instead.",
```

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/__init__.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/rest.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/ui.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/ui.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/handlers/utils.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/models.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/signals.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/_macros.html` & `invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/login_user.html` & `invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html` & `invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/templates/invenio_oauthclient/signup.html` & `invenio-oauthclient-3.0.0/invenio_oauthclient/templates/invenio_oauthclient/signup.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html` & `invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html` & `invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html` & `invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/settings/index.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html` & `invenio-oauthclient-3.0.0/invenio_oauthclient/templates/semantic-ui/invenio_oauthclient/signup.html`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/translations/messages.pot` & `invenio-oauthclient-3.0.0/invenio_oauthclient/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/utils.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/views/client.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/views/client.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient/views/settings.py` & `invenio-oauthclient-3.0.0/invenio_oauthclient/views/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/PKG-INFO` & `invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-oauthclient
-Version: 2.3.0
+Version: 3.0.0
 Summary: "Invenio module that provides OAuth web authorization support."
 Home-page: https://github.com/inveniosoftware/invenio-oauthclient
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -56,14 +56,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.0.0 (released 2023-06-14)
+        
+        - base client: add group handler
+        
         Version 2.3.0 (released 2023-03-13)
         
         - OpenAIRE AAI sandbox remote moved to Keycloak.
         - Keycloak settings helper accept configurable scopes for token request.
         
         Version 2.2.0 (released 2023-03-02)
```

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/SOURCES.txt` & `invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/entry_points.txt` & `invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/invenio_oauthclient.egg-info/requires.txt` & `invenio-oauthclient-3.0.0/invenio_oauthclient.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 blinker>=1.4
 Flask-OAuthlib>=0.9.6
-invenio-accounts>=2.0.2
+invenio-accounts>=3.0.0
 invenio-base>=1.2.11
 invenio-i18n>=2.0.0
 invenio-mail>=1.0.2
 invenio-theme>=1.3.12
 oauthlib<3.0.0,>=1.1.2
 requests-oauthlib<1.2.0,>=0.6.2
 uritools>=1.0.1
```

### Comparing `invenio-oauthclient-2.3.0/requirements-devel.txt` & `invenio-oauthclient-3.0.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/run-tests.sh` & `invenio-oauthclient-3.0.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/setup.cfg` & `invenio-oauthclient-3.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 include_package_data = True
 packages = find:
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	blinker>=1.4
 	Flask-OAuthlib>=0.9.6
-	invenio-accounts>=2.0.2
+	invenio-accounts>=3.0.0
 	invenio-base>=1.2.11
 	invenio-i18n>=2.0.0
 	invenio-mail>=1.0.2
 	invenio-theme>=1.3.12
 	oauthlib>=1.1.2,<3.0.0
 	requests-oauthlib>=0.6.2,<1.2.0
 	uritools>=1.0.1
```

### Comparing `invenio-oauthclient-2.3.0/tests/conftest.py` & `invenio-oauthclient-3.0.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import pytest
 from flask import Flask
 from flask_mail import Mail
 from flask_menu import Menu as FlaskMenu
 from invenio_accounts import InvenioAccounts
 from invenio_db import InvenioDB, db
-from invenio_i18n import Babel
+from invenio_i18n import Babel, InvenioI18N
 from invenio_userprofiles import InvenioUserProfiles
 from invenio_userprofiles.views import blueprint_ui_init
 from sqlalchemy_utils.functions import create_database, database_exists, drop_database
 
 from invenio_oauthclient import InvenioOAuthClient, InvenioOAuthClientREST
 from invenio_oauthclient.contrib.cern_openid import REMOTE_APP as CERN_OPENID_REMOTE_APP
 from invenio_oauthclient.contrib.cern_openid import (
@@ -140,14 +140,15 @@
         THEME_ICONS={"semantic-ui": dict(link="linkify icon")},
     )
     FlaskMenu(base_app)
     Babel(base_app)
     Mail(base_app)
     InvenioDB(base_app)
     InvenioAccounts(base_app)
+    InvenioI18N(base_app)
 
     with base_app.app_context():
         if str(db.engine.url) != "sqlite://" and not database_exists(
             str(db.engine.url)
         ):
             create_database(str(db.engine.url))
         db.create_all()
```

### Comparing `invenio-oauthclient-2.3.0/tests/data/keycloak_realm_info.json` & `invenio-oauthclient-3.0.0/tests/data/keycloak_realm_info.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/data/keycloak_token_response.json` & `invenio-oauthclient-3.0.0/tests/data/keycloak_token_response.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/data/oauth_response_content.json` & `invenio-oauthclient-3.0.0/tests/data/oauth_response_content.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/data/orcid_bio.json` & `invenio-oauthclient-3.0.0/tests/data/orcid_bio.json`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/helpers.py` & `invenio-oauthclient-3.0.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_admin.py` & `invenio-oauthclient-3.0.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_app.py` & `invenio-oauthclient-3.0.0/tests/test_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,17 @@
             filter(
                 lambda table: table.startswith("oauthclient"), db.metadata.tables.keys()
             )
         )
         assert len(tables) == 2
 
 
+@pytest.mark.skip(
+    reason="Incorrect execution order of recipes from invenio-access and invenio-accounts."
+)  # TODO fix this at a later date
 def test_alembic(app):
     """Test alembic recipes."""
     ext = app.extensions["invenio-db"]
 
     with app.app_context():
         if db.engine.name == "sqlite":
             raise pytest.skip("Upgrades are not supported on SQLite.")
```

### Comparing `invenio-oauthclient-2.3.0/tests/test_base_handlers.py` & `invenio-oauthclient-3.0.0/tests/test_base_handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_contrib_cern_openid.py` & `invenio-oauthclient-3.0.0/tests/test_contrib_cern_openid.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_contrib_cern_openid_rest.py` & `invenio-oauthclient-3.0.0/tests/test_contrib_cern_openid_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_contrib_github.py` & `invenio-oauthclient-3.0.0/tests/test_contrib_github.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_contrib_github_rest.py` & `invenio-oauthclient-3.0.0/tests/test_contrib_github_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_contrib_globus.py` & `invenio-oauthclient-3.0.0/tests/test_contrib_globus.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_contrib_keycloak.py` & `invenio-oauthclient-3.0.0/tests/test_contrib_keycloak.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_contrib_orcid.py` & `invenio-oauthclient-3.0.0/tests/test_contrib_orcid.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_contrib_orcid_rest.py` & `invenio-oauthclient-3.0.0/tests/test_contrib_orcid_rest.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_examples_app.py` & `invenio-oauthclient-3.0.0/tests/test_examples_app.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_handlers_rest.py` & `invenio-oauthclient-3.0.0/tests/test_handlers_rest.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pytest
 from flask import session, url_for
 from flask_login import current_user
 from flask_oauthlib.client import OAuth as FlaskOAuth
 from flask_security import login_user, logout_user
 from flask_security.confirmable import _security
 from helpers import check_response_redirect_url_args
+from invenio_accounts.models import Role
 from werkzeug.routing import BuildError
 
 from invenio_oauthclient import InvenioOAuthClientREST, current_oauthclient
 from invenio_oauthclient.errors import AlreadyLinkedError
 from invenio_oauthclient.handlers import token_session_key, token_setter
 from invenio_oauthclient.handlers.rest import (
     authorized_signup_handler,
@@ -68,27 +69,70 @@
         "next_url": next_url,
     }
     resp = authorized_signup_handler(example_response, remote)
     check_response_redirect_url_args(resp, expected_url_args)
 
 
 @pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
+def test_group_handler(remote, app_rest, models_fixture):
+    """Test group handler."""
+    datastore = app_rest.extensions["invenio-accounts"].datastore
+    existing_email = "existing@inveniosoftware.org"
+    user = datastore.find_user(email=existing_email)
+    example_group = [
+        {
+            "id": "rdm-developers",
+            "name": "rdm-developers",
+            "description": "People contributing to RDM.",
+        }
+    ]
+
+    example_response = {"access_token": "test_access_token"}
+    example_account_info = {
+        "user": {
+            "email": existing_email,
+        },
+        "external_id": "1234",
+        "external_method": "test_method",
+    }
+
+    # Mock remote app's handler
+    current_oauthclient.signup_handlers[remote.name] = {
+        "info": lambda resp: example_account_info,
+        "groups": lambda resp: example_group,
+    }
+
+    _security.confirmable = True
+    _security.login_without_confirmation = False
+    user.confirmed_at = None
+
+    authorized_signup_handler(example_response, remote)
+
+    # Assert that the group handler works correctly
+    roles = Role.query.all()
+    assert 1 == len(roles)
+    assert roles[0].id == example_group[0]["id"]
+    assert roles[0].name == example_group[0]["name"]
+    assert roles[0].description == example_group[0]["description"]
+
+
+@pytest.mark.parametrize("remote", REMOTE_APPS, indirect=["remote"])
 def test_unauthorized_signup(remote, app_rest, models_fixture):
     """Test unauthorized redirect on signup callback handler."""
     datastore = app_rest.extensions["invenio-accounts"].datastore
     existing_email = "existing@inveniosoftware.org"
     user = datastore.find_user(email=existing_email)
 
     example_response = {"access_token": "test_access_token"}
     example_account_info = {
         "user": {
             "email": existing_email,
-            "external_id": "1234",
-            "external_method": "test_method",
-        }
+        },
+        "external_id": "1234",
+        "external_method": "test_method",
     }
 
     # Mock remote app's handler
     current_oauthclient.signup_handlers[remote.name] = {
         "info": lambda resp: example_account_info,
     }
```

### Comparing `invenio-oauthclient-2.3.0/tests/test_handlers_ui.py` & `invenio-oauthclient-3.0.0/tests/test_handlers_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,20 +33,29 @@
 from invenio_oauthclient.views.settings import blueprint as blueprint_settings
 
 
 def test_authorized_signup_handler(remote, app, models_fixture):
     """Test authorized signup handler."""
     datastore = app.extensions["invenio-accounts"].datastore
     user = datastore.find_user(email="existing@inveniosoftware.org")
+    existing_email = "existing@inveniosoftware.org"
 
     example_response = {"access_token": "test_access_token"}
+    example_account_info = {
+        "user": {
+            "email": existing_email,
+        },
+        "external_id": "1234",
+        "external_method": "test_method",
+    }
 
     # Mock remote app's handler
     current_oauthclient.signup_handlers[remote.name] = {
-        "setup": lambda token, resp: None
+        "setup": lambda token, resp: None,
+        "info": lambda resp: example_account_info,
     }
 
     # Authenticate user
     oauth_authenticate("dev", user)
 
     # Mock next url
     next_url = "/test/redirect"
@@ -63,31 +72,30 @@
     existing_email = "existing@inveniosoftware.org"
     user = datastore.find_user(email=existing_email)
 
     example_response = {"access_token": "test_access_token"}
     example_account_info = {
         "user": {
             "email": existing_email,
-            "external_id": "1234",
-            "external_method": "test_method",
-        }
+        },
+        "external_id": "1234",
+        "external_method": "test_method",
     }
 
     # Mock remote app's handler
     current_oauthclient.signup_handlers[remote.name] = {
         "info": lambda resp: example_account_info,
     }
 
     _security.confirmable = True
     _security.login_without_confirmation = False
     user.confirmed_at = None
     app.config["OAUTHCLIENT_REMOTE_APPS"][remote.name] = {}
-
     resp = authorized_signup_handler(example_response, remote)
-    check_redirect_location(resp, lambda x: x.startswith("/login/"))
+    check_redirect_location(resp, lambda x: x.startswith("/login"))
 
 
 def test_signup_handler(remote, app, models_fixture):
     """Test signup handler."""
     datastore = app.extensions["invenio-accounts"].datastore
     existing_email = "existing@inveniosoftware.org"
     user = datastore.find_user(email=existing_email)
```

### Comparing `invenio-oauthclient-2.3.0/tests/test_models.py` & `invenio-oauthclient-3.0.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_utils.py` & `invenio-oauthclient-3.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_views.py` & `invenio-oauthclient-3.0.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `invenio-oauthclient-2.3.0/tests/test_views_rest.py` & `invenio-oauthclient-3.0.0/tests/test_views_rest.py`

 * *Files identical despite different names*

