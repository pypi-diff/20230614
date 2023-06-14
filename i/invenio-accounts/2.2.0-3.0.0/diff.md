# Comparing `tmp/invenio-accounts-2.2.0.tar.gz` & `tmp/invenio-accounts-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-accounts-2.2.0.tar", last modified: Tue Apr 25 08:12:03 2023, max compression
+gzip compressed data, was "dist/invenio-accounts-3.0.0.tar", last modified: Wed Jun 14 08:02:36 2023, max compression
```

## Comparing `invenio-accounts-2.2.0.tar` & `invenio-accounts-3.0.0.tar`

### file list

```diff
@@ -1,273 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5645 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9984 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)    55769 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/admin.png
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10254 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7001 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7385 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3842 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/alembic/999dcbd19ace_users_versioning.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py
--rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/context_processors/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/context_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/context_processors/jwt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/datastore.py
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11798 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/hash.py
--rw-r--r--   0 runner    (1001) docker     (122)    13665 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/profiles/
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/profiles/dicts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/profiles/schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/sessions.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/change_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/jwt.html
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1818 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/send_login.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/settings/security.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/templates/security/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/templates/security/email/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/security/email/change_notice_rest.html
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/security/email/change_notice_rest.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/jwt.html
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_login.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html
--rw-r--r--   0 runner    (1001) docker     (122)     4809 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9446 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11937 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10653 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10896 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      936 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9800 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11345 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11153 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11067 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11017 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9461 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10991 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9445 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11093 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10687 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9628 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9761 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9606 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      673 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9653 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9861 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9448 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10747 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10951 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11117 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9668 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10604 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9605 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     7420 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts/views/
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19229 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/views/rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/views/security.py
--rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/invenio_accounts/views/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9984 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8132 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/invenio_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-25 08:12:02.000000 invenio-accounts-2.2.0/invenio_accounts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      851 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     8833 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 08:12:03.000000 invenio-accounts-2.2.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/e2e/e2e_basic_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5430 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     3471 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (122)     7021 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_invenio_accounts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4766 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    11240 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_template_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_token_duration.py
--rw-r--r--   0 runner    (1001) docker     (122)     6706 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3239 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_validated_dicts.py
--rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    18215 2023-04-25 08:11:55.000000 invenio-accounts-2.2.0/tests/test_views_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5805 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10192 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    55769 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/admin.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10254 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7001 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7385 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3842 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/999dcbd19ace_users_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4525 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/context_processors/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/context_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/context_processors/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11798 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13859 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/profiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/profiles/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/profiles/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/jwt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1818 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/send_login.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/settings/security.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/templates/security/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/templates/security/email/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/security/email/change_notice_rest.html
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/security/email/change_notice_rest.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/jwt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_login.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4809 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9446 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11937 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10653 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10896 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9800 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11345 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11153 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11067 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11017 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9461 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10991 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9445 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11093 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10687 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9628 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9761 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9606 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9653 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9861 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9448 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10747 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10951 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11117 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9668 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10604 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9605 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7420 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts/views/
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19229 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/views/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/views/security.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/invenio_accounts/views/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10192 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/invenio_accounts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1546 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8833 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:02:36.000000 invenio-accounts-3.0.0/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/e2e/e2e_basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5430 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_invenio_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4766 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11240 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_template_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_token_duration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6706 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3239 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_validated_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18215 2023-06-14 08:02:27.000000 invenio-accounts-3.0.0/tests/test_views_rest.py
```

### Comparing `invenio-accounts-2.2.0/.editorconfig` & `invenio-accounts-3.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/.github/workflows/i18n-pull.yml` & `invenio-accounts-3.0.0/.github/workflows/i18n-pull.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/.github/workflows/i18n-push.yml` & `invenio-accounts-3.0.0/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/.github/workflows/pypi-publish.yml` & `invenio-accounts-3.0.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/.github/workflows/tests.yml` & `invenio-accounts-3.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/.tx/config` & `invenio-accounts-3.0.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/AUTHORS.rst` & `invenio-accounts-3.0.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/CHANGES.rst` & `invenio-accounts-3.0.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 3.0.0 (released 2023-06-14)
+
+- models: add managed field to groups
+- models: alter primary key type of group (id)
+- cli: pass id on create role action
+
 Version 2.2.0 (released 2023-04-25)
 
 - models: add support for locale in user preferences
 
 Version 2.1.0 (released 2023-03-01)
 
 - global: replace deprecated babelex imports
```

### Comparing `invenio-accounts-2.2.0/CONTRIBUTING.rst` & `invenio-accounts-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/LICENSE` & `invenio-accounts-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/MANIFEST.in` & `invenio-accounts-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/PKG-INFO` & `invenio-accounts-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-accounts
-Version: 2.2.0
+Version: 3.0.0
 Summary: Invenio user management and authentication.
 Home-page: https://github.com/inveniosoftware/invenio-accounts
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -62,14 +62,20 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.0.0 (released 2023-06-14)
+        
+        - models: add managed field to groups
+        - models: alter primary key type of group (id)
+        - cli: pass id on create role action
+        
         Version 2.2.0 (released 2023-04-25)
         
         - models: add support for locale in user preferences
         
         Version 2.1.0 (released 2023-03-01)
         
         - global: replace deprecated babelex imports
```

### Comparing `invenio-accounts-2.2.0/README.rst` & `invenio-accounts-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/docs/Makefile` & `invenio-accounts-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/docs/admin.png` & `invenio-accounts-3.0.0/docs/admin.png`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/docs/api.rst` & `invenio-accounts-3.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/docs/conf.py` & `invenio-accounts-3.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/docs/configuration.rst` & `invenio-accounts-3.0.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/docs/index.rst` & `invenio-accounts-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/docs/make.bat` & `invenio-accounts-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/__init__.py` & `invenio-accounts-3.0.0/invenio_accounts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     from werkzeug import security
 
     security.safe_str_cmp = hmac.compare_digest
 
 from .ext import InvenioAccounts, InvenioAccountsREST, InvenioAccountsUI
 from .proxies import current_accounts
 
-__version__ = "2.2.0"
+__version__ = "3.0.0"
 
 __all__ = (
     "__version__",
     "current_accounts",
     "InvenioAccounts",
     "InvenioAccountsUI",
     "InvenioAccountsREST",
```

### Comparing `invenio-accounts-2.2.0/invenio_accounts/admin.py` & `invenio-accounts-3.0.0/invenio_accounts/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py` & `invenio-accounts-3.0.0/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py` & `invenio-accounts-3.0.0/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py` & `invenio-accounts-3.0.0/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/alembic/999dcbd19ace_users_versioning.py` & `invenio-accounts-3.0.0/invenio_accounts/alembic/999dcbd19ace_users_versioning.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py` & `invenio-accounts-3.0.0/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py` & `invenio-accounts-3.0.0/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py` & `invenio-accounts-3.0.0/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/cli.py` & `invenio-accounts-3.0.0/invenio_accounts/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2015-2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Command Line Interface for accounts."""
 
+import json
 from datetime import datetime
 from functools import wraps
 
 import click
 from flask import current_app
 from flask.cli import with_appcontext
 from flask_security.forms import ConfirmRegisterForm
@@ -44,27 +45,30 @@
 
 
 @users.command("create")
 @click.argument("email")
 @click.password_option()
 @click.option("-a", "--active", default=False, is_flag=True)
 @click.option("-c", "--confirm", default=False, is_flag=True)
+@click.option("-p", "--profile")
 @with_appcontext
 @commit
-def users_create(email, password, active, confirm):
+def users_create(email, password, active, confirm, profile):
     """Create a user."""
     kwargs = dict(email=email, password=password, active="y" if active else "")
 
     form = ConfirmRegisterForm(MultiDict(kwargs), meta={"csrf": False})
 
     if form.validate():
         kwargs["password"] = hash_password(kwargs["password"])
         kwargs["active"] = active
         if confirm:
             kwargs["confirmed_at"] = datetime.utcnow()
+        if profile:
+            kwargs["user_profile"] = json.loads(profile)
         _datastore.create_user(**kwargs)
         click.secho("User created successfully.", fg="green")
         kwargs["password"] = "****"
         click.echo(kwargs)
     else:
         raise click.UsageError("Error creating user. %s" % form.errors)
 
@@ -72,15 +76,15 @@
 @roles.command("create")
 @click.argument("name")
 @click.option("-d", "--description", default=None)
 @with_appcontext
 @commit
 def roles_create(**kwargs):
     """Create a role."""
-    _datastore.create_role(**kwargs)
+    _datastore.create_role(id=kwargs["name"], **kwargs)
     click.secho('Role "%(name)s" created successfully.' % kwargs, fg="green")
 
 
 @roles.command("add")
 @click.argument("user")
 @click.argument("role")
 @with_appcontext
```

### Comparing `invenio-accounts-2.2.0/invenio_accounts/config.py` & `invenio-accounts-3.0.0/invenio_accounts/config.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/context_processors/jwt.py` & `invenio-accounts-3.0.0/invenio_accounts/context_processors/jwt.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/datastore.py` & `invenio-accounts-3.0.0/invenio_accounts/datastore.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2022 CERN.
+# Copyright (C) 2015-2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Session-aware datastore."""
 
 from flask_security import SQLAlchemyUserDatastore
 
+from .models import Role
 from .proxies import current_db_change_history
 from .sessions import delete_user_sessions
 from .signals import datastore_post_commit, datastore_pre_commit
 
 
 class SessionAwareSQLAlchemyUserDatastore(SQLAlchemyUserDatastore):
     """Datastore which deletes active session when a user is deactivated."""
@@ -30,14 +31,31 @@
         return res
 
     def commit(self):
         """Commit a user to its session."""
         datastore_pre_commit.send(session=self.db.session)
         super().commit()
         datastore_post_commit.send(session=self.db.session)
+        current_db_change_history.clear_dirty_sets(self.db.session)
 
     def mark_changed(self, sid, uid=None, rid=None):
         """Save a user to the changed history."""
         if uid:
-            current_db_change_history.updated_users[sid].append(uid)
+            current_db_change_history.add_updated_user(sid, uid)
         elif rid:
-            current_db_change_history.updated_roles[sid].append(uid)
+            current_db_change_history.add_updated_role(sid, rid)
+
+    def update_role(self, role):
+        """Updates roles."""
+        role = self.db.session.merge(role)
+        self.mark_changed(id(self.db.session), rid=role.id)
+        return role
+
+    def create_role(self, **kwargs):
+        """Creates and returns a new role from the given parameters."""
+        role = super().create_role(**kwargs)
+        self.mark_changed(id(self.db.session), rid=role.id)
+        return role
+
+    def find_role_by_id(self, role_id):
+        """Fetches roles searching by id."""
+        return self.role_model.query.filter_by(id=role_id).one_or_none()
```

### Comparing `invenio-accounts-2.2.0/invenio_accounts/errors.py` & `invenio-accounts-3.0.0/invenio_accounts/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/ext.py` & `invenio-accounts-3.0.0/invenio_accounts/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/forms.py` & `invenio-accounts-3.0.0/invenio_accounts/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/hash.py` & `invenio-accounts-3.0.0/invenio_accounts/hash.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/models.py` & `invenio-accounts-3.0.0/invenio_accounts/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2022 CERN.
+# Copyright (C) 2015-2023 CERN.
 # Copyright (C) 2022 KTH Royal Institute of Technology
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Database models for accounts."""
 
+import uuid
 from datetime import datetime
 
 from flask import current_app, session
 from flask_babel import refresh
 from flask_security import RoleMixin, UserMixin
 from invenio_db import db
 from sqlalchemy.dialects import postgresql
@@ -48,34 +49,37 @@
     db.Column(
         "user_id",
         db.Integer(),
         db.ForeignKey("accounts_user.id", name="fk_accounts_userrole_user_id"),
     ),
     db.Column(
         "role_id",
-        db.Integer(),
+        db.String(80),
         db.ForeignKey("accounts_role.id", name="fk_accounts_userrole_role_id"),
     ),
 )
 """Relationship between users and roles."""
 
 
 class Role(db.Model, Timestamp, RoleMixin):
     """Role data model."""
 
     __tablename__ = "accounts_role"
 
-    id = db.Column(db.Integer(), primary_key=True)
+    id = db.Column(db.String(80), primary_key=True, default=str(uuid.uuid4()))
 
     name = db.Column(db.String(80), unique=True)
     """Role name."""
 
     description = db.Column(db.String(255))
     """Role description."""
 
+    is_managed = db.Column(db.Boolean(), default=True, nullable=False)
+    """True when the role is managed by Invenio, and not externally provided."""
+
     # Enables SQLAlchemy version counter
     version_id = db.Column(db.Integer, nullable=False)
     """Used by SQLAlchemy for optimistic concurrency control."""
 
     __mapper_args__ = {"version_id_col": version_id}
 
     def __str__(self):
```

### Comparing `invenio-accounts-2.2.0/invenio_accounts/profiles/__init__.py` & `invenio-accounts-3.0.0/invenio_accounts/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/profiles/dicts.py` & `invenio-accounts-3.0.0/invenio_accounts/profiles/dicts.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/profiles/schemas.py` & `invenio-accounts-3.0.0/invenio_accounts/profiles/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/proxies.py` & `invenio-accounts-3.0.0/invenio_accounts/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/sessions.py` & `invenio-accounts-3.0.0/invenio_accounts/sessions.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/signals.py` & `invenio-accounts-3.0.0/invenio_accounts/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/tasks.py` & `invenio-accounts-3.0.0/invenio_accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/_macros.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/change_password.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/change_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/forgot_password.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/forgot_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/login_user.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/register_user.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/reset_password.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/reset_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/send_confirmation.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/send_confirmation.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/invenio_accounts/settings/security.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/invenio_accounts/settings/security.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html` & `invenio-accounts-3.0.0/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/testutils.py` & `invenio-accounts-3.0.0/invenio_accounts/testutils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/af/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/af/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/da/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/da/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/de/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/de/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/el/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/el/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/es/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/es/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/et/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/et/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/it/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/it/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/messages.pot` & `invenio-accounts-3.0.0/invenio_accounts/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/no/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/no/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.0/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/utils.py` & `invenio-accounts-3.0.0/invenio_accounts/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/views/__init__.py` & `invenio-accounts-3.0.0/invenio_accounts/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/views/rest.py` & `invenio-accounts-3.0.0/invenio_accounts/views/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/views/security.py` & `invenio-accounts-3.0.0/invenio_accounts/views/security.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts/views/settings.py` & `invenio-accounts-3.0.0/invenio_accounts/views/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/invenio_accounts.egg-info/PKG-INFO` & `invenio-accounts-3.0.0/invenio_accounts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-accounts
-Version: 2.2.0
+Version: 3.0.0
 Summary: Invenio user management and authentication.
 Home-page: https://github.com/inveniosoftware/invenio-accounts
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -62,14 +62,20 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.0.0 (released 2023-06-14)
+        
+        - models: add managed field to groups
+        - models: alter primary key type of group (id)
+        - cli: pass id on create role action
+        
         Version 2.2.0 (released 2023-04-25)
         
         - models: add support for locale in user preferences
         
         Version 2.1.0 (released 2023-03-01)
         
         - global: replace deprecated babelex imports
```

### Comparing `invenio-accounts-2.2.0/invenio_accounts.egg-info/SOURCES.txt` & `invenio-accounts-3.0.0/invenio_accounts.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py
 invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py
 invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py
 invenio_accounts/alembic/999dcbd19ace_users_versioning.py
 invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py
 invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py
 invenio_accounts/alembic/eb9743315a9d_add_userprofile.py
+invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py
 invenio_accounts/context_processors/__init__.py
 invenio_accounts/context_processors/jwt.py
 invenio_accounts/profiles/__init__.py
 invenio_accounts/profiles/dicts.py
 invenio_accounts/profiles/schemas.py
 invenio_accounts/templates/invenio_accounts/_macros.html
 invenio_accounts/templates/invenio_accounts/base.html
```

### Comparing `invenio-accounts-2.2.0/invenio_accounts.egg-info/entry_points.txt` & `invenio-accounts-3.0.0/invenio_accounts.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/requirements-devel.txt` & `invenio-accounts-3.0.0/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/setup.cfg` & `invenio-accounts-3.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 	invenio-db[mysql]>=1.0.14
 sqlite = 
 	invenio-db>=1.0.14
 tests = 
 	mock>=1.3.0
 	invenio-app>=1.3.3
 	pytest-black>=0.3.0
-	pytest-invenio>=1.4.6
+	pytest-invenio>=2.1.4
 	sphinx>=4.2.0,<5
 
 [options.entry_points]
 flask.commands = 
 	roles = invenio_accounts.cli:roles
 	users = invenio_accounts.cli:users
 invenio_admin.views =
```

### Comparing `invenio-accounts-2.2.0/tests/conftest.py` & `invenio-accounts-3.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/e2e/conftest.py` & `invenio-accounts-3.0.0/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/e2e/e2e_basic_test.py` & `invenio-accounts-3.0.0/tests/e2e/e2e_basic_test.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_admin.py` & `invenio-accounts-3.0.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_cli.py` & `invenio-accounts-3.0.0/tests/test_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,14 +27,53 @@
     result = runner.invoke(users_create, input="1234\n1234\n")
     assert result.exit_code != 0
 
     # Create user with invalid email
     result = runner.invoke(users_create, ["not-an-email", "--password", "123456"])
     assert result.exit_code == 2
 
+    # Create user with profile
+    result = runner.invoke(
+        users_create,
+        [
+            "--password",
+            "AValidPassword66!",
+            "--profile",
+            '{"full_name" : "Test User"}',
+            "test1@example.com",
+        ],
+    )
+    assert result.exit_code == 0
+
+    # Create user with profile that is not valid JSON
+    result = runner.invoke(
+        users_create,
+        [
+            "--password",
+            "AValidPassword66!",
+            "--profile",
+            "<json>profile</json>",
+            "test2@example.com",
+        ],
+    )
+    assert result.exit_code != 0
+
+    # Create user with JSON profile that will not validate
+    result = runner.invoke(
+        users_create,
+        [
+            "--password",
+            "AValidPassword66!",
+            "--profile",
+            '{"full_name" : "test_user", "extra_data" : "not_allowed"}',
+            "test3@example.com",
+        ],
+    )
+    assert result.exit_code != 0
+
     # Create user
     result = runner.invoke(
         users_create, ["info@inveniosoftware.org", "--password", "123456"]
     )
     assert result.exit_code == 0
```

### Comparing `invenio-accounts-2.2.0/tests/test_forms.py` & `invenio-accounts-3.0.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_hash.py` & `invenio-accounts-3.0.0/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_invenio_accounts.py` & `invenio-accounts-3.0.0/tests/test_invenio_accounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2015-2018 CERN.
+# Copyright (C) 2015-2023 CERN.
 # Copyright (C) 2021      TU Wien.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Module tests."""
 
@@ -110,56 +110,73 @@
     assert not ext.alembic.compare_metadata()
 
 
 def test_datastore_usercreate(app):
     """Test create user."""
     ds = app.extensions["invenio-accounts"].datastore
 
-    with app.app_context():
-        u1 = ds.create_user(
-            email="info@inveniosoftware.org", password="1234", active=True
-        )
-        ds.commit()
-        u2 = ds.find_user(email="info@inveniosoftware.org")
-        assert u1 == u2
-        assert 1 == User.query.filter_by(email="info@inveniosoftware.org").count()
+    u1 = ds.create_user(email="info@inveniosoftware.org", password="1234", active=True)
+    ds.commit()
+    u2 = ds.find_user(email="info@inveniosoftware.org")
+    assert u1 == u2
+    assert 1 == User.query.filter_by(email="info@inveniosoftware.org").count()
 
 
 def test_datastore_rolecreate(app):
-    """Test create user."""
+    """Test create role."""
     ds = app.extensions["invenio-accounts"].datastore
 
-    with app.app_context():
-        r1 = ds.create_role(name="superuser", description="1234")
-        ds.commit()
-        r2 = ds.find_role("superuser")
-        assert r1 == r2
-        assert 1 == Role.query.filter_by(name="superuser").count()
+    r1 = ds.create_role(name="superuser", description="1234")
+    ds.commit()
+    r2 = ds.find_role("superuser")
+    assert r1 == r2
+    assert 1 == Role.query.filter_by(name="superuser").count()
+
+
+def test_datastore_update_role(app):
+    """Test update role."""
+    ds = app.extensions["invenio-accounts"].datastore
+
+    r1 = ds.create_role(id="1", name="superuser", description="1234")
+    ds.commit()
+    r2 = ds.find_role("superuser")
+    assert r1 == r2
+    assert 1 == Role.query.filter_by(name="superuser").count()
+    assert r2.is_managed is True
+
+    r1 = ds.update_role(
+        Role(
+            id="1", name="megauser", description="updated description", is_managed=False
+        )
+    )
+    ds.commit()
+    r2 = ds.find_role("megauser")
+    assert r1 == r2
+    assert r2.description == "updated description"
+    assert r2.is_managed is False
+    assert 1 == Role.query.filter_by(name="megauser").count()
+    assert 0 == Role.query.filter_by(name="superuser").count()
 
 
 def test_datastore_assignrole(app):
     """Create and assign user to role."""
     ds = app.extensions["invenio-accounts"].datastore
 
-    with app.app_context():
-        u = ds.create_user(
-            email="info@inveniosoftware.org", password="1234", active=True
-        )
-        r = ds.create_role(name="superuser", description="1234")
-        ds.add_role_to_user(u, r)
-        ds.commit()
-        u = ds.get_user("info@inveniosoftware.org")
-        assert len(u.roles) == 1
-        assert u.roles[0].name == "superuser"
+    u = ds.create_user(email="info@inveniosoftware.org", password="1234", active=True)
+    r = ds.create_role(name="superuser", description="1234")
+    ds.add_role_to_user(u, r)
+    ds.commit()
+    u = ds.get_user("info@inveniosoftware.org")
+    assert len(u.roles) == 1
+    assert u.roles[0].name == "superuser"
 
 
 def test_view(app):
     """Test view."""
-    with app.app_context():
-        login_url = url_for_security("login")
+    login_url = url_for_security("login")
 
     with app.test_client() as client:
         res = client.get(login_url)
         assert res.status_code == 200
 
 
 def test_configuration(base_app):
@@ -204,20 +221,19 @@
     assert isinstance(app_with_redis_url.kvsession_store, kvsession_store_class)
 
 
 def test_headers_info(app, users):
     """Test if session and user id is set response header."""
     u = users[0]
     url = url_for_security("change_password")
-    with app.app_context():
-        with app.test_client() as client:
-            response = client.get(url)
-            # Not logged in, so only session id available
-            assert not testutils.client_authenticated(client)
-            assert "X-Session-ID" in response.headers
-            assert "X-User-ID" not in response.headers
-            # Login
-            testutils.login_user_via_session(client, email=u["email"])
-            response = client.get(url)
-            cookie = requests.utils.dict_from_cookiejar(client.cookie_jar)
-            assert response.headers["X-Session-ID"] == cookie["session"].split(".")[0]
-            assert int(response.headers["X-User-ID"]) == u["id"]
+    with app.test_client() as client:
+        response = client.get(url)
+        # Not logged in, so only session id available
+        assert not testutils.client_authenticated(client)
+        assert "X-Session-ID" in response.headers
+        assert "X-User-ID" not in response.headers
+        # Login
+        testutils.login_user_via_session(client, email=u["email"])
+        response = client.get(url)
+        cookie = requests.utils.dict_from_cookiejar(client.cookie_jar)
+        assert response.headers["X-Session-ID"] == cookie["session"].split(".")[0]
+        assert int(response.headers["X-User-ID"]) == u["id"]
```

### Comparing `invenio-accounts-2.2.0/tests/test_models.py` & `invenio-accounts-3.0.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_schemas.py` & `invenio-accounts-3.0.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_sessions.py` & `invenio-accounts-3.0.0/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_tasks.py` & `invenio-accounts-3.0.0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_template_context_processors.py` & `invenio-accounts-3.0.0/tests/test_template_context_processors.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_token_duration.py` & `invenio-accounts-3.0.0/tests/test_token_duration.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_utils.py` & `invenio-accounts-3.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_validated_dicts.py` & `invenio-accounts-3.0.0/tests/test_validated_dicts.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_views.py` & `invenio-accounts-3.0.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-2.2.0/tests/test_views_rest.py` & `invenio-accounts-3.0.0/tests/test_views_rest.py`

 * *Files identical despite different names*

