# Comparing `tmp/weblate-language-data-2023.4.tar.gz` & `tmp/weblate-language-data-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblate-language-data-2023.4.tar", last modified: Tue Apr 18 16:08:32 2023, max compression
+gzip compressed data, was "weblate-language-data-2023.5.tar", last modified: Wed Jun 14 06:58:23 2023, max compression
```

## Comparing `weblate-language-data-2023.4.tar` & `weblate-language-data-2023.5.tar`

### file list

```diff
@@ -1,368 +1,368 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1377 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/ambiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)   197247 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/check_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/country_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/language_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)   186242 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/ab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/ab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133937 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/afh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/afh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/afh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/ang/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/ang/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ang/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   153837 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/ar_LY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   136111 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/ars/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ars/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/ast/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142847 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/az/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/az/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146730 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/be/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/be/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   153466 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/be_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146896 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ber/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/ber/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   137044 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ber/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   150856 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/bn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148635 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/bn_BD/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148729 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/bo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/bo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   134736 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/bo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/br/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/br/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147038 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/br/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143695 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ce/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/ce/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142553 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ce/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ckb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/ckb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149665 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ckb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/crh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/crh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141181 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/crh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148277 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/cv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/cv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139601 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/cv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/cy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143032 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144470 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   145026 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)   133962 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/dv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/dv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133937 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/dv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   151966 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/en_GB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142398 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/enm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/enm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/enm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146033 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143955 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142980 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147445 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148717 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152964 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fil/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/fil/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142539 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fil/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143416 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/fur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139637 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/fy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147096 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146504 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148312 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147429 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143727 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144519 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146547 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/hy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/ia/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139500 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ia/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142924 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ie/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ie/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   134228 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ie/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/is/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/is/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143494 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143783 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   157789 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/kab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/kab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   145402 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/kab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/kk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/kk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146931 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/km/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/km/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149887 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/kmr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/kmr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   145991 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/kmr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147356 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ksh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ksh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147717 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ksh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ln/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/ln/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139053 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ln/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143582 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141763 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/lzh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/lzh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   135157 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/lzh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/mk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/mk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147661 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/mk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148358 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ml/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/mr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   156534 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/mr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139136 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/my/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/my/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   151792 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/my/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144618 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143628 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   138352 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/oc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/oc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   137315 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/oc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/or/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/or/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149501 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/or/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152996 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pa_PK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   137206 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/peo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/peo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/peo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144637 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/ps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/ps/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141532 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ps/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143333 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143711 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142502 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143845 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/ro_MD/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133948 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   153109 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/sc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143710 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/si/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141848 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149137 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/skr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/skr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144779 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/skr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148262 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146248 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   151618 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144111 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143641 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141993 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/ta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152126 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/te/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144016 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/te/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   155061 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tlh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   134107 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tok/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tok/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133947 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tok/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144919 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139125 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tzm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tzm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   137837 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tzm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/ug/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/ug/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152368 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152543 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/uz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/uz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   136858 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/uz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148715 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/yue_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139328 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/zgh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/zgh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   157283 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/zgh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148360 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147233 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/weblate_language_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/plural_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/plurals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/rtl.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.753284 weblate-language-data-2023.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-14 06:58:23.753284 weblate-language-data-2023.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-14 06:58:23.753284 weblate-language-data-2023.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1377 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.721284 weblate-language-data-2023.5/weblate_language_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/ambiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)   197247 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/check_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/country_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/language_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186516 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.721284 weblate-language-data-2023.5/weblate_language_data/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/ab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.721284 weblate-language-data-2023.5/weblate_language_data/locale/ab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134150 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/afh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/afh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134139 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/afh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/ang/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/ang/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134139 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ang/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   154065 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/ar_LY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/ar_LY/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   136312 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/ars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/ars/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134139 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ars/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/ast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143054 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/az/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/az/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146946 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   153667 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/be_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/be_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147097 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/ber/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/ber/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   137245 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ber/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   151010 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.705284 weblate-language-data-2023.5/weblate_language_data/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148860 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/bn_BD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148930 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/bo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/bo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134937 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/bo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/br/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.725284 weblate-language-data-2023.5/weblate_language_data/locale/br/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147239 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/br/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143844 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/ce/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/ce/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142754 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ce/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/ckb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/ckb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149866 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ckb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/crh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/crh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   141388 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/crh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148501 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/cv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/cv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139802 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/cv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143292 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144685 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   145170 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)   134163 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/dv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/dv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134138 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/dv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152167 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/en_GB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142945 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/enm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/enm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134139 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/enm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146248 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/eo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.729284 weblate-language-data-2023.5/weblate_language_data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144125 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143203 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147646 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148941 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   153179 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/fil/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/fil/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142740 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/fil/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143570 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/fur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/fur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139838 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/fur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/fy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/fy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147297 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/fy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146711 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148475 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147657 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143865 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144734 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.709284 weblate-language-data-2023.5/weblate_language_data/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146748 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/hy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.733284 weblate-language-data-2023.5/weblate_language_data/locale/ia/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139701 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ia/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143096 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ie/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/ie/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134429 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ie/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143701 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143976 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   158001 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142947 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/kab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/kab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   145603 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/kab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147132 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   150088 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/kmr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/kmr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146192 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/kmr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147520 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ksh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/ksh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147918 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ksh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ln/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/ln/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139254 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ln/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143783 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.737285 weblate-language-data-2023.5/weblate_language_data/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   141964 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/lzh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/lzh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   135358 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/lzh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/mk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/mk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147862 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/mk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148559 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ml/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/mr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   156756 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/mr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139352 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/my/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/my/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   151993 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/my/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144836 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143780 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   138358 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/oc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/oc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   137516 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/oc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/or/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/or/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149756 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/or/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/pa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/pa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   153215 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/pa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/pa_PK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/pa_PK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   137407 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/peo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.741284 weblate-language-data-2023.5/weblate_language_data/locale/peo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134139 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/peo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144779 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/ps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/ps/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   141733 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ps/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143482 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143873 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.713284 weblate-language-data-2023.5/weblate_language_data/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142637 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144061 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/ro_MD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/ro_MD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134149 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   153274 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/sc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/sc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143860 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/sc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/si/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142049 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149338 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/skr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/skr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144930 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/skr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148480 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146449 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.745284 weblate-language-data-2023.5/weblate_language_data/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   151838 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144312 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143870 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142194 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152345 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/te/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144217 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/te/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   155262 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134308 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/tok/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/tok/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134148 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/tok/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   145103 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/tt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/tt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139352 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/tt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/tzm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/tzm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   138038 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/tzm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152569 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152691 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/uz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/uz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   137059 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/uz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148940 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/yue_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.749284 weblate-language-data-2023.5/weblate_language_data/locale/yue_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139529 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/zgh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.753284 weblate-language-data-2023.5/weblate_language_data/locale/zgh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   157433 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/zgh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.753284 weblate-language-data-2023.5/weblate_language_data/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148526 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.717284 weblate-language-data-2023.5/weblate_language_data/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.753284 weblate-language-data-2023.5/weblate_language_data/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147387 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.753284 weblate-language-data-2023.5/weblate_language_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/plural_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/plurals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/rtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 06:58:14.000000 weblate-language-data-2023.5/weblate_language_data/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:58:23.721284 weblate-language-data-2023.5/weblate_language_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-14 06:58:23.000000 weblate-language-data-2023.5/weblate_language_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-14 06:58:23.000000 weblate-language-data-2023.5/weblate_language_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:58:23.000000 weblate-language-data-2023.5/weblate_language_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 06:58:23.000000 weblate-language-data-2023.5/weblate_language_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 06:58:23.000000 weblate-language-data-2023.5/weblate_language_data.egg-info/top_level.txt
```

### Comparing `weblate-language-data-2023.4/LICENSE` & `weblate-language-data-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/PKG-INFO` & `weblate-language-data-2023.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weblate-language-data
-Version: 2023.4
+Version: 2023.5
 Summary: Language definitions for Weblate
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/language-data
 Author: Michal Čihař
 Author-email: michal@weblate.org
 License: MIT
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/language-data/issues
```

### Comparing `weblate-language-data-2023.4/README.rst` & `weblate-language-data-2023.5/README.rst`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/pyproject.toml` & `weblate-language-data-2023.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/setup.cfg` & `weblate-language-data-2023.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weblate-language-data
-version = 2023.4
+version = 2023.5
 description = Language definitions for Weblate
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://weblate.org/
 author = Michal Čihař
 author_email = michal@weblate.org
 license = MIT
```

### Comparing `weblate-language-data-2023.4/setup.py` & `weblate-language-data-2023.5/setup.py`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/weblate_language_data/aliases.py` & `weblate-language-data-2023.5/weblate_language_data/aliases.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "serbo_croatian": "sr_Latn",
     "mspanish": "es_MX",
     "norwegian": "nb_NO",
     "xbelorussian": "be",
     "be_rby": "be_Latn",
     "qz_mm": "my@Zawgyi",
     "es_la": "es",
+    "bp": "pt_BR",
     "val_es": "ca@valencia",
     "no_nb": "nb_NO",
     "nb_nb": "nb_NO",
     "no_no": "nb_NO",
     "es_eu": "eu",
     "ru_r": "ru",
     "ru_rr": "ru",
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/check_languages.py` & `weblate-language-data-2023.5/weblate_language_data/check_languages.py`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/weblate_language_data/countries.py` & `weblate-language-data-2023.5/weblate_language_data/countries.py`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/weblate_language_data/country_codes.py` & `weblate-language-data-2023.5/weblate_language_data/country_codes.py`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/weblate_language_data/language_codes.py` & `weblate-language-data-2023.5/weblate_language_data/language_codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     "bn_bd",
     "bn_in",
     "bnt",
     "bo",
     "bo_cn",
     "bod",
     "bos",
+    "bp",
     "bqi",
     "br",
     "bra",
     "braz_por",
     "brb",
     "bre",
     "brx",
@@ -222,14 +223,15 @@
     "deu",
     "deu_de",
     "dgo",
     "dgr",
     "din",
     "div",
     "dk",
+    "dnk",
     "doi",
     "dry",
     "dsb",
     "dua",
     "dum",
     "dut",
     "dutch_be",
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/languages.py` & `weblate-language-data-2023.5/weblate_language_data/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1202,14 +1202,23 @@
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
         _("Dinka"),
         2,
         "n != 1",
     ),
     (
+        "dnk",
+        # Translators: Language name for ISO code "dnk". The parenthesis clarifies
+        # variant of the language. It could contain a region, age (Old, Middle, ...)
+        # or other variant.
+        _("Dengka"),
+        2,
+        "n != 1",
+    ),
+    (
         "doi",
         # Translators: Language name for ISO code "doi". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
         _("Dogri"),
         2,
         "n != 1",
@@ -5612,37 +5621,37 @@
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
         _("Westphalien"),
         2,
         "n != 1",
     ),
     (
-        "wuu_Hans",
-        # Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+        "wo",
+        # Translators: Language name for ISO code "wo". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
-        _("Wu (Simplified)"),
+        _("Wolof"),
         1,
         "0",
     ),
     (
-        "wuu_Hant",
-        # Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+        "wuu_Hans",
+        # Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
-        _("Wu (Traditional)"),
+        _("Wu (Simplified)"),
         1,
         "0",
     ),
     (
-        "wo",
-        # Translators: Language name for ISO code "wo". The parenthesis clarifies
+        "wuu_Hant",
+        # Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
-        _("Wolof"),
+        _("Wu (Traditional)"),
         1,
         "0",
     ),
     (
         "xal",
         # Translators: Language name for ISO code "xal". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ab/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ab/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ab\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -22,15 +22,15 @@
 msgid "Afar"
 msgstr ""
 
 #. Translators: Language name for ISO code "ab". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Abkhazian"
-msgstr ""
+msgstr "Аԥсшәа"
 
 #. Translators: Language name for ISO code "ace". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Acehnese"
 msgstr ""
 
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/afh/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/afh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: afh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ang/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ang/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ang\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ar/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ar/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # tamer dab <dabsantamer@yahoo.com>, 2020.
 # Hakim Oubouali <hakim.oubouali.skr@gmail.com>, 2020.
 # thami simo <simo.azad@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: thami simo <simo.azad@gmail.com>\n"
 "Language-Team: Arabic <https://hosted.weblate.org/projects/weblate/languages/"
 "ar/>\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -830,14 +830,21 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "المندنكوية"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "الزونخاية"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "الدوجرية"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3972,14 +3979,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "الوُلوفية"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "الصينية (المبسطة)"
@@ -3988,20 +4001,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "الصينية (التقليدية)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "الوُلوفية"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "الوالون"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 # Ayoub Rejal <ayoubrejal@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2020-06-19 09:20+0000\n"
 "Last-Translator: Ayoub Rejal <ayoubrejal@gmail.com>\n"
 "Language-Team: Arabic (Libya) <https://hosted.weblate.org/projects/weblate/"
 "languages/ar_LY/>\n"
 "Language: ar_LY\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -819,14 +819,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3777,30 +3783,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ars/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ars/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ars\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ast/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ast/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Asturian <https://hosted.weblate.org/projects/weblate/"
 "languages/ast/>\n"
 "Language: ast\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -850,14 +850,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3958,14 +3964,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "chinu simplificáu"
@@ -3974,20 +3986,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "chinu tradicional"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/az/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/az/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Meki <mekismith77@gmail.com>, 2020.
 # Nizami <nizamismidov4@gmail.com>, 2022.
 # Ariz Mirzəzadə <by.ariz@bk.ru>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-11-07 18:05+0000\n"
 "Last-Translator: Ariz Mirzəzadə <by.ariz@bk.ru>\n"
 "Language-Team: Azerbaijani <https://hosted.weblate.org/projects/weblate/"
 "languages/az/>\n"
 "Language: az\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -831,14 +831,21 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Baltik"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "doqri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3977,14 +3984,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Çincə (Sadələşdirilmiş)"
@@ -3993,20 +4006,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Çin (Ənənəvi)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Balsa"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/be/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/be/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Zmicer Turok <zmicerturok@gmail.com>, 2019.
 # Zmicer Turok <nashtlumach@gmail.com>, 2019, 2020, 2021.
 # Alex Ky <esthomolupus@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Belarusian <https://hosted.weblate.org/projects/weblate/"
 "languages/be/>\n"
 "Language: be\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -832,14 +832,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Мандынка"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Догры"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3936,14 +3942,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Валоф"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Кітайская (спрошчаная)"
@@ -3952,20 +3964,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Кітайская (традыцыйная)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Валоф"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "калмыцкая"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 # Viktar Vauchkevich <victorenator@gmail.com>, 2018, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Belarusian (latin) <https://hosted.weblate.org/projects/"
 "weblate/languages/be_Latn/>\n"
 "Language: be@latin\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -864,14 +864,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "mandynka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dohry"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -4000,14 +4006,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "valof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "kitajskaja (sproščanaja)"
@@ -4016,20 +4028,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "kitajskaja (tradycyjnaja)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "valof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ber/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ber/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Hakim Oubouali <hakim.oubouali.skr@gmail.com>, 2020.
 # ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ زهير أمازيغ <zouhirdehbi56@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2023-01-22 20:54+0000\n"
 "Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ زهير أمازيغ <zouhirdehbi56@gmail.com>\n"
 "Language-Team: Berber <https://hosted.weblate.org/projects/weblate/languages/"
 "ber/>\n"
 "Language: ber\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -809,14 +809,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3755,34 +3761,34 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr ""
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "ⵜⵛⵉⵏⵡⵉⵜ (ⵜⴰⴼⵔⴰⵔⵜ)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr ""
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/bg/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/bg/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 # Georgi Georgiev <g.georgiev.shumen@gmail.com>, 2021.
 # 109247019824 <stoyan@gmx.com>, 2022.
 # Ясен Арсов <jarsov@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-01-31 01:49+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-02 09:32+0000\n"
 "Last-Translator: Любомир Василев <lyubomirv@gmx.com>\n"
 "Language-Team: Bulgarian <https://hosted.weblate.org/projects/weblate/"
 "languages/bg/>\n"
 "Language: bg\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Афарски"
 
@@ -812,14 +812,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Динка"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Догри"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2435,26 +2441,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Науатъл"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Китайски (традиционен)"
+msgstr "Китайски (мин нан, традиционен)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Китайски (Мин Нан)"
+msgstr "Китайски (мин нан, латиница)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Неаполитански"
 
@@ -3756,32 +3758,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Вестфалски"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Волоф"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "У (опростен)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "У (традиционен)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Волоф"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Калмикски"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/bn/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/bn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 # Oymate <dhruboadittya96@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-06-14 05:12+0000\n"
 "Last-Translator: Oymate <dhruboadittya96@gmail.com>\n"
 "Language-Team: Bengali <https://hosted.weblate.org/projects/weblate/"
 "languages/bn/>\n"
 "Language: bn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -832,14 +832,21 @@
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Dinka"
 msgstr "মানডিংগো"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "ডিংকা"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ডোগরি"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3906,14 +3913,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "উওলোফ"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "চীনা (সরলীকৃত)"
@@ -3922,20 +3935,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "চীনা (ঐতিহ্যবাহী)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "উওলোফ"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "কুমইয়িক"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Atikur Rahman <arahman.dcc2@gmail.com>, 2019.
 # Anonymous <noreply@weblate.org>, 2020.
 # Oymate <dhruboadittya96@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Bengali (Bangladesh) <https://hosted.weblate.org/projects/"
 "weblate/languages/bn_BD/>\n"
 "Language: bn_BD\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -849,14 +849,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "মান্ডিঙ্কা"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ডোগ্রি"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3947,30 +3953,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/bo/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/bo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-12-01 18:52+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Tibetan <https://hosted.weblate.org/projects/weblate/"
 "languages/bo/>\n"
 "Language: bo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -807,14 +807,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3753,14 +3759,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr ""
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "རྒྱ་སྐད་ (རྒྱ་ཡིག་གསར་པ།)"
@@ -3769,20 +3781,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "རྒྱ་སྐད་ (རྒྱ་ཡིག་རྙིང་པ།)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr ""
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/br/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/br/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2016-01-14 15:07+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Breton <https://hosted.weblate.org/projects/weblate/master/br/"
 ">\n"
 "Language: br\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -876,14 +876,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -4069,14 +4075,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (China)"
 msgid "Wu (Simplified)"
 msgstr "Sinaeg (Sina)"
@@ -4085,20 +4097,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Taiwan)"
 msgid "Wu (Traditional)"
 msgstr "Sinaeg (Taiwan)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "kalmouk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ca/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ca/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Joan Montané <joan@montane.cat>, 2019, 2020, 2021.
 # Eduard Ereza Martínez <eduard@ereza.cat>, 2019, 2020, 2021, 2022, 2023.
 # Adolfo Jayme Barrientos <fitojb@ubuntu.com>, 2020.
-# Ecron <ecron_89@hotmail.com>, 2020.
+# Ecron <ecron_89@hotmail.com>, 2020, 2023.
 # Maite Guix <maite.guix@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-14 11:39+0000\n"
-"Last-Translator: Eduard Ereza Martínez <eduard@ereza.cat>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-30 14:51+0000\n"
+"Last-Translator: Ecron <ecron_89@hotmail.com>\n"
 "Language-Team: Catalan <https://hosted.weblate.org/projects/weblate/"
 "languages/ca/>\n"
 "Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "àfar"
 
@@ -810,14 +810,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "bhutanès"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2433,26 +2440,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "nàhuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "xinès (tradicional)"
+msgstr "xinès (Min Nan, tradicional)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "xinès (min nan)"
+msgstr "xinès (min nan, llatí)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napolità"
 
@@ -3754,32 +3757,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "westfalià"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "wòlof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "wu (simplificat)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "wu (tradicional)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "wòlof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "calmuc"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ce/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ce/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ce\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -823,14 +823,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3873,14 +3879,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "волоф"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "атта цийн"
@@ -3889,20 +3901,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "ламастан цийн"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "волоф"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "гӀалмакхойн"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ckb/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ckb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Jwtiyar Nariman <jwtiyar@gmail.com>, 2020.
 # Kurd As <kurd68587@gmail.com>, 2020, 2021.
 # Rener kaka <Rabarajax51@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Kurdish (Central) <https://hosted.weblate.org/projects/"
 "weblate/languages/ckb/>\n"
 "Language: ckb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -816,14 +816,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "دینکا"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "دۆگری"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3820,14 +3826,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "وۆلۆف"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "چینی (ئاسانکراو)"
@@ -3836,20 +3848,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "چینی (کۆن)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "وۆلۆف"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "کالمیک"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/crh/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/crh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: crh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -827,14 +827,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri (Hindistan)"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3882,32 +3888,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr ""
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/cs/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/cs/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Michal Čihař <michal@weblate.org>, 2020, 2021.
 # Jonáš Loskot <ltvlcihory@gmail.com>, 2020.
 # Milan <mobrcian@hotmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/weblate/languages/"
 "cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -826,14 +826,21 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Bhútánština"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dógrí"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3920,14 +3927,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Volofština"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Čínština (zjednodušená)"
@@ -3936,20 +3949,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Čínština (tradiční)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Volofština"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Malajština"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/cv/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/cv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # İlle <derasetad@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Chuvash <https://hosted.weblate.org/projects/weblate/"
 "languages/cv/>\n"
 "Language: cv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -828,14 +828,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Догрилле"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3856,14 +3862,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr ""
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "китай, ҫӑмӑллатнӑ ҫыру"
@@ -3872,20 +3884,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "китай, традициллӗ ҫыру"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr ""
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/cy/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/cy/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # dreigiau <sterilgrimed23@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2023-03-09 22:56+0000\n"
 "Last-Translator: dreigiau <sterilgrimed23@gmail.com>\n"
 "Language-Team: Welsh <https://hosted.weblate.org/projects/weblate/languages/"
 "cy/>\n"
 "Language: cy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -821,15 +821,15 @@
 msgid "German (Luxembourg)"
 msgstr "Almaeneg (Luxembourg)"
 
 #. Translators: Language name for ISO code "del". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Delaware"
-msgstr ""
+msgstr "Delaware"
 
 #. Translators: Language name for ISO code "den". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slave (Athapascan)"
 msgstr ""
 
@@ -844,14 +844,21 @@
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Dinka"
 msgstr "Sango"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Dsonca"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -886,15 +893,15 @@
 msgid "Dhivehi"
 msgstr "Dhivehi"
 
 #. Translators: Language name for ISO code "dyu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dyula"
-msgstr ""
+msgstr "Dyula"
 
 #. Translators: Language name for ISO code "dz". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dzongkha"
 msgstr "Dzongkha"
 
@@ -1881,15 +1888,15 @@
 msgid "Kamba (Kenya)"
 msgstr ""
 
 #. Translators: Language name for ISO code "kaw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kawi"
-msgstr ""
+msgstr "Kawi"
 
 #. Translators: Language name for ISO code "kbd". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Kabuverdianu"
 msgid "Kabardian"
@@ -2083,15 +2090,15 @@
 msgid "Kumyk"
 msgstr "Cwmiceg"
 
 #. Translators: Language name for ISO code "kut". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kutenai"
-msgstr ""
+msgstr "Kutenai"
 
 #. Translators: Language name for ISO code "kv". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Komi"
 msgstr "Comi"
 
@@ -2237,15 +2244,15 @@
 msgid "Luba-Lulua"
 msgstr "Luba-Lulua"
 
 #. Translators: Language name for ISO code "lui". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Luiseno"
-msgstr ""
+msgstr "Luiseno"
 
 #. Translators: Language name for ISO code "lun". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Lunda"
 msgstr "Rwndi"
@@ -3688,15 +3695,15 @@
 msgid "Tongan"
 msgstr "Tongeg"
 
 #. Translators: Language name for ISO code "tog". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tonga (Nyasa)"
-msgstr ""
+msgstr "Tonga (Nyasa)"
 
 #. Translators: Language name for ISO code "tok". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Toki Pona"
 msgstr "Toki Pona"
 
@@ -3956,14 +3963,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Woloff"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "Tsieinëeg Symledig"
@@ -3972,20 +3985,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "Tsieinëeg Traddodiadol"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Woloff"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Canareg"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/da/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/da/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # scootergrisen <scootergrisen@gmail.com>, 2018, 2019, 2020, 2021.
 # Aputsiak Niels Janussen <aputtu@gmail.com>, 2021.
 # Aputsiaĸ Niels Janussen <aj@isit.gl>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Danish <https://hosted.weblate.org/projects/weblate/languages/"
 "da/>\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -817,14 +817,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Dinka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3818,14 +3825,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Kinesisk (forenklet)"
@@ -3834,20 +3847,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Kinesisk (traditionelt)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/de/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # Christian Eichert <c@zp1.net>, 2021.
 # VfBFan <drop0815@posteo.de>, 2021, 2023.
 # Andrej Shadura <andrew@shadura.me>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-01 03:03+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-05 03:49+0000\n"
 "Last-Translator: VfBFan <drop0815@posteo.de>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/weblate/languages/"
 "de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -815,14 +815,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2444,26 +2450,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl/Aztekisch"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Chinesisch (traditionell)"
+msgstr "Min Nan/Minnan (traditionell)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Min Nan/Minnan"
+msgstr "Min Nan/Minnan (lateinisch)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolitanisch"
 
@@ -3765,32 +3767,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfälisch"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (vereinfacht)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (traditionell)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Oiratisch/Kalmückisch"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/django.pot` & `weblate-language-data-2023.5/weblate_language_data/locale/django.pot`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -805,14 +805,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3745,30 +3751,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/dv/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/dv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: dv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/el/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/el/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Eugenia Russell <eugenia.russell2019@gmail.com>, 2021.
 # J. Lavoie <j.lavoie@net-c.ca>, 2021.
 # george kitsoukakis <norhorn@gmail.com>, 2021, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-02-05 15:59+0000\n"
 "Last-Translator: george kitsoukakis <norhorn@gmail.com>\n"
 "Language-Team: Greek <https://hosted.weblate.org/projects/weblate/languages/"
 "el/>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -815,14 +815,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Ντίνκα"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Ντογκρικά"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3803,14 +3809,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Γουολοφικά"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Κινέζικα (Απλοποιημένα)"
@@ -3819,20 +3831,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Κινέζικα (Παραδοσιακά)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Γουολοφικά"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Καλμίκ"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # Adolfo Jayme Barrientos <fitojb@ubuntu.com>, 2021.
 # Andrej Shadura <andrew@shadura.me>, 2022.
 # Andi Chandler <andi@gowling.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-04-02 13:34+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-06-12 14:52+0000\n"
 "Last-Translator: Andi Chandler <andi@gowling.com>\n"
 "Language-Team: English (United Kingdom) <https://hosted.weblate.org/projects/"
 "weblate/languages/en_GB/>\n"
 "Language: en_GB\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.17-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -104,21 +104,21 @@
 msgid "Akkadian"
 msgstr "Akkadian"
 
 #. Translators: Language name for ISO code "ale". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Aleut"
-msgstr ""
+msgstr "Aleut"
 
 #. Translators: Language name for ISO code "alt". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Altai (Southern)"
-msgstr ""
+msgstr "Altai (Southern)"
 
 #. Translators: Language name for ISO code "am". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Amharic"
 msgstr "Amharic"
 
@@ -200,39 +200,39 @@
 msgid "Arabic (Yemen)"
 msgstr "Arabic (Yemen)"
 
 #. Translators: Language name for ISO code "arc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Aramaic"
-msgstr ""
+msgstr "Aramaic"
 
 #. Translators: Language name for ISO code "arn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mapudungun"
 msgstr "Mapudungun"
 
 #. Translators: Language name for ISO code "arp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arapaho"
-msgstr ""
+msgstr "Arapaho"
 
 #. Translators: Language name for ISO code "ars". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arabic (Najdi)"
 msgstr "Arabic (Najdi)"
 
 #. Translators: Language name for ISO code "arw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arawak"
-msgstr ""
+msgstr "Arawak"
 
 #. Translators: Language name for ISO code "as". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Assamese"
 msgstr "Assamese"
 
@@ -254,29 +254,27 @@
 msgid "Avaric"
 msgstr "Avaric"
 
 #. Translators: Language name for ISO code "avk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kotava"
-msgstr ""
+msgstr "Kotava"
 
 #. Translators: Language name for ISO code "awa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Awadhi"
-msgstr ""
+msgstr "Awadhi"
 
 #. Translators: Language name for ISO code "ay". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Aymará"
 msgid "Aymara"
-msgstr "Aymará"
+msgstr "Aymara"
 
 #. Translators: Language name for ISO code "ayc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Aymara (Southern)"
 msgstr "Aymara (Southern)"
 
@@ -285,30 +283,28 @@
 #. or other variant.
 msgid "Azerbaijani"
 msgstr "Azerbaijani"
 
 #. Translators: Language name for ISO code "azb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Azerbaijani, South"
 msgid "Azerbaijani (Southern)"
-msgstr "Azerbaijani, South"
+msgstr "Azerbaijani (Southern)"
 
 #. Translators: Language name for ISO code "ba". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bashkir"
 msgstr "Bashkir"
 
 #. Translators: Language name for ISO code "bal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Baluchi"
-msgstr ""
+msgstr "Baluchi"
 
 #. Translators: Language name for ISO code "ban". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Balinese"
 msgstr "Balinese"
 
@@ -318,15 +314,15 @@
 msgid "Bavarian"
 msgstr "Bavarian"
 
 #. Translators: Language name for ISO code "bas". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Basa (Cameroon)"
-msgstr ""
+msgstr "Basa (Cameroon)"
 
 #. Translators: Language name for ISO code "be". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Belarusian"
 msgstr "Belarusian"
 
@@ -336,27 +332,27 @@
 msgid "Belarusian (latin)"
 msgstr "Belarusian (latin)"
 
 #. Translators: Language name for ISO code "bej". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Beja"
-msgstr ""
+msgstr "Beja"
 
 #. Translators: Language name for ISO code "bem". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bemba"
 msgstr "Bemba"
 
 #. Translators: Language name for ISO code "ber". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Berber"
-msgstr ""
+msgstr "Berber"
 
 #. Translators: Language name for ISO code "bez". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bena"
 msgstr "Bena"
 
@@ -372,39 +368,39 @@
 msgid "Bihari"
 msgstr "Bihari"
 
 #. Translators: Language name for ISO code "bho". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bhojpuri"
-msgstr ""
+msgstr "Bhojpuri"
 
 #. Translators: Language name for ISO code "bi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bislama"
 msgstr "Bislama"
 
 #. Translators: Language name for ISO code "bik". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bikol"
-msgstr ""
+msgstr "Bikol"
 
 #. Translators: Language name for ISO code "bin". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bini"
-msgstr ""
+msgstr "Bini"
 
 #. Translators: Language name for ISO code "bla". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Siksika"
-msgstr ""
+msgstr "Siksika"
 
 #. Translators: Language name for ISO code "bm". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bambara"
 msgstr "Bambara"
 
@@ -426,53 +422,51 @@
 msgid "Bengali (India)"
 msgstr "Bengali (India)"
 
 #. Translators: Language name for ISO code "bnt". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bantu (Other)"
-msgstr ""
+msgstr "Bantu (Other)"
 
 #. Translators: Language name for ISO code "bo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tibetan"
 msgstr "Tibetan"
 
 #. Translators: Language name for ISO code "bo_CN". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Tibetan"
 msgid "Tibetan (China)"
-msgstr "Tibetan"
+msgstr "Tibetan (China)"
 
 #. Translators: Language name for ISO code "bqi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bakhtiari"
-msgstr ""
+msgstr "Bakhtiari"
 
 #. Translators: Language name for ISO code "br". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Breton"
 msgstr "Breton"
 
 #. Translators: Language name for ISO code "bra". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Braj"
-msgstr ""
+msgstr "Braj"
 
 #. Translators: Language name for ISO code "brb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Brao"
-msgstr ""
+msgstr "Brao"
 
 #. Translators: Language name for ISO code "brx". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bodo"
 msgstr "Bodo"
 
@@ -494,21 +488,21 @@
 msgid "Bosnian (latin)"
 msgstr "Bosnian (latin)"
 
 #. Translators: Language name for ISO code "bua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Buriat"
-msgstr ""
+msgstr "Buriat"
 
 #. Translators: Language name for ISO code "bug". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Buginese"
-msgstr ""
+msgstr "Buginese"
 
 #. Translators: Language name for ISO code "byn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bilen"
 msgstr "Bilen"
 
@@ -524,27 +518,27 @@
 msgid "Valencian"
 msgstr "Valencian"
 
 #. Translators: Language name for ISO code "ca_AD". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Catalan (Andorra)"
-msgstr ""
+msgstr "Catalan (Andorra)"
 
 #. Translators: Language name for ISO code "cad". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Caddo"
-msgstr ""
+msgstr "Caddo"
 
 #. Translators: Language name for ISO code "cak". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kaqchikel"
-msgstr ""
+msgstr "Kaqchikel"
 
 #. Translators: Language name for ISO code "car". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Galibi Carib"
 msgstr "Galibi Carib"
 
@@ -572,63 +566,63 @@
 msgid "Chamorro"
 msgstr "Chamorro"
 
 #. Translators: Language name for ISO code "chb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chibcha"
-msgstr ""
+msgstr "Chibcha"
 
 #. Translators: Language name for ISO code "chg". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chagatai"
-msgstr ""
+msgstr "Chagatai"
 
 #. Translators: Language name for ISO code "chk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chuukese"
-msgstr ""
+msgstr "Chuukese"
 
 #. Translators: Language name for ISO code "chm". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mari"
 msgstr "Mari"
 
 #. Translators: Language name for ISO code "chn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chinook jargon"
-msgstr ""
+msgstr "Chinook jargon"
 
 #. Translators: Language name for ISO code "cho". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Choctaw"
-msgstr ""
+msgstr "Choctaw"
 
 #. Translators: Language name for ISO code "chp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chipewyan"
-msgstr ""
+msgstr "Chipewyan"
 
 #. Translators: Language name for ISO code "chr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Cherokee"
 msgstr "Cherokee"
 
 #. Translators: Language name for ISO code "chy". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Cheyenne"
-msgstr ""
+msgstr "Cheyenne"
 
 #. Translators: Language name for ISO code "ckb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kurdish (Central)"
 msgstr "Kurdish (Central)"
 
@@ -649,48 +643,46 @@
 #. or other variant.
 msgid "Montenegrin"
 msgstr "Montenegrin"
 
 #. Translators: Language name for ISO code "cnr_Cyrl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Bosnian (cyrillic)"
 msgid "Montenegrin (cyrillic)"
-msgstr "Bosnian (cyrillic)"
+msgstr "Montenegrin (cyrillic)"
 
 #. Translators: Language name for ISO code "co". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Corsican"
 msgstr "Corsican"
 
 #. Translators: Language name for ISO code "cop". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Coptic"
-msgstr ""
+msgstr "Coptic"
 
 #. Translators: Language name for ISO code "cpe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Creoles and pidgins (English based)"
-msgstr ""
+msgstr "Creoles and pidgins (English based)"
 
 #. Translators: Language name for ISO code "cpf". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Creoles and pidgins (French-based)"
-msgstr ""
+msgstr "Creoles and pidgins (French-based)"
 
 #. Translators: Language name for ISO code "cpp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Creoles and pidgins (Portuguese-based)"
-msgstr ""
+msgstr "Creoles and pidgins (Portuguese-based)"
 
 #. Translators: Language name for ISO code "cr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Cree"
 msgstr "Cree"
 
@@ -700,15 +692,15 @@
 msgid "Crimean Tatar"
 msgstr "Crimean Tatar"
 
 #. Translators: Language name for ISO code "crp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Creoles and pidgins"
-msgstr ""
+msgstr "Creoles and pidgins"
 
 #. Translators: Language name for ISO code "cs". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Czech"
 msgstr "Czech"
 
@@ -718,15 +710,15 @@
 msgid "Kashubian"
 msgstr "Kashubian"
 
 #. Translators: Language name for ISO code "cu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slavonic (Old Church)"
-msgstr ""
+msgstr "Slavonic (Old Church)"
 
 #. Translators: Language name for ISO code "cv". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chuvash"
 msgstr "Chuvash"
 
@@ -748,15 +740,15 @@
 msgid "Dakota"
 msgstr "Dakota"
 
 #. Translators: Language name for ISO code "dar". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dargwa"
-msgstr ""
+msgstr "Dargwa"
 
 #. Translators: Language name for ISO code "de". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "German"
 msgstr "German"
 
@@ -796,57 +788,63 @@
 msgid "German (Luxembourg)"
 msgstr "German (Luxembourg)"
 
 #. Translators: Language name for ISO code "del". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Delaware"
-msgstr ""
+msgstr "Delaware"
 
 #. Translators: Language name for ISO code "den". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slave (Athapascan)"
-msgstr ""
+msgstr "Slave (Athapascan)"
 
 #. Translators: Language name for ISO code "dgr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogrib"
 msgstr "Dogrib"
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Darai"
-msgstr ""
+msgstr "Darai"
 
 #. Translators: Language name for ISO code "dsb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Lower Sorbian"
 msgstr "Lower Sorbian"
 
 #. Translators: Language name for ISO code "dua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Duala"
-msgstr ""
+msgstr "Duala"
 
 #. Translators: Language name for ISO code "dum". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dutch (Middle)"
 msgstr "Dutch (Middle)"
 
@@ -856,15 +854,15 @@
 msgid "Dhivehi"
 msgstr "Dhivehi"
 
 #. Translators: Language name for ISO code "dyu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dyula"
-msgstr ""
+msgstr "Dyula"
 
 #. Translators: Language name for ISO code "dz". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dzongkha"
 msgstr "Dzongkha"
 
@@ -874,61 +872,57 @@
 msgid "Ewe"
 msgstr "Ewe"
 
 #. Translators: Language name for ISO code "efi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Efik"
-msgstr ""
+msgstr "Efik"
 
 #. Translators: Language name for ISO code "egl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Sicilian"
 msgid "Emilian"
-msgstr "Sicilian"
+msgstr "Emilian"
 
 #. Translators: Language name for ISO code "egy". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Egyptian (Ancient)"
-msgstr ""
+msgstr "Egyptian (Ancient)"
 
 #. Translators: Language name for ISO code "eka". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ekajuk"
-msgstr ""
+msgstr "Ekajuk"
 
 #. Translators: Language name for ISO code "el". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Greek"
 msgstr "Greek"
 
 #. Translators: Language name for ISO code "elx". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Elamite"
-msgstr ""
+msgstr "Elamite"
 
 #. Translators: Language name for ISO code "en". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "English"
 msgstr "English"
 
 #. Translators: Language name for ISO code "en@pirate". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "English (India)"
 msgid "English (Pirate)"
-msgstr "English (India)"
+msgstr "English (Pirate)"
 
 #. Translators: Language name for ISO code "en_AU". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "English (Australia)"
 msgstr "English (Australia)"
 
@@ -967,34 +961,28 @@
 #. or other variant.
 msgid "English (Philippines)"
 msgstr "English (Philippines)"
 
 #. Translators: Language name for ISO code "en_Shaw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "English (India)"
 msgid "English (Shavian)"
-msgstr "English (India)"
+msgstr "English (Shavian)"
 
 #. Translators: Language name for ISO code "en_Shaw_GB". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "English (United Kingdom)"
 msgid "English (Shavian, United Kingdom)"
-msgstr "English (United Kingdom)"
+msgstr "English (Shavian, United Kingdom)"
 
 #. Translators: Language name for ISO code "en_Shaw_US". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "English (United States)"
 msgid "English (Shavian, United States)"
-msgstr "English (United States)"
+msgstr "English (Shavian, United States)"
 
 #. Translators: Language name for ISO code "en_US". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "English (United States)"
 msgstr "English (United States)"
 
@@ -1033,26 +1021,22 @@
 #. or other variant.
 msgid "Spanish"
 msgstr "Spanish"
 
 #. Translators: Language name for ISO code "es@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Spanish (Colombia)"
 msgid "Spanish (formal)"
-msgstr "Spanish (Colombia)"
+msgstr "Spanish (formal)"
 
 #. Translators: Language name for ISO code "es@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Spanish (Panama)"
 msgid "Spanish (informal)"
-msgstr "Spanish (Panama)"
+msgstr "Spanish (informal)"
 
 #. Translators: Language name for ISO code "es_419". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Spanish (Latin America)"
 msgstr "Spanish (Latin America)"
 
@@ -1164,21 +1148,21 @@
 msgid "Basque"
 msgstr "Basque"
 
 #. Translators: Language name for ISO code "ewo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ewondo"
-msgstr ""
+msgstr "Ewondo"
 
 #. Translators: Language name for ISO code "ext". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Extremaduran"
-msgstr ""
+msgstr "Extremaduran"
 
 #. Translators: Language name for ISO code "fa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Persian"
 msgstr "Persian"
 
@@ -1188,21 +1172,21 @@
 msgid "Dari"
 msgstr "Dari"
 
 #. Translators: Language name for ISO code "fan". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Fang (Equatorial Guinea)"
-msgstr ""
+msgstr "Fang (Equatorial Guinea)"
 
 #. Translators: Language name for ISO code "fat". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Fanti"
-msgstr ""
+msgstr "Fanti"
 
 #. Translators: Language name for ISO code "ff". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Fulah"
 msgstr "Fulah"
 
@@ -1230,15 +1214,15 @@
 msgid "Faroese"
 msgstr "Faroese"
 
 #. Translators: Language name for ISO code "fon". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Fon"
-msgstr ""
+msgstr "Fon"
 
 #. Translators: Language name for ISO code "fr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "French"
 msgstr "French"
 
@@ -1289,18 +1273,16 @@
 #. or other variant.
 msgid "French (Senegal)"
 msgstr "French (Senegal)"
 
 #. Translators: Language name for ISO code "frc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (Canada)"
 msgid "French (Louisiana)"
-msgstr "French (Canada)"
+msgstr "French (Louisiana)"
 
 #. Translators: Language name for ISO code "frm". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "French (Middle)"
 msgstr "French (Middle)"
 
@@ -1316,15 +1298,15 @@
 msgid "Franco-Provençal"
 msgstr "Franco-Provençal"
 
 #. Translators: Language name for ISO code "frr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Frisian (Northern)"
-msgstr ""
+msgstr "Frisian (Northern)"
 
 #. Translators: Language name for ISO code "frs". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Frisian (Eastern)"
 msgstr "Frisian (Eastern)"
 
@@ -1346,33 +1328,33 @@
 msgid "Irish"
 msgstr "Irish"
 
 #. Translators: Language name for ISO code "gaa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ga"
-msgstr ""
+msgstr "Ga"
 
 #. Translators: Language name for ISO code "gay". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gayo"
-msgstr ""
+msgstr "Gayo"
 
 #. Translators: Language name for ISO code "gba". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gbaya (Central African Republic)"
 msgstr "Gbaya (Central African Republic)"
 
 #. Translators: Language name for ISO code "gbm". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Garhwali"
-msgstr ""
+msgstr "Garhwali"
 
 #. Translators: Language name for ISO code "gd". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gaelic"
 msgstr "Gaelic"
 
@@ -1394,21 +1376,21 @@
 msgid "Galician"
 msgstr "Galician"
 
 #. Translators: Language name for ISO code "glk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gilaki"
-msgstr ""
+msgstr "Gilaki"
 
 #. Translators: Language name for ISO code "gmh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "High German (Middle)"
-msgstr ""
+msgstr "High German (Middle)"
 
 #. Translators: Language name for ISO code "gn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Guarani"
 msgstr "Guarani"
 
@@ -1418,45 +1400,45 @@
 msgid "High German (Old)"
 msgstr "High German (Old)"
 
 #. Translators: Language name for ISO code "gon". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gondi"
-msgstr ""
+msgstr "Gondi"
 
 #. Translators: Language name for ISO code "gor". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gorontalo"
-msgstr ""
+msgstr "Gorontalo"
 
 #. Translators: Language name for ISO code "got". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gothic"
-msgstr ""
+msgstr "Gothic"
 
 #. Translators: Language name for ISO code "grb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Grebo"
-msgstr ""
+msgstr "Grebo"
 
 #. Translators: Language name for ISO code "grc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Greek (Ancient)"
-msgstr ""
+msgstr "Greek (Ancient)"
 
 #. Translators: Language name for ISO code "gsw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Alemannic"
-msgstr ""
+msgstr "Alemannic"
 
 #. Translators: Language name for ISO code "gu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gujarati"
 msgstr "Gujarati"
 
@@ -1466,33 +1448,33 @@
 msgid "Gujarati (India)"
 msgstr "Gujarati (India)"
 
 #. Translators: Language name for ISO code "guc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wayuu"
-msgstr ""
+msgstr "Wayuu"
 
 #. Translators: Language name for ISO code "gug". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Guaraní (Paraguayan)"
-msgstr ""
+msgstr "Guaraní (Paraguayan)"
 
 #. Translators: Language name for ISO code "gum". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Guambiano"
-msgstr ""
+msgstr "Guambiano"
 
 #. Translators: Language name for ISO code "gun". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Guaraní (Mbyá)"
-msgstr ""
+msgstr "Guaraní (Mbyá)"
 
 #. Translators: Language name for ISO code "guw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gun"
 msgstr "Gun"
 
@@ -1502,27 +1484,27 @@
 msgid "Manx"
 msgstr "Manx"
 
 #. Translators: Language name for ISO code "gwi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gwichʼin"
-msgstr ""
+msgstr "Gwichʼin"
 
 #. Translators: Language name for ISO code "ha". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hausa"
 msgstr "Hausa"
 
 #. Translators: Language name for ISO code "hai". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Haida"
-msgstr ""
+msgstr "Haida"
 
 #. Translators: Language name for ISO code "haw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hawaiian"
 msgstr "Hawaiian"
 
@@ -1532,15 +1514,15 @@
 msgid "Hebrew"
 msgstr "Hebrew"
 
 #. Translators: Language name for ISO code "he_IL". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hebrew (Israel)"
-msgstr ""
+msgstr "Hebrew (Israel)"
 
 #. Translators: Language name for ISO code "hi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hindi"
 msgstr "Hindi"
 
@@ -1556,21 +1538,21 @@
 msgid "Hiligaynon"
 msgstr "Hiligaynon"
 
 #. Translators: Language name for ISO code "hit". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hittite"
-msgstr ""
+msgstr "Hittite"
 
 #. Translators: Language name for ISO code "hmn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hmong"
-msgstr ""
+msgstr "Hmong"
 
 #. Translators: Language name for ISO code "hne". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chhattisgarhi"
 msgstr "Chhattisgarhi"
 
@@ -1610,21 +1592,21 @@
 msgid "Hungarian"
 msgstr "Hungarian"
 
 #. Translators: Language name for ISO code "hup". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hupa"
-msgstr ""
+msgstr "Hupa"
 
 #. Translators: Language name for ISO code "hus". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Huastec"
-msgstr ""
+msgstr "Huastec"
 
 #. Translators: Language name for ISO code "hy". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Armenian"
 msgstr "Armenian"
 
@@ -1640,15 +1622,15 @@
 msgid "Interlingua"
 msgstr "Interlingua"
 
 #. Translators: Language name for ISO code "iba". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Iban"
-msgstr ""
+msgstr "Iban"
 
 #. Translators: Language name for ISO code "id". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Indonesian"
 msgstr "Indonesian"
 
@@ -3820,14 +3802,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Chinese (Simplified)"
@@ -3836,20 +3824,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Chinese (Traditional)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/enm/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/enm/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: enm\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/eo/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/eo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Pierre Soubourou <pierre.soubourou@gmail.com>, 2019.
 # tuxayo/Victor Grousset <victor@tuxayo.net>, 2019.
 # Nikolay Korotkiy <sikmir@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Esperanto <https://hosted.weblate.org/projects/weblate/"
 "languages/eo/>\n"
 "Language: eo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -857,14 +857,21 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Dinka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogra"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3989,14 +3996,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "volofa"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Ĉina (simpligita)"
@@ -4005,20 +4018,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Ĉina (tradicia)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "volofa"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Valama"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/es/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/es/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Franco <francobenedetti.59+github1@gmail.com>, 2018, 2019, 2022.
+# Franco <francobenedetti.59+github1@gmail.com>, 2018, 2019, 2022, 2023.
 # Adalberto Alvarez Perez <adalprofe@gmail.com>, 2018.
 # Adolfo Jayme Barrientos <fitojb@ubuntu.com>, 2019, 2020, 2021, 2022.
 # Andrés S <andres.segovia.dev@gmail.com>, 2019.
 # David Leal <halfpacho@gmail.com>, 2021.
 # Pablo Hinojosa <pablohn6@gmail.com>, 2022.
 # gallegonovato <fran-carro@hotmail.es>, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-03 18:36+0000\n"
-"Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-06-12 14:52+0000\n"
+"Last-Translator: Franco <francobenedetti.59+github1@gmail.com>\n"
 "Language-Team: Spanish <https://hosted.weblate.org/projects/weblate/"
 "languages/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -812,14 +812,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Dinka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2435,26 +2442,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Náhuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Chino (tradicional)"
+msgstr "Chino (mǐn nán, tradicional)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Chino (min nan)"
+msgstr "Chino (mǐn nán, latino)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
 
@@ -3756,32 +3759,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfalia"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wólof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Chino Wu (simplificado)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Chino Wu (tradicional)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wólof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Calmuco"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/et/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/et/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Janar Leas <janar.leas@gmail.com>, 2019.
 # Priit Jõerüüt <hwlate@joeruut.com>, 2020, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2023-03-10 11:02+0000\n"
 "Last-Translator: Priit Jõerüüt <hwlate@joeruut.com>\n"
 "Language-Team: Estonian <https://hosted.weblate.org/projects/weblate/"
 "languages/et/>\n"
 "Language: et\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -807,14 +807,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "dinka"
 
+# src/trans.h:27
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "denka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3757,32 +3764,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "westfaleni"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "volofi"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "uu (lihtsustatud)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "uu (traditsiooniline)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "volofi"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "kalmõki"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/eu/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/eu/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # S <sendoasojo@gmail.com>, 2019.
 # Osoitz <oelkoro@gmail.com>, 2020.
 # Iñigo Zendegi Urzelai <izendegi@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Basque <https://hosted.weblate.org/projects/weblate/languages/"
 "eu/>\n"
 "Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -852,14 +852,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandinkera"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogriera"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3989,14 +3995,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "wolofera"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Txinera (sinplifikatuta)"
@@ -4005,20 +4017,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Txinera (tradizionala)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "wolofera"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "kalmykera"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/fa/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/fa/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Abbas Baharforoosh <abahar1996@gmail.com>, 2020.
 # Mostafa Ahangarha <ahangarha@gmail.com>, 2020.
 # Mokhtar Garmehi <Mokhtar_garmeh@yahoo.com>, 2021, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-02-23 00:57+0000\n"
 "Last-Translator: Mokhtar Garmehi <Mokhtar_garmeh@yahoo.com>\n"
 "Language-Team: Persian <https://hosted.weblate.org/projects/weblate/"
 "languages/fa/>\n"
 "Language: fa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -825,14 +825,21 @@
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Dinka"
 msgstr "ماندینکایی"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "دینکایی"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "دوگری"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3885,14 +3892,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ولوفی"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "چینی (ساده شده)"
@@ -3901,20 +3914,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "چینی (سنتی)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ولوفی"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "مالزیایی"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/fi/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/fi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Demian Wright <wright.demian+weblate@gmail.com>, 2021.
 # Jiri Nakola <github@nakola.fi>, 2022.
 # J. Lavoie <j.lavoie@net-c.ca>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2023-01-05 16:51+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Finnish <https://hosted.weblate.org/projects/weblate/"
 "languages/fi/>\n"
 "Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -813,14 +813,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "dinka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3794,14 +3801,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Kiina (yksinkertainen)"
@@ -3810,20 +3823,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Kiina (perinteinen)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmukki"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/fil/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/fil/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 # Marco Santos <enum.scima@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-08-19 03:21+0000\n"
 "Last-Translator: Marco Santos <enum.scima@gmail.com>\n"
 "Language-Team: Filipino <https://hosted.weblate.org/projects/weblate/"
 "languages/fil/>\n"
 "Language: fil\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -808,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3790,14 +3796,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Tsino (Pinasimple)"
@@ -3806,20 +3818,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Tsino (Tradisyonal)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/fr/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 # J. Lavoie <j.lavoie@net-c.ca>, 2020, 2021, 2022.
 # Simon Picot <simonpicot06@gmail.com>, 2021.
 # tachyglossues <tachyglossues@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-01-31 01:05+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-05 03:49+0000\n"
 "Last-Translator: tachyglossues <tachyglossues@gmail.com>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/weblate/languages/"
 "fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -811,14 +811,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2434,26 +2440,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Chinois (Traditionnel)"
+msgstr "Chinois (Min Nan, traditionnel)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Minnan"
+msgstr "Chinois (Min Nan, latin)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitain"
 
@@ -3755,32 +3757,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (simplifié)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (Traditionnel)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmouk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/fur/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/fur/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # adecorte <adecorte@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-12-24 02:14+0000\n"
 "Last-Translator: adecorte <adecorte@gmail.com>\n"
 "Language-Team: Friulian <https://hosted.weblate.org/projects/weblate/"
 "languages/fur/>\n"
 "Language: fur\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -821,14 +821,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3857,14 +3863,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "cinês semplificât"
@@ -3873,20 +3885,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "cinês tradizionâl"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/fy/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/fy/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Frisian <https://hosted.weblate.org/projects/weblate/"
 "languages/fy/>\n"
 "Language: fy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -879,14 +879,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -4075,14 +4081,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (China)"
 msgid "Wu (Simplified)"
 msgstr "Sineesk (Sina)"
@@ -4091,20 +4103,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Taiwan)"
 msgid "Wu (Traditional)"
 msgstr "Sineesk (Taiwan)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/gl/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/gl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Iván Seoane <ivanrsm1997@gmail.com>, 2018, 2019.
 # Iváns <ivanrsm1997@gmail.com>, 2019, 2020.
 # gallegonovato <fran-carro@hotmail.es>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-11-25 19:42+0000\n"
 "Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
 "Language-Team: Galician <https://hosted.weblate.org/projects/weblate/"
 "languages/gl/>\n"
 "Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -808,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka (hablado por los Dinka)"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3927,14 +3933,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "wólof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Chinés (Sinxelo)"
@@ -3943,20 +3955,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Chinés (Tradicional)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "wólof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/he/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/he/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # Omeritzics Games <omeritzicschwartz@gmail.com>, 2020.
 # Omer I.S. <omeritzicschwartz@gmail.com>, 2021.
 # Tzvika <mmm_45@walla.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-01-31 01:49+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-21 12:25+0000\n"
 "Last-Translator: Yaron Shahrabani <sh.yaron@gmail.com>\n"
 "Language-Team: Hebrew <https://hosted.weblate.org/projects/weblate/languages/"
 "he/>\n"
 "Language: he\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "עפרית"
 
@@ -809,14 +809,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "דינקאית"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "דוגרי"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2432,26 +2438,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "נאוואטל"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "סינית מסורתית"
+msgstr "סינית מסורתית (מין של האי נאן)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "סינית (מין של האי נאן)"
+msgstr "סינית (מין של האי נאן, לטינית)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "נפוליטנית"
 
@@ -3753,32 +3755,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "וסטפלית"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "וולוף"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "וו מפושטת"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "וו מסורתית"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "וולוף"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "קלמיקית"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/hi/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/hi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # Deepak Mathur <deepakmathur174@gmail.com>, 2020.
 # KushagraKarira <kushagrakarira@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-12-17 17:49+0000\n"
 "Last-Translator: KushagraKarira <kushagrakarira@gmail.com>\n"
 "Language-Team: Hindi <https://hosted.weblate.org/projects/weblate/languages/"
 "hi/>\n"
 "Language: hi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -815,14 +815,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "दिन्का"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "भुटानी"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "डोग्री"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3908,14 +3915,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "वोलोफ"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "सरलीकृत चीनी"
@@ -3924,20 +3937,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "पारंपरिक चीनी"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "वोलोफ"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "मलय"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/hr/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/hr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Marino <mrabach@gmail.com>, 2019, 2020.
 # Milo Ivir <mail@milotype.de>, 2019, 2020, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-03-03 21:37+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-26 05:38+0000\n"
 "Last-Translator: Milo Ivir <mail@milotype.de>\n"
 "Language-Team: Croatian <https://hosted.weblate.org/projects/weblate/"
 "languages/hr/>\n"
 "Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
 "%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afarski"
 
@@ -808,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2431,26 +2437,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatlski"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Kineski (tradicionalni)"
+msgstr "Kineski (Min Nan, tradicionalni)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Kineski (Min Nan)"
+msgstr "Kineski (Min Nan, latinica)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitanski"
 
@@ -3752,32 +3754,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Vestfalski"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Volof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (pojednostavljeni)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (tradicionalni)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Volof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/hu/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/hu/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # ovari <ovari123@zoho.com>, 2020.
 # Balázs Meskó <meskobalazs@mailbox.org>, 2021, 2022.
 # f3rr31 <5920873@disroot.org>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-01-25 02:44+0000\n"
 "Last-Translator: Balázs Meskó <meskobalazs@mailbox.org>\n"
 "Language-Team: Hungarian <https://hosted.weblate.org/projects/weblate/"
 "languages/hu/>\n"
 "Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -820,14 +820,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "dinka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3834,14 +3841,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Volof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Kínai (egyszerűsített)"
@@ -3850,20 +3863,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Kínai (hagyományos)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Volof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmük"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/hy/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/hy/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2015.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2016-01-14 14:59+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Armenian <https://hosted.weblate.org/projects/weblate/master/"
 "hy/>\n"
 "Language: hy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -851,14 +851,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "դոգրի"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3971,14 +3977,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "վոլոֆ"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "պարզեցված չինարեն"
@@ -3987,20 +3999,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "ավանդական չինարեն"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "վոլոֆ"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "կալմիկերեն"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ia/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ia/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ia\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -823,14 +823,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3873,14 +3879,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "chinese simplificate"
@@ -3889,20 +3901,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "chinese traditional"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "calmuco"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/id/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/id/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 # Arif Budiman <arifpedia@gmail.com>, 2016-2017, 2020.
 # Andika Triwidada <andika@gmail.com>, 2018, 2020, 2021.
 # ditokp <ditokpl@gmail.com>, 2018.
 # frottle <catatan.kungkong@gmail.com>, 2020.
 # Reza Almanda <rezaalmanda27@gmail.com>, 2021.
 # Linerly <linerly@protonmail.com>, 2022, 2023.
 # Taufik A. Wicaksono <taufikadi.wicaksono@tutamail.com>, 2022.
-# Taufik Adi Wicaksono <taufikadi.wicaksono@tutamail.com>, 2022.
+# Taufik Adi Wicaksono <taufikadi.wicaksono@tutamail.com>, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-01 03:03+0000\n"
-"Last-Translator: Linerly <linerly@protonmail.com>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-23 04:52+0000\n"
+"Last-Translator: Taufik Adi Wicaksono <taufikadi.wicaksono@tutamail.com>\n"
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/weblate/"
 "languages/id/>\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -813,14 +813,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2436,26 +2442,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Cina (Tradisional)"
+msgstr "Cina (Min Nan, Tradisional)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Cina (Min Nan)"
+msgstr "Cina (Min Nan, Latin)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolitan"
 
@@ -3757,32 +3759,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalia"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (Sederhana)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (Tradisional)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ie/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ie/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # OIS <mistresssilvara@hotmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-03-26 11:37+0000\n"
 "Last-Translator: OIS <mistresssilvara@hotmail.com>\n"
 "Language-Team: Occidental <https://hosted.weblate.org/projects/weblate/"
 "languages/ie/>\n"
 "Language: ie\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -806,14 +806,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3750,30 +3756,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/is/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/is/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Weblate <noreply@weblate.org>, 2020.
 # Sveinn í Felli <sv1@fellsnet.is>, 2020, 2021, 2022, 2023.
 # Þórhalla Guðmundsdóttir Beck <plergux@outlook.com>, 2020, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: Sveinn í Felli <sv1@fellsnet.is>\n"
 "Language-Team: Icelandic <https://hosted.weblate.org/projects/weblate/"
 "languages/is/>\n"
 "Language: is\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -808,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3752,32 +3758,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (einfölduð)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (hefðbundin)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/it/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/it/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 # Pierfrancesco Passerini <p.passerini@gmail.com>, 2019, 2020, 2021.
 # coronabond <coronabond@airmail.cc>, 2020, 2022.
 # Antenore Gatta <antenore@simbiosi.org>, 2020.
 # J. Lavoie <j.lavoie@net-c.ca>, 2020, 2021.
 # giuseppe <g.pecoraro@odissea.at>, 2021.
 # ROBERTO BORIOTTI <roberto.boriotti@gmail.com>, 2021.
 # bovirus <roberto.boriotti@canon.it>, 2022, 2023.
+# Massimo Pissarello <mapi68@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-01 03:03+0000\n"
-"Last-Translator: bovirus <roberto.boriotti@canon.it>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-11 14:49+0000\n"
+"Last-Translator: Massimo Pissarello <mapi68@gmail.com>\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/weblate/"
 "languages/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 "X-Poedit-SourceCharset: UTF-8\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
@@ -815,14 +816,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2438,26 +2445,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Cinese (Tradizionale)"
+msgstr "Cinese (Min Nan, Tradizionale)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Cinese (Min Nan)"
+msgstr "Cinese (Min Nan, Latino)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napoletano"
 
@@ -3759,32 +3762,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (semplificato)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (tradizionale)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ja/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # ht1722 <taichi_19990611@yahoo.co.jp>, 2022.
 # amano <amano@users.noreply.hosted.weblate.org>, 2023.
 # SAIHAZE <saihaze@outlook.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-04-02 00:21+0000\n"
-"Last-Translator: Kyotaro Iijima <kyotaro.eyes@gmail.com>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-15 08:50+0000\n"
+"Last-Translator: amano <amano@users.noreply.hosted.weblate.org>\n"
 "Language-Team: Japanese <https://hosted.weblate.org/projects/weblate/"
 "languages/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.17-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "アファル語"
 
@@ -871,14 +871,23 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "ディンカ語"
 
+# 国国
+# スーダン南部
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "ディンカ語"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ドーグリー語"
 
 # ロシア Darghinian
@@ -2607,26 +2616,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ナワトル語"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "中国語 (繁体字)"
+msgstr "中国語 (閩南語、繁体字)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "中国語 (ビン南)"
+msgstr "中国語 (閩南語、ラテン文字)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ナポリ語"
 
@@ -4012,32 +4017,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "ウエストファーレン語"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ウォロフ語"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "吳語 (簡体字)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "吳語 (繁体字)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ウォロフ語"
-
 # エチオピア
 # ワッラモ語とも
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "カルムイク語"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ka/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ka/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # George Salukvadze <giosal90@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-08-25 13:17+0000\n"
 "Last-Translator: George Salukvadze <giosal90@gmail.com>\n"
 "Language-Team: Georgian <https://hosted.weblate.org/projects/weblate/"
 "languages/ka/>\n"
 "Language: ka\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -806,14 +806,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "დინკა"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "დოგრი"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3764,14 +3770,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ვოლოფური"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "გამარტივებული ჩინური"
@@ -3780,20 +3792,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "ტრადიციული ჩინური"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ვოლოფური"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "ყალმუხური"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/kab/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/kab/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Muḥend Belqasem <belkacem77@gmail.com>, 2020.
 # Ouchene <merzouk.ouchene@laposte.net>, 2020.
 # Kahina Messaoudi <messaoudikahina02@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Kabyle <https://hosted.weblate.org/projects/weblate/languages/"
 "kab/>\n"
 "Language: kab\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -838,14 +838,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Tamandinkat"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Tadugrit"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3940,14 +3946,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Tawuluft"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Tacinwat (Taḥerfit)"
@@ -3956,20 +3968,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Tacinwat (Tamansayt)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Tawuluft"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/kk/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/kk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Weblate <noreply@weblate.org>, 2019.
 # WWWesten <wwwesten@gmail.com>, 2019.
 # Kuwanish Orinbay <firstpeople111@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Kazakh <https://hosted.weblate.org/projects/weblate/languages/"
 "kk/>\n"
 "Language: kk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -858,14 +858,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandınka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogrı"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3994,14 +4000,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Ýolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Hanzý (jeńil)"
@@ -4010,20 +4022,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Hanzý (dástúr)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Ýolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "қалмақ тілі"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/km/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/km/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # ប៉ុកណូ រ៉ូយ៉ាល់ <royalpokno68@gmail.com>, 2019, 2020, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Khmer (Central) <https://hosted.weblate.org/projects/weblate/"
 "languages/km/>\n"
 "Language: km\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -834,14 +834,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ដូហ្គ្រី"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3948,14 +3954,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "វូឡុហ្វ"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "ចិន​អក្សរ​កាត់"
@@ -3964,20 +3976,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "ចិន​អក្សរ​ពេញ"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "វូឡុហ្វ"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "កាលមីគ"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/kmr/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/kmr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Pêşeroja paşerojê <cyax1@protonmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-01-14 19:28+0000\n"
 "Last-Translator: Pêşeroja paşerojê <cyax1@protonmail.com>\n"
 "Language-Team: Kurdish (Northern) <https://hosted.weblate.org/projects/"
 "weblate/languages/kmr/>\n"
 "Language: kmr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -860,14 +860,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandînkayî"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogrî"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3998,14 +4004,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolofî"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Çînî (Sadekirî)"
@@ -4014,20 +4026,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Çînî (Kevneşopî)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolofî"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ko/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ko/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 # Hoseok Seo <ddinghoya@gmail.com>, 2022.
 # 이정희 <daemul72@gmail.com>, 2023.
 # Yi Yunseok <ironyunseok@protonmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-13 06:26+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-15 08:51+0000\n"
 "Last-Translator: 이정희 <daemul72@gmail.com>\n"
 "Language-Team: Korean <https://hosted.weblate.org/projects/weblate/languages/"
 "ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "아파르어"
 
@@ -813,14 +813,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "딩카어"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "발트어"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "도그리어"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2437,26 +2444,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "나우아틀어"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "중국어 (번체)"
+msgstr "중국어 (민난어, 번체)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "중국어 (북경)"
+msgstr "중국어 (민난어, 라틴어)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "나폴리어"
 
@@ -3760,32 +3763,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "베스트팔리아"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "월로프어"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "우어 (간체)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "우어 (번체)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "월로프어"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "칼미크어"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ksh/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ksh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2014-10-01 09:41+0200\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Colognian <https://hosted.weblate.org/projects/weblate/master/"
 "ksh/>\n"
 "Language: ksh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -874,14 +874,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -4066,14 +4072,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (China)"
 msgid "Wu (Simplified)"
 msgstr "Schenehsesch (us Schihna)"
@@ -4082,20 +4094,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Taiwan)"
 msgid "Wu (Traditional)"
 msgstr "Schenehsesch (us Taiwan)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmükkesch"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ln/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ln/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Lingala <https://hosted.weblate.org/projects/weblate/"
 "languages/ln/>\n"
 "Language: ln\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -845,14 +845,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3925,30 +3931,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/lt/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/lt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Lithuanian <https://hosted.weblate.org/projects/weblate/"
 "languages/lt/>\n"
 "Language: lt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -854,14 +854,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "Mandinkų"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3964,14 +3970,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "volofų"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "kinų (supaprastinta)"
@@ -3980,20 +3992,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "kinų (tradicinė)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "volofų"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "kalmukų"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/lv/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/lv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # Coool (github.com/Coool) <coool@mail.lv>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-11-01 13:11+0000\n"
 "Last-Translator: Coool (github.com/Coool) <coool@mail.lv>\n"
 "Language-Team: Latvian <https://hosted.weblate.org/projects/weblate/"
 "languages/lv/>\n"
 "Language: lv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -807,14 +807,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinku"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogru"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3884,14 +3890,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Vestfāleņu"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Volofu"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "ķīniešu vienkāršotā"
@@ -3900,20 +3912,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "ķīniešu tradicionālā"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Volofu"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Valūniešu"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/lzh/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/lzh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # Xiang Heng Wei <yylteam@hotmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2023-01-21 09:23+0000\n"
 "Last-Translator: Xiang Heng Wei <yylteam@hotmail.com>\n"
 "Language-Team: Chinese (Literary) <https://hosted.weblate.org/projects/"
 "weblate/languages/lzh/>\n"
 "Language: lzh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -806,14 +806,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3776,14 +3782,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr ""
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "中文(简体)"
@@ -3792,20 +3804,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "中文(繁体)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr ""
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/mk/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/mk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Macedonian <https://hosted.weblate.org/projects/weblate/"
 "languages/mk/>\n"
 "Language: mk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -865,14 +865,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "динка"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "догри"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3987,14 +3993,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "волофски"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "поедноставен кинески"
@@ -4003,20 +4015,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "традиционален кинески"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "волофски"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Валонски"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ml/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ml/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ml\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -825,14 +825,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "ഡിങ്കാ"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ഡോഗ്രീ"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3877,14 +3883,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "വോളോഫ്"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "ലളിതമാക്കിയ ചൈനീസ്"
@@ -3893,20 +3905,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "പരമ്പരാഗത ചൈനീസ്"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "വോളോഫ്"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "കൽമൈക്"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/mr/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/mr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # Prachi Joshi <josprachi@yahoo.com>, 2019, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Marathi <https://hosted.weblate.org/projects/weblate/"
 "languages/mr/>\n"
 "Language: mr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -844,14 +844,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "मँडिंका"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "डेन्गका"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "डोगरी"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3953,14 +3959,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "पश्चिमफलिएन"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "वोलोफ"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "चीनी (सरलीकृत)"
@@ -3969,20 +3981,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "चीनी (पारंपारिक)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "वोलोफ"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "कलम्यक"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ms/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ms/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ms\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -835,14 +835,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Baltic"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Dogri"
 msgstr "Margin"
 
@@ -3939,14 +3946,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "Cina Ringkas"
@@ -3955,20 +3968,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "Cina Tradisional"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Bahasa Melayu"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/my/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/my/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Sithu Aung <sithu.aung015@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Burmese <https://hosted.weblate.org/projects/weblate/"
 "languages/my/>\n"
 "Language: my\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -839,14 +839,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ဒိုဂရီ"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3926,14 +3932,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ဝူလိုဖ်"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "တရုတ် (ခေတ်ပေါ်)"
@@ -3942,20 +3954,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "တရုတ် (ရိုးရာ)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ဝူလိုဖ်"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "ကာလ်မိုက်"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/nb/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/nb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Kurt Eilertsen <kurt@kheds.com>, 2018.
 # Petter Reinholdtsen <pere-weblate@hungry.com>, 2019.
 # FTno <ft-002@tutanota.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-09-30 22:09+0000\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/weblate/"
 "languages/nb_NO/>\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -833,14 +833,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Thuongjang"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "dzongkha"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3910,14 +3917,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfalisk"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Kinesisk (Forenklet)"
@@ -3926,20 +3939,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Kinesisk (Tradisjonell)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Vietnamesisk"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/nl/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 # Jaimie85 <alsemgeest@gmail.com>, 2020.
 # Heimen Stoffels <vistausss@outlook.com>, 2020, 2021.
 # Heimen Stoffels <vistausss@fastmail.com>, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-01-31 01:49+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-05 03:49+0000\n"
 "Last-Translator: Heimen Stoffels <vistausss@fastmail.com>\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/weblate/languages/"
 "nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -810,14 +810,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Dinka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2433,26 +2440,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Chinees (traditioneel)"
+msgstr "Chinees (Min Nan, traditioneel)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Chinees (Min Nan)"
+msgstr "Chinees (Min Nan, Latijn)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitaans"
 
@@ -3754,32 +3757,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfaals"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (vereenvoudigd)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (traditioneel)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/nn/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/nn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: nn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -815,14 +815,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Dzongkha"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3837,34 +3844,34 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Wu (Simplified)"
 msgstr "forenkla kinesisk"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Wu (Traditional)"
 msgstr "tradisjonell kinesisk"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Malayisk"
 
@@ -3998,20 +4005,14 @@
 #. Translators: Language name for ISO code "zza". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Zaza"
 msgstr "Kasakhisk"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
-
 #, fuzzy
 #~ msgid "Wu"
 #~ msgstr "Naurisk"
 
 #, fuzzy
 #~ msgid "Portuguese (Brazil"
 #~ msgstr "Portugisisk"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/oc/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/oc/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: oc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -817,14 +817,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3856,32 +3862,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolòf"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr ""
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolòf"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/or/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/or/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # Pro Neon <proneon267@gmail.com>, 2019.
+# Subham Jena <subhamjena8465@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2019-08-11 12:03+0000\n"
-"Last-Translator: Pro Neon <proneon267@gmail.com>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-11 14:49+0000\n"
+"Last-Translator: Subham Jena <subhamjena8465@gmail.com>\n"
 "Language-Team: Odia <https://hosted.weblate.org/projects/weblate/languages/"
 "or/>\n"
 "Language: or\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 3.8-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "ଅଫାର୍"
 
@@ -66,18 +67,16 @@
 #. or other variant.
 msgid "Afrikaans"
 msgstr "ଆଫ୍ରିକୀୟ"
 
 #. Translators: Language name for ISO code "afh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Maithili"
 msgid "Afrihili"
-msgstr "ମୈଥିଳୀ"
+msgstr "ଆଫ୍ରିହିଲି"
 
 #. Translators: Language name for ISO code "aii". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Samaritan Aramaic"
 msgid "Assyrian Neo-Aramaic"
@@ -845,14 +844,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "ଡ଼ିଙ୍କା"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "ଡେଙ୍କା"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ଡୋଗ୍ରୀ"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3917,14 +3922,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ୱୋଲଫ୍"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "ସରଳୀକୃତ ଚାଇନିଜ୍‌"
@@ -3933,20 +3944,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "ପାରମ୍ପରିକ ଚାଇନିଜ୍‌"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ୱୋଲଫ୍"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "କାଲ୍ମୀକ୍"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/pa/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/pa/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Aman ALam <alam.yellow@gmail.com>, 2019, 2020.
 # bgo-eiu <huyaqoob+toolforge@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-11-02 08:51+0000\n"
 "Last-Translator: bgo-eiu <huyaqoob+toolforge@gmail.com>\n"
 "Language-Team: Punjabi <https://hosted.weblate.org/projects/weblate/"
 "languages/pa/>\n"
 "Language: pa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -840,14 +840,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "ਮੰਡਿਨਕਾ"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "ਡੇਂਗਕਾ"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ਡੋਗਰੀ"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3952,14 +3958,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "ਵੈਸਟਫਾਲੀਨ"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ਵੋਲੋਫ"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "ਚੀਨੀ (ਰਿਵਾਇਤੀ)"
@@ -3968,20 +3980,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "ਚੀਨੀ (ਰਿਵਾਇਤੀ)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ਵੋਲੋਫ"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "ਕਾਲਮਾਇਕ"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # bgo-eiu <huyaqoob+toolforge@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-10-29 21:05+0000\n"
 "Last-Translator: bgo-eiu <huyaqoob+toolforge@gmail.com>\n"
 "Language-Team: Punjabi (Pakistan) <https://hosted.weblate.org/projects/"
 "weblate/languages/pa_PK/>\n"
 "Language: pa_PK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -808,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "ڈِنکا"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ڈوگری"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3759,30 +3765,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/peo/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/peo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: peo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/pl/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/pl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # Stanisław Stefan Krukowski <pet209a1@riseup.net>, 2020.
 # Damian Tokarski <damianwolennicy@gmail.com>, 2021.
 # Agnieszka C <aga_04@o2.pl>, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-01-31 01:49+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-06 05:50+0000\n"
 "Last-Translator: Agnieszka C <aga_04@o2.pl>\n"
 "Language-Team: Polish <https://hosted.weblate.org/projects/weblate/languages/"
 "pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "afar"
 
@@ -815,14 +815,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2438,26 +2444,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "chiński (tradycyjny)"
+msgstr "chiński (Min Nan, tradycyjny)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "chiński (Min Nan)"
+msgstr "chiński (Min Nan, łaciński)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "neapolitański"
 
@@ -3759,32 +3761,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "westfalski"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "wu (uproszczony)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "wu (tradycyjny)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "kałmucki"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ps/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ps/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ps\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -824,14 +824,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ډوګري"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3881,14 +3887,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ولوف"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "چیني (ساده شوی)"
@@ -3897,20 +3909,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "دوديزه چيني"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ولوف"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "ملایا"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/pt/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/pt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # Pedro Albuquerque <pmra@gmx.com>, 2019.
 # Manuela Silva <mmsrs@sky.com>, 2019, 2020.
 # rummsi <rummsi@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-03-13 13:15+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-06-09 19:47+0000\n"
 "Last-Translator: ssantos <ssantos@web.de>\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/weblate/"
 "languages/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -809,14 +809,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "dinka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2432,26 +2439,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Chinês (Tradicional)"
+msgstr "Chinês (Min Nan, Tradicional)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Chinês (Min Nan)"
+msgstr "Chinês (Min Nan, latim)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
 
@@ -3753,32 +3756,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfaliano"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (simplificado)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (tradicional)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Calmuc"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Luiz Fernando Ranghetti <elchevive@opensuse.org>, 2018, 2019, 2022.
 # Rafael Fontenelle <rafaelff@gnome.org>, 2018, 2019, 2020, 2021, 2022, 2023.
 # José Elias Júnior <jose.elias.0703@gmail.com>, 2020.
 # Eduardo Addad de Oliveira <duduaddad@gmail.com>, 2020, 2021, 2023.
 # Wellington Terumi Uemura <wellingtonuemura@gmail.com>, 2021.
 # Fred Maranhão <fred.maranhao@gmail.com>, 2021.
-# Claudio Filho F Filho <filhocf@gmail.com>, 2022.
+# Claudio Filho F Filho <filhocf@gmail.com>, 2022, 2023.
 # Luckumi <lipezinhofilipe@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-01-31 01:49+0000\n"
-"Last-Translator: Rafael Fontenelle <rafaelff@gnome.org>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-06-01 07:02+0000\n"
+"Last-Translator: Claudio Filho F Filho <filhocf@gmail.com>\n"
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
 "weblate/languages/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -813,14 +813,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinco"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Bengali"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2436,26 +2443,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Náuatle"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Chinês (tradicional)"
+msgstr "Chinês (Min Nan, Tradicional)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Chinês (Min Nan)"
+msgstr "Chinês (Min Nan, Latim)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
 
@@ -3757,32 +3760,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfaliano"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (simplificado)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (tradicional)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Calmuco"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # ssantos <ssantos@web.de>, 2020, 2021, 2022, 2023.
 # Dinis Medeiros <dinismedeiros@gmail.com>, 2021.
 # Hugo Carvalho <hugokarvalho@hotmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-03-13 13:15+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-29 10:50+0000\n"
 "Last-Translator: ssantos <ssantos@web.de>\n"
 "Language-Team: Portuguese (Portugal) <https://hosted.weblate.org/projects/"
 "weblate/languages/pt_PT/>\n"
 "Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -809,14 +809,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2432,26 +2438,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Chinês (Tradicional)"
+msgstr "Chinês (Min Nan, Tradicional)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Chinês (Min Nan)"
+msgstr "Chinês (Min Nan, Latim)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
 
@@ -3753,32 +3755,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfaliano"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (simplificado)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (tradicional)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Calmuc"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ro/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Christian Eichert <c@zp1.net>, 2021.
 # Licaon Kter <licaon.kter@protonmail.com>, 2021, 2022.
 # Simona Iacob <s@zp1.net>, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2023-02-10 20:35+0000\n"
 "Last-Translator: Simona Iacob <s@zp1.net>\n"
 "Language-Team: Romanian <https://hosted.weblate.org/projects/weblate/"
 "languages/ro/>\n"
 "Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -811,14 +811,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Baltic"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3788,14 +3795,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfalien"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Chineză (simplificată)"
@@ -3804,20 +3817,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Chineză (tradițională)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kallmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ro_MD\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ru/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 # Nikolay Korotkiy <sikmir@gmail.com>, 2019.
 # Golubev Alexander <fatzer2@gmail.com>, 2020, 2021.
 # Alex Ky <esthomolupus@gmail.com>, 2020.
 # Artem <KovalevArtem.ru@gmail.com>, 2020.
 # Mingun <Alexander_Sergey@mail.ru>, 2020.
 # Nikita Epifanov <nikgreens@protonmail.com>, 2020.
 # Serg Bormant <bormant@mail.ru>, 2020.
-# Andrei Stepanov <adem4ik@gmail.com>, 2020, 2022.
+# Andrei Stepanov <adem4ik@gmail.com>, 2020, 2022, 2023.
 # Yaron Shahrabani <sh.yaron@gmail.com>, 2021.
 # S3aBreeze <paperwork@evilcorp.ltd>, 2021, 2022.
 # Ivan <goz9ae93qun@temp.mailbox.org>, 2021.
 # Blueberry <igory.ygr200@gmail.com>, 2021.
 # Viktor <xasertop@gmail.com>, 2022.
 # Vin <k3kelm4vw@mozmail.com>, 2022, 2023.
 # S3aBreeze <S3aBreeze@users.noreply.hosted.weblate.org>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-01 03:03+0000\n"
-"Last-Translator: S3aBreeze <S3aBreeze@users.noreply.hosted.weblate.org>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-05 03:49+0000\n"
+"Last-Translator: Andrei Stepanov <adem4ik@gmail.com>\n"
 "Language-Team: Russian <https://hosted.weblate.org/projects/weblate/"
 "languages/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
 "%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Афарский"
 
@@ -824,14 +824,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Динка"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Динка"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Догри"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2447,26 +2454,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Науатль"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Китайский (традиционный)"
+msgstr "Китайский (миньнань, традиционный)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Китайский (миньнань)"
+msgstr "Китайский (миньнань, латинский)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Неаполитанский"
 
@@ -3768,32 +3771,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Вестфальский"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Волоф"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "У (упрощённый)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "У (традиционный)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Волоф"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Калмыцкий"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/sc/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/sc/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Ajeje Brazorf <lmelonimamo@yahoo.it>, 2018, 2019, 2020, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-01 03:03+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-08 17:57+0000\n"
 "Last-Translator: Ajeje Brazorf <lmelonimamo@yahoo.it>\n"
 "Language-Team: Sardinian <https://hosted.weblate.org/projects/weblate/"
 "languages/sc/>\n"
 "Language: sc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -806,14 +806,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2429,26 +2435,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Tzinesu (Traditzionale)"
+msgstr "Tzinesu (Min Nan, traditzionale)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Tzinesu (Min Nan)"
+msgstr "Tzinesu (Min Nan, caràteres latinos)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napoletanu"
 
@@ -3750,32 +3752,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westphalianu"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (Semplificadu)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (Traditzionale)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/si/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/si/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # HelaBasa <R45XvezA@protonmail.ch>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-03-06 07:50+0000\n"
 "Last-Translator: HelaBasa <R45XvezA@protonmail.ch>\n"
 "Language-Team: Sinhala <https://hosted.weblate.org/projects/weblate/"
 "languages/si/>\n"
 "Language: si\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -810,14 +810,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ඩොග්රි"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3784,14 +3790,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "වොලොෆ්"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "සරල චීන"
@@ -3800,20 +3812,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "සාම්ප්‍රදායික චීන"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "වොලොෆ්"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "කල්මික්"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/sk/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/sk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Ivan Pleva <ivan.pleva@tutanota.com>, 2020.
 # Marek freezy Víger <marek.viger@gmail.com>, 2020.
 # Milan <mobrcian@hotmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Slovak <https://hosted.weblate.org/projects/weblate/languages/"
 "sk/>\n"
 "Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -840,14 +840,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "mandinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogričtina"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3976,14 +3982,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Volofština"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Čínština (zlednodušená)"
@@ -3992,20 +4004,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Čínština (tradičná)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Volofština"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Vallónsky"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/skr/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/skr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # پرویز قادر <mpqadir@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-03-01 14:17+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-08 17:57+0000\n"
 "Last-Translator: پرویز قادر <mpqadir@gmail.com>\n"
 "Language-Team: Saraiki <https://hosted.weblate.org/projects/weblate/"
 "languages/skr/>\n"
 "Language: skr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-rc\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "افار"
 
@@ -806,14 +806,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "ڈنکا"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ڈوگری"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2429,26 +2435,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ناہوٹی"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "چینی (روایتی)"
+msgstr "چینی (من نان، روایتی)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "چینی (من نان)"
+msgstr "چینی (من نان، لاطینی)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "نیپولیٹں"
 
@@ -3750,32 +3752,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "ویسٹ فالین"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "وولوف"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "وو (سادہ)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "وو (رواٰیتی)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "وولوف"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "کلمیاک"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/sl/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/sl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Štefan Baebler <stefan.baebler@gmail.com>, 2020.
 # Domen <mitenem@outlook.com>, 2020.
 # Martin Srebotnjak <miles@filmsi.net>, 2020, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Slovenian <https://hosted.weblate.org/projects/weblate/"
 "languages/sl/>\n"
 "Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -826,14 +826,21 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "mandinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "dzongkha"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogrib"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3907,14 +3914,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "volofščina"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "kitajščina (poenostavljeno)"
@@ -3923,20 +3936,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "kitajščina (tradicionalno)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "volofščina"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "malajščina"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/sq/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/sq/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Automatically generated, 2014.
 #
 # Besnik Bleta <besnik@programeshqip.org>, 2020, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Besnik Bleta <besnik@programeshqip.org>\n"
 "Language-Team: Albanian <https://hosted.weblate.org/projects/weblate/"
 "languages/sq/>\n"
 "Language: sq\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -846,14 +846,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinkisht"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3949,14 +3955,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "uolofisht"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "Kineze (E thjeshtuar)"
@@ -3965,20 +3977,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "Kineze (Tradicionale)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "uolofisht"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "kalmikisht"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/sr/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/sr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # markomi1 <okram.je.car.4@gmail.com>, 2020.
 # Слободан Симић(Slobodan Simić) <slsimic@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Serbian <https://hosted.weblate.org/projects/weblate/"
 "languages/sr/>\n"
 "Language: sr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -818,14 +818,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "динка"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "динка"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "догри"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3826,14 +3833,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "волофски"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "кинески (поједностављени)"
@@ -3842,20 +3855,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "кинески (традиционални)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "волофски"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "калмик"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Weblate <noreply@weblate.org>, 2019.
 # Mihajlo Djordjevic <djordjevic.mihajlo@gmail.com>, 2019.
 # Слободан Симић(Slobodan Simić) <slsimic@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Serbian (latin) <https://hosted.weblate.org/projects/weblate/"
 "languages/sr_Latn/>\n"
 "Language: sr_Latn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -817,14 +817,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3825,14 +3831,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "volofski"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "kineski (pojednostavljeni)"
@@ -3841,20 +3853,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "kineski (tradicionalni)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "volofski"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "kalmik"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/sv/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/sv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Johan Jacobsson <johan.jacobsson@telia.com>, 2018, 2019, 2020, 2021, 2022, 2023.
 # Filip Bengtsson <filipbengtsson@live.se>, 2019.
 # Mattias Münster <mattiasmun@gmail.com>, 2019.
 # tygyh <jonis9898@hotmail.com>, 2022.
+# Kristoffer Grundström <swedishsailfishosuser@tutanota.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-11 13:41+0000\n"
-"Last-Translator: Johan Jacobsson <johan.jacobsson@telia.com>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-24 06:55+0000\n"
+"Last-Translator: Kristoffer Grundström <swedishsailfishosuser@tutanota.com>\n"
 "Language-Team: Swedish <https://hosted.weblate.org/projects/weblate/"
 "languages/sv/>\n"
 "Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -807,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinka"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2430,26 +2437,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Kinesiska (traditionell)"
+msgstr "Kinesiska (Min Nan, Traditionell)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Kinesiska (Minnan)"
+msgstr "Kinesiska (Min Nan, Latin)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitanska"
 
@@ -3752,32 +3755,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Westfaliska"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (förenklad)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (traditionell)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmuckiska"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/sw/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/sw/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -846,14 +846,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Kidogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3946,14 +3952,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Lugha ya Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "Kichina (Kilichorahisishwa)"
@@ -3962,20 +3974,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "Kichina cha Jadi"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Lugha ya Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kikalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ta/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ta/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Tamil <https://hosted.weblate.org/projects/weblate/languages/"
 "ta/>\n"
 "Language: ta\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -850,14 +850,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "மன்டின்கா"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "டெங்கா"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "டோக்ரி"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3958,14 +3964,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "வடக்கு பாலியன்"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ஓலோஃப்"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "எளிதாக்கப்பட்ட சீனம்"
@@ -3974,20 +3986,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "பாரம்பரிய சீனம்"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ஓலோஃப்"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "கல்மைக்"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/te/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/te/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: te\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -808,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "డింకా"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "డొగ్రి"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3786,14 +3792,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "వొలోఫ్"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "సరళీకృత చైనీస్"
@@ -3802,20 +3814,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "సాంప్రదాయక చైనీస్"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "వొలోఫ్"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "కల్మిక్"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/th/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/th/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # AefghThreenine <aefgh39622@gmail.com>, 2020, 2021.
 # ทรงพล คำผุย <songpon.ming@gmail.com>, 2022.
 # BANKUU <bankuu@gorutan.net>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-10-12 18:26+0000\n"
 "Last-Translator: BANKUU <bankuu@gorutan.net>\n"
 "Language-Team: Thai <https://hosted.weblate.org/projects/weblate/languages/"
 "th/>\n"
 "Language: th\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -808,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "ดิงกา"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "โฑครี"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3796,14 +3802,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "โวลอฟ"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "จีน (ตัวย่อ)"
@@ -3812,20 +3824,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "จีน (ตัวเต็ม)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "โวลอฟ"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "คัลมืยค์"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/tlh/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/tlh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Christine Long <lilmamachrislong33@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-01-26 17:54+0000\n"
 "Last-Translator: Christine Long <lilmamachrislong33@gmail.com>\n"
 "Language-Team: Klingon <https://hosted.weblate.org/projects/weblate/"
 "languages/tlh/>\n"
 "Language: tlh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -806,14 +806,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3746,30 +3752,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/tok/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/tok/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: tok\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3744,30 +3750,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/tr/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/tr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 # MESUT AKCAN <makcan@gmail.com>, 2018.
 # Mesut Akcan <makcan@gmail.com>, 2019.
 # Ali Demirtas <alidemirtas94@gmail.com>, 2019.
 # Oğuz Ersen <oguzersen@protonmail.com>, 2019, 2020, 2021.
 # Burak Yavuz <hitowerdigit@hotmail.com>, 2020, 2021, 2022.
 # Oğuz Ersen <oguz@ersen.moe>, 2023.
 # Kaya Zeren <kayazeren@gmail.com>, 2023.
+# Eren İnce <erenince@proton.me>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-01 03:03+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-05 03:49+0000\n"
 "Last-Translator: Kaya Zeren <kayazeren@gmail.com>\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/weblate/"
 "languages/tr/>\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afarca"
 
@@ -814,14 +815,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "Dinkaca"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "Dengka"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2441,26 +2448,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "Çince (Geleneksel)"
+msgstr "Çince (Min Nan, Geleneksel)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "Çince (Min Nan)"
+msgstr "Çince (Min Nan, Latin)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolice"
 
@@ -3766,32 +3769,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "Vestfalyaca"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "Wu (Basitleştirilmiş)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "Wu (Geleneksel)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "Kalmyk"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/tt/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/tt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: tt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -815,14 +815,21 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Дзонgхача"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3844,14 +3851,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Волофча"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "гадиләштерелгән кытай"
@@ -3860,20 +3873,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "традицион кытай"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Волофча"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Малайча"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/tzm/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/tzm/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # Weblate <noreply@weblate.org>, 2020.
 # Hakim Oubouali <hakim.oubouali.skr@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Tamazight (Central Atlas) <https://hosted.weblate.org/"
 "projects/weblate/languages/tzm/>\n"
 "Language: tzm\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -821,14 +821,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr ""
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3855,30 +3861,30 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Simplified)"
+msgid "Wolof"
 msgstr ""
 
-#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wu (Traditional)"
+msgid "Wu (Simplified)"
 msgstr ""
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Wolof"
+msgid "Wu (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr ""
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/ug/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/ug/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Abdusalam <1810010207@s.upc.edu.cn>, 2020.
 # Anonymous <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Uyghur <https://hosted.weblate.org/projects/weblate/languages/"
 "ug/>\n"
 "Language: ug\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -845,14 +845,20 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Mandinka"
 msgid "Dinka"
 msgstr "ماندىنكاچە"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "دوگرىچە"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3951,14 +3957,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ۋولوفچە"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
 msgstr "خەنزۇچە (ئاددىيلاشتۇرۇلغان)"
@@ -3967,20 +3979,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
 msgstr "خەنزۇچە (ئەنئەنىۋى)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ۋولوفچە"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "قالماقچە"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/uk/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # Ihor Hordiichuk <igor_ck@outlook.com>, 2020, 2021, 2023.
 # Tymofii Lytvynenko <till.svit@gmail.com>, 2023.
 # Skrripy <rozihrash.ya6w7@simplelogin.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-10 20:35+0000\n"
-"Last-Translator: Skrripy <rozihrash.ya6w7@simplelogin.com>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-05 03:49+0000\n"
+"Last-Translator: Ihor Hordiichuk <igor_ck@outlook.com>\n"
 "Language-Team: Ukrainian <https://hosted.weblate.org/projects/weblate/"
 "languages/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : n%10==1 && n%100!=11 ? 0 : n"
 "%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "афарська"
 
@@ -815,14 +815,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "дінка"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr "денгка"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "догрі"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2438,26 +2444,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "науатль"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "китайська (традиційна)"
+msgstr "китайська (міньнань, традиційна)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "китайська (мінь-нан)"
+msgstr "китайська (міньнань)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "неаполітанська"
 
@@ -3759,32 +3761,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "вестфальська"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "волоф"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "уська (спрощена)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "уська (традиційна)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "волоф"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "калмицька"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/uz/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/uz/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: uz\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -808,14 +808,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr ""
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3782,14 +3788,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "volof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "xitoy (soddalashgan)"
@@ -3798,20 +3810,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "xitoy (an’anaviy)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "volof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "qalmoq"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/vi/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/vi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Victor Tran <vicr12345@gmail.com>, 2019.
 # bruh <quangtrung02hn16@gmail.com>, 2021.
 # Ngô Quốc Đạt <datlechin@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: 2022-01-23 23:35+0000\n"
 "Last-Translator: Ngô Quốc Đạt <datlechin@gmail.com>\n"
 "Language-Team: Vietnamese <https://hosted.weblate.org/projects/weblate/"
 "languages/vi/>\n"
 "Language: vi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -836,14 +836,21 @@
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Dinka"
 msgstr "Tiếng Man-đin-gô"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Dengka"
+msgstr "Tiếng Đin-ca"
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "Tiếng Dogri"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3990,14 +3997,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "Tiếng Wolof"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "Tiếng Trung (Giản thể)"
@@ -4006,20 +4019,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "Tiếng Trung (Phồn thể)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "Tiếng Wolof"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Kalmyk"
 msgstr "Tiếng Oua-la-mô"
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: yue\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -804,14 +804,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "丁卡文"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "多格來文"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -3766,14 +3772,20 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "沃洛夫文"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "簡體中文"
@@ -3782,20 +3794,14 @@
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "繁體中文"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "沃洛夫文"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "卡爾梅克文"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/zgh/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/zgh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ زهير أمازيغ <zouhirdehbi56@gmail.com>, 2023.
 # ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ ZOUHIR DEHBI <zouhirdehbi56@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-10 20:35+0000\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-15 08:51+0000\n"
 "Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ ZOUHIR DEHBI <zouhirdehbi56@gmail.com>\n"
 "Language-Team: Tamazight (Standard Moroccan) <https://hosted.weblate.org/"
 "projects/weblate/languages/zgh/>\n"
 "Language: zgh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "ⵜⴰⴼⴰⵔⵉⵜ"
 
@@ -807,14 +807,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "ⵜⴰⴷⵉⵏⴽⵉⵜ"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "ⵜⴰⴷⵓⴳⵔⵉⵜ"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2430,26 +2436,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ⵜⴰⵏⴰⵀⵡⴰⵜⵍⵜ"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
 msgstr "ⵜⴰⵛⵉⵏⵡⵉⵜ (ⵜⴰⵣⴰⵢⴽⵓⵜ)"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "ⵜⴰⵛⵉⵏⵡⵉⵜ (ⵎⵉⵏ ⵏⴰⵏ)"
+msgstr "ⵜⴰⵛⵉⵏⵡⵉⵜ (ⵎⵉⵏ ⵏⴰⵏ, ⵜⴰⵍⴰⵜⵉⵏⵉⵜ)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ⵜⴰⵏⴰⴱⵓⵍⵉⵜ"
 
@@ -3751,32 +3753,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "ⵜⴰⵡⵉⵙⵜⴼⴰⵍⵉⵏⵜ"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "ⵜⴰⵡⵓⵍⵓⴼⵜ"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "ⵜⴰⵡⵓⵜ (ⵜⴰⴼⵔⴰⵔⵜ)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "ⵜⴰⵡⵓⵜ (ⵜⴰⵣⴰⵢⴽⵓⵜ)"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "ⵜⴰⵡⵓⵍⵓⴼⵜ"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "ⵜⴰⴽⴰⵍⵎⵉⴽⵜ"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 # Eric <hamburger1024@duck.com>, 2022.
 # Eric <hamburger2048@users.noreply.hosted.weblate.org>, 2023.
 # SAIHAZE <saihaze@outlook.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-01 03:03+0000\n"
-"Last-Translator: SAIHAZE <saihaze@outlook.com>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-05 03:49+0000\n"
+"Last-Translator: Eric <hamburger2048@users.noreply.hosted.weblate.org>\n"
 "Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/"
 "weblate/languages/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "阿法尔语"
 
@@ -828,14 +828,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "丁卡语"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "多格拉语"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2451,26 +2457,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "纳瓦特尔语"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "中文（繁体）"
+msgstr "中文（闽南，繁体）"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "中文（闽南语）"
+msgstr "中文（闽南，拉丁字母）"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "那不勒斯语"
 
@@ -3772,32 +3774,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "威斯特伐利亚语"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "沃洛夫语"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "吴语（简体）"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "吴语（繁体）"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "沃洛夫语"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "卡尔梅克语"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po` & `weblate-language-data-2023.5/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Chang-Chia Tseng <pswo10680@gmail.com>, 2018, 2019, 2020, 2021, 2022, 2023.
-# byStarTW <pan93412@gmail.com>, 2019, 2020, 2021, 2022.
+# byStarTW <pan93412@gmail.com>, 2019, 2020, 2021, 2022, 2023.
 # Wei-cheng Kung <wck317@pchome.com.tw>, 2019.
 # Jeff Huang <s8321414@gmail.com>, 2020, 2021.
 # louies0623 <louies0623@gmail.com>, 2021.
 # 菘菘 <rrt467778@gmail.com>, 2021.
 # 峡州仙士 <c@cjh0613.com>, 2021.
 # Lee Albert <vicedon@gmail.com>, 2021.
 # Supaplex <bejokeup@gmail.com>, 2021.
 # yangyangdaji <1504305527@qq.com>, 2022.
 # Toomore Chiang <toomore0929@gmail.com>, 2022.
 # SAIHAZE <saihaze@outlook.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-04-18 13:19+0200\n"
-"PO-Revision-Date: 2023-02-01 03:03+0000\n"
-"Last-Translator: Chang-Chia Tseng <pswo10680@gmail.com>\n"
+"POT-Creation-Date: 2023-06-14 08:55+0200\n"
+"PO-Revision-Date: 2023-05-05 03:49+0000\n"
+"Last-Translator: pan93412 <pan93412@gmail.com>\n"
 "Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
 "weblate/languages/zh_Hant/>\n"
 "Language: zh_Hant\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "阿法語"
 
@@ -817,14 +817,20 @@
 
 #. Translators: Language name for ISO code "din". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dinka"
 msgstr "丁卡語"
 
+#. Translators: Language name for ISO code "dnk". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Dengka"
+msgstr ""
+
 #. Translators: Language name for ISO code "doi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dogri"
 msgstr "多格拉語"
 
 #. Translators: Language name for ISO code "dry". The parenthesis clarifies
@@ -2440,26 +2446,22 @@
 #. or other variant.
 msgid "Nahuatl"
 msgstr "納瓦特爾語"
 
 #. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Chinese (Min Nan, Traditional)"
-msgstr "漢語（正體字）"
+msgstr "漢語（閩南語，正體字）"
 
 #. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Min Nan)"
 msgid "Chinese (Min Nan, Latin)"
-msgstr "閩南語"
+msgstr "漢語（閩南語，拉丁字）"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "那不勒斯語"
 
@@ -3761,32 +3763,32 @@
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
 msgstr "威斯特伐利亞語"
 
+#. Translators: Language name for ISO code "wo". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Wolof"
+msgstr "沃洛夫語"
+
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
 msgstr "吳語（簡體字）"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
 msgstr "吳語（正體字）"
 
-#. Translators: Language name for ISO code "wo". The parenthesis clarifies
-#. variant of the language. It could contain a region, age (Old, Middle, ...)
-#. or other variant.
-msgid "Wolof"
-msgstr "沃洛夫語"
-
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
 msgstr "卡爾梅克語"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
```

### Comparing `weblate-language-data-2023.4/weblate_language_data/plural_tags.py` & `weblate-language-data-2023.5/weblate_language_data/plural_tags.py`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/weblate_language_data/plurals.py` & `weblate-language-data-2023.5/weblate_language_data/plurals.py`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.4/weblate_language_data/population.py` & `weblate-language-data-2023.5/weblate_language_data/population.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,15 @@
     "de_AT": 8593666,
     "de_CH": 6134912,
     "de_LU": 395880,
     "del": 0,
     "den": 2299,
     "dgr": 2110,
     "din": 0,
+    "dnk": 0,
     "doi": 2652180,
     "dry": 0,
     "dsb": 6973,
     "dua": 133176,
     "dum": 0,
     "dv": 388044,
     "dyu": 6667328,
@@ -158,30 +159,30 @@
     "ee": 4690856,
     "efi": 2996391,
     "egl": 31201,
     "egy": 0,
     "eka": 0,
     "el": 12292240,
     "elx": 0,
-    "en": 1636485035,
-    "en@pirate": 1636485035,
+    "en": 1636485517,
+    "en@pirate": 1636485517,
     "en_AU": 24447840,
     "en_CA": 32416926,
     "en_GB": 64445878,
     "en_IE": 5073038,
     "en_IN": 251957100,
     "en_NZ": 4826970,
     "en_PH": 69875840,
     "en_Shaw": 0,
     "en_Shaw_GB": 0,
     "en_Shaw_US": 0,
     "en_US": 319333440,
     "en_XA": 0,
     "en_ZA": 17503716,
-    "en_devel": 1636485035,
+    "en_devel": 1636485517,
     "enm": 0,
     "eo": 301,
     "es": 493528078,
     "es@formal": 493528078,
     "es@informal": 493528078,
     "es_419": 0,
     "es_AR": 45479100,
@@ -633,17 +634,17 @@
     "wa": 679800,
     "wae": 11376,
     "wal": 1946034,
     "war": 3166927,
     "was": 0,
     "wen": 0,
     "wep": 0,
+    "wo": 11025493,
     "wuu_Hans": 83641200,
     "wuu_Hant": 83641200,
-    "wo": 11025493,
     "xal": 0,
     "xh": 10182944,
     "xog": 2292409,
     "yao": 722356,
     "yap": 6555,
     "yi": 997213,
     "yo": 28685568,
```

### Comparing `weblate-language-data-2023.4/weblate_language_data.egg-info/PKG-INFO` & `weblate-language-data-2023.5/weblate_language_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weblate-language-data
-Version: 2023.4
+Version: 2023.5
 Summary: Language definitions for Weblate
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/language-data
 Author: Michal Čihař
 Author-email: michal@weblate.org
 License: MIT
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/language-data/issues
```

### Comparing `weblate-language-data-2023.4/weblate_language_data.egg-info/SOURCES.txt` & `weblate-language-data-2023.5/weblate_language_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

