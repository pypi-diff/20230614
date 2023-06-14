# Comparing `tmp/invenio-accounts-3.0.1.tar.gz` & `tmp/invenio-accounts-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-accounts-3.0.1.tar", last modified: Wed Jun 14 08:38:41 2023, max compression
+gzip compressed data, was "dist/invenio-accounts-3.0.2.tar", last modified: Wed Jun 14 14:56:16 2023, max compression
```

## Comparing `invenio-accounts-3.0.1.tar` & `invenio-accounts-3.0.2.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10293 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)    55769 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/admin.png
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10254 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7001 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7385 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3842 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/999dcbd19ace_users_versioning.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py
--rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4525 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/context_processors/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/context_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/context_processors/jwt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/datastore.py
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    11798 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/hash.py
--rw-r--r--   0 runner    (1001) docker     (122)    13859 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/profiles/
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/profiles/dicts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/profiles/schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/sessions.py
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/change_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/jwt.html
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1818 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/send_login.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/settings/security.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/templates/security/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/templates/security/email/
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/security/email/change_notice_rest.html
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/security/email/change_notice_rest.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/base_cover.html
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/jwt.html
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/send_login.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html
--rw-r--r--   0 runner    (1001) docker     (122)     4809 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9446 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11937 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10653 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10896 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9800 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11345 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11153 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11067 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11017 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9461 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      718 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10991 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9445 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11093 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10687 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9628 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9761 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9606 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9653 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9861 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9448 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10747 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10951 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    11117 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9668 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10604 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     9605 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     7420 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts/views/
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19229 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/views/rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/views/security.py
--rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/invenio_accounts/views/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/invenio_accounts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10293 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-14 08:38:40.000000 invenio-accounts-3.0.1/invenio_accounts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)     1546 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     8833 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 08:38:41.000000 invenio-accounts-3.0.1/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/e2e/e2e_basic_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5430 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_invenio_accounts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4766 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    11240 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_template_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_token_duration.py
--rw-r--r--   0 runner    (1001) docker     (122)     6706 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3239 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_validated_dicts.py
--rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    18215 2023-06-14 08:38:29.000000 invenio-accounts-3.0.1/tests/test_views_rest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2006 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2522 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5945 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      878 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10396 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7449 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    55769 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/admin.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10254 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7001 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7385 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3842 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2247 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/999dcbd19ace_users_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2293 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4525 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/context_processors/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/context_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/context_processors/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11798 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4071 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13859 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/profiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3359 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/profiles/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/profiles/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/jwt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1818 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1260 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/send_login.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/settings/security.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/templates/security/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/templates/security/email/
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/security/email/change_notice_rest.html
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/security/email/change_notice_rest.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/base_cover.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1726 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/jwt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/send_login.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4809 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9446 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11937 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10653 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3467 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10896 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9800 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4106 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11345 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11153 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11067 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3995 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11017 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9461 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      718 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9631 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10991 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9445 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11093 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3076 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10687 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      715 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9628 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9761 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9606 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9653 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9641 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9861 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9448 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10747 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10951 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    11117 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9668 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10604 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     9605 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7420 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts/views/
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19229 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/views/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/views/security.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/invenio_accounts/views/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10396 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/invenio_accounts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1546 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8833 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-14 14:56:16.000000 invenio-accounts-3.0.2/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3709 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/e2e/e2e_basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5430 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_invenio_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4766 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11240 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_template_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_token_duration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6706 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3239 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_validated_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6325 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18215 2023-06-14 14:56:07.000000 invenio-accounts-3.0.2/tests/test_views_rest.py
```

### Comparing `invenio-accounts-3.0.1/.editorconfig` & `invenio-accounts-3.0.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/.github/workflows/i18n-pull.yml` & `invenio-accounts-3.0.2/.github/workflows/i18n-pull.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/.github/workflows/i18n-push.yml` & `invenio-accounts-3.0.2/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/.github/workflows/pypi-publish.yml` & `invenio-accounts-3.0.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/.github/workflows/tests.yml` & `invenio-accounts-3.0.2/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   Tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
           python-version: [3.7, 3.8, 3.9]
           requirements-level: [min, pypi]
           cache-service: [redis]
-          db-service: [postgresql10, postgresql13]
+          db-service: [postgresql10, postgresql13, mysql8]
           exclude:
           - python-version: 3.7
             requirements-level: pypi
 
           - python-version: 3.8
             requirements-level: min
 
@@ -40,14 +40,17 @@
           include:
           - db-service: postgresql10
             DB_EXTRAS: "postgresql"
 
           - db-service: postgresql13
             DB_EXTRAS: "postgresql"
 
+          - db-service: mysql8
+            DB_EXTRAS: "mysql"
+
     env:
       CACHE: ${{ matrix.cache-service }}
       DB: ${{ matrix.db-service }}
       EXTRAS: tests,admin,${{ matrix.DB_EXTRAS }}
     steps:
       - name: Checkout
         uses: actions/checkout@v2
```

### Comparing `invenio-accounts-3.0.1/.tx/config` & `invenio-accounts-3.0.2/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/AUTHORS.rst` & `invenio-accounts-3.0.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/CHANGES.rst` & `invenio-accounts-3.0.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 3.0.2 (released 2023-06-14)
+
+- alembic: adapt recipe to mysql
+
 Version 3.0.1 (released 2023-06-14)
 
 - alembic: fix upgrade recipes
 
 Version 3.0.0 (released 2023-06-14)
 
 - models: add managed field to groups
```

### Comparing `invenio-accounts-3.0.1/CONTRIBUTING.rst` & `invenio-accounts-3.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/LICENSE` & `invenio-accounts-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/MANIFEST.in` & `invenio-accounts-3.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/PKG-INFO` & `invenio-accounts-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-accounts
-Version: 3.0.1
+Version: 3.0.2
 Summary: Invenio user management and authentication.
 Home-page: https://github.com/inveniosoftware/invenio-accounts
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -62,14 +62,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.0.2 (released 2023-06-14)
+        
+        - alembic: adapt recipe to mysql
+        
         Version 3.0.1 (released 2023-06-14)
         
         - alembic: fix upgrade recipes
         
         Version 3.0.0 (released 2023-06-14)
         
         - models: add managed field to groups
```

### Comparing `invenio-accounts-3.0.1/README.rst` & `invenio-accounts-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/docs/Makefile` & `invenio-accounts-3.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/docs/admin.png` & `invenio-accounts-3.0.2/docs/admin.png`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/docs/api.rst` & `invenio-accounts-3.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/docs/conf.py` & `invenio-accounts-3.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/docs/configuration.rst` & `invenio-accounts-3.0.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/docs/index.rst` & `invenio-accounts-3.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/docs/make.bat` & `invenio-accounts-3.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/__init__.py` & `invenio-accounts-3.0.2/invenio_accounts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     from werkzeug import security
 
     security.safe_str_cmp = hmac.compare_digest
 
 from .ext import InvenioAccounts, InvenioAccountsREST, InvenioAccountsUI
 from .proxies import current_accounts
 
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 
 __all__ = (
     "__version__",
     "current_accounts",
     "InvenioAccounts",
     "InvenioAccountsUI",
     "InvenioAccountsREST",
```

### Comparing `invenio-accounts-3.0.1/invenio_accounts/admin.py` & `invenio-accounts-3.0.2/invenio_accounts/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py` & `invenio-accounts-3.0.2/invenio_accounts/alembic/62efc52773d4_create_useridentity_table.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py` & `invenio-accounts-3.0.2/invenio_accounts/alembic/843bc79c426f_create_accounts_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py` & `invenio-accounts-3.0.2/invenio_accounts/alembic/9848d0149abd_create_accounts_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/alembic/999dcbd19ace_users_versioning.py` & `invenio-accounts-3.0.2/invenio_accounts/alembic/999dcbd19ace_users_versioning.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py` & `invenio-accounts-3.0.2/invenio_accounts/alembic/dfbdf43a3e96_separate_login_info.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py` & `invenio-accounts-3.0.2/invenio_accounts/alembic/e12419831262_add_new_columns_on_sessionactivity.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py` & `invenio-accounts-3.0.2/invenio_accounts/alembic/eb9743315a9d_add_userprofile.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py` & `invenio-accounts-3.0.2/invenio_accounts/alembic/f2522cdd5fcd_change_accountsrole_primary_key_to_string.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,26 +5,45 @@
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Change AccountsRole primary key to string."""
 
 import sqlalchemy as sa
 from alembic import op
+from sqlalchemy_utils import get_referencing_foreign_keys
+
+from invenio_accounts.models import Role
 
 # revision identifiers, used by Alembic.
 revision = "f2522cdd5fcd"
 down_revision = "eb9743315a9d"
 branch_labels = ()
 depends_on = None
 
 
 def upgrade():
     """Upgrade database."""
     # Drop primary key and all foreign keys
-    op.execute("ALTER TABLE accounts_role DROP CONSTRAINT pk_accounts_role CASCADE;")
+    ctx = op.get_context()
+    if ctx.connection.engine.name == "mysql":
+        # mysql does not support CASCADE on drop constraint command
+        dependent_tables = get_referencing_foreign_keys(Role)
+
+        for fk in dependent_tables:
+            op.drop_constraint(
+                fk.constraint.name, fk.constraint.table.name, type_="foreignkey"
+            )
+
+        op.execute("ALTER TABLE accounts_role MODIFY COLUMN id INT")
+
+        op.drop_constraint("pk_accounts_role", "accounts_role", type_="primary")
+    else:
+        op.execute(
+            "ALTER TABLE accounts_role DROP CONSTRAINT pk_accounts_role CASCADE;"
+        )
 
     op.alter_column(
         "accounts_userrole",
         "role_id",
         existing_type=sa.Integer,
         type_=sa.String(80),
         postgresql_using="role_id::integer",
@@ -43,15 +62,17 @@
     op.add_column(
         "accounts_role",
         sa.Column(
             "is_managed", sa.Boolean(name="is_managed"), default=True, nullable=True
         ),
     )
     op.execute("UPDATE accounts_role SET is_managed = true;")
-    op.alter_column("accounts_role", "is_managed", nullable=False)
+    op.alter_column(
+        "accounts_role", "is_managed", existing_type=sa.Boolean, nullable=False
+    )
 
     # Re-create the foreign key constraint
     op.create_foreign_key(
         "fk_accounts_userrole_role_id",
         "accounts_userrole",
         "accounts_role",
         ["role_id"],
@@ -59,15 +80,29 @@
     )
 
 
 def downgrade():
     """Downgrade database."""
     # Drop new column `is_managed`
     op.drop_column("accounts_role", "is_managed")
-    op.execute("ALTER TABLE accounts_role DROP CONSTRAINT pk_accounts_role CASCADE;")
+    ctx = op.get_context()
+    if ctx.connection.engine.name == "mysql":
+        # mysql does not support CASCADE on drop constraint command
+        dependent_tables = get_referencing_foreign_keys(Role)
+
+        for fk in dependent_tables:
+            op.drop_constraint(
+                fk.constraint.name, fk.constraint.table.name, type_="foreignkey"
+            )
+
+        op.drop_constraint("pk_accounts_role", "accounts_role", type_="primary")
+    else:
+        op.execute(
+            "ALTER TABLE accounts_role DROP CONSTRAINT pk_accounts_role CASCADE;"
+        )
 
     op.alter_column(
         "accounts_userrole",
         "role_id",
         existing_type=sa.String(80),
         type_=sa.Integer,
         postgresql_using="role_id::integer",
```

### Comparing `invenio-accounts-3.0.1/invenio_accounts/api.py` & `invenio-accounts-3.0.2/invenio_accounts/api.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/cli.py` & `invenio-accounts-3.0.2/invenio_accounts/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/config.py` & `invenio-accounts-3.0.2/invenio_accounts/config.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/context_processors/jwt.py` & `invenio-accounts-3.0.2/invenio_accounts/context_processors/jwt.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/datastore.py` & `invenio-accounts-3.0.2/invenio_accounts/datastore.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/errors.py` & `invenio-accounts-3.0.2/invenio_accounts/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/ext.py` & `invenio-accounts-3.0.2/invenio_accounts/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/forms.py` & `invenio-accounts-3.0.2/invenio_accounts/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/hash.py` & `invenio-accounts-3.0.2/invenio_accounts/hash.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/models.py` & `invenio-accounts-3.0.2/invenio_accounts/models.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/profiles/__init__.py` & `invenio-accounts-3.0.2/invenio_accounts/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/profiles/dicts.py` & `invenio-accounts-3.0.2/invenio_accounts/profiles/dicts.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/profiles/schemas.py` & `invenio-accounts-3.0.2/invenio_accounts/profiles/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/proxies.py` & `invenio-accounts-3.0.2/invenio_accounts/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/sessions.py` & `invenio-accounts-3.0.2/invenio_accounts/sessions.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/signals.py` & `invenio-accounts-3.0.2/invenio_accounts/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/tasks.py` & `invenio-accounts-3.0.2/invenio_accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/_macros.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/change_password.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/change_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/forgot_password.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/forgot_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/login_user.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/register_user.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/reset_password.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/reset_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/send_confirmation.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/send_confirmation.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/invenio_accounts/settings/security.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/invenio_accounts/settings/security.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/_macros.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/change_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/forgot_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/reset_password.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/send_confirmation.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html` & `invenio-accounts-3.0.2/invenio_accounts/templates/semantic-ui/invenio_accounts/settings/security.html`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/testutils.py` & `invenio-accounts-3.0.2/invenio_accounts/testutils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/af/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/af/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ar/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/bg/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ca/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/cs/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/da/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/da/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/de/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/de/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/el/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/el/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/es/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/es/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/et/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/et/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/fa/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/fr/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/gl/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/hr/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/hu/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/it/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/it/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ja/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ka/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/lt/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/messages.pot` & `invenio-accounts-3.0.2/invenio_accounts/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/no/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/no/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/pl/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/pt/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ro/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/ru/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/rw/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/sk/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/sv/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/tr/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/uk/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-accounts-3.0.2/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-accounts-3.0.2/invenio_accounts/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/utils.py` & `invenio-accounts-3.0.2/invenio_accounts/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/views/__init__.py` & `invenio-accounts-3.0.2/invenio_accounts/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/views/rest.py` & `invenio-accounts-3.0.2/invenio_accounts/views/rest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/views/security.py` & `invenio-accounts-3.0.2/invenio_accounts/views/security.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts/views/settings.py` & `invenio-accounts-3.0.2/invenio_accounts/views/settings.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts.egg-info/PKG-INFO` & `invenio-accounts-3.0.2/invenio_accounts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-accounts
-Version: 3.0.1
+Version: 3.0.2
 Summary: Invenio user management and authentication.
 Home-page: https://github.com/inveniosoftware/invenio-accounts
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -62,14 +62,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.0.2 (released 2023-06-14)
+        
+        - alembic: adapt recipe to mysql
+        
         Version 3.0.1 (released 2023-06-14)
         
         - alembic: fix upgrade recipes
         
         Version 3.0.0 (released 2023-06-14)
         
         - models: add managed field to groups
```

### Comparing `invenio-accounts-3.0.1/invenio_accounts.egg-info/SOURCES.txt` & `invenio-accounts-3.0.2/invenio_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/invenio_accounts.egg-info/entry_points.txt` & `invenio-accounts-3.0.2/invenio_accounts.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/requirements-devel.txt` & `invenio-accounts-3.0.2/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/run-tests.sh` & `invenio-accounts-3.0.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/setup.cfg` & `invenio-accounts-3.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/conftest.py` & `invenio-accounts-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/e2e/conftest.py` & `invenio-accounts-3.0.2/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/e2e/e2e_basic_test.py` & `invenio-accounts-3.0.2/tests/e2e/e2e_basic_test.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_admin.py` & `invenio-accounts-3.0.2/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_cli.py` & `invenio-accounts-3.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_forms.py` & `invenio-accounts-3.0.2/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_hash.py` & `invenio-accounts-3.0.2/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_invenio_accounts.py` & `invenio-accounts-3.0.2/tests/test_invenio_accounts.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_models.py` & `invenio-accounts-3.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_schemas.py` & `invenio-accounts-3.0.2/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_sessions.py` & `invenio-accounts-3.0.2/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_tasks.py` & `invenio-accounts-3.0.2/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_template_context_processors.py` & `invenio-accounts-3.0.2/tests/test_template_context_processors.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_token_duration.py` & `invenio-accounts-3.0.2/tests/test_token_duration.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_utils.py` & `invenio-accounts-3.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_validated_dicts.py` & `invenio-accounts-3.0.2/tests/test_validated_dicts.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_views.py` & `invenio-accounts-3.0.2/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `invenio-accounts-3.0.1/tests/test_views_rest.py` & `invenio-accounts-3.0.2/tests/test_views_rest.py`

 * *Files identical despite different names*

