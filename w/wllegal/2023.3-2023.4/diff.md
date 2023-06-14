# Comparing `tmp/wllegal-2023.3.tar.gz` & `tmp/wllegal-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wllegal-2023.3.tar", last modified: Sun May 14 17:52:54 2023, max compression
+gzip compressed data, was "wllegal-2023.4.tar", last modified: Wed Jun 14 06:50:58 2023, max compression
```

## Comparing `wllegal-2023.3.tar` & `wllegal-2023.4.tar`

### file list

```diff
@@ -1,364 +1,364 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-14 17:52:39.000000 wllegal-2023.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-14 17:52:39.000000 wllegal-2023.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-14 17:52:54.012804 wllegal-2023.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-14 17:52:39.000000 wllegal-2023.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-14 17:52:39.000000 wllegal-2023.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-14 17:52:39.000000 wllegal-2023.3/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 17:52:39.000000 wllegal-2023.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-14 17:52:54.016804 wllegal-2023.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-14 17:52:39.000000 wllegal-2023.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.988804 wllegal-2023.3/wllegal/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.960804 wllegal-2023.3/wllegal/locale/ab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/ab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/afh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/afh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/afh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/ang/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/ang/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ang/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43956 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/ar_LY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/ar_LY/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ar_LY/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/ars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/ars/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ars/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/ast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/ast/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/az/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/az/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    22950 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/be/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/be/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    51927 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/be_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/be_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/be_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/ber/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/ber/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18400 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ber/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    24991 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/bn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18306 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/bn_BD/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/bn_BD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/bn_BD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/bo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/bo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/bo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.964804 wllegal-2023.3/wllegal/locale/br/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/br/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20023 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/br/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43210 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/ce/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/ce/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ce/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/ckb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/ckb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42004 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ckb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/crh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/crh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/crh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42245 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/cv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/cv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18372 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/cv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/cy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    27595 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    44615 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    18131 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/dv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/dv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/dv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    27108 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/en_GB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    35284 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/en_GB/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/enm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/enm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/enm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43236 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.996804 wllegal-2023.3/wllegal/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19185 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.968804 wllegal-2023.3/wllegal/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    37379 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/fil/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/fil/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    22555 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/fil/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    44543 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/fur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/fur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19070 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/fur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/fy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/fy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19085 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/fy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42571 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    44257 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18486 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    41060 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    28357 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/hy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/ia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/ia/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ia/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    41417 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/ie/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/ie/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ie/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/is/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/is/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    25297 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42632 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43398 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.972804 wllegal-2023.3/wllegal/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/kab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/kab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    28379 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/kab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/kk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/kk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    48303 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/km/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/km/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    23619 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/kmr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.000804 wllegal-2023.3/wllegal/locale/kmr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/kmr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42753 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/ksh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/ksh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ksh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/ln/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/ln/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ln/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19231 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    25393 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/lzh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/lzh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/lzh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/mk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/mk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/mk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/ml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18284 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ml/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/mr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/mr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/ms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/my/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/my/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/my/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    41606 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43330 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/oc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/oc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18150 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/oc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.976804 wllegal-2023.3/wllegal/locale/or/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/or/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/or/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/pa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/pa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18800 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/pa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/pa_PK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/pa_PK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/pa_PK/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/peo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/peo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18296 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/peo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42891 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/ps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/ps/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ps/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43310 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42558 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.004804 wllegal-2023.3/wllegal/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    35312 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    37058 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/ro_MD/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/ro_MD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ro_MD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    54338 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/sc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/sc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/sc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/si/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39512 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/skr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/skr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/skr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.980804 wllegal-2023.3/wllegal/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43534 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    22902 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/sr_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42005 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/ta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    20168 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/te/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/te/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18986 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/tlh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/tok/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/tok/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18255 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/tok/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.008804 wllegal-2023.3/wllegal/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42530 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/tt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/tt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/tt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/tzm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/tzm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/tzm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/ug/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/ug/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    52448 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/uz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/uz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/uz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/yue_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/yue_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18248 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/yue_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.984804 wllegal-2023.3/wllegal/locale/zgh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/zgh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/zgh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.988804 wllegal-2023.3/wllegal/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    38905 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.988804 wllegal-2023.3/wllegal/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    38496 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/settings_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.988804 wllegal-2023.3/wllegal/templates/legal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/templates/legal/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templates/legal/documents/contracts.html
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templates/legal/documents/privacy.html
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templates/legal/documents/summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templates/legal/documents/tos.html
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templates/security.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templates/weblate_503.html
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templates/weblate_50x.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:54.012804 wllegal-2023.3/wllegal/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/templatetags/lawlinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-14 17:52:39.000000 wllegal-2023.3/wllegal/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 17:52:53.992804 wllegal-2023.3/wllegal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-14 17:52:53.000000 wllegal-2023.3/wllegal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-14 17:52:53.000000 wllegal-2023.3/wllegal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 17:52:53.000000 wllegal-2023.3/wllegal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 17:52:53.000000 wllegal-2023.3/wllegal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-14 17:52:53.000000 wllegal-2023.3/wllegal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-14 06:50:38.000000 wllegal-2023.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-14 06:50:38.000000 wllegal-2023.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-14 06:50:58.873922 wllegal-2023.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 06:50:38.000000 wllegal-2023.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-14 06:50:38.000000 wllegal-2023.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-14 06:50:38.000000 wllegal-2023.4/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 06:50:38.000000 wllegal-2023.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-14 06:50:58.877922 wllegal-2023.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-06-14 06:50:38.000000 wllegal-2023.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.845922 wllegal-2023.4/wllegal/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/ab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/ab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/afh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/afh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/afh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/ang/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/ang/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ang/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43955 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/ar_LY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/ar_LY/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ar_LY/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/ars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/ars/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ars/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/ast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/az/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/az/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    22949 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    51926 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.817921 wllegal-2023.4/wllegal/locale/be_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/be_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    23470 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/be_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/ber/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/ber/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18399 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ber/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    24835 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/bn_BD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal/locale/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/bn_BD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/bo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/bo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/bo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/br/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/br/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/br/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43209 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/ce/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/ce/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ce/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/ckb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/ckb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42003 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ckb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/crh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/crh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/crh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42318 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/cv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/cv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/cv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19892 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    27600 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    44973 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/dv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/dv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/dv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/en_GB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/en_GB/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.821922 wllegal-2023.4/wllegal/locale/enm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/enm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/enm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20933 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/eo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43296 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.853922 wllegal-2023.4/wllegal/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    37064 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/fil/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/fil/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    22554 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/fil/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    44825 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/fur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/fur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/fur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/fy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/fy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/fy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42570 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    44531 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18485 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    40415 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    28356 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/hy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/ia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/ia/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ia/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    41544 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.825922 wllegal-2023.4/wllegal/locale/ie/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/ie/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ie/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    25296 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.857922 wllegal-2023.4/wllegal/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42738 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43550 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/kab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/kab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/kab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    48302 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    23618 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/kmr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/kmr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18417 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/kmr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42878 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/ksh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/ksh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ksh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/ln/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/ln/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ln/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    25392 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/lzh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/lzh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18106 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/lzh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/mk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/mk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/mk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/ml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ml/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/mr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    25685 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/mr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/ms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.861922 wllegal-2023.4/wllegal/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/my/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/my/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18868 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/my/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    41605 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.829922 wllegal-2023.4/wllegal/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42667 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/oc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/oc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/oc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/or/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/or/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/or/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/pa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/pa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18799 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/pa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/pa_PK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/pa_PK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18345 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/pa_PK/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/peo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/peo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18295 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/peo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43062 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/ps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/ps/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ps/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43090 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42557 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    35311 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36676 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/ro_MD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/ro_MD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ro_MD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.865922 wllegal-2023.4/wllegal/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    53924 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/sc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/sc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18150 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/sc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/si/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39511 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/skr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/skr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/skr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.833922 wllegal-2023.4/wllegal/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43533 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.837922 wllegal-2023.4/wllegal/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.837922 wllegal-2023.4/wllegal/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    21122 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/sr_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.837922 wllegal-2023.4/wllegal/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42198 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.837922 wllegal-2023.4/wllegal/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18178 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.837922 wllegal-2023.4/wllegal/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.837922 wllegal-2023.4/wllegal/locale/te/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/te/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19222 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/tok/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/tok/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/tok/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43498 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/tt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/tt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/tt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/tzm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.869922 wllegal-2023.4/wllegal/locale/tzm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/tzm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    53453 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/uz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/locale/uz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/uz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19579 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/yue_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/locale/yue_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18247 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/yue_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/zgh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/locale/zgh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18586 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/zgh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    38744 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    37918 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/settings_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.841922 wllegal-2023.4/wllegal/templates/legal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/templates/legal/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templates/legal/documents/contracts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templates/legal/documents/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templates/legal/documents/summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templates/legal/documents/tos.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templates/security.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templates/weblate_503.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templates/weblate_50x.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.873922 wllegal-2023.4/wllegal/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/templatetags/lawlinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-14 06:50:38.000000 wllegal-2023.4/wllegal/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:50:58.849922 wllegal-2023.4/wllegal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-14 06:50:58.000000 wllegal-2023.4/wllegal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-14 06:50:58.000000 wllegal-2023.4/wllegal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:50:58.000000 wllegal-2023.4/wllegal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 06:50:58.000000 wllegal-2023.4/wllegal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 06:50:58.000000 wllegal-2023.4/wllegal.egg-info/top_level.txt
```

### Comparing `wllegal-2023.3/LICENSE` & `wllegal-2023.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/PKG-INFO` & `wllegal-2023.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wllegal
-Version: 2023.3
+Version: 2023.4
 Summary: Hosted Weblate legal stuff
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/wllegal
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: GPL-3.0-or-later
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/wllegal/issues
```

### Comparing `wllegal-2023.3/README.rst` & `wllegal-2023.4/README.rst`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/pyproject.toml` & `wllegal-2023.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/setup.cfg` & `wllegal-2023.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wllegal
-version = 2023.3
+version = 2023.4
 description = Hosted Weblate legal stuff
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://weblate.org/
 author = Michal Čihař
 author_email = michal@cihar.com
 license = GPL-3.0-or-later
```

### Comparing `wllegal-2023.3/setup.py` & `wllegal-2023.4/setup.py`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/wllegal/locale/ab/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ab/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ab\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/afh/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/afh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: afh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ang/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ang/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ang\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ar/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ar/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # ButterflyOfFire <ButterflyOfFire@protonmail.com>, 2018, 2019, 2020.
 # mohammadA <mohammadAbdulhadi1@gmail.com>, 2018, 2019.
 # Omar Aglan <omar.aglan91@yahoo.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2023-04-18 06:44+0000\n"
 "Last-Translator: Meno25 <meno25mail@gmail.com>\n"
 "Language-Team: Arabic <https://hosted.weblate.org/projects/weblate/legal/ar/"
 ">\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -197,15 +197,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "كل البيانات الشخصية مخزنة في الاتحاد الأوروبي."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "الوصول إلى البيانات الشخصية"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ar_LY/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ar_LY/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ar_LY\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ars/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ars/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ars\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ast/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ast/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Xuacu Saturio <xuacusk8@gmail.com>, 2018, 2020.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-01-28 08:55+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Asturian <https://hosted.weblate.org/projects/weblate/legal/"
 "ast/>\n"
 "Language: ast\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -172,15 +172,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Reset repository"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Reaniciar el depósitu"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/az/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/az/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-11-07 19:02+0000\n"
 "Last-Translator: Ariz Mirzəzadə <by.ariz@bk.ru>\n"
 "Language-Team: Azerbaijani <https://hosted.weblate.org/projects/weblate/"
 "legal/az/>\n"
 "Language: az\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -188,15 +188,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Bütün Şəxsi Məlumatlar Avropa Birliyində saxlanılır."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Şəxsi məlumatlara giriş"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/be/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/be/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # anonymous <noreply@weblate.org>, 2019.
 # Zmicer Turok <nashtlumach@gmail.com>, 2019, 2020.
 # Alex Ky <esthomolupus@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-10-17 00:57+0000\n"
 "Last-Translator: Viktar Vauchkevich <victorenator@gmail.com>\n"
 "Language-Team: Belarusian <https://hosted.weblate.org/projects/weblate/legal/"
 "be/>\n"
 "Language: be\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -197,15 +197,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Усе асабістыя даныя захоўваюцца на тэрыторыі Еўрапейскага Звязу."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Доступ да асабістых даных"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/be_Latn/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/be_Latn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Automatically generated, 2014.
 # Viktar Vauchkevich <victorenator@gmail.com>, 2018.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-01-28 08:55+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Belarusian (latin) <https://hosted.weblate.org/projects/"
 "weblate/legal/be_Latn/>\n"
 "Language: be@latin\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -190,15 +190,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access the internal repository"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Dostup da ŭnutranaha repazitoryja"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ber/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ber/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2023-01-17 20:50+0000\n"
 "Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ زهير أمازيغ <zouhirdehbi56@gmail.com>\n"
 "Language-Team: Berber <https://hosted.weblate.org/projects/weblate/legal/ber/"
 ">\n"
 "Language: ber\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -162,15 +162,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/bg/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/bg/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,43 +2,44 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-10-27 06:43+0000\n"
-"Last-Translator: 109247019824 <stoyan@gmx.com>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-15 13:29+0000\n"
+"Last-Translator: Любомир Василев <lyubomirv@gmx.com>\n"
 "Language-Team: Bulgarian <https://hosted.weblate.org/projects/weblate/legal/"
 "bg/>\n"
 "Language: bg\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Подизпълнители на основание чл. 28 от ОРОЗД (GDPR)"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Състояние към октомври 2020 г."
+msgstr "Състояние към март 2023 г."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
+"Ние се съобразяваме с регламент № %(law_679_2016)s – Общият регламент "
+"относно защитата на данните (ОРЗД), също познат като GDPR. Този документ "
+"съдържа всички необходими спецификации."
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
 msgstr "Администратор на лични данни"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
@@ -57,34 +58,31 @@
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
 msgstr "Лични данни, обработвани от Weblate"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
-"Weblate обработва лични данните данни, които потребителят предоставя при "
+"Weblate обработва само онези лични данни, които потребителят предоставя при "
 "използване на услугата:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Име и е-поща"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
 msgstr ""
-"Това е нужна, за да се виждат данните Ви в подаванията в системата за "
-"контрол на версиите"
+"Те се използват, за да се виждат данните Ви в подаванията в системата за "
+"контрол на версиите."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "Освен това, е-пощата се използва за известия от наблюдаваните събития"
+msgstr ""
+"Освен това, е-пощата се използва и за известия относно наблюдаваните събития."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Отпечатък от паролата"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -95,28 +93,25 @@
 msgstr "Паролите се съхраняват хеширани с Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP адрес и име на браузъра"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Това се съхранява в случай, че има важни промени по акаунта Ви (напр. "
 "промяна на паролата), за да може да се направи анализ в случай, че акаунтът "
-"Ви бъде откраднат"
+"Ви бъде откраднат."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Дани за фактуриране"
+msgstr "Данни за фактуриране"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
 
@@ -178,17 +173,17 @@
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Достъп до личните данни"
+#| msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
+msgstr "Разкриване на личните данни"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
@@ -269,35 +264,27 @@
 #: wllegal/templates/legal/documents/privacy.html:93
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
 "Ние съхраняваме лични данни (напр. адреса на е-пощата Ви). Те ще бъдат "
-"изтрити от нашата база данни, когато изтриете акаунта си."
+"изтрити от нашата база данни, ако изтриете акаунта си."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
-"Преводите Ви са защитени от лиценз, който е определени от всеки проект за "
+"Към преводите Ви се прилага лиценз, който е определен от всеки проект за "
 "превод."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
```

### Comparing `wllegal-2023.3/wllegal/locale/bn/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/bn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-07-13 16:14+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Bengali <https://hosted.weblate.org/projects/weblate/legal/bn/"
 ">\n"
 "Language: bn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/bn_BD/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/bn_BD/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2018.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: bn_BD\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/bo/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/bo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: bo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/br/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/br/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2018-01-30 18:47+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Breton <https://hosted.weblate.org/projects/weblate/master/br/"
 ">\n"
 "Language: br\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -176,15 +176,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Git repository"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Kavlec'h Git"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ca/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ca/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Joan Montané <joan@montane.cat>, 2018, 2019.
 # Eduard Ereza Martínez <eduard@ereza.cat>, 2019.
 # Adolfo Jayme Barrientos <fitojb@ubuntu.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-02-13 15:58+0000\n"
 "Last-Translator: Eduard Ereza Martínez <eduard@ereza.cat>\n"
 "Language-Team: Catalan <https://hosted.weblate.org/projects/weblate/legal/ca/"
 ">\n"
 "Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -206,15 +206,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Totes les dades personals s'emmagatzemen a la Unió Europea."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Accés a les dades personals"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ce/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ce/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ce\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ckb/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ckb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-06-20 06:46+0000\n"
 "Last-Translator: Kurd As <kurd68587@gmail.com>\n"
 "Language-Team: Kurdish (Central) <https://hosted.weblate.org/projects/"
 "weblate/legal/ckb/>\n"
 "Language: ckb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -194,15 +194,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "هەموو داتا کەسیەکان خەزن کراون لە یەکێتی ئەوروپا."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "دەستگەیشتن بە داتا کەسییەکان"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/crh/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/django.pot`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Weblate <noreply@weblate.org>, 2020.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: crh\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -156,15 +158,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/cs/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2012, 2018, 2019.
 # Pavel Borecki <pavel.borecki@gmail.com>, 2018, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-03-09 22:56+0000\n"
-"Last-Translator: Petr Branberger <petr@webrun.cz>\n"
-"Language-Team: Czech <https://hosted.weblate.org/projects/weblate/legal/cs/"
-">\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-20 18:47+0000\n"
+"Last-Translator: Michal Čihař <michal@weblate.org>\n"
+"Language-Team: Czech <https://hosted.weblate.org/projects/weblate/legal/cs/>"
+"\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subdodavatelé v souladu s článkem 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Stav k říjnu 2020."
+msgstr "Stav k březnu 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -68,24 +66,20 @@
 "naší služby:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Jméno a e-mailová adresa"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Tyto slouží pro identifikaci zápisů v systému správy verzí"
+msgstr "Tyto slouží pro identifikaci zápisů v systému správy verzí."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "E-mail dále slouží pro upozorňování na uživatelem sledované události"
+msgstr "E-mail dále slouží pro upozorňování na uživatelem sledované události."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Otisk (hash) hesla"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -96,36 +90,32 @@
 msgstr "Hesla jsou uložena ve formě otisku pomocí Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP adresa a název webového prohlížeče"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Tyto jsou zaznamenány v případě zásadních změn ve vašem účtu (např. při "
-"změně hesla) z důvodu diagnostiky v případě krádeže vašeho účtu"
+"změně hesla) z důvodu diagnostiky v případě krádeže vašeho účtu."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Fakturační údaje"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Údaje nezbytné k vystavení faktury jsou shromažďovány při nákupu služby od "
+"nás."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Důvod a zákonný rámec zpracování Osobních Údajů"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -188,58 +178,61 @@
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 "Osoby, které pro nás zajišťují technický provoz a zabezpečení našich služeb."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Zpracovatelé plateb při nákupu služby od nás."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Všechna Osobní Údaje jsou uloženy v Evropské Unii."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Přístup k Osobním Údajům"
+msgid "Disclosure of the Personal Data"
+msgstr "Zpřístupnění Osobních Údajů"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Osobní Údaje mohou být zpřístupněny třetím stranám za omezených okolností, "
+"pokud se Správce v dobré víře domnívá, že to vyžaduje zákon, například na "
+"základě soudního předvolání nebo jiného soudního či správního příkazu."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"V případě, že je Správce ze zákona povinen Osobní Údaje zpřístupnit, pokusí "
+"se Uživatele předem informovat e-mailem (pokud to není Správci zakázáno nebo "
+"by to bylo zbytečné) o tom, že byla podána žádost o Osobní Údaje, aby mohl "
+"Uživatel vznést námitku proti zpřístupnění. Pokud Uživatel žádost o "
+"zpřístupnění neodmítne, může být Správce ze zákona povinen Osobní údaje "
+"předat."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "Doba uložení Osobních Údajů"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr "Osobní Údaje jsou uloženy ve Službě dokud uživatel nesmaže svůj účet."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Informace o přístupu mohou být uchovávána déle za účelem zjištění, výkonu "
 "nebo obrany právních nároků."
 
@@ -306,30 +299,22 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "Odstranění, opravu a získání vašich Osobních Údajů lze provést ze správy "
 "účtu a je plně automatizované."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Zpracováváme soukromé údaje (např. e-mailovou adresu), tyto údaje odstraníme "
-"z naší databáze, jakmile odstraníte svůj účet."
+"Zpracováváme osobní údaje (např. e-mailovou adresu); tyto údaje odstraníme z "
+"naší databáze, jakmile odstraníte svůj účet."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "Vaše překlady budou šířeny na základě licence, která je uvedena u každého "
 "překladu."
 
@@ -342,22 +327,24 @@
 "napořád."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Zvolené jméno je na vás a e-mailovou adresu použitou pro odevzdání může "
+"systém Weblate maskovat, aby chránil vaše soukromí."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Používáme cookie k poskytování našich služeb."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Nepoužíváme žádné soubory cookie třetích stran."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Zobrazit anglickou verzi"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -637,14 +624,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"Ve smyslu <a href=\"%(url)s\">článku 7</a> GDPR Uživatel tímto uděluje "
+"souhlas se shromažďováním, uchováváním a zpracováním osobních údajů podle <a "
+"href=\"%(privacy_url)s\">Zásad ochrany osobních údajů</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Překlady"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -675,26 +665,21 @@
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "Přispěním do Projektu Uživatel souhlasí s licencí, kterou Projekt určil."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"Uživatel souhlasí s použitím svého jména a e-mailu jako autora v zápisech "
-"VCS. Uživatel chápe, že tento souhlas je kvůli povaze VCS neodvolatelný."
+"Uživatel souhlasí s použitím jména a e-mailu jako autora v zápisech VCS. "
+"Uživatel chápe, že tento souhlas je kvůli povaze VCS neodvolatelný."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -730,23 +715,19 @@
 "příslušností."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Účinek"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-"Tyto Všeobecné Smluvní Podmínky nabývají platnosti a účinnosti dne 1.září "
-"2017."
+"Tyto Všeobecné Smluvní Podmínky nabývají platnosti a účinnosti dne 15. "
+"května 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "V případě, že od nás zakoupíte službu, budou dále uchovávány údaje nutné "
 #~ "k vystavení faktur"
```

### Comparing `wllegal-2023.3/wllegal/locale/cv/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/cv/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2020-07-08 09:41+0000\n"
 "Last-Translator: İlle <derasetad@gmail.com>\n"
 "Language-Team: Chuvash <https://hosted.weblate.org/projects/weblate/legal/cv/"
 ">\n"
 "Language: cv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/cy/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/cy/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Weblate <noreply@weblate.org>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 # Rhoslyn Prys <rprys@posteo.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2023-04-23 20:04+0000\n"
 "Last-Translator: dreigiau <sterilgrimed23@gmail.com>\n"
 "Language-Team: Welsh <https://hosted.weblate.org/projects/weblate/legal/cy/"
 ">\n"
 "Language: cy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -183,15 +183,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Mynediad i'r Data Personol"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/da/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/da/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # scootergrisen, 2018.
 # scootergrisen <scootergrisen@gmail.com>, 2018, 2019, 2020.
 # Allan Nordhøy <epost@anotheragency.no>, 2018.
 # anonymous <noreply@weblate.org>, 2019.
 # Henrik Dankvardt <dankvardt@gmail.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-05-20 08:34+0000\n"
-"Last-Translator: Aputsiak Niels Janussen <aj@isit.gl>\n"
-"Language-Team: Danish <https://hosted.weblate.org/projects/weblate/legal/da/"
-">\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-31 21:51+0000\n"
+"Last-Translator: Michael Millet <mikevlet@protonmail.com>\n"
+"Language-Team: Danish <https://hosted.weblate.org/projects/weblate/legal/da/>"
+"\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.7-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Underleverandører i henhold til artikel 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 #, fuzzy
@@ -201,15 +201,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Alle personlige data er lagret i den Europæiske Union."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Adgang til den personlige data"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -356,23 +356,23 @@
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
-msgstr "Se engelsk version"
+msgstr "Vis engelsk udgave"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"Servicevilkår er autoritativt på engelsk, oversættelser leveres for at gøre "
-"det lettere for dig."
+"Dokumentet Tjenestevilkår er autoritativt på engelsk, oversættelser leveres "
+"for din bekvemmelighed."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 "Brugerens og udbyderens rettigheder og forpligtelser som følge af brugen af "
@@ -470,15 +470,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr "betyder %(provider)s, Reg. nr. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Personlige data"
+msgstr "Personlige Data"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.3/wllegal/locale/de/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/de/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -8,37 +8,35 @@
 # Krombel <krombel@krombel.de>, 2018.
 # István Koren <istvank@gmx.de>, 2018.
 # nautilusx <mail.ka@mailbox.org>, 2019, 2020.
 # Swann Martinet <swann.ranskassa@laposte.net>, 2019.
 # iLocIT! <matthiasc@ilocit.de>, 2019, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-05-11 05:51+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-20 18:47+0000\n"
 "Last-Translator: VfBFan <drop0815@posteo.de>\n"
-"Language-Team: German <https://hosted.weblate.org/projects/weblate/legal/de/"
-">\n"
+"Language-Team: German <https://hosted.weblate.org/projects/weblate/legal/de/>"
+"\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Unterauftragsverarbeiter nach Art. 28 DSGVO"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Stand: Oktober 2020."
+msgstr "Stand: März 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -76,26 +74,22 @@
 "Verwendung des Dienstes zur Verfügung stellt:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Benutzername und E-Mail-Adresse"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Beide werden zur Identifikation bei den VCS-Commits genutzt"
+msgstr "Beide werden zur Identifikation bei den VCS-Commits genutzt."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
 "E-Mail wird zusätzlich zu Benachrichtigungen über beobachtete Ereignisse "
-"verwendet"
+"verwendet."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Kennwort in Hash-Form"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -107,37 +101,33 @@
 msgstr "Passwörter werden mit Argon2 gehasht gespeichert."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP-Adresse und Browser-Name"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Sie werden für den Fall wichtiger Veränderungen an Ihrem Konto (z. B. "
 "Passwortänderungen) aufgezeichnet, um feststellen zu können, ob Ihr Konto "
-"gekapert wurde"
+"gekapert wurde."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Rechnungsinformationen"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Die für die Ausstellung einer Rechnung erforderlichen Daten werden erhoben, "
+"wenn Sie eine Dienstleistung bei uns erwerben."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Zweck und Rechtsgrundlage der Verarbeitung personenbezogener Daten"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -203,61 +193,68 @@
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 "Personen, die mit der technischen Sicherstellung des Dienstes beauftragt "
 "sind."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Zahlungsabwickler beim Kauf einer Dienstleistung von uns."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 "Alle personenbezogenen Daten werden in der Europäischen Union gespeichert."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Zugriff auf die persönlichen Daten"
+msgid "Disclosure of the Personal Data"
+msgstr "Offenlegung der personenbezogenen Daten"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Die personenbezogenen Daten können in begrenztem Umfang an Dritte "
+"weitergegeben werden, wenn der für die Verarbeitung Verantwortliche in gutem "
+"Glauben davon ausgeht, dass dies gesetzlich vorgeschrieben ist, z. B. "
+"aufgrund einer Vorladung oder einer anderen gerichtlichen oder behördlichen "
+"Anordnung."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Falls der für die Verarbeitung Verantwortliche gesetzlich zur Weitergabe der "
+"personenbezogenen Daten verpflichtet ist, wird versucht, den Nutzer vorab "
+"per E-Mail darüber zu informieren (es sei denn, dies ist dem für die "
+"Verarbeitung Verantwortlichen untersagt oder wäre aussichtslos), dass ein "
+"Antrag auf Weitergabe der personenbezogenen Daten gestellt wurde, damit der "
+"Nutzer der Weitergabe widersprechen kann. Widerspricht der Nutzer dem Antrag "
+"auf Weitergabe nicht, kann der für die Verarbeitung Verantwortliche "
+"gesetzlich verpflichtet sein, die personenbezogenen Daten herauszugeben."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "Aufbewahrung personenbezogener Daten"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Die personenbezogenen Daten werden im Dienst gespeichert, bis der Benutzer "
 "sein Konto für diesen Dienst löscht."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Zugriffsprotokollinformationen können für einen längeren Zeitraum zum Zwecke "
 "der Begründung, Ausübung oder Verteidigung von Rechtsansprüchen erhoben "
 "werden."
@@ -327,31 +324,22 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "Das Entfernen, Korrigieren und Abrufen Ihrer persönlichen Daten kann über "
 "die Kontoverwaltung erfolgen und ist vollständig automatisiert."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Wir verarbeiten private Daten (wie beispielsweise Ihre E-Mail-Adresse). "
-"Diese Daten werden jedoch aus unserer Datenbank entfernt, sobald Sie Ihr "
-"Benutzerkonto löschen."
+"Wir verarbeiten personenbezogene Daten (z. B. Ihre E-Mail-Adresse); diese "
+"werden aus unserer Datenbank gelöscht, wenn Sie Ihr Konto löschen."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "Die von Ihnen angefertigten Übersetzungen werden unter der Lizenz "
 "veröffentlicht, die für das jeweilige Übersetzungsprojekt spezifiziert ist."
 
@@ -364,22 +352,25 @@
 "Versionsverwaltung (VCS) verwendet und bleiben dort für immer gespeichert."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Der gewählte Name liegt bei Ihnen und die E-Mail-Adresse, die für Commits "
+"verwendet wird, kann vom Weblate-System maskiert werden, um Ihre "
+"Privatsphäre zu schützen."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Wir verwenden Cookies, um unsere Dienste bereitzustellen."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Wir verwenden keine Cookies von Drittanbietern."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Englische Version anzeigen"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -400,15 +391,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:20
 msgid "Definitions"
 msgstr "Definitionen"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr "In diesen Service-Bedingungen:"
+msgstr "In diesen Nutzungsbedingungen:"
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
 msgstr "Vereinbarung"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
@@ -458,15 +449,15 @@
 "meint jede Datendatei, die vom Webserver des Dienstes an den Computer des "
 "Benutzers oder ein anderes mit dem Internet verbundenes Geräts gesendet "
 "wird, die es ermöglicht, eine eindeutige Identifizierung des Webbrowsers des "
 "Benutzers zu erhalten"
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
-msgstr "GDPR"
+msgstr "DSGVO"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
@@ -616,17 +607,17 @@
 
 #: wllegal/templates/legal/documents/tos.html:84
 msgid ""
 "The User agrees to use the Service only in a manner not jeopardizing "
 "technical software and/or hardware means of the Provider and/or such means "
 "in the Provider’s use."
 msgstr ""
-"Der Nutzer verpflichtet sich, den Service nur in einer Weise zu nutzen, die "
-"die technischen Soft- und/oder Hardwaremittel des Anbieters und/oder solche "
-"Mittel bei der Nutzung durch den Anbieter nicht gefährdet."
+"Der Nutzer verpflichtet sich, den Service nur in einer Weise zu nutzen, "
+"welche die technischen Soft- und/oder Hardwaremittel des Anbieters und/oder "
+"solche Mittel bei der Nutzung durch den Anbieter nicht gefährdet."
 
 #: wllegal/templates/legal/documents/tos.html:86
 msgid ""
 "The User agrees to refrain from use of the Service in bad faith and/or "
 "deliberately causing any damage to the Service."
 msgstr ""
 "Der Nutzer verpflichtet sich, die Nutzung des Dienstes in böswilliger "
@@ -670,14 +661,18 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"Im Sinne von <a href=\"%(url)s\">Artikel 7</a> der DSGVO erteilt der Nutzer "
+"hiermit seine Zustimmung zur Erhebung, Speicherung und Verarbeitung der "
+"personenbezogenen Daten gemäß der <a href=\"%(privacy_url)s"
+"\">Datenschutzerklärung</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Übersetzungen"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -712,28 +707,23 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "Der Benutzer stimmt durch seine Mitarbeit an einem Projekt automatisch der "
 "Lizenz, die für Projektbeiträge im Projekt festgelegt ist, zu."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"Der Benutzer willigt in die Verwendung seines eigenen Namens und seiner E-"
-"Mail-Adresse als Urheber in VCS-Commits ein. Der Benutzer nimmt zur "
-"Kenntnis, dass diese Einwilligung aufgrund der Beschaffenheit des VCS "
-"unwiderruflich ist."
+"Der Nutzer erklärt sich damit einverstanden, dass Name und E-Mail-Adresse "
+"als Urheberschaft in den VCS-Commits verwendet werden. Der Nutzer nimmt zur "
+"Kenntnis, dass diese Gewährung aufgrund der Art des VCS nicht widerruflich "
+"ist."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -769,21 +759,17 @@
 "Republik mit materieller und örtlicher Zuständigkeit entschieden."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Effekt"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "Diese Nutzungsbedingungen treten am 1. September 2017 in Kraft."
+msgstr "Diese Nutzungsbedingungen treten am 15. Mai 2023 in Kraft."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "Wenn Sie eine Dienstleistung von uns erwerben, erfassen wir zusätzliche "
 #~ "Rechnungsinformationen, die für die Ausstellung einer Rechnung "
```

### Comparing `wllegal-2023.3/wllegal/locale/django.pot` & `wllegal-2023.4/wllegal/locale/sw/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"Language: sw\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -158,15 +159,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/dv/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/enm/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: dv\n"
+"Language: enm\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/el/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/el/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # THANOS SIOURDAKIS <siourdakisthanos@gmail.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-12-16 08:54+0000\n"
 "Last-Translator: george kitsoukakis <norhorn@gmail.com>\n"
 "Language-Team: Greek <https://hosted.weblate.org/projects/weblate/legal/el/"
 ">\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -180,15 +180,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Όλα τα Προσωπικά Δεδομένα αποθηκεύονται στην Ευρωπαϊκή Ένωση."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Πρόσβαση στα Προσωπικά Δεδομένα"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/en_GB/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/en_GB/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Robert Readman <robert_readman@hotmail.com>, 2018.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-04-02 13:34+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-31 21:51+0000\n"
 "Last-Translator: Andi Chandler <andi@gowling.com>\n"
 "Language-Team: English (United Kingdom) <https://hosted.weblate.org/projects/"
 "weblate/legal/en_GB/>\n"
 "Language: en_GB\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.17-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subcontractors in accordance with Art. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Status as of October 2020."
+msgstr "Status as of March 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -67,24 +65,20 @@
 msgstr "Weblate only processes Personal Data the User provides by using it:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Name and e-mail address"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "These are used to identify you in the VCS commits"
+msgstr "These are used to identify you in the VCS commits."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "Additionally, e-mail is used for notification of watched events"
+msgstr "Additionally, e-mail is used for notification of watched events."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Password in hashed form"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -95,36 +89,32 @@
 msgstr "Passwords are stored hashed using Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP address and browser name"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "These are logged in case of important changes to your account (e.g. password "
-"change) to allow diagnosis in case your account is stolen"
+"change) to allow diagnosis in case your account is stolen."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Billing information"
+msgstr "Billing info"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Necessary details to issue an invoice is collected when purchasing a service "
+"from us."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Purpose and legal basis of processing Personal Data"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -185,66 +175,69 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Persons which are contracted for technical assurance of the service."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Payment processors when purchasing a service from us."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "All Personal Data is stored in the European Union."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Access to the Personal Data"
+msgid "Disclosure of the Personal Data"
+msgstr "Disclosure of the Personal Data"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"The Personal Data might be disclosed to third parties in limited "
+"circumstances when the Controller has a good faith belief it is required by "
+"law, such as under a subpoena or other judicial or administrative order."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"In case the Controller is required by law to disclose the Personal Data, an "
+"attempt will be made to provide the User with prior notice by e-mail (unless "
+"the Controller is prohibited, or it would be futile) that a request for the "
+"Personal Data has been made to allow the User to object to the disclosure. "
+"If the User does not challenge the disclosure request, the Controller may be "
+"legally required to turn over the Personal Data."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "The Personal Data retention"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"Access log information might be collected for a longer period for the "
-"purpose of establishing, exercising or defending legal claims."
+"Access log info might be collected for a longer period for the purpose of "
+"establishing, exercising or defending legal claims."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "Your rights"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
@@ -304,35 +297,27 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"We process private data (such as your e-mail address), those will be "
-"discarded from our database as soon as you remove your account."
+"We process personal data (such as your e-mail address); those will be "
+"discarded from our database if you remove your account."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
-"Your translations are made under license which is specified by each "
+"Your translations are made under the licence which is specified by each "
 "translation."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
@@ -340,22 +325,24 @@
 "indefinitely."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Chosen name is up to you and the e-mail address used for commits can be "
+"masked by Weblate system to protect your privacy."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "We use cookies to deliver our services."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "We don’t use any third-party cookies."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "View English version"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -633,14 +620,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
+"hereby gives consent to collecting, storage, and processing of the Personal "
+"Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Translations"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -673,27 +663,22 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "The User agrees, upon contributing to a Project, to the licence the Project "
 "has specified."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"The User agrees to use of own name and e-mail as authorship in the VCS "
-"commits. The User understands that this grant is non revocable due to nature "
-"of the VCS."
+"The User agrees to use of name and e-mail as authorship in the VCS commits. "
+"The User understands that this grant is non-revocable due to the nature of "
+"the VCS."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -729,23 +714,18 @@
 "substantive and local jurisdiction."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Effect"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-"These Terms of Service shall come into force and effect on 1st September "
-"2017."
+"These Terms of Service shall come into force and effect on 15th May 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
```

### Comparing `wllegal-2023.3/wllegal/locale/enm/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/lzh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: enm\n"
+"Language: lzh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/eo/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/eo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Michal Čihař <michal@cihar.com>, 2019.
 # Pierre Soubourou <pierre.soubourou@gmail.com>, 2019.
 # tuxayo/Victor Grousset <victor@tuxayo.net>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2019-08-18 06:22+0000\n"
 "Last-Translator: tuxayo/Victor Grousset <victor@tuxayo.net>\n"
 "Language-Team: Esperanto <https://hosted.weblate.org/projects/weblate/hosted/"
 "eo/>\n"
 "Language: eo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -173,15 +173,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/es/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,35 @@
 # Laura Arjona Reina <larjona@larjona.net>, 2018.
 # Franco <francobenedetti.59+github1@gmail.com>, 2018, 2019.
 # Adalberto Alvarez Perez <adalprofe@gmail.com>, 2018.
 # emma peel <emma.peel@riseup.net>, 2018.
 # Adolfo Jayme Barrientos <fitojb@ubuntu.com>, 2019, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-02-16 17:55+0000\n"
-"Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-22 13:52+0000\n"
+"Last-Translator: Juan Benites <benitesjn@gmail.com>\n"
 "Language-Team: Spanish <https://hosted.weblate.org/projects/weblate/legal/es/"
 ">\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subcontratistas de acuerdo al art. 28 del RGPD"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Estado a partir de octubre de 2020."
+msgstr "Estado en marzo de 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -72,26 +70,22 @@
 "al utilizarlo:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Nombre y dirección de correo"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Estos se utilizan para identificarle en las consignas de VCS"
+msgstr "Se utilizan para identificarte en los commits del VCS."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"Además, el correo electrónico se utiliza para la notificación de sucesos "
-"monitorizados"
+"Además, se utiliza el correo electrónico para notificar los eventos "
+"vigilados."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Contraseña en forma de resumen criptográfico"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -102,37 +96,33 @@
 msgstr "Las contraseñas se almacenan transformadas con la función Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "Dirección IP y nombre del navegador"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Estos se registran en caso de cambios importantes en su cuenta (por ejemplo, "
-"cambio de contraseña) para permitir el diagnóstico en caso de que su cuenta "
-"sea robada"
+"Se registran en caso de cambios importantes en tu cuenta (por ejemplo, "
+"cambio de contraseña) para permitir el diagnóstico en caso de robo de tu "
+"cuenta."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Datos de facturación"
+msgstr "Información sobre la facturación"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Los datos necesarios para emitir una factura se recopilan al comprarnos un "
+"servicio."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Propósito y marco jurídico para el procesamiento de datos personales"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -195,66 +185,71 @@
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 "Personas que son contratadas para el aseguramiento técnico del servicio."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Procesadores de pago al comprar un servicio nuestro."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Todos los datos personales se almacenan en la Unión Europea."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Acceso a los datos personales"
+msgid "Disclosure of the Personal Data"
+msgstr "Divulgación de los datos personales"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Los Datos Personales podrían revelarse a terceros en circunstancias "
+"limitadas cuando el Responsable del Tratamiento crea de buena fe que así lo "
+"exige la ley, como en virtud de una citación u otra orden judicial o "
+"administrativa."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"En caso de que el Responsable del tratamiento esté obligado por ley a "
+"revelar los Datos personales, se intentará notificar previamente al Usuario "
+"por correo electrónico (a menos que el Responsable del tratamiento lo tenga "
+"prohibido o sea inútil) que se ha solicitado la entrega de los Datos "
+"personales para que el Usuario pueda oponerse a la revelación. Si el usuario "
+"no se opone a la solicitud de divulgación, el responsable del tratamiento "
+"puede verse obligado legalmente a entregar los datos personales."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "La conservación de datos personales"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Los datos personales se almacenan en el servicio hasta que el usuario "
 "elimina su cuenta del servicio."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"La información de los accesos a la cuenta serán almacenados por más tiempo "
-"con el objetivo de establecer, ejercer o defender demandas judiciales."
+"La información del registro de acceso podría recopilarse durante un período "
+"más largo con el fin de establecer, ejercer o defender reclamaciones legales."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "Sus derechos"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
@@ -315,59 +310,53 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "La eliminación, corrección y recuperación de sus Datos Personales puede "
 "hacerse desde la gestión de la cuenta, y está totalmente automatizada."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Procesamos datos privados (como, por ejemplo, su dirección de correo "
-"electrónico); estos se descartarán de nuestra base de datos cuando elimine "
-"su cuenta."
+"Tratamos datos personales (como tu dirección de correo electrónico), que "
+"serán eliminados de nuestra base de datos si eliminas tu cuenta."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
-"Sus traducciones se realizan en virtud de la licencia que se especifica en "
-"cada proyecto de traducción."
+"Tus traducciones se realizan bajo la licencia que se especifica en cada "
+"traducción."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 "Su nombre y dirección de correo electrónico se utilizan en las consignas de "
 "los sistemas de control de versiones, y permanecerán allí indefinidamente."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"El nombre elegido depende de ti y la dirección de correo electrónico "
+"utilizada para los comentarios puede ser enmascarada por el sistema de "
+"Weblate para proteger tu privacidad."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Utilizamos cookies para ofrecer nuestros servicios."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "No utilizamos cookies de terceros."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Ver la versión en inglés"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -653,14 +642,18 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"En el sentido del <a href=\"%(url)s\">Artículo 7</a> del RGPD, el Usuario da "
+"su consentimiento para la recogida, almacenamiento y tratamiento de los "
+"Datos Personales de acuerdo con la <a href=\"%(privacy_url)s\">Política de "
+"Privacidad</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Traducciones"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -694,28 +687,22 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "El Usuario acepta, al contribuir a un proyecto, la licencia que tal proyecto "
 "ha especificado."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"El Usuario acepta el uso de su nombre y dirección de correo como autoría en "
-"las consignas en los sistemas de control de versiones (VCS, por sus siglas "
-"en inglés). El usuario entiende que esta aceptación no es revocable por la "
-"naturaleza de los VCS."
+"El Usuario acepta el uso de su nombre y correo electrónico como autor en los "
+"commits del VCS. El Usuario entiende que esta concesión no es revocable "
+"debido a la naturaleza del VCS."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -751,22 +738,18 @@
 "jurisdicción sustantiva y local."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Vigencia"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-"Estos Términos de Servicio entrarán en vigor el 1 de septiembre de 2017."
+"Las presentes Condiciones Generales entrarán en vigor el 15 de mayo de 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "En caso comprar un servicio, recopilamos la información de facturación "
 #~ "adicional necesaria para emitir una factura"
```

### Comparing `wllegal-2023.3/wllegal/locale/et/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/et/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Michal Čihař <michal@cihar.com>, 2019.
 # Janar Leas <janar.leas@gmail.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2023-03-10 11:02+0000\n"
 "Last-Translator: Priit Jõerüüt <hwlate@joeruut.com>\n"
 "Language-Team: Estonian <https://hosted.weblate.org/projects/weblate/legal/"
 "et/>\n"
 "Language: et\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -190,15 +190,15 @@
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 "Kõik isiklikud andmed on salvestatud Euroopa Lidus asuvatel andmekandjatel."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Ligipääs isiklikele andmetele"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/eu/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/eu/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Michal Čihař <michal@cihar.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 # S <sendoasojo@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2020-04-08 03:31+0000\n"
 "Last-Translator: BiziA <adrianpena.hf@gmail.com>\n"
 "Language-Team: Basque <https://hosted.weblate.org/projects/weblate/legal/eu/"
 ">\n"
 "Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -166,15 +166,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/fa/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/fa/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-07-08 17:16+0000\n"
 "Last-Translator: CodeWriter21 <codewriter21@gmail.com>\n"
 "Language-Team: Persian <https://hosted.weblate.org/projects/weblate/legal/fa/"
 ">\n"
 "Language: fa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -161,15 +161,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/fi/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/fi/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,35 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Nikolay Korotkiy <sikmir@gmail.com>, 2019.
 # Jiri Grönroos <jiri.gronroos@iki.fi>, 2019.
 # Tuomas Hietala <tuomas.hietala@iki.fi>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-06-01 21:18+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-24 06:55+0000\n"
 "Last-Translator: Jiri Nakola <github@nakola.fi>\n"
 "Language-Team: Finnish <https://hosted.weblate.org/projects/weblate/legal/fi/"
 ">\n"
 "Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.13-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "Alihankkijat Art. 28 GDPR :n mukaisesti"
+msgstr "Alihankkijat artiklan mukaisesti. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Tilanne lokakuussa 2020."
+msgstr "Tilanne maaliskuussa 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -69,24 +67,20 @@
 "sitä:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Nimi ja sähköpostiosoite"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Näitä käytetään tunnistamaan sinut VCS-sitoumuksissa"
+msgstr "Näitä käytetään tunnistamaan sinut VCS-sitoumuksissa."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "Lisäksi sähköpostilla tiedotetaan katsotuista tapahtumista"
+msgstr "Lisäksi sähköpostilla tiedotetaan katsotuista tapahtumista."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Salasana tiivistetyssä muodossa"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -97,36 +91,31 @@
 msgstr "Salasanat tallennetaan tiivistettynä Argon2:lla."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP-osoite ja selaimen nimi"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Ne kirjataan, jos tiliisi tehdään tärkeitä muutoksia (esim. salasanan "
-"vaihto), jotta voidaan tehdä diagnoosi, jos tilisi varastetaan"
+"Ne kirjataan, jos tiliisi tehdään tärkeitä muutoksia (esim. salasanan vaihto)"
+", jotta voidaan tehdä diagnoosi, jos tilisi varastetaan."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Laskutustiedot"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Tarvittavat tiedot laskun laatimiseen kerätään ostettaessa meiltä palvelua."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Henkilötietojen käsittelyn tarkoitus ja oikeusperusta"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -187,25 +176,23 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Henkilöt, joilla on sopimus palvelun teknisestä varmistuksesta."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Maksunkäsittelijät ostaessasi palvelua meiltä."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Kaikki henkilökohtaiset tiedot säilötään Euroopan unionin alueella."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Pääsy henkilötietoihin"
+msgid "Disclosure of the Personal Data"
+msgstr "Henkilötietojen luovuttaminen"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
```

### Comparing `wllegal-2023.3/wllegal/locale/fil/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/fil/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-07-16 03:14+0000\n"
 "Last-Translator: Marco Santos <enum.scima@gmail.com>\n"
 "Language-Team: Filipino <https://hosted.weblate.org/projects/weblate/legal/"
 "fil/>\n"
 "Language: fil\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -202,15 +202,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Nakatago sa European Union ang lahat ng mga Personal na Data."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Access sa Personal na Data"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/fr/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/fr/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,37 +4,35 @@
 # ButterflyOfFire <ButterflyOfFire@protonmail.com>, 2018.
 # Estébastien Robespi <estebastien@mailbox.org>, 2019.
 # Nathan <bonnemainsnathan@gmail.com>, 2019.
 # Julien Humbert <julroy67@gmail.com>, 2020.
 # Localisation Lab <ao@localizationlab.org>, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-03-21 06:01+0000\n"
-"Last-Translator: Ldm Public <ldmpub@gmail.com>\n"
-"Language-Team: French <https://hosted.weblate.org/projects/weblate/legal/fr/"
-">\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-20 18:47+0000\n"
+"Last-Translator: Julien Humbert <julroy67@gmail.com>\n"
+"Language-Team: French <https://hosted.weblate.org/projects/weblate/legal/fr/>"
+"\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Sous-traitant conformément à l’art. 28 de la RGPD"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Statut à partir d’octobre 2020."
+msgstr "Statut en date de mars 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -72,28 +70,24 @@
 "lorsqu’il utilise nos services :"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Nom et adresse courriel"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
 msgstr ""
 "Elles sont utilisées pour vous identifier dans le système de contrôle des "
-"versions"
+"versions."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
 "Par ailleurs, votre adresse courriel est utilisée pour les notifications "
-"relatives aux événements que vous surveillez"
+"relatives aux événements que vous surveillez."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Mot de passe haché"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -104,37 +98,33 @@
 msgstr "Les mots de passe sont stockés sous forme hachée Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "Adresse IP et nom de votre navigateur Internet"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Ils sont journalisés en cas de modifications importantes de votre compte "
 "(par exemple, un changement de mot de passe) afin de permettre un diagnostic "
-"en cas de vol de votre compte"
+"en cas de vol de votre compte."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Informations de facturation"
+msgstr "Infos de facturation"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Les données nécessaires à l’établissement d’une facture sont collectées lors "
+"de l’achat d’un service chez nous."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Objectif et bases légales du traitement des Données Personnelles"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -200,61 +190,66 @@
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 "Personnes qui sont sous-contrat pour assurer le fonctionnement technique du "
 "service."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Les organismes de paiement lors de l’achat d’un service chez nous."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 "Toutes les données personnelles sont conservées dans l’Union Européenne."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Accès aux données personnelles"
+msgid "Disclosure of the Personal Data"
+msgstr "Divulgation de données personnelles"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Les données personnelles peuvent être divulguées à des tiers dans des "
+"circonstances limitées lorsque le contrôleur croit de bonne foi que la loi "
+"l’exige, par exemple dans le cadre d’une citation à comparaître ou d’une "
+"autre ordonnance judiciaire ou administrative."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Si le contrôleur est tenu par la loi de divulguer les données personnelles, "
+"il s’efforcera d’informer l’utilisateur au préalable par courrier "
+"électronique (à moins que le contrôleur n’en ait l’interdiction ou que cela "
+"soit futile) qu’une demande de données personnelles a été faite pour "
+"permettre à l’utilisateur de s’opposer à la divulgation. Si l’utilisateur ne "
+"conteste pas la demande de divulgation, le responsable du traitement peut "
+"être légalement tenu de communiquer les données personnelles."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "La conservation des données personnelles"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Les données personnelles sont conservées par le Service tant que "
 "l’utilisateur n’a pas supprimé son compte du service."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Les informations du journal d’accès peuvent être recueillies pendant une "
 "période plus longue dans le but d’établir, d’exercer ou de défendre des "
 "droits légaux."
@@ -324,31 +319,23 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "La destruction, la correction et la récupération de vos données personnelles "
 "peuvent être réalisées depuis votre Compte et sont entièrement automatisées."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
 "Nous collections des données personnelles (tel que votre adresse de courrier "
-"électronique), celles-ci seront supprimées de notre base de données dès que "
-"vous supprimez votre compte."
+"électronique), celles-ci seront supprimées de notre base de données si vous "
+"supprimez votre compte."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "Vos traductions sont soumises à une licence qui est précisée pour chacun des "
 "projets."
 
@@ -361,22 +348,25 @@
 "système de contrôle de versions, de façon permanente."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Le nom est choisi par vous et l’adresse courriel utilisée pour vos "
+"contributions peut être masquée par le système Weblate pour protéger votre "
+"vie privée."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Nous utilisons des cookies pour fournir nos services."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Nous n’utilisons pas de témoins de connexion tiers."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Voir la version anglaise"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -663,14 +653,18 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"Au sens de l’<a href=\"%(url)s\">Article 7</a> du RGPD, l’Utilisateur donne "
+"consentement pour la collecte, le stockage, et le traitement des Données "
+"Personnelles selon la <a href=\"%(privacy_url)s\">politique de "
+"confidentialité</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Traductions"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -703,27 +697,22 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "L’Utilisateur accepte, en contribuant à un Projet, la licence que le Projet "
 "a spécifiée."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"L’Utilisateur accepte que ses propres nom et courriel soient utilisés lors "
-"des archivages dans le système de contrôle des versions. Cette autorisation "
-"est irrévocable compte tenu de la nature même du système de contrôle des "
+"L’utilisateur accepte que ses nom et courriel soient utilisés lors des "
+"archivages dans le système de contrôle des versions. Cette autorisation est "
+"irrévocable compte tenu de la nature même du système de contrôle des "
 "versions."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
@@ -762,23 +751,19 @@
 "compétence matérielle et locale."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Date d’effet"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-"Ces Conditions Générales d’Utilisation sont effectives à compter du 1er "
-"septembre 2017."
+"Ces Conditions Générales d’Utilisation sont effectives à compter du 5 mai "
+"2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "Dans le cas où vous achetez l’un de nos services, nous recueillons des "
 #~ "informations supplémentaires nécessaires à l’émission d’une facture"
```

### Comparing `wllegal-2023.3/wllegal/locale/fur/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/fur/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Weblate <noreply@weblate.org>, 2019.
 # Fabio Tomat <f.t.public@gmail.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2019-12-04 18:50+0000\n"
 "Last-Translator: anonymous <noreply@weblate.org>\n"
 "Language-Team: Friulian <https://hosted.weblate.org/projects/weblate/hosted/"
 "fur/>\n"
 "Language: fur\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -163,15 +163,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/fy/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/fy/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2018-01-30 18:47+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Frisian <https://hosted.weblate.org/projects/weblate/master/"
 "fy/>\n"
 "Language: fy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -168,15 +168,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/gl/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/gl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Iván <ivanrsm1997@gmail.com>, 2018.
 # Iván Seoane <ivanrsm1997@gmail.com>, 2018, 2019.
 # Iváns <ivanrsm1997@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-10-03 16:19+0000\n"
 "Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
 "Language-Team: Galician <https://hosted.weblate.org/projects/weblate/legal/"
 "gl/>\n"
 "Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -199,15 +199,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Tódolos datos persoais son almacenados na Unión Europea."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Acceso ós datos persoais"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/he/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/he/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Yaron Shahrabani <sh.yaron@gmail.com>, 2018, 2019, 2020.
 # ButterflyOfFire <ButterflyOfFire@protonmail.com>, 2018.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-11-27 12:52+0000\n"
-"Last-Translator: Omer I.S. <omeritzicschwartz@gmail.com>\n"
-"Language-Team: Hebrew <https://hosted.weblate.org/projects/weblate/legal/he/"
-">\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-21 12:25+0000\n"
+"Last-Translator: Yaron Shahrabani <sh.yaron@gmail.com>\n"
+"Language-Team: Hebrew <https://hosted.weblate.org/projects/weblate/legal/he/>"
+"\n"
 "Language: he\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1) ? 0 : ((n == 2) ? 1 : ((n > 10 && "
 "n % 10 == 0) ? 2 : 3));\n"
-"X-Generator: Weblate 4.10-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "קבלנים בהתאם לסעיף 28 ב־GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "המצב נכון לאוקטובר 2020."
+msgstr "המצב נכון למרץ 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -68,25 +66,21 @@
 "ב־Weblate מתבצע עיבוד אך ורק על נתונים אישיים שמסופקים על ידי המשתמשים:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "שם וכתובת דוא״ל"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "אלו משמשים לזהות אותך בהגשות למערכת ניהול הגרסאות"
+msgstr "אלו משמשים לזהות אותך בהגשות למערכת ניהול הגרסאות."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"בנוסף, נעשה שימוש בכתובת הדוא״ל לטובת שליחת התרעות על אירועים אליהם נרשמת"
+"בנוסף, נעשה שימוש בכתובת הדוא״ל לטובת שליחת התרעות על אירועים אליהם נרשמת."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "הסיסמה בתצורת גיבוב"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -97,36 +91,30 @@
 msgstr "ססמאות מאוחסנות ומגובבות בעזרת Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "כתובת IP ושם הדפדפן"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "אלו מתועדים למקרה שיתרחשו שינויים חשובים לחשבונך (למשל: החלפת סיסמה) כדי "
-"לאפשר ניתוח במקרה של גניבת החשבון שלך"
+"לאפשר ניתוח במקרה של גניבת החשבון שלך."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "פרטי חיוב"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
-msgstr ""
+msgstr "פרטים חיוניים להנפקת חשבונית נאספים בעת רכישת אישור מאתנו."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "תכלית ובסיס משפטי לעיבוד של נתונים אישיים"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -184,58 +172,59 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "אנשים פרטיים שחתמו על חוזה לתחזוקה טכנית של השירות."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "מעבדי תשלום כשרוכשים מאתנו שירות."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "כל המידע האישי מאוחסן באיחוד האירופי."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "גישה לנתונים האישיים"
+msgid "Disclosure of the Personal Data"
+msgstr "חשיפת נתונים אישיים"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"הנתונים האישיים עלולים להיחשף בפני גורמי צד־שלישי בנסיבות מוגבלות כאשר השולט "
+"מאמין בלב שלם שיש לכך דרישה חוקית, כגון תחת זימון לבית משפט או צו משפטי או "
+"מנהלי כזה או אחר."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"אם השולט נדרש על פי חוק לחשוף את הנתונים האישיים, יתבצע ניסיון לספק למשתמש "
+"הודעה מוקדם בדוא״ל (אלא אם כן אסור לשולט לעשות זאת או שאין בכך טעם) שהוגשה "
+"בקשה לקבלת הנתונים האישיים כדי לאפשר למשתמש להתנגד לחשיפה. אם המשתמש בחר שלא "
+"להגיב לבקשת החשיפה, השולט יכול להידרש למסור את הנתונים האישיים על פי חוק."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "החזקת הנתונים האישיים"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr "הנתונים האישיים מאוחסנים בשירות עד שהמשתמש מוחק את החשבון שלו בשירות."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "מידע מיומן הגישה עשוי להיאסף לתקופה ארוכה יותר לטובת הקמה, תרגול או הגנה מול "
 "טענות משפטיות."
 
@@ -300,56 +289,50 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "ההסרה, התיקון וקבלת הנתונים האישיים שלך זמינים דרך ניהול החשבון בצורה "
 "אוטומטית לחלוטין."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
 "אנו מעבדים נתונים אישיים (כגון כתובת הדוא״ל שלך), נתונים אלו נמחקים ממסד "
-"הנתונים שלנו עם הסרת החשבון שלך."
+"הנתונים שלנו עם בחירתך להסרת החשבון שלך."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
-msgstr "על התרגומים שלך חלים הרישיונות שצוינו בידי מיזם התרגום עצמו."
+msgstr "התרגומים שלך כפופים לרישיונות שצוינו בידי מיזם התרגום עצמו."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 "נעשה שימוש בשמך ובכתובת הדוא״ל שלך בהגשות למערכת בקרת גרסאות הקוד, אלו "
 "יישארו שם לנצח."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"השם הנבחר הוא לבחירתך ואת כתובת הדוא״ל שבשימוש Weblate יכול למסך כדי להגן על "
+"הפרטיות שלך."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "אנו משתמשים בעוגיות כדי להגיש את השירותים שלנו."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "איננו משתמשים בעוגיות מצד־שלישי."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "הצגת הגרסה האנגלית"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -612,14 +595,16 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"בהתאם ל<a href=\"%(url)s\">סעיף 7</a> ב־GDPR המשתמש מסכים לאיסוף, אחסון "
+"ועיבוד הפרטים האישיים בכפוף ל<a href=\"%(privacy_url)s\">מדיניות הפרטיות</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "תרגומים"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -649,19 +634,14 @@
 #: wllegal/templates/legal/documents/tos.html:111
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr "המשתמש מסכים, מעצם תרומתו למיזם, לרישיון בו נוקט המיזם."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
 "המשתמש מסכים שהשימוש בשמו ובכתובת הדוא״ל שלו כסמכות יוצרת בהגשות למערכות "
 "ניהול הקוד. המשתמש מבין שהרשאה זו בלתי הפיכה עקב טבעה של מערכת ניהול קוד."
@@ -702,21 +682,17 @@
 "הצ׳כית שתחום השיפוט שלו עצמאי ומקומי."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "תוקף"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "תנאי השירות האלו ייכנסו לתוקף משפטי ב־1 בספטמבר 2017."
+msgstr "תנאי השירות האלו ייכנסו לתוקף משפטי ב־15 במאי 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "במקרה של רכישת שירותים מאתנו, אנו אוספים פרטי חיוב נוספים שנחוצים להנפקת "
 #~ "חשבונית"
```

### Comparing `wllegal-2023.3/wllegal/locale/hi/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/hi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-10-17 00:57+0000\n"
 "Last-Translator: Ritwik <ritwikraghav14@gmail.com>\n"
 "Language-Team: Hindi <https://hosted.weblate.org/projects/weblate/legal/hi/"
 ">\n"
 "Language: hi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -162,15 +162,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/hr/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/hr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2019.
 # Milo Ivir <mail@milotype.de>, 2019, 2020.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-09-22 15:42+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-06-02 06:31+0000\n"
 "Last-Translator: Milo Ivir <mail@milotype.de>\n"
 "Language-Team: Croatian <https://hosted.weblate.org/projects/weblate/legal/"
 "hr/>\n"
 "Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "Podkooperanti sukladno čl. 28 GDPR-a"
+msgstr "Podugovarači sukladno čl. 28 GDPR-a"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Stanje od listopada 2020."
+msgstr "Stanje od ožujka 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -70,26 +68,22 @@
 "Weblatea:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Ime i e-adresa"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
 msgstr ""
-"Koriste se kako bi te se identificiralo u promjenama u sustavu za kontrolu "
-"verzija"
+"Ovi se podaci koriste kako bi te se identificiralo u promjenama u sustavu za "
+"kontrolu verzija."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "E-adresa se koristi i za obavijesti događaja koje pratiš"
+msgstr "Dodatno tome se e-adresa koristi i za obavijesti praćenih događaja."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Šifrirana lozinka"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -100,36 +94,32 @@
 msgstr "Lozinke se spremaju šifrirano pomoću Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP adresa i ime preglednika"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Bilježe se u slučaju značajnih promjena na tvom računu (npr. promjena "
-"lozinke) i služe za provođenje dijagnoze u slučaju da se tvoj račun ukrade"
+"Ovi se podaci bilježe se u slučaju značajnih promjena u tvom računu (npr. "
+"promjena lozinke) i služe za dijagnozu u slučaju da se tvoj račun ukrade."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Podaci naplate"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Potrebni podaci za izdavanje računa prikupljaju se prilikom kupnje jedne od "
+"naših usluga."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Svrha i pravna osnova za obradu osobnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -189,25 +179,23 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Osobe s kojima je zaključen ugovor za tehničko osiguravanje usluge."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Procesori plaćanja prilikom kupnje jedne od naših usluga."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Svi osobni podaci spremaju se u Europskoj uniji."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Pristup osobnim podacima"
+msgid "Disclosure of the Personal Data"
+msgstr "Otkrivanje osobnih podataka"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
@@ -231,18 +219,14 @@
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Osobni podaci se spremaju u usluzi sve dok korisnik ne izbriše svoj račun na "
 "usluzi."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Podaci o pristupanjima mogu se prikupljati na duže vremensko razdoblje u "
 "svrhu utvrđivanja, ostvarivanja ili zaštite pravnih zahtjeva."
 
@@ -308,30 +292,22 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "Uklanjanje, ispravljanje i dohvaćanje tvojih osobnih podataka može se "
 "izvršiti na stranici za upravljanje računom i potpuno je automatizirano."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Obrađujemo privatne podatke (kao što je tvoja e-adresa). Podaci se uklanjaju "
-"iz naše baze podataka čim ukloniš račun."
+"Obrađujemo osobne podatke (kao što je tvoja e-adresa). Ti se podaci "
+"uklanjaju iz naše baze podataka ako ukloniš račun."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "Tvoji se prijevodi izrađuju pod licencom koja je određena za svaki prijevod."
 
 #: wllegal/templates/legal/documents/summary.html:7
@@ -343,22 +319,24 @@
 "Tamo će ostati zauvijek."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Odaberi ime proizvoljno. E-mail adresa koja se koristi za promjene se može "
+"maskirati pomoću Weblate sustava za zaštitu tvoje privatnosti."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Koristimo kolačiće za dostavljanje naših usluga."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Ne koristimo kolačiće trećih strana."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Pogledaj englesku verziju"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -637,14 +615,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"U smislu <a href=\"%(url)s\">članka 7</a> GDPR-a, korisnik ovime daje "
+"privolu za prikupljanje, spremanje i obradu osobnih podataka u skladu s <a "
+"href=\"%(privacy_url)s&quot;\">Politikom privatnosti</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Prijevodi"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -676,27 +657,22 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "Nakon doprinošenja projektu, korisnik se slaže s licencom koju je projekt "
 "odredio."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"Korisnik pristaje koristiti vlastito ime i e-adresu kao autorstvo promjena u "
-"sustavu za kontrolu verzija. Korisnik shvaća da se ova dozvola ne može "
-"opozvati zbog same prirode sustava za kontrolu verzija."
+"Korisnik pristaje koristiti ime i e-adresu kao autorstvo promjena u sustavu "
+"za kontrolu verzija. Korisnik razumije da se ova dozvola ne može opozvati "
+"zbog same prirode sustava za kontrolu verzija."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -731,21 +707,17 @@
 "usluge rješava sud Republike Češke koji ima materijalnu i lokalnu nadležnost."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Stupanje na snagu"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "Ovi uvjeti pružanja usluge stupaju na snagu 1. rujna 2017."
+msgstr "Ovi uvjeti usluge stupaju na snagu 15. svibnja 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "U slučaju da od nas kupiš uslugu, prikupljamo dodatne podatke naplate, "
 #~ "koji su potrebni za izdavanje računa"
```

### Comparing `wllegal-2023.3/wllegal/locale/hu/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/hu/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # János Néhrer <iiamnot@gmail.com>, 2019.
 # miles <varota@gmail.com>, 2019.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-02-22 09:57+0000\n"
 "Last-Translator: Bálint László <balint.laszlo.2011@gmail.com>\n"
 "Language-Team: Hungarian <https://hosted.weblate.org/projects/weblate/legal/"
 "hu/>\n"
 "Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -192,15 +192,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Minden személyes adat az Európai Unióban van tárolva."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Hozzáférés a személyes adatokhoz"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/hy/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/hy/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2015.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2019-07-22 07:40+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Armenian <https://hosted.weblate.org/projects/weblate/hosted/"
 "hy/>\n"
 "Language: hy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -172,15 +172,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Reset repository"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Վերակայել պահեստարանը"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ia/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ms/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Weblate <noreply@weblate.org>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ia\n"
+"Language: ms\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -156,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/id/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/id/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,35 @@
 # Arif Budiman <arifpedia@gmail.com>, 2016-2018.
 # Andika Triwidada <andika@gmail.com>, 2018.
 # anonymous <noreply@weblate.org>, 2019.
 # frottle <monochromefrog@gmail.com>, 2020.
 # frottle <catatan.kungkong@gmail.com>, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-04-08 07:31+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-25 14:51+0000\n"
 "Last-Translator: Taufik Adi Wicaksono <taufikadi.wicaksono@tutamail.com>\n"
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/weblate/legal/"
 "id/>\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.12-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subkontraktor Sesuai dengan Art. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Status per Oktober 2020."
+msgstr "Status per Maret 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -64,114 +62,107 @@
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
 msgstr "Data Pribadi yang diolah oleh Weblate"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
 msgstr ""
-"Weblate hanya mengolah Data Pribadi yang disediakan oleh Pengguna secara:"
+"Weblate hanya memproses Data Pribadi yang diberikan oleh Pengguna melalui:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Nama dan alamat surel"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Ini digunakan untuk mengidentifikasi Anda dalam commit VCS"
+msgstr "Ini digunakan untuk mengidentifikasi Anda dalam commit VCS."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"Selain itu, surel digunakan untuk memberi notifikasi pada proyek yang diikuti"
+"Selain itu, surel digunakan untuk memberikan notifikasi pada proyek yang "
+"diikuti."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "Kata sandi dalam bentuk yang ditagarkan"
+msgstr "Kata sandi dalam bentuk hash"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
 msgstr "Digunakan untuk autentikasi Pengguna, bila telah dikonfigurasi"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr "Kata sandi disimpan di-hash memakai Argon2."
+msgstr "Kata sandi disimpan dan di-hash memakai Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "Alamat IP dan nama peramban web"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Ini dicatat jika ada perubahan penting pada akun Anda (seperti Perubahan "
-"kata sandi) untuk memungkinkan pemeriksaan seandainya akun Anda dicuri"
+"kata sandi) untuk memungkinkan pemeriksaan seandainya akun Anda dicuri."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Informasi penagihan"
+msgstr "Info penagihan"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Rincian yang diperlukan untuk menerbitkan faktur dikumpulkan saat membeli "
+"layanan dari kami."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Tujuan dan dasar hukum pengolahan Data Pribadi"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "Data Pribadi Anda akan digunakan untuk keperluan Layanan:"
+msgstr "Data Pribadi Anda akan digunakan untuk tujuan Layanan:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
 "contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 "
 "(1) b. GDPR</a>)"
 msgstr ""
-"untuk menyediakan layanan kami di Layanan, untuk menghubungi Anda dalam hal-"
-"hal mengenai layanan kami (juga melalui surel dan pesan) dan untuk "
+"untuk menyediakan layanan kami di bagian Layanan, untuk menghubungi Anda "
+"dalam hal-hal mengenai layanan kami (juga melalui surel dan pesan) dan untuk "
 "memastikan fungsionalitas teknis dari layanan kami dalam pemenuhan kewajiban "
 "kontrak atau prakontrak (<a href=\" %(url)s\">Pasal 6 (1) b. GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
-"untuk menganalisis penggunaan Anda atas layanan kami dan meningkatkan "
+"untuk menganalisis penggunaan Anda atas layanan kami dan untuk meningkatkan "
 "layanan kami (<a href=\"%(url)s\">Pasal 6 (1) b. dan f. GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:49
 #, python-format
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
-"dengan persetujuan tegas dari Anda atau instruksi untuk melanjutkan kegiatan "
-"bisnis kami atau mengirimkan buletin kepada Anda (<a href=\"%(url)s\">Pasal "
-"6 (1) a. GDPR</a>)"
+"dengan persetujuan atau instruksi tertulis dari Anda untuk menjalankan "
+"aktivitas bisnis kami atau mengirimkan buletin kepada Anda (<a href=\"%(url)"
+"s\">Pasal 6 (1) a. GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
 msgstr "Akses ke Data Pribadi"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
@@ -190,66 +181,71 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Orang-orang yang dikontrak untuk memberikan jaminan teknis layanan."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Pemroses pembayaran saat membeli layanan dari kami."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Semua Data Pribadi disimpan di Uni Eropa."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Akses ke Data Pribadi"
+msgid "Disclosure of the Personal Data"
+msgstr "Pengungkapan Data Pribadi"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Data Pribadi dapat diungkapkan kepada pihak ketiga dalam keadaan terbatas "
+"ketika Pengendali memiliki itikad baik bahwa hal tersebut diwajibkan oleh "
+"hukum, seperti di bawah panggilan pengadilan atau perintah peradilan atau "
+"administratif lainnya."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Jika Pengendali diwajibkan oleh hukum untuk mengungkapkan Data Pribadi, "
+"upaya akan dilakukan untuk memberikan pemberitahuan sebelumnya kepada "
+"Pengguna melalui surel (kecuali jika Pengendali dilarang, atau akan sia-sia) "
+"bahwa permintaan Data Pribadi telah dibuat untuk memungkinkan Pengguna "
+"mengajukan keberatan atas pengungkapan tersebut. Jika Pengguna tidak "
+"mengajukan keberatan atas permintaan pengungkapan tersebut, Pengendali dapat "
+"diwajibkan secara hukum untuk menyerahkan Data Pribadi."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
-msgstr "Penyimpanan Data Pribadi"
+msgstr "Retensi Data Pribadi"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Data Pribadi disimpan dalam Layanan sampai Pengguna menghapus akun mereka di "
 "layanan."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"Informasi mengenai log akses dapat dikumpulkan untuk jangka waktu yang lebih "
-"lama untuk tujuan membangun, menjalankan, atau mempertahankan klaim hukum."
+"Info mengenai log akses dapat dikumpulkan untuk jangka waktu yang lebih lama "
+"untuk tujuan membangun, menjalankan, atau mempertahankan klaim hukum."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "Hak Anda"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
@@ -271,16 +267,16 @@
 #: wllegal/templates/legal/documents/privacy.html:85
 #, python-format
 msgid ""
 "Gain access to all your Personal Data that Weblate uses or processes, and "
 "even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 msgstr ""
 "Mendapatkan akses ke semua Data Pribadi Anda yang digunakan atau diolah oleh "
-"Weblate, dan bahkan dapatkan semua salinannya (<a href=\"%(url)s\">Pasal 15 "
-"GDPR</a>)"
+"Weblate, dan bahkan mendapatkan semua salinannya (<a href=\"%(url)s\">Pasal "
+"15 GDPR</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:86
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
 "Memperbaiki Data Pribadi yang diolah oleh Weblate jika menurut Anda terdapat "
@@ -311,30 +307,22 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "Penghapusan, koreksi, dan pengambilan Data Pribadi Anda dapat dilakukan dari "
 "manajemen akun, dan sepenuhnya berjalan otomatis."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Kami mengolah data pribadi (seperti alamat surel Anda), dan akan dibuang "
-"dari basis data kami segera setelah Anda menghapus akun Anda."
+"Kami mengolah data pribadi (seperti alamat surel Anda); mereka akan dibuang "
+"dari basis data kami jika Anda menghapus akun Anda."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "Terjemahan Anda dibuat berdasarkan lisensi yang ditentukan oleh setiap "
 "terjemahan."
 
@@ -345,22 +333,24 @@
 msgstr "Nama dan surel Anda digunakan di VCS, mereka akan tetap ada selamanya."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Nama yang dipilih terserah Anda dan alamat surel yang digunakan untuk commit "
+"dapat disembunyikan oleh sistem Weblate untuk melindungi privasi Anda."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Kami menggunakan kuki untuk memberikan layanan kami."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Kami tidak menggunakan kuki pihak ketiga mana pun."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Lihat versi Bahasa Inggris"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -397,21 +387,21 @@
 "Consent"
 msgstr ""
 "berarti Persetujuan Lisensi dalam arti Pasal 2358 et seq. dari Kode Sipil "
 "disimpulkan oleh dan antara Pengguna dan Penyedia atas Persetujuan"
 
 #: wllegal/templates/legal/documents/tos.html:29
 msgid "Civil Code"
-msgstr "Kode Sipil"
+msgstr "Hukum Perdata"
 
 #: wllegal/templates/legal/documents/tos.html:30
 #, python-format
 msgid "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
 msgstr ""
-"berarti UU No. %(law_89_2012)s Coll., Kode Sipil, sebagaimana diamandemenkan"
+"berarti UU No. %(law_89_2012)s Coll., Hukum Perdata, sebagaimana telah diubah"
 
 #: wllegal/templates/legal/documents/tos.html:32
 msgid "Consent"
 msgstr "Persetujuan"
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
@@ -454,15 +444,15 @@
 msgstr "Lisensi"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
-"berarti lisensi non eksklusif yang diberikan oleh Penyedia kepada Pengguna "
+"berarti lisensi noneksklusif yang diberikan oleh Penyedia kepada Pengguna "
 "untuk penggunaan Layanan"
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
 msgstr "Penyedia"
 
 #: wllegal/templates/legal/documents/tos.html:46
@@ -643,14 +633,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"Dalam arti <a href=\"%(url)s\">Pasal 7</a> GDPR, Pengguna dengan ini "
+"memberikan persetujuan untuk mengumpulkan, menyimpan, dan memproses Data "
+"Pribadi sesuai dengan <a href=\"%(privacy_url)s\">Kebijakan Privasi</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Terjemahan"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -683,38 +676,33 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "Pengguna menyetujui, ketika memberikan kontribusi pada sebuah Proyek, "
 "lisensi yang telah ditentukan oleh Proyek."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"Pengguna setuju untuk menggunakan nama dan surel mereka sendiri sebagai "
-"kepengarangan pada commit VCS. Pengguna memahami bahwa hibah ini tidak dapat "
-"dibatalkan karena sifat VCS."
+"Pengguna setuju untuk menggunakan nama dan surel sebagai kepengarangan pada "
+"commit VCS. Pengguna memahami bahwa pemberian ini tidak dapat dibatalkan "
+"karena sifat VCS."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
 msgstr ""
-"Dalam arti Pasal 89 UU No. %(law_480_2004)s Coll., tentang komunikasi "
-"elektronik, sebagaimana diamendemenkan, Pengguna diberi informasi bahwa "
-"Layanan menggunakan kuki."
+"Dalam arti Pasal 89 Undang-Undang No. %(law_480_2004)s Coll, tentang "
+"komunikasi elektronik, sebagaimana telah diubah, Pengguna diberitahu bahwa "
+"Layanan ini menggunakan Kuki."
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid "The Service uses Cookies to personalise content."
 msgstr "Layanan menggunakan Kuki untuk mempersonalisasi konten."
 
 #: wllegal/templates/legal/documents/tos.html:123
 msgid "Governing Law"
@@ -739,21 +727,17 @@
 "yang memiliki yuridiksi substansif dan lokal."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Masa Berlaku"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "Persyaratan Layanan ini mulai berlaku pada tanggal 1 September 2017."
+msgstr "Persyaratan Layanan ini mulai berlaku pada tanggal 15 Mei 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "Jika Anda membeli layanan ini, Informasi penagihan yang diperlukan akan "
 #~ "dikumpulkan untuk menerbitkan faktur"
```

### Comparing `wllegal-2023.3/wllegal/locale/ie/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/nn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ie\n"
+"Language: nn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/is/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/is/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2023-01-31 21:41+0000\n"
 "Last-Translator: Sveinn í Felli <sv1@fellsnet.is>\n"
 "Language-Team: Icelandic <https://hosted.weblate.org/projects/weblate/legal/"
 "is/>\n"
 "Language: is\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -199,15 +199,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Öll persónuleg gögn eru vistuð í Evrópusambandinu."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Aðgangur að persónulegum gögnum"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/it/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/it/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,38 +6,36 @@
 # Michele <miguel2000@livecom.it>, 2018.
 # Manuel Tassi <manueltassi91@gmail.com>, 2018.
 # Pierfrancesco Passerini <p.passerini@gmail.com>, 2019.
 # Valter Mura <valtermura@gmail.com>, 2019.
 # Valentina Grassi <vale.grassi11@gmail.com>, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-12-11 11:48+0000\n"
-"Last-Translator: Pierfrancesco Passerini <p.passerini@gmail.com>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-28 02:39+0000\n"
+"Last-Translator: bovirus <roberto.boriotti@canon.it>\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/weblate/legal/it/"
 ">\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 "X-Poedit-SourceCharset: UTF-8\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subappaltatori in conformità con l'Art. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Aggiornato ad Ottobre 2020."
+msgstr "Aggiornato a Marzo 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -75,24 +73,20 @@
 "servizio:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Nome utente e email"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Questi sono usati per identificarti nelle modifiche VCS"
+msgstr "Questi sono usati per identificarti nelle modifiche VCS."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "Inoltre, l'e-mail è usata per le notifiche degli eventi monitorati"
+msgstr "Inoltre, l'email è usata per le notifiche degli eventi monitorati."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Hash della password"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -103,37 +97,33 @@
 msgstr "Le password vengono archiviate con hash usando Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "Indirizzo IP e nome browser"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Questi sono registrati in casi di importanti modifiche al tuo account (ad "
+"Questi sono registrati in casi di importanti modifiche all' account (ad "
 "esempio modifica della password) per consentire la diagnosi nel caso in cui "
-"il tuo account venga rubato"
+"l'account venga rubato."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
-msgstr "Dati di fatturazione"
+msgstr "Dati fatturazione"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"I dettagli necessari per emettere una fattura vengono da noi raccolti al "
+"momento dell'acquisto di un servizio."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Scopo e base giuridica del trattamento dei dati personali"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -196,60 +186,65 @@
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr ""
 "Persone che sono state assunte per l'espletamento tecnico del servizio."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Tipologia pagamento al momento dell'acquisto di un servizio."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Tutti i dati personali sono memorizzati nell'Unione Europea."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Accesso ai dati personali"
+msgid "Disclosure of the Personal Data"
+msgstr "Divulgazione dati personali"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"I dati personali potrebbero essere divulgati a terzi in circostanze limitate "
+"quando il Titolare ritiene in buona fede che ciò sia richiesto dalla legge, "
+"ad esempio in virtù di un mandato di comparizione o di un altro ordine "
+"giudiziario o amministrativo."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Nel caso in cui il Titolare sia tenuto per legge a divulgare i dati "
+"personali, si cercherà di fornire all'utente un preavviso via email (a meno "
+"che il Titolare non lo vieti, o sarebbe inutile) che è stato autorizzata una "
+"richiesta di divulgazione dei dati personali per consentire all'Utente di "
+"opporsi alla divulgazione. Se l'Utente non contesta la richiesta di "
+"divulgazione, il Titolare potrebbe essere obbligato per legge a consegnare i "
+"Dati Personali."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "La conservazione dei dati personali"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "I dati personali sono memorizzati nel servizio fino a quando l'utente non "
 "elimina il proprio account nel servizio."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Le informazioni del registro di accesso potrebbero essere raccolte per un "
 "periodo più lungo al fine di stabilire, esercitare o difendere i reclami "
 "legali."
@@ -317,35 +312,27 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "La rimozione, correzione e recupero dei tuoi Dati Personali può essere "
 "effettuata dalla gestione dell'account ed è completamente automatizzata."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Elaboriamo dati privati (come l'indirizzo email), che verranno eliminati dal "
-"nostro database non appena rimuoverai il tuo account."
+"Noi elaboriamo i dati personali (come l'indirizzo email), che verranno "
+"eliminati dal nostro database non appena rimuoverai il tuo account."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
-"Le tue traduzioni sono create sotto licenza che è specifica per ogni "
+"Le tue traduzioni sono create sotto la licenza che è specifica per ogni "
 "traduzione."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
@@ -353,34 +340,36 @@
 "indefinitamente."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Il nome scelto dipende da te e per proteggere la tua privacy l'indirizzo "
+"email usato per i commit può essere mascherato dal sistema Weblate."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Noi usiamo i cookie per espletare i nostri servizi."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Non usiamo cookie di terze parti."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Visualizza la versione inglese"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"Il documento \"Termini di servizio\" ufficiale è in inglese. Le traduzioni "
-"sono fornite per comodità dell'utente."
+"Il documento dei \"Termini del servizio\" è in inglese. Le traduzioni sono "
+"fornite per comodità dell'utente."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
 "I diritti e le responsabilità dell'utente e del fornitore derivanti dall'uso "
@@ -423,17 +412,17 @@
 msgstr "Consenso"
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
-"indica il consenso dell'utente con i presenti Termini di servizio e altri "
-"documenti legali espresso selezionando la casella di controllo durante la "
-"registrazione"
+"indica, selezionando la casella di controllo durante la registrazione, il "
+"consenso dell'utente con i presenti \"Termini del Servizio\" ed altri "
+"documenti legali espliciti"
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
 msgstr "Cookie"
 
 #: wllegal/templates/legal/documents/tos.html:36
@@ -572,25 +561,25 @@
 #: wllegal/templates/legal/documents/tos.html:78
 msgid ""
 "By concluding Agreement under Article 2.1 of this Agreement, the following "
 "provisions of this Article 3 of the Terms of Service come into force."
 msgstr ""
 "Con la conclusione dell'Accordo ai sensi dell'articolo 2.1 del presente "
 "Accordo, entrano in vigore le seguenti disposizioni del presente articolo 3 "
-"dei Termini di servizio."
+"dei Termini di Servizio."
 
 #: wllegal/templates/legal/documents/tos.html:80
 msgid ""
 "The Provider presents the User with a License Agreement and the User accepts "
 "this License Agreement, all this under the terms and conditions stated in "
 "these Terms of Service."
 msgstr ""
-"Il Fornitore concede all'Utente un Accordo di Licenza e l'Utente accetta "
+"Il Fornitore concede all'utente un Accordo di Licenza e l'utente accetta "
 "tale Licenza nel rispetto dei termini e delle condizioni stabilite nei "
-"Termini di Servizio."
+"Termini del Servizio."
 
 #: wllegal/templates/legal/documents/tos.html:82
 msgid ""
 "The Provider shall have the right to shut down, adjust, modify or make the "
 "Service unavailable on the web address at any time."
 msgstr ""
 "Il Fornitore avrà il diritto di chiudere, regolare, modificare o rendere in "
@@ -637,26 +626,30 @@
 #: wllegal/templates/legal/documents/tos.html:95
 msgid ""
 "If the User is an entrepreneur, it hereby expressly waives its right to "
 "compensation from the Provider for damage unintentionally caused by the "
 "Provider to the User through a breach of any obligation contained in these "
 "Terms of Service and/or resulting from the use of the Service."
 msgstr ""
-"Se l'Utente è un imprenditore, rinuncia espressamente al suo diritto al "
-"risarcimento da parte del Fornitore per danni causati involontariamente dal "
-"Fornitore all'Utente attraverso la violazione di qualsiasi obbligo contenuto "
-"in questi Termini di Servizio e/o risultante dall'uso del Servizio."
+"Se l'utente è un imprenditore, rinuncia espressamente al suo diritto al "
+"risarcimento da parte del fornitore per danni causati involontariamente dal "
+"fornitore all'utente attraverso la violazione di qualsiasi obbligo contenuto "
+"nei Termini del Servizio e/o risultante dall'uso del servizio."
 
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"Ai sensi dell'<a href=\"%(url)s\">Articolo 7</a> del GDPR, l'Utente "
+"acconsente alla raccolta, alla conservazione e al trattamento dei dati "
+"personali secondo l'<a href=\"%(privacy_url)s\">Informativa sulla privacy</"
+"a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Traduzioni"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -690,27 +683,22 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "L'utente accetta, dopo aver contribuito a un progetto, la licenza "
 "specificata dal progetto."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"L'utente accetta di usare il suo nome e l'email come paternità nei commit "
-"VCS. L'utente comprende che questa accettazione non è revocabile a causa "
-"della natura del VCS."
+"L'utente accetta di usare il nome e l'email come paternità nei commit VCS. "
+"L'utente comprende che questa accettazione non è revocabile a causa della "
+"natura del VCS."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -728,15 +716,15 @@
 msgstr "Legge applicabile"
 
 #: wllegal/templates/legal/documents/tos.html:125
 msgid ""
 "These Terms of Service shall be governed by the laws of the Czech Republic "
 "with exclusion of conflict rules."
 msgstr ""
-"I presenti Termini di servizio sono regolati dalle leggi della Repubblica "
+"I presenti Termini del Servizio sono regolati dalle leggi della Repubblica "
 "Ceca con esclusione delle eventuali regole in conflitto."
 
 #: wllegal/templates/legal/documents/tos.html:127
 msgid ""
 "Any disputes arising on the basis of the Agreement and/or these Terms of "
 "Service shall be resolved by the court of the Czech republic having "
 "substantive and local jurisdiction."
@@ -746,21 +734,17 @@
 "sostanziale e locale."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Effetto"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "I presenti Termini di servizio entrano in vigore dal 1 settembre 2017."
+msgstr "I presenti Termini del Servizio entrano in vigore dal 15 Maggio 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "Nel caso di acquisto del servizio, avremo bisogno di ulteriori "
 #~ "informazioni necessarie per l'emissione della fattura"
```

### Comparing `wllegal-2023.3/wllegal/locale/ja/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,35 @@
 # Kyotaro Iijima <kyotaro.eyes@gmail.com>, 2018, 2019, 2020.
 # Tetsuro Shimazaki <shimazaki@shima-office.com>, 2018, 2019, 2020.
 # Ryo Nakano <ryonakaknock3@gmail.com>, 2018, 2019.
 # Scott Anecito <scott.anecito@protonmail.com>, 2019.
 # amano <amano.hajime@gmail.com>, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-03-02 10:37+0000\n"
-"Last-Translator: maboroshin <maboroshin@users.noreply.hosted.weblate.org>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-20 18:48+0000\n"
+"Last-Translator: Kyotaro Iijima <kyotaro.eyes@gmail.com>\n"
 "Language-Team: Japanese <https://hosted.weblate.org/projects/weblate/legal/"
 "ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "GDPR 第 28 条に従う協力者"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "2020 年10 月 現在。"
+msgstr "2023 年 3 月 現在。"
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -69,24 +67,20 @@
 msgstr "Weblate は、利用者が提供する個人情報のみ使用します。"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "名前とメールアドレス"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "これらは、VCS のコミットにおいて、あなたを識別するために使用されます"
+msgstr "これらは、VCS のコミットにおいて、利用者を識別するために使用されます。"
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "また、監視中のイベントの通知にはメールを使用します"
+msgstr "また、監視中のイベントの通知にはメールを使用します。"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "ハッシュ形式のパスワード"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -97,36 +91,29 @@
 msgstr "パスワードは Argon2 でハッシュ化して保存します。"
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP アドレスとブラウザー名"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
-msgstr ""
-"アカウントが盗まれた場合の解析用に、アカウントの重要な変更 (例：パスワードの"
-"変更) のログを記録しています"
+msgstr "アカウントが盗まれた場合の解析用に、アカウントの重要な変更 "
+"(例：パスワードの変更) のログを記録しています。"
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "請求情報"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
-msgstr ""
+msgstr "請求書の発行に必要な情報は、当社からサービスを購入した時点で収集されます。"
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "個人情報の管理の目的と法的根拠"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -183,63 +170,62 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "サービスの技術的保証を契約した個人。"
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "当社からサービスを購入するときの決済事業者。"
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "すべての個人情報は EU 内で保管しています。"
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "個人情報へのアクセス"
+msgid "Disclosure of the Personal Data"
+msgstr "個人情報の開示"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"個人データは、召喚状やその他の司法または行政命令など、管理者が法律に基づく要"
+"求であると確認できた場合、限られた状況で第三者に開示される場合があります。"
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"管理者が法律により個人データの開示を求められた場合、利用者に対し事前にメール"
+"にて開示請求があった旨を通知します（禁止されている場合、または無駄な場合を除"
+"く）。利用者が開示請求に異議を唱えない場合、管理者は個人データの引き渡しを法"
+"的に要求される場合があります。"
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "個人情報の保有"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr "個人情報は、利用者がアカウントを削除するまで、サービスに保管されます。"
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
-msgstr ""
-"アクセス ログ情報は、法的な請求、行使、防御を目的として、長期間にわたって収集"
+msgstr "アクセス ログ情報は、法的な請求、行使、防御を目的として、長期間にわたって収集"
 "することがあります。"
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "お客様の権利"
 
 #: wllegal/templates/legal/documents/privacy.html:79
@@ -298,56 +284,50 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "個人情報の削除、修正、取得はアカウント管理から行うことができ、完全に自動化さ"
 "れています。"
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
-msgstr ""
-"個人情報（メールアドレスなど）は厳重に扱います。アカウントを削除した際は、"
-"データベースから即時に廃棄します。"
+msgstr "個人情報（メールアドレスなど）は厳重に扱います。アカウントを削除した際は、デ"
+"ータベースから廃棄します。"
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
-msgstr "あなたの翻訳は、各翻訳で指定されているライセンスの下で行われます。"
+msgstr "あなたの翻訳は、各翻訳で指定されているライセンスに基づいて行われます。"
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 "あなたの名前とメールアドレスは、VCS のコミットにおいて使用されます。保管に期"
 "限はありません。"
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"使用する名前の選択権はお客様にあります。コミットに使用されるメールアドレスは"
+"、プライバシーを保護するために Weblate "
+"のシステムによって隠ぺいすることができます。"
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "サービスの提供のために Cookie を使用します。"
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "サードパーティの Cookie は使用していません。"
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "英語版の表示"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -612,14 +592,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"GDPR の <a href=\"%(url)s\">第 7 条</a>が意図する範囲内で、利用者は個人データ"
+"の収集、保存、および処理に関して、<a href=\"%(privacy_url)s\""
+">プライバシーポリシー</a> に従って同意するものとする。"
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "翻訳"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -649,27 +632,22 @@
 #: wllegal/templates/legal/documents/tos.html:111
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr "利用者は、プロジェクトへの寄稿時に指定したライセンスに同意します。"
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"利用者は、VCS のコミットの作成者として自分の名前と電子メールを使用することに"
-"同意します。利用者は、VCS の仕様上、この許可が取り消し不能であることに納得し"
-"ます。"
+"利用者は、VCS のコミットの作成者として自分の名前とメールアドレスを使用するこ"
+"とに同意します。利用者は、VCS "
+"の仕様上、この許可が取り消し不能であることを理解しています。"
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -702,21 +680,17 @@
 "を有するチェコ共和国の裁判所により解決します。"
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "効力"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "これらの利用規約は、2017年9月1日に発効します。"
+msgstr "これらの利用規約は、2013 年 5 月 5 日に発効します。"
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "サービスを購入された場合、請求書の発行に必要な追加の請求情報を収集します"
```

### Comparing `wllegal-2023.3/wllegal/locale/ka/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ka/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-09-17 14:21+0000\n"
 "Last-Translator: Temuri Doghonadze <temuri.doghonadze@gmail.com>\n"
 "Language-Team: Georgian <https://hosted.weblate.org/projects/weblate/legal/"
 "ka/>\n"
 "Language: ka\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/kab/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/kab/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-01-28 08:55+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Kabyle <https://hosted.weblate.org/projects/weblate/legal/kab/"
 ">\n"
 "Language: kab\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -193,15 +193,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Meṛṛa isefka udmawanen ttwaḥerzen deg Tidukkla n Turuft."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Anekcum ɣer yisefka udmawanen"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/kk/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/kk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # WWWesten <wwwesten@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-01-28 08:55+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Kazakh <https://hosted.weblate.org/projects/weblate/legal/kk/"
 ">\n"
 "Language: kk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -215,15 +215,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Barlyq Derbes Derekter Eýropalyq Odaqta saqtalady."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Derbes Derekterge qatynaý"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/km/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/km/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2020-11-13 11:28+0000\n"
 "Last-Translator: ប៉ុកណូ រ៉ូយ៉ាល់ <royalpokno68@gmail.com>\n"
 "Language-Team: Khmer (Central) <https://hosted.weblate.org/projects/weblate/"
 "legal/km/>\n"
 "Language: km\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -181,15 +181,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/kmr/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/kmr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2018-07-23 11:06+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Kurdish <https://hosted.weblate.org/projects/weblate/master/"
 "ku/>\n"
 "Language: ku\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ko/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ko/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 # This file is distributed under the same license as the PACKAGE package.
 # 송태섭 <xotjq237@gmail.com>, 2018, 2019.
 # k ks <kmshts@naver.com>, 2019.
 # Jun Hyung Shin <shmishmi79@gmail.com>, 2019.
 # Lee Yunseok <ironyunseok@protonmail.com>, 2019, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-05-14 17:32+0000\n"
-"Last-Translator: 이정희 <daemul72@gmail.com>\n"
-"Language-Team: Korean <https://hosted.weblate.org/projects/weblate/legal/ko/"
-">\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-06-04 10:49+0000\n"
+"Last-Translator: Hoseok Seo <ddinghoya@gmail.com>\n"
+"Language-Team: Korean <https://hosted.weblate.org/projects/weblate/legal/ko/>"
+"\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "GDPR Art. 28에 따른 협력업체"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "2020년 10월 현재 상태."
+msgstr "2023년 3월 현재 상태입니다."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -69,24 +67,20 @@
 msgstr "우리는 사용자가 제공한 개인 정보만 처리합니다:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "이름과 전자우편 주소"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "이들은 VCS 커밋에서 사용자를 식별하는데 사용됩니다"
+msgstr "이는 VCS 커밋에서 사용자를 식별하는 데 사용됩니다."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "또한 전자우편은 시청한 사건의 알림에 사용됩니다"
+msgstr "또한 이메일은 시청한 이벤트의 알림에 사용됩니다."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "해시 형식의 암호"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -97,36 +91,29 @@
 msgstr "비밀번호는 Argon2를 사용하여 해시 저장됩니다."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP 주소와 브라우저 이름"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
-msgstr ""
-"계정에 중요한 변경 사항이 있을 경우 (예 : 암호 변경) 로그인하여 계정을 도난당"
-"했는 지를 진단할 수 있습니다"
+msgstr "계정에 중요한 변경 사항 (예: 비밀번호 변경)이 있는 경우 계정이 도난당했을 때 "
+"진단을 위해 기록됩니다."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "결제 정보"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
-msgstr ""
+msgstr "당사에서 서비스를 구매할 때 인보이스 발행에 필요한 세부 정보를 수집합니다."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "개인 정보 처리의 목적 및 법적 근거"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -184,65 +171,65 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "서비스의 기술 보증 계약을 맺은 사람."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "당사에서 서비스를 구매할 때 결제 처리자입니다."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "모든 개인 정보는 유럽 연합에 저장됩니다."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "개인 자료에 접근하기"
+msgid "Disclosure of the Personal Data"
+msgstr "개인 데이터 공개"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"개인 데이터는 소환장이나 기타 사법 또는 행정 명령 등 법에 의해 요구된다고 "
+"선의로 판단하는 경우 제한된 상황에서 제3자에게 개인정보를 공개할 수 있습니다."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"개인 데이터 법에 따라 개인정보를 공개해야 하는 경우, 개인 데이터는 사용자가 "
+"공개에 이의를 제기할 수 있도록 개인정보에 대한 요청이 이루어졌다는 사실을 "
+"사용자에게 이메일로 사전 통지 (개인정보처리자가 금지하거나 무의미한 경우를 "
+"제외하고)하려고 노력할 것입니다. 사용자가 공개 요청에 이의를 제기하지 않는 "
+"경우, 개인 데이터는 법적으로 개인 데이터를 넘겨야 할 수 있습니다."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "개인 자료 보존"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "개인 자료는 사용자가 서비스에서 계정을 삭제하기 전까지 서비스에 저장됩니다."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
-msgstr ""
-"액세스 로그 정보는 법적 요구의 수립, 활동 및 방어의 목적을 위해 장기간 수집됩"
-"니다."
+msgstr "접속 로그 정보는 법적 요구의 수립, 활동 및 방어의 목적을 위해 장기간 "
+"수집됩니다."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "당신의 권리"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
@@ -301,55 +288,49 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "자신의 개인 자료의 제거, 수정과 검색은 계정 관리에서 수행 할 수 있으며, 완전"
 "히 자동화되어 있습니다."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"귀하의 전자우편 주소와 같은 비공개 자료를 관리하며 귀하의 계정을 삭제하는 즉"
-"시 자료베이스에서 삭제됩니다."
+"당사는 개인 데이터(예: 귀하의 이메일 주소)를 처리하며, 귀하가 계정을 "
+"삭제하면 해당 데이터는 당사 데이터베이스에서 삭제됩니다."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
-msgstr "귀하의 번역은 각 번역본에 명시된 라이선스 하에 작성됩니다."
+msgstr "번역은 각 번역에 명시된 라이센스에 따라 이루어집니다."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 "귀하의 이름과 전자우편 주소는 VCS 커밋에 사용되며 무한정 머무를 것입니다."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"커밋에 사용되는 이메일 주소는 개인 정보 보호를 위해 웨블레이트 시스템에서 "
+"마스킹할 수 있으며, 선택한 이름은 귀하에게 달려 있습니다."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "우리는 우리의 서비스를 제공하기 위해 쿠키를 사용합니다."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "당사는 타사 쿠키를 사용하지 않습니다."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "영어 버전 보기"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -617,14 +598,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"<a href=\"%(url)s\">제7조</a>의 의미 내에서 사용자는 <a href=\"%(privacy_url)"
+"s\">개인정보 처리방침</a>에 따라 개인정보를 수집, 저장 및 처리하는 데 "
+"동의합니다."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "번역"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -654,27 +638,21 @@
 #: wllegal/templates/legal/documents/tos.html:111
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr "사용자는 프로젝트에 기여할 때 지정된 라이선스에 동의합니다."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"사용자는 이름과 전자우편을 버전 관리 시스템(VCS) 커밋에 저작자로 사용하는 것"
-"에 동의합니다. 사용자는 이 허가가 VCS의 특성으로 인해 취소할 수 없음을 이해합"
-"니다."
+"사용자는 VCS 커밋에서 이름과 이메일을 권한으로 사용하는 데 동의합니다. "
+"사용자는 VCS의 특성상 이 권한 부여가 취소할 수 없음을 이해합니다."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -707,21 +685,17 @@
 "관할권을 보유한 체코 공화국 법원에 의해 해결됩니다."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "효과"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "본 서비스 약관은 2017 년 9월 1일 부터 시행되며 효력을 발휘합니다."
+msgstr "본 서비스 약관은 2023년 5월 15일부터 발효됩니다."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "우리에게서 서비스를 구매하는 경우, 우리는 청구서 발행을 위해 필요한 추가 "
 #~ "결제 정보를 모읍니다"
```

### Comparing `wllegal-2023.3/wllegal/locale/ksh/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ksh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2014-10-01 09:41+0200\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Colognian <https://hosted.weblate.org/projects/weblate/master/"
 "ksh/>\n"
 "Language: ksh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -168,15 +168,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ln/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ln/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2017-11-26 20:48+0000\n"
 "Last-Translator: Jean-Maurice Omankoy <jean_mau@hotmail.com>\n"
 "Language-Team: Lingala <https://hosted.weblate.org/projects/weblate/master/"
 "ln/>\n"
 "Language: ln\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -164,15 +164,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/lt/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/lt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # anonymous <noreply@weblate.org>, 2019.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2019-07-22 07:40+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Lithuanian <https://hosted.weblate.org/projects/weblate/"
 "hosted/lt/>\n"
 "Language: lt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -169,15 +169,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/lv/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/lv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-11-07 19:02+0000\n"
 "Last-Translator: Coool (github.com/Coool) <coool@mail.lv>\n"
 "Language-Team: Latvian <https://hosted.weblate.org/projects/weblate/legal/lv/"
 ">\n"
 "Language: lv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -200,15 +200,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Visi personas dati tiek glabāti Eiropas Savienībā."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Piekļuve personas datiem"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/lzh/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ro_MD/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: lzh\n"
+"Language: ro_MD\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/mk/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/mk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2019-07-22 07:40+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Macedonian <https://hosted.weblate.org/projects/weblate/"
 "hosted/mk/>\n"
 "Language: mk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -161,15 +161,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ml/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ml/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2020-12-22 00:29+0000\n"
 "Last-Translator: vachan-maker <vachan2014carmel@gmail.com>\n"
 "Language-Team: Malayalam <https://hosted.weblate.org/projects/weblate/legal/"
 "ml/>\n"
 "Language: ml\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/mr/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/mr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # Prachi Joshi <josprachi@yahoo.com>, 2019, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-01-28 08:55+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Marathi <https://hosted.weblate.org/projects/weblate/legal/mr/"
 ">\n"
 "Language: mr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -164,15 +164,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ms/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/si/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ms\n"
+"Language: si\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/my/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/my/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2020-07-31 06:28+0000\n"
 "Last-Translator: Sithu Aung <sithu.aung015@gmail.com>\n"
 "Language-Team: Burmese <https://hosted.weblate.org/projects/weblate/legal/my/"
 ">\n"
 "Language: my\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -164,15 +164,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "ပုဂ္ဂိုလ်ရေး အချက်အလက် ရယူသုံးစွဲမှု"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/nb/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/nb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # ButterflyOfFire <ButterflyOfFire@protonmail.com>, 2018.
 # Kurt Eilertsen <kurt@kheds.com>, 2018.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-03-19 07:31+0000\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/weblate/"
 "legal/nb_NO/>\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -203,15 +203,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "All personlig data er lagret i den europeiske unionen."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Tilgang til personlige data"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/nl/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/nl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 # Thomas De Rocker <thomasderocker@outlook.com>, 2018, 2019.
 # Frans de Jonge <fransdejonge+weblate.org@gmail.com>, 2019.
 # Jaimie85 <alsemgeest@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-09-22 15:42+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-15 13:29+0000\n"
 "Last-Translator: Heimen Stoffels <vistausss@fastmail.com>\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/weblate/legal/nl/"
 ">\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subondernemers conform artikel 28 van de GPDR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Status vanaf oktober 2020."
+msgstr "Status vanaf maart 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -70,25 +68,21 @@
 "verstrekt:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Naam en e-mailadres"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Deze worden gebruikt om u te identificeren in VCS-commits"
+msgstr "Deze worden gebruikt om u te identificeren in VCS-commits."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"Uw e-mailadres wordt ook gebruikt voor melding van gevolgde gebeurtenissen"
+"Uw e-mailadres wordt ook gebruikt voor melding van gevolgde gebeurtenissen."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Wachtwoord in hash-vorm"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -99,29 +93,23 @@
 msgstr "Wachtwoorden worden versleuteld opgeslagen met Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP-adres en browsernaam"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Deze worden bijgehouden in geval van belangrijke wijzigingen aan uw account "
 "(bijvoorbeeld wachtwoordwijziging), voor een diagnose in geval van een "
-"gestolen account"
+"gestolen account."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Facturatie-informatie"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
@@ -204,15 +192,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Alle persoonlijke gegevens worden opgeslagen in de Europese Unie."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Toegang tot de persoonlijke gegevens"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -237,18 +225,14 @@
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "De persoonlijke gegevens worden in de dienst opgeslagen totdat de gebruiker "
 "zijn account in de dienst verwijdert."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Toegangslogboek-informatie kan voor een langere periode verzameld worden met "
 "het oog op vaststelling, uitoefening of verdediging van rechtsvorderingen."
 
@@ -318,58 +302,52 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "U kunt uw persoonlijke gegevens wissen, aanpassen en benaderen via "
 "accountbeheer. Dit proces is volledig geautomatiseerd."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
 "Wij verwerken persoonlijke gegevens (zoals uw e-mailadres). Deze worden uit "
-"onze database verwijderd zodra u uw account verwijdert."
+"onze databank verwijderd als u uw account verwijdert."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
-"Uw vertalingen worden gemaakt onder licentie die door elke vertaling wordt "
-"opgegeven."
+"Uw vertalingen worden gemaakt onder de licentie die door elke vertaling "
+"wordt opgegeven."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 "Uw naam en e-mailadres worden gebruikt in VCS commits. Ze blijven daar voor "
 "onbepaalde tijd."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Een naam kan naar eigen inzicht worden gekozen. Het e-mailadres van commits "
+"kan door Weblate worden verborgen om uw privacy te waarborgen."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "We gebruiken cookies om onze diensten aan te bieden."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "We maken geen gebruik van externe cookies."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Engelstalige versie lezen"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
```

### Comparing `wllegal-2023.3/wllegal/locale/nn/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/tt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: nn\n"
+"Language: tt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/oc/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/oc/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: oc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -158,15 +158,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/or/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/crh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Weblate <noreply@weblate.org>, 2019.
+# Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: or\n"
+"Language: crh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -156,15 +156,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/pa/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/pa/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Sanjna <r.sanjna@yahoo.com>, 2019.
 # Aman ALam <alam.yellow@gmail.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-02-12 23:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Punjabi <https://hosted.weblate.org/projects/weblate/legal/pa/"
 ">\n"
 "Language: pa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -164,15 +164,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/pa_PK/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/uz/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-10-24 16:14+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-02-12 16:39+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Punjabi (Pakistan) <https://hosted.weblate.org/projects/"
-"weblate/legal/pa_PK/>\n"
-"Language: pa_PK\n"
+"Language-Team: Uzbek <https://hosted.weblate.org/projects/weblate/legal/uz/"
+">\n"
+"Language: uz\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.14.2-dev\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -338,15 +338,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "کوکیاں"
+msgstr "Cookies"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -380,15 +380,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "نِجی ڈیٹا"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -399,15 +399,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "پروجیکٹ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -435,15 +435,15 @@
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "ورژن کنترول سسٹم"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
```

### Comparing `wllegal-2023.3/wllegal/locale/peo/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/pa_PK/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-09-04 12:20+0000\n"
-"Last-Translator: sayyed hamed nasib <cghamed752@chmail.ir>\n"
-"Language-Team: Persian (Old) <https://hosted.weblate.org/projects/weblate/"
-"legal/peo/>\n"
-"Language: peo\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2022-10-24 16:14+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Punjabi (Pakistan) <https://hosted.weblate.org/projects/"
+"weblate/legal/pa_PK/>\n"
+"Language: pa_PK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1-dev\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"X-Generator: Weblate 4.14.2-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -338,15 +338,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr ""
+msgstr "کوکیاں"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -370,25 +370,25 @@
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr "ارائه دهنده"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "نِجی ڈیٹا"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -399,15 +399,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr ""
+msgstr "پروجیکٹ"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -435,15 +435,15 @@
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr ""
+msgstr "ورژن کنترول سسٹم"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
```

### Comparing `wllegal-2023.3/wllegal/locale/pl/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/pl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,36 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Piotr Sokół <psokol.l10n@gmail.com>, 2016.
 # WaldiS <admin@sto.ugu.pl>, 2018, 2019.
 # Stanisław Krukowski <pet209a1@riseup.net>, 2018.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-10-21 09:56+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-20 18:48+0000\n"
 "Last-Translator: Agnieszka C <aga_04@o2.pl>\n"
-"Language-Team: Polish <https://hosted.weblate.org/projects/weblate/legal/pl/"
-">\n"
+"Language-Team: Polish <https://hosted.weblate.org/projects/weblate/legal/pl/>"
+"\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Podwykonawcy zgodnie z Art. 28 RODO"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Stan na październik 2020."
+msgstr "Stan na marzec 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -71,25 +69,21 @@
 "ich użyciu:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Nazwa i adres e-mail"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Służą one do identyfikacji użytkownika w commitach na VCS"
+msgstr "Służą one do identyfikacji użytkownika w commitach na VCS."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"Ponadto wiadomość e-mail służy do powiadamiania o obserwowanych zdarzeniach"
+"Ponadto wiadomość e-mail służy do powiadamiania o obserwowanych zdarzeniach."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Hasło w formie haszowanej"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -100,36 +94,31 @@
 msgstr "Hasła są przechowywane w postaci zaszyfrowanej przy użyciu Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "Adres IP i nazwa przeglądarki"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Są one rejestrowane w przypadku ważnych zmian na koncie (np. Zmiana hasła) w "
-"celu umożliwienia diagnozy w przypadku kradzieży konta"
+"Są one rejestrowane w przypadku ważnych zmian na koncie (np. zmiana hasła) w "
+"celu umożliwienia diagnozy w przypadku kradzieży konta."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Informacje rozliczeniowe"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Dane niezbędne do wystawienia faktury zbierane są przy zakupie u nas usługi."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Cel i podstawa prawna przetwarzania danych osobowych"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -192,60 +181,65 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Osoby, które są objęte umową o zapewnienie techniczne usługi."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Podmioty przetwarzające płatności przy zakupie u nas usługi."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Wszystkie dane osobowe są przechowywane w Unii Europejskiej."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Dostęp do danych osobowych"
+msgid "Disclosure of the Personal Data"
+msgstr "Ujawnienie danych osobowych"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Dane Osobowe mogą zostać ujawnione stronom trzecim w ograniczonych "
+"okolicznościach, gdy Administrator w dobrej wierze uważa, że jest to "
+"wymagane przez prawo, na przykład na podstawie wezwania sądowego lub innego "
+"nakazu sądowego, lub administracyjnego."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"W przypadku gdy przepisy prawa zobowiązują Administratora do ujawnienia "
+"Danych Osobowych, zostanie podjęta próba uprzedniego powiadomienia "
+"Użytkownika drogą elektroniczną (o ile Administrator nie zabrania lub byłoby "
+"to daremne), że żądanie udostępnienia Danych Osobowych zostało dokonane w "
+"celu umożliwienia Użytkownikowi wyrażenia sprzeciwu wobec ujawnienia. Jeżeli "
+"Użytkownik nie zakwestionuje żądania ujawnienia, Administrator może być "
+"prawnie zobowiązany do przekazania Danych Osobowych."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "Przechowywanie danych osobowych"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Dane osobowe są przechowywane w serwisie, dopóki użytkownik nie usunie "
 "swojego konta w usłudze."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Informacje z dziennika dostępu mogą być gromadzone przez dłuższy okres w "
 "celu ustalenia, wykonania lub obrony roszczeń prawnych."
 
@@ -312,58 +306,52 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "Usuwanie, poprawianie i odzyskiwanie swoich danych osobowych może odbywać "
 "się z poziomu zarządzania kontem i jest w pełni zautomatyzowane."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Przetwarzamy prywatne dane (takie jak adres e-mail), które zostaną usunięte "
-"z naszej bazy danych, gdy tylko usuniesz swoje konto."
+"Przetwarzamy dane osobowe (takie jak Twój adres e-mail); zostaną one "
+"usunięte z naszej bazy danych, jeśli usuniesz swoje konto."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
-"Twoje tłumaczenia są tworzone na licencji specyficznej dla każdego "
-"tłumaczenia."
+"Twoje tłumaczenia są wykonywane na licencji określonej przy każdym "
+"tłumaczeniu."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 "Twoje imię, nazwisko i adres e-mail są używane w commitach na VCS i "
 "pozostaną tam na stałe."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Wybrana nazwa zależy od Ciebie, a adres e-mail używany do commitów może być "
+"maskowany przez system Weblate w celu ochrony Twojej prywatności."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Używamy ciasteczek do świadczenia naszych usług."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Nie używamy żadnych plików cookie stron trzecich."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Zobacz wersję angielską"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -647,14 +635,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"W rozumieniu <a href=\"%(url)s\">art. 7</a> RODO Użytkownik niniejszym "
+"wyraża zgodę na gromadzenie, przechowywanie i przetwarzanie Danych Osobowych "
+"zgodnie z <a href=\"%(privacy_url)s \">Polityka prywatności</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Tłumaczenia"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -687,27 +678,22 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "Użytkownik, zgadzając się na udział w Projekcie, wyraża zgodę na licencję "
 "określoną przez Projekt."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"Użytkownik zgadza się używać własnego nazwiska i adresu e-mail jako "
-"autorstwa w commitach na VCS. Użytkownik rozumie, że tego grantu nie można "
-"odwołać ze względu na charakter VCS."
+"Użytkownik wyraża zgodę na używanie imienia i nazwiska oraz adresu e-mail "
+"jako autorstwa w commitach na VCS. Użytkownik rozumie, że przyznanie to jest "
+"nieodwołalne ze względu na charakter VCS."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -743,23 +729,18 @@
 "merytoryczną i lokalną."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Efekt"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-"Niniejsze Warunki świadczenia usług wchodzą w życie z dniem 1 września 2017 "
-"r."
+"Niniejsze Warunki świadczenia usług wchodzą w życie z dniem 15 maja 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "W przypadku zakupu usługi od nas, zbieramy dodatkowe informacje "
 #~ "rozliczeniowe niezbędne do wystawienia faktury"
```

### Comparing `wllegal-2023.3/wllegal/locale/ps/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/dv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ps\n"
+"Language: dv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/pt/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/pt/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Pedro Albuquerque <palbuquerque73@gmail.com>, 2018.
 # ssantos <ssantos@web.de>, 2018, 2019.
 # Pedro Albuquerque <pmra@gmx.com>, 2019.
 # Manuela Silva <mmsrs@sky.com>, 2019, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-10-21 09:56+0000\n"
-"Last-Translator: SC <lalocas@protonmail.com>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-29 10:51+0000\n"
+"Last-Translator: ssantos <ssantos@web.de>\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/weblate/legal/"
 "pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Subcontratados de acordo com o art. 28 RGPD"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Estado em outubro de 2020."
+msgstr "Estado de março de 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -71,26 +69,20 @@
 "utilizando-os:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Nome e endereço de ''e-mail''"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Estes são utilizados para identificá-lo nas submissões de VCS"
+msgstr "Estes são utilizados para identificá-lo nas submissões de VCS."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr ""
-"Adicionalmente, o ''e-mail'' é utilizado para a notificação de eventos "
-"vigiados"
+msgstr "Além disso, o email é usado para a notificação de eventos observados."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Palavra-passe em formato \"hash\""
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -206,15 +198,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Todos os \"Dados Pessoais\" são guardados na União Europeia."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Acesso aos Dados Pessoais"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/pt_BR/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Luiz Fernando Ranghetti <elchevive@opensuse.org>, 2018.
 # Rafael Fontenelle <rafaelff@gnome.org>, 2018, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-11-11 23:03+0000\n"
 "Last-Translator: Felipe <felipefplzx@gmail.com>\n"
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
 "weblate/legal/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -195,15 +195,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Todos os Dados Pessoais são armazenados na União Europeia."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Acesso aos Dados Pessoais"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/pt_PT/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-12-05 00:50+0000\n"
 "Last-Translator: ssantos <ssantos@web.de>\n"
 "Language-Team: Portuguese (Portugal) <https://hosted.weblate.org/projects/"
 "weblate/legal/pt_PT/>\n"
 "Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -204,15 +204,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Todos os \"Dados Pessoais\" são guardados na União Europeia."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Acesso aos Dados Pessoais"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ro/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # Romanian translations for PACKAGE package.
 # Copyright (C) 2014 THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-10-21 09:56+0000\n"
-"Last-Translator: Simona Iacob <s@zp1.net>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-25 14:51+0000\n"
+"Last-Translator: Licaon Kter <licaon.kter@protonmail.com>\n"
 "Language-Team: Romanian <https://hosted.weblate.org/projects/weblate/legal/"
 "ro/>\n"
 "Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
 "20)) ? 1 : 2;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 "Subcontractanți în conformitate cu art. 28 GDPR (Regulamentul general "
 "privind protecția datelor)"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Situația din octombrie 2020."
+msgstr "Situația din martie 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -72,25 +70,21 @@
 "le furnizează prin utilizarea acestuia:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Numele și adresa de e-mail"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Acestea sunt folosite pentru a vă identifica în VCS commits"
+msgstr "Acestea sunt folosite pentru a vă identifica în cadrul editărilor VCS."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"În plus, e-mailul este utilizat pentru notificarea evenimentelor urmărite"
+"În plus, e-mailul este utilizat pentru notificarea evenimentelor urmărite."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Parola în formă hașurată"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -101,29 +95,23 @@
 msgstr "Parolele sunt stocate sub formă de hash folosind Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "Adresa IP și numele browserului"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Acestea sunt înregistrate în cazul unor modificări importante ale contului "
 "dvs. (de exemplu, schimbarea parolei) pentru a permite diagnosticarea în "
-"cazul în care contul dvs. este furat"
+"cazul în care contul dvs. este furat."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Informații de facturare"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
@@ -206,15 +194,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Toate datele cu caracter personal sunt stocate în Uniunea Europeană."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Accesul la datele cu caracter personal"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ro_MD/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ia/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Weblate <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ro_MD\n"
+"Language: ia\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +156,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ru/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,36 @@
 # WWWesten <wwwesten@gmail.com>, 2019.
 # solokot <solokot@gmail.com>, 2019.
 # Andrei Stepanov <adem4ik@gmail.com>, 2019.
 # Vadim Nekhai <vadimnekhai@gmail.com>, 2019.
 # Golubev Alexander <fatzer2@gmail.com>, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-01-06 19:48+0000\n"
-"Last-Translator: Артём Котлубай <artemkotlubai@yandex.ru>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-06-07 10:50+0000\n"
+"Last-Translator: S3aBreeze <S3aBreeze@users.noreply.hosted.weblate.org>\n"
 "Language-Team: Russian <https://hosted.weblate.org/projects/weblate/legal/ru/"
 ">\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.15.1-dev\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Субподрядчики в соответствии со ст. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Состояние на октябрь 2020 года."
+msgstr "Состояние на март 2023 года."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -77,25 +75,21 @@
 "предоставляет при использования нашей услуги:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Имя и адрес эл. почты"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Используются для идентификации в VCS-коммитах"
+msgstr "Используются для идентификации в VCS-коммитах."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
 msgstr ""
-"Кроме того, эл. почта используется для уведомлений об отслеживаемых событиях"
+"Кроме того, эл. почта используется для уведомлений об отслеживаемых событиях."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Пароль в хэшированном виде"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -106,29 +100,23 @@
 msgstr "Пароли хранятся хэшированными с помощью Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP-адрес и название браузера"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Они журналируются на случай существенных изменений в вашей учётной записи "
-"(например, смена пароля), чтобы позволить диагностику в случае кражи вашей "
-"учётной записи"
+"Они журналируются на случай существенных изменений в вашей учётной записи ("
+"например, смена пароля), чтобы позволить диагностику в случае кражи вашей "
+"учётной записи."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Платёжная информация"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
@@ -207,15 +195,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Все личностные данные хранятся в Европейском союзе."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Доступ к личностным данным"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/sc/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/sc/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: sc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -158,15 +158,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/si/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ie/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: si\n"
+"Language: ie\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/sk/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/sk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Michal Čihař <michal@cihar.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 # Ivan Pleva <ivan.pleva@tutanota.com>, 2019, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-09-25 20:39+0000\n"
 "Last-Translator: Milan <mobrcian@hotmail.com>\n"
 "Language-Team: Slovak <https://hosted.weblate.org/projects/weblate/legal/sk/"
 ">\n"
 "Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -199,15 +199,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Všetky Osobné údaje sa uchovávajú v Európskej únii."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Prístup k Osobným údajom"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/skr/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/skr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2023-04-01 00:26+0000\n"
 "Last-Translator: پرویز قادر <mpqadir@gmail.com>\n"
 "Language-Team: Saraiki <https://hosted.weblate.org/projects/weblate/legal/"
 "skr/>\n"
 "Language: skr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -166,15 +166,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "سارا ذاتی ڈیٹا یورپی یونین وچ سٹور تھیندا ہے۔"
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "ذاتی ڈیٹا تے رسائی"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/sl/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/sl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Domen <mitenem@outlook.com>, 2018, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-01-07 02:39+0000\n"
 "Last-Translator: Matej U <mateju@src.gnome.org>\n"
 "Language-Team: Slovenian <https://hosted.weblate.org/projects/weblate/legal/"
 "sl/>\n"
 "Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -175,15 +175,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Allow changes in the local repository"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Dovoli spremembe v lokalni shrambi"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/sq/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/sq/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Automatically generated, 2014.
 # Michal Čihař <michal@cihar.com>, 2019.
 # Besnik Bleta <besnik@programeshqip.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-12-14 21:49+0000\n"
 "Last-Translator: Besnik Bleta <besnik@programeshqip.org>\n"
 "Language-Team: Albanian <https://hosted.weblate.org/projects/weblate/legal/"
 "sq/>\n"
 "Language: sq\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -200,15 +200,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Krejt të Dhënat Personale depozitohen në Bashkimin Europian."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Përdorim të Dhëna Personale"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/sr/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/sr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Branko Kokanovic <branko@kokanovic.org>, 2018.
 # Z. Cs. <zbus021@gmail.com>, 2019.
 # anonymous <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-02-11 21:50+0000\n"
 "Last-Translator: Слободан Симић(Slobodan Simić) <slsimic@gmail.com>\n"
 "Language-Team: Serbian <https://hosted.weblate.org/projects/weblate/legal/sr/"
 ">\n"
 "Language: sr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -172,15 +172,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Сви лични подаци су смештени у Европској унији."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Приступ личним подацима"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/sr_Latn/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/sr_Latn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Nikola Perović <nikolaperovicccc@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-02-09 02:02+0000\n"
 "Last-Translator: Слободан Симић(Slobodan Simić) <slsimic@gmail.com>\n"
 "Language-Team: Serbian (latin) <https://hosted.weblate.org/projects/weblate/"
 "legal/sr_Latn/>\n"
 "Language: sr_Latn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -169,15 +169,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Svi lični podaci su smešteni u Evropskoj uniji."
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Pristup ličnim podacima"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/sv/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/sv/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # Jonatan Nyberg <jonatan.nyberg.karl@gmail.com>, 2018, 2019.
 # Johan Jacobsson <johan.jacobsson@telia.com>, 2018, 2019.
 # Filip Bengtsson <filipbengtsson@live.se>, 2019.
 # G Ran Berg <jagflashardinxbox360@gmail.com>, 2019.
 # Mattias Münster <mattiasmun@gmail.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-10-24 16:18+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-27 08:16+0000\n"
 "Last-Translator: Johan Jacobsson <johan.jacobsson@telia.com>\n"
 "Language-Team: Swedish <https://hosted.weblate.org/projects/weblate/legal/sv/"
 ">\n"
 "Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Underleverantörer i enlighet med artikel 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Status i oktober 2020."
+msgstr "Status i mars 2023."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -68,24 +66,20 @@
 "genom att använda den:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Användarnamn och mejl"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Dessa används för att identifiera dig i VCS-arkiveringar"
+msgstr "Dessa används för att identifiera dig i VCS-arkiveringar."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "Dessutom används mejl-adressen för aviseringar om bevakade händelser"
+msgstr "Dessutom används mejladressen för aviseringar om bevakade händelser."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Lösenordet i hashat format"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -96,36 +90,32 @@
 msgstr "Lösenord lagras hashade med Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP-adress och webbläsarnamn"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Dessa loggas vid viktiga ändringar i ditt konto (t. ex. lösenordsändring) "
-"för att tillåta diagnos om ditt konto blir stulet"
+"för att tillåta diagnos om ditt konto blir stulet."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Faktureringsinformation"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Nödvändiga uppgifter för att utfärda en faktura samlas in när du köper en "
+"tjänst från oss."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Syfte och rättslig grund för behandling av personuppgifter"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -186,60 +176,66 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Personer som anlitas för teknisk försäkran om tjänsten."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Betalningsprocessorer när du köper en tjänst från oss."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Alla personuppgifter lagras i Europeiska unionen."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Åtkomst till persondata"
+msgid "Disclosure of the Personal Data"
+msgstr "Utlämnande av personuppgifter"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Personuppgifterna kan lämnas ut till tredje part under begränsade "
+"omständigheter när den personuppgiftsansvarige i god tro anser att det krävs "
+"enligt lag, t.ex. enligt en stämning eller annat rättsligt eller "
+"administrativt beslut."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Om den personuppgiftsansvarige enligt lag är skyldig att avslöja "
+"personuppgifterna, kommer ett försök att göras för att ge användaren "
+"förhandsmeddelande via mejl (såvida inte den personuppgiftsansvarige är "
+"förbjuden, eller det skulle vara meningslöst) om en begäran om "
+"personuppgifterna har gjorts för att användaren ska kunna invända mot "
+"utlämnandet. Om Användaren inte ifrågasätter begäran om utlämnande kan den "
+"personuppgiftsansvarige vara juridiskt skyldig att lämna över "
+"Personuppgifterna."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "Lagringen av personuppgifter"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Persondata lagras i tjänsten tills användaren raderar sitt konto hos "
 "tjänsten."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Åtkomstlogginformation kan samlas in under en längre tid för att fastställa, "
 "utöva eller försvara rättsliga anspråk."
 
@@ -307,56 +303,51 @@
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
 "Borttagning, korrigering och hämtning av dina personuppgifter kan göras från "
 "kontohanteringen och är helt automatiserad."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Vi behandlar privata data (till exempel din e-postadress), de kommer att "
-"kasseras från vår databas så snart du tar bort ditt konto."
+"Vi behandlar personuppgifter (t.ex. din mejladress). De kommer att tas bort "
+"från vår databas om du tar bort ditt konto."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
-msgstr "Dina översättningar görs under licens som anges av varje översättning."
+msgstr ""
+"Dina översättningar görs under den licens som anges för varje översättning."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 "Ditt namn och din e-postadress används i VCS-åtaganden, den kommer att "
 "stanna där på obestämd tid."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Valet av namn är upp till dig och den mejladress som används för åtaganden "
+"kan maskeras av Weblate-systemet för att skydda din integritet."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Vi använder kakor för att leverera våra tjänster."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Vi använder inga cookies från tredje part."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Visa versionen på engelska"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -637,14 +628,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"I enlighet med <a href=\"%(url)s\">artikel 7</a> i GDPR ger användaren "
+"härmed sitt samtycke till insamling, lagring och behandling av "
+"personuppgifterna enligt <a href=\"%(privacy_url)s\">Integritetspolicyn</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Översättningar"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -677,27 +671,22 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "Användaren samtycker, vid bidrag till ett projekt, till licensen som "
 "projektet har specificerat."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"Användaren samtycker till att använda eget namn och e-post som författarskap "
-"i VCS begår. Användaren förstår att detta bidrag inte kan återkallas på "
-"grund av arten av VCS."
+"Användaren samtycker till att namn och mejladress används som författarskap "
+"i VCS Commits. Användaren är införstådd med att detta bidrag inte kan "
+"återkallas på grund av VCS:s natur."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -733,21 +722,18 @@
 "lokal jurisdiktion."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Effekt"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "Dessa användarvillkor träder i kraft den 1 september 2017."
+msgstr ""
+"Dessa användarvillkor träder i kraft och gäller från och med den 15 maj 2023."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "Om du köper tjänst från oss, samlar vi in ytterligare "
 #~ "faktureringsinformation som är nödvändig för att utfärda en faktura"
```

### Comparing `wllegal-2023.3/wllegal/locale/sw/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/tlh/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
+# Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: sw\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2019-07-22 07:41+0000\n"
+"Last-Translator: Michal Čihař <michal@cihar.com>\n"
+"Language-Team: Klingon <https://hosted.weblate.org/projects/weblate/hosted/"
+"tlh/>\n"
+"Language: tlh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 3.8-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -159,15 +159,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -398,15 +398,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr ""
+msgstr "jInmol"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -414,16 +414,18 @@
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
+#, fuzzy
+#| msgid "New password (again)"
 msgid "Translation Memory"
-msgstr ""
+msgstr "mu'wIj chu' (jatlhqa')"
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
@@ -522,15 +524,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr ""
+msgstr "mughmeH"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -593,7 +595,12 @@
 msgid "Effect"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
+
+#, fuzzy
+#~| msgid "Last name"
+#~ msgid "Repositories limit"
+#~ msgstr "pong Qav"
```

### Comparing `wllegal-2023.3/wllegal/locale/ta/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ta/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-01-13 15:57+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Tamil <https://hosted.weblate.org/projects/weblate/legal/ta/"
 ">\n"
 "Language: ta\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -168,15 +168,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/te/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ps/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: te\n"
+"Language: ps\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/th/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/th/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-04-05 12:11+0000\n"
-"Last-Translator: TopTheWorst <topbkk57@gmail.com>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-27 08:16+0000\n"
+"Last-Translator: สุริยา ชอบชอยยิกๆๆ <kkbaatlove@gmail.com>\n"
 "Language-Team: Thai <https://hosted.weblate.org/projects/weblate/legal/th/>\n"
 "Language: th\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.12-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr ""
+msgstr "ผู้ทำสัญญาช่วงตามที่บัญญัติในมาตรา 28 แห่ง GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
-msgstr ""
+msgstr "kkbaatlove1"
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -38,15 +38,15 @@
 #| msgid "Versions"
 msgid "Personal Data Controller"
 msgstr "รุ่น"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr ""
+msgstr "%(provider)s, เลขจดทะเบียน %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
@@ -163,15 +163,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/tlh/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/tok/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Michal Čihař <michal@cihar.com>, 2019.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2019-07-22 07:41+0000\n"
-"Last-Translator: Michal Čihař <michal@cihar.com>\n"
-"Language-Team: Klingon <https://hosted.weblate.org/projects/weblate/hosted/"
-"tlh/>\n"
-"Language: tlh\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-04-28 16:51+0000\n"
+"Last-Translator: Sena <jn-sena@proton.me>\n"
+"Language-Team: Toki Pona <https://hosted.weblate.org/projects/weblate/legal/"
+"tok/>\n"
+"Language: tok\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 3.8-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -159,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -379,15 +380,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "sona jan"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
@@ -398,15 +399,15 @@
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
-msgstr "jInmol"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
@@ -414,18 +415,16 @@
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:60
-#, fuzzy
-#| msgid "New password (again)"
 msgid "Translation Memory"
-msgstr "mu'wIj chu' (jatlhqa')"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:61
 msgid "means the optional translation memory service provided within Weblate"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:63
 msgid "User"
@@ -524,15 +523,15 @@
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
-msgstr "mughmeH"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
@@ -595,12 +594,7 @@
 msgid "Effect"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:132
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
 msgstr ""
-
-#, fuzzy
-#~| msgid "Last name"
-#~ msgid "Repositories limit"
-#~ msgstr "pong Qav"
```

### Comparing `wllegal-2023.3/wllegal/locale/tok/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/peo/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-04-28 16:51+0000\n"
-"Last-Translator: Sena <jn-sena@proton.me>\n"
-"Language-Team: Toki Pona <https://hosted.weblate.org/projects/weblate/legal/"
-"tok/>\n"
-"Language: tok\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2022-09-04 12:20+0000\n"
+"Last-Translator: sayyed hamed nasib <cghamed752@chmail.ir>\n"
+"Language-Team: Persian (Old) <https://hosted.weblate.org/projects/weblate/"
+"legal/peo/>\n"
+"Language: peo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.14.1-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
 msgid "Status as of March 2023."
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -370,25 +370,25 @@
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr ""
+msgstr "ارائه دهنده"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "sona jan"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.3/wllegal/locale/tr/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/tr/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,511 +4,509 @@
 # Emin Tufan Çetin <etcetin@gmail.com>, 2018, 2020.
 # MESUT AKCAN <makcan@gmail.com>, 2018.
 # Mesut Akcan <makcan@gmail.com>, 2019.
 # Burak Yavuz <hitowerdigit@hotmail.com>, 2019.
 # Ali Demirtas <alidemirtas94@gmail.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-01-31 21:41+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-06-09 16:48+0000\n"
 "Last-Translator: Kaya Zeren <kayazeren@gmail.com>\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/weblate/legal/tr/"
 ">\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
-msgstr "GPDR'nin 28. Maddesi uyarınca alt yükleniciler"
+msgstr "GPDR 28. maddesi uyarınca alt yükleniciler"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Ekim 2020 itibarıyla durum."
+msgstr "2020 Ekim ayındaki durum."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 "GDPR olarak da bilinen Genel Veri Koruma Yönetmeliği %(law_679_2016)s sayılı "
-"Yönetmeliğe uyuyoruz. Bu belge gerekli özellikleri içermektedir."
+"yönetmeliğe uyuyoruz. Bu belgede gerekli tanımlar bulunmaktadır."
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "Kişisel Veri Denetleyici"
+msgstr "Kişisel Veri Sorumlusu"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, Kayıt. No. %(reg_no)s"
+msgstr "%(provider)s, Sicil No. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
-"Weblate %(privacy_contact)s aracılığıyla ulaşılabilecek bir veri koruma "
-"görevlisi atadı."
+"Weblate %(privacy_contact)s üzerinden ulaşılabilecek bir Veri Koruma "
+"Sorumlusu atadı."
 
 #: wllegal/templates/legal/documents/privacy.html:17
 msgid "Personal Data processed by Weblate"
 msgstr "Weblate tarafından işlenen Kişisel Veriler"
 
 #: wllegal/templates/legal/documents/privacy.html:20
 msgid "Weblate only processes Personal Data the User provides by using it:"
-msgstr "Weblate, yalnızca Kullanıcının sağladığı Kişisel Verileri kullanır:"
+msgstr ""
+"Weblate, yalnızca kullanıcı tarafından verilen Kişisel Veriler’i kullanır:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
-msgstr "İsim ve e-posta adresi"
+msgstr "Ad ve e-posta adresi"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Bunlar VCS işlemelerinde sizi tanımlamak için kullanılır"
+msgstr ""
+"Bunlar sürüm denetimi sistemi gönderimlerinde sizi tanımlamak için "
+"kullanılır."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "Ek olarak, e-posta izlenen etkinliklerin bildirimi için kullanılır"
+msgstr ""
+"Ek olarak, e-posta adresi izlenen etkinlikleri bildirmek için kullanılır."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
-msgstr "Sağlama biçiminde parola"
+msgstr "Karılmış biçimde parola"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
 msgstr "Yapılandırılmışsa, Kullanıcının kimliğini doğrulamak için kullanılır"
 
 #: wllegal/templates/legal/documents/privacy.html:31
 msgid "Passwords are stored hashed using Argon2."
-msgstr "Parolalar, Argon2 kullanılarak karma olarak saklanır."
+msgstr "Parolalar, Argon2 kullanılarak karılmış olarak kaydedilir."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP adresi ve tarayıcı adı"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"Bunlar, hesabınızda önemli değişiklikler olduğunda (örn. parola değişikliği) "
-"hesabınızın çalınması durumunda tanıya izin vermek için günlüklenir"
+"Hesabınızda önemli değişiklikler olduğunda (parola değişikliği gibi) "
+"hesabınızın çalınması gibi durumlarda tanılamayı sağlamak bu bilgilerin "
+"günlük kaydı alınır."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Fatura bilgileri"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"Bizden bir hizmet satın alındığında fatura düzenlemek için gerekli bilgiler "
+"alınır."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
-msgstr "Kişisel Verilerin işlenmesinin amacı ve yasal dayanağı"
+msgstr "Kişisel Veriler’in işlenmesinin amacı ve yasal dayanağı"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
-msgstr "Kişisel Verileriniz, Hizmet işlemleri için kullanılacaktır:"
+msgstr "Kişisel Veriler’iniz, Hizmet işlemleri için kullanılır:"
 
 #: wllegal/templates/legal/documents/privacy.html:47
 #, python-format
 msgid ""
 "for providing our services on the Service, to contact you in matters "
 "regarding our services (also by means of e-mails and messaging) and to "
 "ensure the technical functionality of our services fulfillment of "
 "contractual or pre-contractual obligations (<a href=\"%(url)s\">Article 6 "
 "(1) b. GDPR</a>)"
 msgstr ""
-"hizmetlerimizi hizmet ile sunmak için, hizmetlerimizle ilgili konularda "
-"sizinle iletişim kurmak (ayrıca e-posta ve iletiler yoluyla) ve "
-"hizmetlerimizin teknik işlevselliğini sözleşme veya sözleşme öncesi "
-"yükümlülüklerin yerine getirilmesini sağlamak <a href=\"%(url)s\">Madde 6 "
-"(1) b. GDPR</a>)"
+"hizmetlerimizi sunmak, hizmetlerimizle ilgili konularda sizinle iletişim "
+"kurmak (ayrıca e-posta ve iletiler yoluyla) ve hizmetlerimizin teknik "
+"özelliklerini sözleşme veya sözleşme öncesi yükümlülüklerin yerine "
+"getirilmesini sağlamak <a href=\"%(url)s\">GDPR 6. madde (1) b.</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:48
 #, python-format
 msgid ""
 "to analyze your use of our services and improve our services (<a href="
 "\"%(url)s\">Article 6 (1) b. and f. GDPR</a>)"
 msgstr ""
-"Hizmetlerimizi kullanımınızı analiz etmek ve hizmetlerimizi iyileştirmek "
-"için (<a href=\"%(url)s\">Madde 66 (1) b. ve f. GDPR</a>)"
+"hizmetlerimizi kullanmanızı incelemek ve hizmetlerimizi iyileştirmek için ("
+"<a href=\"%(url)s\">GDPR 6. madde (1) b. ve f.</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:49
 #, python-format
 msgid ""
 "with your express consent or instruction to carry out our business "
 "activities or send you newsletters (<a href=\"%(url)s\">Article 6 (1) a. "
 "GDPR</a>)"
 msgstr ""
-"ticari faaliyetlerimizi yürütmek veya size haber bültenleri göndermek için "
-"açık rızanız veya talimatınızla (<a href=\"%(url)s\">Madde 6 (1) a. GDPR</a>)"
+"ticari faaliyetlerimizi yürütmek veya size duyurular göndermek için açık "
+"rızanız veya isteğinizle (<a href=\"%(url)s\">GDPR 6. madde (1) a.</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:52
 msgid "Access to the Personal Data"
-msgstr "Kişisel Verilere Erişim"
+msgstr "Kişisel Veriler’e erişim"
 
 #: wllegal/templates/legal/documents/privacy.html:54
 msgid ""
 "The Controller has made all reasonable technical means to protect the "
 "Personal Data. Only authorized persons can access the Personal Data."
 msgstr ""
-"Denetleyici, Kişisel Verileri korumak için tüm makul teknik imkanları "
-"sağlamıştır. Kişisel Verilere yalnızca yetkili kişiler erişebilir."
+"Sorumlu, Kişisel Veriler’i korumak için tüm makul teknik olanakları "
+"sağlamıştır. Kişisel Veriler’e yalnızca yetkili kişiler erişebilir."
 
 #: wllegal/templates/legal/documents/privacy.html:56
 msgid ""
 "Third parties which can gain access to the Personal Data when necessary are:"
-msgstr "Gerekli olduğunda Kişisel Verilere erişebilecek üçüncü taraflar:"
+msgstr "Gerekli olduğunda Kişisel Veriler’e erişebilecek üçüncü taraflar:"
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
-msgstr "Servisin teknik güvencesini sağlayan sözleşmeli kişiler."
+msgstr "Hizmet’in teknik güvencesini sağlayan sözleşmeli kişiler."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Bizden bir hizmet satın alındığında ödeme aracıları."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Tüm Kişisel Veriler Avrupa Birliği sınırları içinde saklanır."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Kişisel Verilere Erişim"
+msgid "Disclosure of the Personal Data"
+msgstr "Kişisel Veriler’in açıklanması"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Kişisel Veriler, Sorumlu’nun bir mahkeme celbi veya diğer adli veya idari "
+"bir emir gibi yasaların gerektirdiğine iyi niyetle inandığı sınırlı "
+"durumlarda üçüncü taraflara açıklanabilir."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Sorumlu’nun yasalarca Kişisel Veriler’i açıklamasının gerekli olması "
+"durumunda, Kullanıcı’nın açıklamaya itiraz etmesini sağlamak için, Kullanıcı’"
+"ya Kişisel Veriler’i ile ilgili bir istekte bulunulduğu konusunda e-posta "
+"yoluyla önceden bildirimde bulunulmaya çalışılır (Sorumlu’nun bunu yapması "
+"engellenmediği veya boşuna olmadığı sürece). Kullanıcı açıklama isteğine "
+"itiraz etmezse, sorumlunun Kişisel Veriler’i teslim etmesi yasal olarak "
+"gerekli olabilir."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
-msgstr "Kişisel Verilerin saklanması"
+msgstr "Kişisel Veriler’in tutulması"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
-"Kişisel Veriler, Kullanıcı hizmetteki hesabını silene kadar Hizmette "
-"saklanır."
+"Kişisel Veriler, Kullanıcı Hizmet’teki hesabını silene kadar hizmet üzerinde "
+"tutulur."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
-"Erişim günlüğü bilgileri, yasal taleplerin oluşturulması, kullanılması veya "
+"Erişim günlüğü bilgileri, yasal isteklerin oluşturulması, kullanılması veya "
 "savunulması amacıyla daha uzun bir süre için toplanabilir."
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "Haklarınız"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
 "The User provides use of Personal Data voluntarily. Without this Personal "
 "Data Weblate is not able to provide our services."
 msgstr ""
-"Kullanıcı, kişisel verilerin gönüllü olarak kullanılmasını sağlar. Bu "
-"kişisel veriler olmadan Weblate hizmetlerini sağlayamaz."
+"Kullanıcı, Kişisel Veriler’ini gönüllü olarak kullanıma sunar. Bu Kişisel "
+"Veriler olmadan Weblate hizmetlerini alamaz."
 
 #: wllegal/templates/legal/documents/privacy.html:81
 msgid ""
 "We want you to always be in control of your Personal Data. To this end, you "
 "have certain rights that allow for it. Under certain conditions, you may:"
 msgstr ""
-"Kişisel verilerinizin her zaman kontrolunuzda olmasını istiyoruz. Bu amaçla, "
-"bunu sağlayacak belirli haklarınız var. Belirli koşullar altında şunları "
-"yapabilirsiniz:"
+"Kişisel Veriler’inizin her zaman kontrolunuzda olmasını istiyoruz. Bu "
+"amaçla, bunu sağlayacak belirli haklarınız var. Belirli koşullar altında "
+"şunları yapabilirsiniz:"
 
 #: wllegal/templates/legal/documents/privacy.html:85
 #, python-format
 msgid ""
 "Gain access to all your Personal Data that Weblate uses or processes, and "
 "even get a copy of all of it (<a href=\"%(url)s\">Article 15 GDPR</a>)"
 msgstr ""
-"Weblate'in kullandığı veya işlediği tüm Kişisel Verilerinize erişin ve hatta "
-"tümünün bir kopyasını alın (<a href=\"%(url)s\">Madde 15 GDPR</a>)"
+"Weblate tarafından kullanılan veya işlenen tüm Kişisel Veriler’inize "
+"erişebilir ve tümünün bir kopyasını alabilirsiniz (<a href=\"%(url)s\">GDPR "
+"15. madde</a>)"
 
 #: wllegal/templates/legal/documents/privacy.html:86
 msgid ""
 "Correct the Personal Data that Weblate processes if you think that there are "
 "mistakes"
 msgstr ""
-"Hata olduğunu düşünüyorsanız, Weblate'in işlediği Kişisel Verileri düzeltin"
+"Bir yanlışlık olduğunu düşünüyorsanız, Weblate tarafından işlenenen Kişisel "
+"Veriler’inizi düzeltebilirsiniz"
 
 #: wllegal/templates/legal/documents/privacy.html:87
 msgid "Order us to delete your Personal Data"
-msgstr "Bizden Kişisel Verilerinizi silmemizi isteyin"
+msgstr "Bizden Kişisel Veriler’inizi silmemizi isteyebilirsiniz"
 
 #: wllegal/templates/legal/documents/privacy.html:88
 msgid "Restrict the Personal Data processing"
-msgstr "Kişisel Verilerin işlenmesini kısıtlayın"
+msgstr "Kişisel Veriler’inizin işlenmesini kısıtlayabilirsiniz"
 
 #: wllegal/templates/legal/documents/privacy.html:89
 msgid "Object to processing"
-msgstr "Verilerin işlenmesine karşı çıkın"
+msgstr "Kişisel Veriler’inizin işlenmesini reddebilirsiniz"
 
 #: wllegal/templates/legal/documents/privacy.html:90
 msgid ""
 "Receive your Personal Data in a commonly used and machine-readable format or "
 "to transmit this Personal Data to a different provider."
 msgstr ""
-"Kişisel Verilerinizi yaygın olarak kullanılan ve makine tarafından "
-"okunabilir bir biçimde alın veya bu Kişisel Verileri farklı bir sağlayıcıya "
-"iletin."
+"Kişisel Veriler’inizi yaygın olarak kullanılan ve bilgisayar tarafından "
+"okunabilecek bir biçimde alabilir veya bu Kişisel Veriler’i farklı bir "
+"Hizmet Sağlayıcı’ya iletebilirsiniz."
 
 #: wllegal/templates/legal/documents/privacy.html:93
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr ""
-"Kişisel Verilerinizin kaldırılması, düzeltilmesi ve geri alınması hesap "
-"yönetiminden yapılabilir ve tamamen otomatikleştirilmiştir."
+"Kişisel Veriler’inizi silme, düzeltme ve geri alma işlemleri hesap yönetimi "
+"bölümünden yapılabilir ve tamamen otomatikleştirilmiştir."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Özel verileri (eposta adresiniz gibi) işleriz, bunlar siz hesabınızı "
-"kaldırır kaldırmaz veri tabanımızdan atılır."
+"Kişisel Veriler’inizi (e-posta adresiniz gibi) işleriz, bunlar siz "
+"hesabınızı siler silmez veri tabanımızdan kaldırılır."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
-msgstr "Çevirileriniz her çeviri tarafından belirtilen lisans altında yapılır."
+msgstr ""
+"Çevirileriniz her çeviri için belirtilmiş lisans koşulları altında yapılır "
+"ve kullanılır."
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
-"Adınız ve e-posta adresiniz VCS işlemelerinde kullanılır, orada süresiz "
-"olarak kalır."
+"Adınız ve e-posta adresiniz sürüm denetimi sistemi gönderimlerinde "
+"kullanılır ve orada süresiz olarak kalır."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Seçilen ad size bağlıdır ve gönderimler için kullanılan e-posta adresi "
+"gizliliğinizi korumak için Weblate sistemi tarafından maskelenebilir."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
-msgstr "Hizmetlerimizi sunmak için tanımlama bilgileri kullanıyoruz."
+msgstr "Hizmetlerimizi sunmak için Tanımlama Bilgileri’ni kullanıyoruz."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Herhangi bir üçüncü taraf Tanımlama Bilgileri kullanmıyoruz."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "İngilizce sürümü görüntüle"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
 "The Terms of Service document is authoritative in English, translations are "
 "provided for your convenience."
 msgstr ""
-"Kullanım koşulları belgesinin İngilizce biçimi geçerlidir. Çeviriler size "
-"kolaylık sağlaması için sunulmuştur."
+"Hizmet Kullanım Koşulları belgesinin İngilizce biçimi geçerlidir. Çeviriler "
+"size kolaylık sağlaması için sunulmuştur."
 
 #: wllegal/templates/legal/documents/tos.html:17
 msgid ""
 "The rights and obligations of the User and the Provider resulting from the "
 "use of the Service are governed by these Terms of Service."
 msgstr ""
-"Hizmetin kullanımından kaynaklanan kullanıcı ve hizmet sağlayıcının hak ve "
-"yükümlülükleri, bu kullanım koşullarına tabidir."
+"Hizmetin kullanımından kaynaklanan Kullanıcı ve Hizmet Sağlayıcı’nın hak ve "
+"yükümlülükleri, bu Hizmet Kullanım Koşulları metnine tabidir."
 
 #: wllegal/templates/legal/documents/tos.html:20
 msgid "Definitions"
 msgstr "Tanımlar"
 
 #: wllegal/templates/legal/documents/tos.html:22
 msgid "In these Terms of Service:"
-msgstr "Bu kullanım koşullarında:"
+msgstr "Bu Hizmet Kullanım Koşulları’nda:"
 
 #: wllegal/templates/legal/documents/tos.html:26
 msgid "Agreement"
-msgstr "Anlaşma"
+msgstr "Sözleşme"
 
 #: wllegal/templates/legal/documents/tos.html:27
 msgid ""
 "means License Agreement within the meaning of Article 2358 et seq. of the "
 "Civil Code concluded by and between the User and the Provider upon the "
 "Consent"
 msgstr ""
-"2358 ve devamı maddeleri anlamları Lisans Anlaşması anlamına gelir. Medeni "
-"Kanun'un Kullanıcı ve Sağlayıcının Rıza Üzerindeki Sonucu"
+"Medeni Kanun'un 2358. maddesi ve devamı anlamında, Kullanıcı ile Hizmet "
+"Sağlayıcı arasında Rıza üzerine ve Kullanıcı ile Hizmet Sağlayıcı arasında "
+"akdedilen Lisans Sözleşmesi anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:29
 msgid "Civil Code"
 msgstr "Medeni Kanun"
 
 #: wllegal/templates/legal/documents/tos.html:30
 #, python-format
 msgid "means Act No. %(law_89_2012)s Coll., the Civil Code, as amended"
 msgstr ""
-"%(law_89_2012)s Coll. Kanunu, değiştirilen şekliyle Medeni Kanun anlamına "
-"gelir"
+"Medeni Kanun'un değiştirildiği şekliyle %(law_89_2012)s Coll. sayılı Kanun "
+"anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:32
 msgid "Consent"
 msgstr "Rıza"
 
 #: wllegal/templates/legal/documents/tos.html:33
 msgid ""
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
-"Hesap açarken kutuya tıklamak bu kullanım koşulları ve diğer yasal "
-"belgelerin kullanıcı tarafından onaylandığı anlamına gelir"
+"Kullanıcı’nın bu Hizmet Kullanım Koşulları’nı ve hesap açma sırasında onay "
+"kutusunu işaretleyerek ifade edilen diğer yasal belgeleri kabul ettiği "
+"anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "Tanımlama bilgileri"
+msgstr "Tanımlama Bilgileri"
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
-"Hizmetin web sunucusu tarafından Kullanıcının bilgisayarına veya İnternet'e "
-"bağlı diğer cihazlara gönderilen ve kullanıcının web tarayıcısının benzersiz "
-"bir şekilde tanımlanmasını sağlayan herhangi bir veri dosyası anlamına gelir"
+"Hizmet’in internet sunucusu tarafından Kullanıcı’nın bilgisayarına veya "
+"internet bağlantısı olan başka bir aygıta gönderilen ve Kullanıcı’nın "
+"tarayıcısının benzersiz bir şekilde tanımlanmasını sağlayan herhangi bir "
+"veri dosyası anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:39
 msgid "GDPR"
 msgstr "GDPR"
 
 #: wllegal/templates/legal/documents/tos.html:40
 #, python-format
 msgid ""
 "means EU Regulation No. %(law_679_2016)s, the General Data Protection "
 "Regulation"
 msgstr ""
-"%(law_679_2016)s sayılı AB Yönetmeliği, Genel Veri Koruma Yönetmeliği "
-"anlamına gelir"
+"Genel Veri Koruma Yönetmeliği olan %(law_679_2016)s No'lu AB Tüzüğü anlamına "
+"gelir"
 
 #: wllegal/templates/legal/documents/tos.html:42
 msgid "License"
 msgstr "Lisans"
 
 #: wllegal/templates/legal/documents/tos.html:43
 msgid ""
 "means non-exclusive license granted by the Provider to the User for use of "
 "the Service"
 msgstr ""
-"Hizmetin kullanımı için Sağlayıcı tarafından Kullanıcıya verilen münhasır "
-"olmayan lisans anlamına gelir"
+"Hizmet’in kullanımı için Hizmet Sağlayıcı tarafından Kullanıcı’ya verilen "
+"münhasır olmayan lisans anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:45
 msgid "Provider"
-msgstr "Sağlayıcı"
+msgstr "Hizmet Sağlayıcı"
 
 #: wllegal/templates/legal/documents/tos.html:46
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s, Kayıt No. %(reg_no)s manasındadır"
+msgstr "%(provider)s anlamına gelir, Sicil No. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "Kişisel Veri"
+msgstr "Kişisel Veriler"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
-"kullanıcı tarafından hizmete ve/veya tanımlama bilgilerine eklenen "
-"%(law_679_2016)s sayılı AB Yönetmeliği anlamındaki kişisel veriler anlamına "
-"gelir"
+"Kullanıcı tarafından Hizmet’e ve/veya Tanımlama Bilgileri’ne eklenen "
+"%(law_679_2016)s sayılı AB Tüzüğü anlamında Kişisel Veriler anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:51
 msgid "Owner"
-msgstr "Sahibi"
+msgstr "Sahip"
 
 #: wllegal/templates/legal/documents/tos.html:52
 msgid "means the User who can manage Project"
 msgstr "Projeyi yönetebilen Kullanıcı anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:54
 msgid "Project"
 msgstr "Proje"
 
 #: wllegal/templates/legal/documents/tos.html:55
 msgid "means translation project operated on the Service"
-msgstr "Hizmette çalıştırılan çeviri projesi anlamına gelir"
+msgstr "Hizmet’te yürütülen çeviri projesi anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:57
 msgid "Service"
 msgstr "Hizmet"
 
 #: wllegal/templates/legal/documents/tos.html:58
 msgid ""
 "means the website and services based on Weblate operated by the Provider"
 msgstr ""
-"Sağlayıcı tarafından işletilen Weblate'e dayalı web sitesi ve hizmetler "
+"Sağlayıcı tarafından işletilen Weblate temelli internet sitesi ve hizmetler "
 "anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:60
 msgid "Translation Memory"
 msgstr "Çeviri belleği"
 
 #: wllegal/templates/legal/documents/tos.html:61
@@ -521,231 +519,230 @@
 msgstr "Kullanıcı"
 
 #: wllegal/templates/legal/documents/tos.html:64
 msgid ""
 "means any legal entity or an individual other than the Provider, who is "
 "using the Service"
 msgstr ""
-"Hizmet'i kullanan Sağlayıcı dışındaki herhangi bir tüzel kişi veya bir kişi "
-"anlamına gelir"
+"Hizmet'i kullanan Hizmet Sağlayıcı dışındaki herhangi bir tüzel kişi veya "
+"bir kişi anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:66
 msgctxt "Definition in terms of service"
 msgid "VCS"
-msgstr "VCS"
+msgstr "Sürüm Denetimi Sistemi"
 
 #: wllegal/templates/legal/documents/tos.html:67
 msgid ""
 "means distributed version control system used by the Project such as Git or "
 "Mercurial"
 msgstr ""
 "Git veya Mercurial gibi Proje tarafından kullanılan dağıtılmış sürüm denetim "
 "sistemi anlamına gelir"
 
 #: wllegal/templates/legal/documents/tos.html:71
 msgid "License Agreement Conclusion"
-msgstr "Lisans Anlaşmasının Sonuçlandırılması"
+msgstr "Lisans Sözleşmesinin sonuçlandırılması"
 
 #: wllegal/templates/legal/documents/tos.html:73
 msgid ""
 "The License Agreement is concluded upon the User’s Acceptance of the "
 "Provider’s Offer."
 msgstr ""
-"Lisans Anlaşması, Kullanıcının Sağlayıcının Teklifini Kabul Etmesi ile "
-"sonuçlandırılır."
+"Lisans Sözleşmesi, Kullanıcı’nın Hizmet Sağlayıcı’nın teklifini kabul etmesi "
+"ile sonuçlandırılır."
 
 #: wllegal/templates/legal/documents/tos.html:76
 msgid "License Agreement"
-msgstr "Lisans Anlaşması"
+msgstr "Lisans Sözleşmesi"
 
 #: wllegal/templates/legal/documents/tos.html:78
 msgid ""
 "By concluding Agreement under Article 2.1 of this Agreement, the following "
 "provisions of this Article 3 of the Terms of Service come into force."
 msgstr ""
-"Bu anlaşmanın 2.1 maddesi uyarınca anlaşma imzalandığında, kullanım "
-"koşullarının 3. maddesinin aşağıdaki hükümleri yürürlüğe girer."
+"Bu Sözleşme’nin 2.1. maddesi uyarınca Sözleşme’nin akdedilmesiyle, Hizmet "
+"Kullanım Koşulları’nın bu 3. madde altındaki hükümleri yürürlüğe girer."
 
 #: wllegal/templates/legal/documents/tos.html:80
 msgid ""
 "The Provider presents the User with a License Agreement and the User accepts "
 "this License Agreement, all this under the terms and conditions stated in "
 "these Terms of Service."
 msgstr ""
-"Hizmet sağlayıcı, kullanıcıya bir lisans anlaşması sunar ve kullanıcı, bu "
-"kullanım koşullarında belirtilen hüküm ve koşullar altında bu lisans "
-"anlaşmasını kabul eder."
+"Hizmet Sağlayıcı, Kullanıcı’ya bir Lisans Sözleşmesi sunar ve Kullanıcı bu "
+"Lisans Sözleşmesi’ni, tüm bunları bu Hizmet Kullanım Koşulları’nda "
+"belirtilen hüküm ve koşullar altında kabul eder."
 
 #: wllegal/templates/legal/documents/tos.html:82
 msgid ""
 "The Provider shall have the right to shut down, adjust, modify or make the "
 "Service unavailable on the web address at any time."
 msgstr ""
-"Sağlayıcı, Hizmeti web adresinde istediği zaman kapatma, ayarlama, "
-"değiştirme veya kullanılmaz duruma getirme hakkına sahip olacaktır."
+"Hizmet Sağlayıcı, herhangi bir zamanda Hizmet’i internet adresinden kapatma, "
+"ayarlama, değiştirme veya kullanılamaz hale getirme hakkına sahiptir."
 
 #: wllegal/templates/legal/documents/tos.html:84
 msgid ""
 "The User agrees to use the Service only in a manner not jeopardizing "
 "technical software and/or hardware means of the Provider and/or such means "
 "in the Provider’s use."
 msgstr ""
-"Kullanıcı, Hizmeti sadece Sağlayıcının teknik yazılımını ve/veya donanımını "
-"ve/veya Sağlayıcının kullanımındaki bu tür araçları tehlikeye atmayacak "
-"şekilde kullanmayı kabul eder."
+"Kullanıcı, Hizmeti yalnızca Hizmet Sağlayıcı’nın teknik yazılımını ve/veya "
+"donanım araçlarını ve/veya Hizmet Sağlayıcı’nın kullanımındaki bu tür "
+"araçları tehlikeye atmayacak şekilde kullanmayı kabul eder."
 
 #: wllegal/templates/legal/documents/tos.html:86
 msgid ""
 "The User agrees to refrain from use of the Service in bad faith and/or "
 "deliberately causing any damage to the Service."
 msgstr ""
-"Kullanıcı, Hizmeti kötü niyetle kullanmaktan ve / veya Hizmetin zarar "
-"görmesine neden olmaktan kaçınmayı kabul eder."
+"Kullanıcı, Hizmet’i kötü niyetle kullanmaktan ve/veya kasıtlı olarak Hizmet’"
+"e herhangi bir zarar vermekten kaçınacağını kabul eder."
 
 #: wllegal/templates/legal/documents/tos.html:88
 msgid ""
 "The User agrees to refrain from bypassing the Service’s software and/or "
 "technical hardware means, in particular the security systems."
 msgstr ""
-"Kullanıcı, Hizmet'in yazılımını ve / veya teknik donanım araçlarını, "
-"özellikle güvenlik sistemlerini atlamaktan kaçınmayı kabul eder."
+"Kullanıcı, Hizmet’in yazılım ve/veya teknik donanım araçlarını, özellikle de "
+"güvenlik sistemlerini aşmaktan kaçınacağını kabul eder."
 
 #: wllegal/templates/legal/documents/tos.html:91
 msgid "Liability for Damage"
 msgstr "Hasar Sorumluluğu"
 
 #: wllegal/templates/legal/documents/tos.html:93
 msgid ""
 "The User hereby renders it undisputed that the Provider shall not be liable "
 "for any damage caused to the User resulting from the use of the Service."
 msgstr ""
-"Kullanıcı, Hizmetin kullanımından kaynaklanan Kullanıcıya verilecek "
-"zararlardan Sağlayıcının sorumlu olmayacağını tartışmasız kılmaktadır."
+"Kullanıcı, Hizmet Sağlayıcı’nın, Kullanıcı’ya Hizmet’in kullanımından "
+"kaynaklanarak verilebilecek herhangi bir zarardan sorumlu olmayacağını kabul "
+"eder."
 
 #: wllegal/templates/legal/documents/tos.html:95
 msgid ""
 "If the User is an entrepreneur, it hereby expressly waives its right to "
 "compensation from the Provider for damage unintentionally caused by the "
 "Provider to the User through a breach of any obligation contained in these "
 "Terms of Service and/or resulting from the use of the Service."
 msgstr ""
-"Kullanıcı bir girişimci ise, bu kullanım koşullarında yer alan ve/veya "
-"hizmetin kullanımından doğacak herhangi bir yükümlülüğü ihlal etmek "
-"suretiyle, hizmet sağlayıcının istemeden kullanıcıya doğuracağı zararlar "
-"için hizmet sağlayıcıdan tazminat etme hakkından açıkça feragat eder."
+"Kullanıcı bir girişimci ise, bu Hizmet Kullanım Koşulları’nda yer alan ve/"
+"veya Hizmet’in kullanımından kaynaklanan herhangi bir yükümlülüğün ihlali "
+"nedeniyle Hizmet Sağlayıcı tarafından Kullanıcı’ya kasıtsız olarak "
+"verilebilecek zararlar için Hizmet Sağlayıcı’dan tazminat alma hakkından "
+"açıkça feragat eder."
 
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"GDPR <a href=\"%(url)s\">7. maddesi</a> anlamında Kullanıcı, <a href=\""
+"%(privacy_url)s\">Kişisel Veriler’in Gizlilik İlkesi’ne</a> uygun olarak "
+"toplanmasına, depolanmasına ve işlenmesine izin verir."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Çeviriler"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
 "The Service organizes translation into individual Projects, where the Owner "
 "is responsible for managing them and for specifying accurately the license "
 "of the Project."
 msgstr ""
-"Hizmet, Sahibi'nin bunları yönetmekten ve Proje lisansını doğru bir şekilde "
-"belirlemekten sorumlu olduğu bireysel Projelere çeviri organize eder."
+"Hizmet, Sahibinin bunları yönetmekten ve Proje’nin lisansını doğru bir "
+"şekilde belirlemekten sorumlu olduğu bireysel Proje’lerde çevirleri organize "
+"eder."
 
 #: wllegal/templates/legal/documents/tos.html:107
 msgid ""
 "Not specifying translation license means that the translations are available "
 "under same license as the given Project itself."
 msgstr ""
-"Çeviri lisansının belirtilmemesi, çevirilerin verilen Projenin kendisiyle "
-"aynı lisans altında mevcut olduğu anlamına gelir."
+"Çeviri lisansının belirtilmemesi, çevirilerin belirtilen Proje’nin "
+"kendisiyle aynı lisans koşullarına tabi olduğu anlamına gelir."
 
 #: wllegal/templates/legal/documents/tos.html:109
 msgid ""
 "Should the Project opt in for the Translation Memory, license to use the "
 "translation is granted to all Translation Memory users."
 msgstr ""
-"Projenin Çeviri Belleği'ni seçmesi halinde, çeviriyi kullanma lisansı tüm "
-"Çeviri Belleği kullanıcılarına verilir."
+"Proje’nin Çeviri Belleği'ni kullanmayı seçmesi durumunda, çeviriyi kullanma "
+"lisansı tüm Çeviri Belleği kullanıcılarına verilir."
 
 #: wllegal/templates/legal/documents/tos.html:111
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
-"Kullanıcı, bir Projeye katkıda bulunduktan sonra, Proje'nin belirttiği "
+"Kullanıcı, bir Proje’ye katkıda bulunduktan sonra, Proje için belirtilmiş "
 "lisansı kabul eder."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"Kullanıcı VCS taahhütlerinde yazar olarak kendi adı ve e-posta adresini "
-"kullanmayı kabul eder. Kullanıcı, bu onayın VCS'nin niteliği nedeniyle geri "
-"alınamaz olduğunu bilir."
+"Kullanıcı, Sürüm Denetimi Sistemi gönderimlerinin sorumlusu olarak ad ve e-"
+"posta kullanmayı kabul eder. Kullanıcı, Sürüm Denetimi Sistemi’nin doğası "
+"gereği bu gönderimin geri alınamayacağını kabul eder."
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
 msgstr ""
-"%(law_480_2004)s Coll. kanununun 89. maddesi uyarınca, elektronik "
-"iletişimde, değiştirildiği şekliyle, kullanıcıya hizmetin tanımlama "
-"bilgileri kaydettiği bildirilir."
+"Elektronik iletişimde, değiştirildiği şekliyle, %(law_480_2004)s sayılı "
+"Kanun'un 89. maddesi anlamında, Kullanıcı, Hizmet’in Tanımlama Bilgileri’ni "
+"kullandığı konusunda bilgilendirilir."
 
 #: wllegal/templates/legal/documents/tos.html:120
 msgid "The Service uses Cookies to personalise content."
-msgstr "Hizmet, içeriği kişiselleştirmek için tanımlama bilgilerini kullanır."
+msgstr "Hizmet, içeriği kişiselleştirmek için Tanımlama Bilgileri’ni kullanır."
 
 #: wllegal/templates/legal/documents/tos.html:123
 msgid "Governing Law"
 msgstr "Geçerli Kanun"
 
 #: wllegal/templates/legal/documents/tos.html:125
 msgid ""
 "These Terms of Service shall be governed by the laws of the Czech Republic "
 "with exclusion of conflict rules."
 msgstr ""
-"Bu kullanım koşulları, çatışma kurallarının dışında Çek Cumhuriyeti "
-"yasalarına tabidir."
+"Bu Hizmet Kullanım Koşulları, ihtilaf kuralları dışında üzere Çek "
+"Cumhuriyeti yasalarına tabidir."
 
 #: wllegal/templates/legal/documents/tos.html:127
 msgid ""
 "Any disputes arising on the basis of the Agreement and/or these Terms of "
 "Service shall be resolved by the court of the Czech republic having "
 "substantive and local jurisdiction."
 msgstr ""
-"Anlaşma ve/veya bu kullanım koşulları temelinde ortaya çıkan anlaşmazlıklar, "
-"temel ve yerel yargı yetkisine sahip Çek Cumhuriyeti mahkemesi tarafından "
-"çözümlenecektir."
+"Sözleşmeye ve/veya bu Hizmet Kullanım Koşulları’na göre ortaya çıkan "
+"herhangi bir anlaşmazlık, maddi ve yerel yargı yetkisine sahip Çek "
+"Cumhuriyeti mahkemeleri tarafından çözülecektir."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Etki"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "Bu kullanım koşulları 1 Eylül 2017 tarihinde yürürlüğe girecektir."
+msgstr ""
+"Bu Hizmet Kullanım Koşulları 15 Mayıs 2023 tarihinde yürürlüğe girecek ve "
+"etkin olacaktır."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "Bizden hizmet satın almanız durumunda, fatura çıkarmak için gerekli ek "
 #~ "fatura bilgilerini topluyoruz"
```

### Comparing `wllegal-2023.3/wllegal/locale/tt/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/te/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: tt\n"
+"Language: te\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
@@ -157,15 +157,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/tzm/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/tzm/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2021-01-28 08:55+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Tamazight (Central Atlas) <https://hosted.weblate.org/"
 "projects/weblate/legal/tzm/>\n"
 "Language: tzm\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/ug/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/ug/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2018-07-23 11:06+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Uyghur <https://hosted.weblate.org/projects/weblate/master/ug/"
 ">\n"
 "Language: ug\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -160,15 +160,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/uk/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/uk/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -3,38 +3,36 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2013.
 # Андрій Бандура <andriykopanytsia@gmail.com>, 2018, 2019.
 # Tymofij Lytvynenko <till.svit@gmail.com>, 2019, 2020.
 # Vadim Nekhai <vadimnekhai@gmail.com>, 2019.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2021-10-21 09:56+0000\n"
-"Last-Translator: Ihor Hordiichuk <igor_ck@outlook.com>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-20 18:48+0000\n"
+"Last-Translator: Yuri Chornoivan <yurchor@ukr.net>\n"
 "Language-Team: Ukrainian <https://hosted.weblate.org/projects/weblate/legal/"
 "uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.9-dev\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "Субпідрядники відповідно до ст. 28 GDPR"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "Станом на жовтень 2020 року."
+msgstr "Станом на березень 2023 року."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -71,24 +69,20 @@
 "використання наших послуг:"
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "Ім'я користувача та електронна пошта"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "Використовуються для ідентифікації вас під час під зміни коду VCS"
+msgstr "Використовуються для ідентифікації вас під час під зміни коду VCS."
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "Крім того, адреса ел. пошти використовується для сповіщень"
+msgstr "Крім того, адреса ел. пошти використовується для сповіщень."
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "Пароль у гешованій формі"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -99,36 +93,32 @@
 msgstr "Хеші паролів зберігаються з використанням Argon2."
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP адреса і назва вебпереглядача"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
 "Записуються для випадку важливих змін у ваш обліковий запис (наприклад, "
-"зміна пароля), щоб зробити діагностику в разі крадіжки облікового запису"
+"зміна пароля), щоб зробити діагностику в разі крадіжки облікового запису."
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "Платіжні відомості"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
 msgstr ""
+"При придбанні наших послуг ми збираємо потрібні для надання рахунку-фактури "
+"дані."
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "Ціль і правова основа опрацювання особистих даних"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -190,60 +180,63 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "Особи, з якими укладено контракт на технічне забезпечення послуг."
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "Обробники сплати при придбанні наших послуг."
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "Все особисті дані зберігаються в Європейському Союзі."
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "Доступ до особистих даних"
+msgid "Disclosure of the Personal Data"
+msgstr "Розкриття особистих даних"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"Особисті дані може бути розкрито для сторонніх осіб у обмежених випадках, "
+"коли Контролер має певність, що це потрібно за законом, зокрема у випадках "
+"отримання повісток або інших юридичних або адміністративних приписів."
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"Якщо Контролерові за законом слід розкрити особисті дані, буде зроблено "
+"попередню спробу надати користувачеві сповіщення електронною поштою (якщо це "
+"не заборонено для Контролера або не є марним) про те, що надійшов запит щодо "
+"особистих даних, щоб користувач міг заперечити проти розкриття цих даних. "
+"Якщо користувач не оскаржить запиту щодо розкриття, у Контролера можуть "
+"виникнути юридичні зобов'язання щодо розкриття особистих даних."
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "Право зберігання особистих даних"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr ""
 "Особисті дані зберігаються службою до тих пір, поки відвідувач не видалить "
 "свій обліковий запис."
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr ""
 "Доступ до відомостей про вхід може бути отриманий на триваліший період часу "
 "з ціллю пред'явлення, здійснення або захисту за судовими позовами."
 
@@ -311,30 +304,22 @@
 "from the account management, and is fully automated."
 msgstr ""
 "Вилучення, виправлення та отримання ваших особистих даних можна виконувати "
 "за допомогою сторінки керування обліковим записом. Обробку даних повністю "
 "автоматизовано."
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"Ми обробляємо особисті дані (наприклад, адреса електронної пошти). Вони "
+"Ми обробляємо особисті дані (наприклад, адресу електронної пошти). Вони "
 "будуть викинуті з нашої бази даних щойно ви вилучите свій профіль."
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
 msgstr ""
 "Ваші переклади зроблені на умовах ліцензії, яка вказана на кожен переклад."
 
 #: wllegal/templates/legal/documents/summary.html:7
@@ -346,22 +331,25 @@
 "залишаться там назавжди."
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
 msgstr ""
+"Вибране ім'я є вашою особистою справою, а адресу електронної пошти, яка "
+"використовується для внесків, може бути замасковано системою Weblate з метою "
+"захисту ваших конфіденційних даних."
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "Ми використовуємо реп'яшки, щоб доставити наші послуги."
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "Ми не використовуємо жодних сторонніх кук."
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "Переглянути англійську версію"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -645,14 +633,17 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"У межах значення <a href=\"%(url)s\">Статті 7</a> GDPR Користувач надає "
+"згоду на збирання, зберігання та обробку особистих даних відповідно до <a "
+"href=\"%(privacy_url)s\">Правил конфіденційності</a>."
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "Переклади"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -684,19 +675,14 @@
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr ""
 "Користувач погоджується з ліцензією, зазначеної Проєктом при внесенні вкладу "
 "в Проєкт."
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
 "Користувач погоджується на використання свого імені та електронної пошти для "
 "вказівки авторства в VCS-поданнях. Користувач розуміє, що даний дозвіл є "
@@ -740,21 +726,17 @@
 "місцеві суди."
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "Дія"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "Поточні Умови обслуговування набувають чинності з 1 вересня 2017 року."
+msgstr "Поточні Умови обслуговування набувають чинності з 15 травня 2023 року."
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr ""
 #~ "У випадку, коли ви купуєте цю послугу в нас, ми збираємо додаткові "
 #~ "платіжні відомості, необхідні для виставлення рахунку"
```

### Comparing `wllegal-2023.3/wllegal/locale/uz/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/zgh/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,50 +3,52 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-02-12 16:39+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Uzbek <https://hosted.weblate.org/projects/weblate/legal/uz/"
-">\n"
-"Language: uz\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-04-02 01:08+0000\n"
+"Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ ZOUHIR DEHBI <zouhirdehbi56@gmail.com>\n"
+"Language-Team: Tamazight (Standard Moroccan) <https://hosted.weblate.org/"
+"projects/weblate/legal/zgh/>\n"
+"Language: zgh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
+#, fuzzy
+#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr ""
+msgstr "ⴰⵙⵓⵔⵙ ⵙⴳ ⴽⵟⵓⴱⵕ 2020."
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr ""
+msgstr "ⵜⵉⴹⴰⴼ ⵏ ⵜⵎⵓⵛⴰ ⵜⵉⵏⵉⵎⴰⵏⵉⵏ"
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr ""
+msgstr "%(provider)s,ⵓⵟⵟⵓⵏ ⵏ ⵓⵣⵎⵎⴻⵎ. %(reg_no)s"
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
@@ -160,15 +162,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -338,15 +340,15 @@
 "means the User’s consent with these Terms of Service and other legal "
 "documents expressed by checking the checkbox during the registration"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:35
 #: wllegal/templates/legal/documents/tos.html:116
 msgid "Cookies"
-msgstr "Cookies"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:36
 msgid ""
 "means any datafile sent by the web server of the Service to the User’s "
 "computer or other device connected to the Internet, which enable obtaining "
 "unique identification of the User’s web browser"
 msgstr ""
@@ -380,15 +382,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr ""
+msgstr "ⵜⵉⵎⵓⵛⴰ ⵜⵓⴷⵎⴰⵡⴰⵏⵉⵏ"
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.3/wllegal/locale/vi/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/vi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Michal Čihař <michal@cihar.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-01-23 23:35+0000\n"
 "Last-Translator: Ngô Quốc Đạt <datlechin@gmail.com>\n"
 "Language-Team: Vietnamese <https://hosted.weblate.org/projects/weblate/legal/"
 "vi/>\n"
 "Language: vi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -171,15 +171,15 @@
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
 #, fuzzy
 #| msgid "Failed to generate key: %s"
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr "Xảy ra lỗi khi tạo khóa: %s"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/yue_Hant/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/yue_Hant/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
 "PO-Revision-Date: 2022-08-21 08:34+0000\n"
 "Last-Translator: Ray <ray.cfu@protonmail.com>\n"
 "Language-Team: Yue <https://hosted.weblate.org/projects/weblate/legal/yue/>\n"
 "Language: yue\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -159,15 +159,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
```

### Comparing `wllegal-2023.3/wllegal/locale/zgh/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/or/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Weblate <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Hosted Weblate \n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2023-04-02 01:08+0000\n"
-"Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ ZOUHIR DEHBI <zouhirdehbi56@gmail.com>\n"
-"Language-Team: Tamazight (Standard Moroccan) <https://hosted.weblate.org/"
-"projects/weblate/legal/zgh/>\n"
-"Language: zgh\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Automatically generated\n"
+"Language-Team: none\n"
+"Language: or\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.17-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr ""
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "ⴰⵙⵓⵔⵙ ⵙⴳ ⴽⵟⵓⴱⵕ 2020."
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:9
 msgid "Personal Data Controller"
-msgstr "ⵜⵉⴹⴰⴼ ⵏ ⵜⵎⵓⵛⴰ ⵜⵉⵏⵉⵎⴰⵏⵉⵏ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:12
 #, python-format
 msgid "%(provider)s, Reg. No. %(reg_no)s"
-msgstr "%(provider)s,ⵓⵟⵟⵓⵏ ⵏ ⵓⵣⵎⵎⴻⵎ. %(reg_no)s"
+msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:15
 #, python-format
 msgid ""
 "Weblate has appointed a data protection officer who may be reached via "
 "%(privacy_contact)s."
 msgstr ""
@@ -162,15 +156,15 @@
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:65
-msgid "Disclossure of the Personal Data"
+msgid "Disclosure of the Personal Data"
 msgstr ""
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
@@ -382,15 +376,15 @@
 #, python-format
 msgid "means %(provider)s, Reg. No. %(reg_no)s"
 msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:48
 #: wllegal/templates/legal/documents/tos.html:98
 msgid "Personal Data"
-msgstr "ⵜⵉⵎⵓⵛⴰ ⵜⵓⴷⵎⴰⵡⴰⵏⵉⵏ"
+msgstr ""
 
 #: wllegal/templates/legal/documents/tos.html:49
 #, python-format
 msgid ""
 "means personal data within the meaning of EU Regulation No. %(law_679_2016)s "
 "inserted by the User into the Service and/or Cookies"
 msgstr ""
```

### Comparing `wllegal-2023.3/wllegal/locale/zh_Hans/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -9,37 +9,35 @@
 # YONGLE <tanyongle0633@gmail.com>, 2019.
 # 微别累特 <1365143958@qq.com>, 2019.
 # chr56 <chr0056@gmail.com>, 2020.
 # Michal Čihař <michal@cihar.com>, 2020.
 # Changpeng Sun <zzjbcn@gmail.com>, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-11-09 12:47+0000\n"
-"Last-Translator: yangyangdaji <1504305527@qq.com>\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-05-20 18:48+0000\n"
+"Last-Translator: Eric <hamburger2048@users.noreply.hosted.weblate.org>\n"
 "Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/"
 "weblate/legal/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "分包商依照欧盟《通用数据保护条例》第28条之规定"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "自 2020 年 10 月起的状态。"
+msgstr "截至 2023 年 3 月的状态。"
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -73,24 +71,20 @@
 msgstr "Weblate 仅处理用户通过使用它提供的个人数据："
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "姓名和电子邮箱地址"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "这些信息将用于在版本控制系统提交（VCS commits）中识别你"
+msgstr "这些信息用于在版本控制系统提交（VCS commits）中识别你的身份。"
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "另外，电子邮箱地址用于接收你关注的事件的消息通知"
+msgstr "另外，电子邮箱地址用于接收你关注的事件的消息通知。"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "散列形式的密码"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -101,36 +95,30 @@
 msgstr "密码以 Argon2 散列形式存储。"
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP 地址和浏览器名称"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
 msgstr ""
-"这些记录已存储以备在你的账户有重要的变更时（例如更改密码）判断你的账号是否已"
-"被盗取"
+"这些记录已存储以备在你的账户有重要的变更时（例如更改密码）判断你的账号是否被"
+"盗取。"
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "账单信息"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
-msgstr ""
+msgstr "从我们这里购买服务时会收集开具发票所必需的详细信息。"
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "处理个人资料的目的和法律依据"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -187,58 +175,57 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "签订技术保证服务合同的人员。"
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "处理从我们这里购买服务事宜的支付处理商。"
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "所有个人数据都存储在欧盟。"
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "访问个人数据"
+msgid "Disclosure of the Personal Data"
+msgstr "个人数据披露"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
+"在有限情况下，个人数据可能会被披露给多个第三方，当数据收集方相信这么做是法律"
+"所要求的，比如收到法庭传票或其他司法或行政命令。"
 
 #: wllegal/templates/legal/documents/privacy.html:69
 msgid ""
 "In case the Controller is required by law to disclose the Personal Data, an "
 "attempt will be made to provide the User with prior notice by e-mail (unless "
 "the Controller is prohibited, or it would be futile) that a request for the "
 "Personal Data has been made to allow the User to object to the disclosure. "
 "If the User does not challenge the disclosure request, the Controller may be "
 "legally required to turn over the Personal Data."
 msgstr ""
+"如果法律要求数据收集方披露个人数据，将尝试通过电子邮件提前通知用户 （除非收集"
+"方被禁止这么做，或者这是徒劳的）有关方面提出了索取个人资料的要求，以便用户反"
+"对披露。如果用户未对披露要求提出异议，则收集方可能会被法律要求交出个人数据。"
 
 #: wllegal/templates/legal/documents/privacy.html:71
 msgid "The Personal Data retention"
 msgstr "个人数据保留"
 
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr "个人数据存储在服务中，直到用户删除其在服务中的账户。"
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
 msgstr "为了建立、行使或辩护法律索赔，可能会收集更长时间的访问日志信息。"
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
@@ -295,56 +282,49 @@
 #: wllegal/templates/legal/documents/privacy.html:93
 msgid ""
 "The removal, correction, and retrieval of your Personal Data can be done "
 "from the account management, and is fully automated."
 msgstr "删除、更正和检索您的个人数据可以从账户管理完成，且完全自动化。"
 
 #: wllegal/templates/legal/documents/summary.html:4
-#, fuzzy
-#| msgid ""
-#| "We process private data (such as your e-mail address), those will be "
-#| "discarded from our database as soon as you remove your account."
 msgid ""
 "We process personal data (such as your e-mail address); those will be "
 "discarded from our database if you remove your account."
 msgstr ""
-"我们会处理私有数据（如您的电子邮箱地址），在您删除账号时，将会从我们的数据库"
-"中删除相关内容。"
+"我们处理个人数据（如您的电子邮箱地址），如您删除账号，相关内容会从我们的数据"
+"库中被扔掉。"
 
 #: wllegal/templates/legal/documents/summary.html:5
-#, fuzzy
-#| msgid ""
-#| "Your translations are made under license which is specified by each "
-#| "translation."
 msgid ""
 "Your translations are made under the license which is specified by each "
 "translation."
-msgstr "你的翻译是在每个翻译指定的许可证下进行的。"
+msgstr "您的译文在每个翻译项目指定的许可证下进行。"
 
 #: wllegal/templates/legal/documents/summary.html:7
 msgid ""
 "Your name and e-mail address is used in VCS commits, it will stay there "
 "indefinitely."
 msgstr ""
 "在版本控制系统提交（VCS commits）中会使用您的姓名及电子邮箱地址，它将不限期保"
 "存。"
 
 #: wllegal/templates/legal/documents/summary.html:8
 msgid ""
 "Chosen name is up to you and the e-mail address used for commits can be "
 "masked by Weblate system to protect your privacy."
-msgstr ""
+msgstr "所选名称由您决定，还可以借助 Weblate "
+"系统隐藏用于提交翻译的电子邮箱地址以保护您的隐私。"
 
 #: wllegal/templates/legal/documents/summary.html:11
 msgid "We use cookies to deliver our services."
 msgstr "我们使用 cookie 以提供服务。"
 
 #: wllegal/templates/legal/documents/summary.html:12
 msgid "We don’t use any third-party cookies."
-msgstr ""
+msgstr "我们不使用任何第三方 cookies。"
 
 #: wllegal/templates/legal/documents/tos.html:10
 msgid "View English version"
 msgstr "查看英文版"
 
 #: wllegal/templates/legal/documents/tos.html:11
 msgid ""
@@ -591,14 +571,16 @@
 #: wllegal/templates/legal/documents/tos.html:101
 #, python-format
 msgid ""
 "Within the meaning of <a href=\"%(url)s\">Article 7</a> of the GDPR the User "
 "hereby gives consent to collecting, storage, and processing of the Personal "
 "Data according to the <a href=\"%(privacy_url)s\">Privacy Policy</a>."
 msgstr ""
+"在 GDPR <a href=\"%(url)s\">Article 7</a> 的意义范围内，用户特此同意根据 <a "
+"href=\"%(privacy_url)s\">隐私政策</a> 收集、存储并处理个人数据。"
 
 #: wllegal/templates/legal/documents/tos.html:103
 msgid "Translations"
 msgstr "翻译"
 
 #: wllegal/templates/legal/documents/tos.html:105
 msgid ""
@@ -623,26 +605,21 @@
 #: wllegal/templates/legal/documents/tos.html:111
 msgid ""
 "The User agrees, upon contributing to a Project, to the license the Project "
 "has specified."
 msgstr "用户在向项目贡献时同意项目指定的许可证。"
 
 #: wllegal/templates/legal/documents/tos.html:113
-#, fuzzy
-#| msgid ""
-#| "The User agrees to use of own name and e-mail as authorship in the VCS "
-#| "commits. The User understands that this grant is non revocable due to "
-#| "nature of the VCS."
 msgid ""
 "The User agrees to use of name and e-mail as authorship in the VCS commits. "
 "The User understands that this grant is non-revocable due to the nature of "
 "the VCS."
 msgstr ""
-"用户同意在版本控制系统（VCS）提交中使用他自己的姓名和电子邮箱地址作为作者身"
-"份。用户需理解，由于版本控制系统（VCS）的性质，此授权不可撤销。"
+"用户同意在版本控制系统（VCS）提交中使用姓名和电子邮箱地址作为作者身份。用户理"
+"解，由于版本控制系统（VCS）的性质，此授权不可撤销。"
 
 #: wllegal/templates/legal/documents/tos.html:118
 #, python-format
 msgid ""
 "Within the meaning of Article 89 Act No. %(law_480_2004)s Coll., on "
 "electronic communication, as amended, the User is informed that the Service "
 "uses Cookies."
@@ -674,21 +651,17 @@
 "院解决。"
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "影响"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "本服务条款将于2017年9月1日生效。"
+msgstr "本服务条款于 2023 年 3 月 15 日起生效。"
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr "如果您从我们这里购买服务，我们会收集开具发票所需的其他账单信息"
 
 #~ msgid "Payment processors."
```

### Comparing `wllegal-2023.3/wllegal/locale/zh_Hant/LC_MESSAGES/django.po` & `wllegal-2023.4/wllegal/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Chang-Chia Tseng <pswo10680@gmail.com>, 2018, 2019.
 # Louies <louies0623@gmail.com>, 2019.
 # Lzmxya <lzmxya@gmail.com>, 2019.
 # byStarTW <pan93412@gmail.com>, 2019, 2020.
 msgid ""
 msgstr ""
-"Project-Id-Version: Hosted Weblate \n"
+"Project-Id-Version: Hosted Weblate\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/wllegal/issues\n"
-"POT-Creation-Date: 2023-05-14 17:43+0000\n"
-"PO-Revision-Date: 2022-06-10 17:19+0000\n"
+"POT-Creation-Date: 2023-05-17 14:12+0000\n"
+"PO-Revision-Date: 2023-06-02 06:31+0000\n"
 "Last-Translator: pan93412 <pan93412@gmail.com>\n"
 "Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
 "weblate/legal/zh_Hant/>\n"
 "Language: zh_Hant\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.13-dev\n"
+"X-Generator: Weblate 4.18-dev\n"
 
 #: wllegal/templates/legal/documents/contracts.html:3
 msgid "Subcontractors in Accordance with Art. 28 GDPR"
 msgstr "轉包商遵守《通用資料保護法》第28條之細則"
 
 #: wllegal/templates/legal/documents/contracts.html:10
-#, fuzzy
-#| msgid "Status as of October 2020."
 msgid "Status as of March 2023."
-msgstr "2020年10月時狀態。"
+msgstr "截至 2023 年 3 月的狀態。"
 
 #: wllegal/templates/legal/documents/privacy.html:6
 #, python-format
 msgid ""
 "We comply with the Regulation No. %(law_679_2016)s, the General Data "
 "Protection Regulation, also known as GDPR. This document includes necessary "
 "specifications."
@@ -67,24 +65,20 @@
 msgstr "Weblate 只處理「使用者」經由我們服務提供的「個人資料」："
 
 #: wllegal/templates/legal/documents/privacy.html:25
 msgid "Name and e-mail address"
 msgstr "名稱和電子郵件地址"
 
 #: wllegal/templates/legal/documents/privacy.html:26
-#, fuzzy
-#| msgid "These are used to identify you in the VCS commits"
 msgid "These are used to identify you in the VCS commits."
-msgstr "這些是用來辨識您在 VCS 的提交"
+msgstr "這些是用來辨識您在 VCS 的提交。"
 
 #: wllegal/templates/legal/documents/privacy.html:27
-#, fuzzy
-#| msgid "Additionally, e-mail is used for notification of watched events"
 msgid "Additionally, e-mail is used for notification of watched events."
-msgstr "另外，電子郵件用於通知關注的事件"
+msgstr "另外，電子郵件用於通知關注的事件。"
 
 #: wllegal/templates/legal/documents/privacy.html:29
 msgid "Password in hashed form"
 msgstr "雜湊形式的密碼"
 
 #: wllegal/templates/legal/documents/privacy.html:30
 msgid "Used to authenticate the User, if configured"
@@ -95,36 +89,29 @@
 msgstr "密碼使用 Argon2 雜湊儲存。"
 
 #: wllegal/templates/legal/documents/privacy.html:33
 msgid "IP address and browser name"
 msgstr "IP 位址與瀏覽器名稱"
 
 #: wllegal/templates/legal/documents/privacy.html:34
-#, fuzzy
-#| msgid ""
-#| "These are logged in case of important changes to your account (e.g. "
-#| "password change) to allow diagnosis in case your account is stolen"
 msgid ""
 "These are logged in case of important changes to your account (e.g. password "
 "change) to allow diagnosis in case your account is stolen."
-msgstr ""
-"之所以記錄這些資訊，是為了知道您的帳號是否有重大變動（例如：更動密碼），依此"
-"分析您的帳號是否被盜取"
+msgstr "之所以記錄這些資訊，是為了知道您的帳號是否有重大變動（例如：更動密碼），依此"
+"分析您的帳號是否被盜取。"
 
 #: wllegal/templates/legal/documents/privacy.html:36
-#, fuzzy
-#| msgid "Billing information"
 msgid "Billing info"
 msgstr "結帳資訊"
 
 #: wllegal/templates/legal/documents/privacy.html:37
 msgid ""
 "Necessary details to issue an invoice is collected when purchasing a service "
 "from us."
-msgstr ""
+msgstr "從我們這裡購買服務時會收集開立發票所需的詳細資訊。"
 
 #: wllegal/templates/legal/documents/privacy.html:41
 msgid "Purpose and legal basis of processing Personal Data"
 msgstr "「個人資料」處理的用途與法律基礎"
 
 #: wllegal/templates/legal/documents/privacy.html:43
 msgid "Your Personal Data will be used for the purposes of the Service:"
@@ -181,25 +168,23 @@
 
 #: wllegal/templates/legal/documents/privacy.html:59
 msgid "Persons which are contracted for technical assurance of the service."
 msgstr "本服務的技術保證合約人員。"
 
 #: wllegal/templates/legal/documents/privacy.html:60
 msgid "Payment processors when purchasing a service from us."
-msgstr ""
+msgstr "處理從我們這裡購買服務事宜的付款處理商。"
 
 #: wllegal/templates/legal/documents/privacy.html:63
 msgid "All Personal Data is stored in the European Union."
 msgstr "所有「個人資料」皆儲存於歐盟地區。"
 
 #: wllegal/templates/legal/documents/privacy.html:65
-#, fuzzy
-#| msgid "Access to the Personal Data"
-msgid "Disclossure of the Personal Data"
-msgstr "存取「個人資料」"
+msgid "Disclosure of the Personal Data"
+msgstr "「個人資料」的披露"
 
 #: wllegal/templates/legal/documents/privacy.html:67
 msgid ""
 "The Personal Data might be disclosed to third parties in limited "
 "circumstances when the Controller has a good faith belief it is required by "
 "law, such as under a subpoena or other judicial or administrative order."
 msgstr ""
@@ -221,24 +206,19 @@
 #: wllegal/templates/legal/documents/privacy.html:73
 msgid ""
 "The Personal Data is stored in the Service until the User deletes their "
 "account on the service."
 msgstr "「個人資料」儲存於本「服務」中，直至「使用者」刪除本服務中其帳號為止。"
 
 #: wllegal/templates/legal/documents/privacy.html:75
-#, fuzzy
-#| msgid ""
-#| "Access log information might be collected for a longer period for the "
-#| "purpose of establishing, exercising or defending legal claims."
 msgid ""
 "Access log info might be collected for a longer period for the purpose of "
 "establishing, exercising or defending legal claims."
-msgstr ""
-"存取動作的紀錄資訊可能收藏更長時間，以因應法律索取時之證實、運用、防衛等用"
-"途。"
+msgstr "存取動作的紀錄資訊可能收藏更長時間，以因應法律索取時之證實、運用、防衛等用途"
+"。"
 
 #: wllegal/templates/legal/documents/privacy.html:77
 msgid "Your rights"
 msgstr "您的權利"
 
 #: wllegal/templates/legal/documents/privacy.html:79
 msgid ""
@@ -682,21 +662,17 @@
 "法院解決。"
 
 #: wllegal/templates/legal/documents/tos.html:130
 msgid "Effect"
 msgstr "生效"
 
 #: wllegal/templates/legal/documents/tos.html:132
-#, fuzzy
-#| msgid ""
-#| "These Terms of Service shall come into force and effect on 1st September "
-#| "2017."
 msgid ""
 "These Terms of Service shall come into force and effect on 15th May 2023."
-msgstr "這些「服務條款」應在2017年9月1日實施並生效。"
+msgstr "這些「服務條款」應在2023 年 3 月 15 日實施並生效。"
 
 #~ msgid ""
 #~ "In case you purchase service from us, we collect additional billing "
 #~ "information necessary for issuing an invoice"
 #~ msgstr "如果您向我們購買服務，我們會收集開立發票所需的其他結帳資訊"
 
 #~ msgid "Payment processors."
```

### Comparing `wllegal-2023.3/wllegal/templates/legal/documents/privacy.html` & `wllegal-2023.4/wllegal/templates/legal/documents/privacy.html`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,20 @@
 
 <p>{% blocktrans %}The Controller has made all reasonable technical means to protect the Personal Data. Only authorized persons can access the Personal Data.{% endblocktrans %}</p>
 
 <p>{% blocktrans %}Third parties which can gain access to the Personal Data when necessary are:{% endblocktrans %}</p>
 
 <ul>
     <li>{% blocktrans %}Persons which are contracted for technical assurance of the service.{% endblocktrans %}</li>
-    <li>{% blocktrans %}Payment processors when purchasing a service from us.{% endblocktrans %}</li>
+    <li>{% blocktrans %}If you purchase a service from us, a payment processor gets essential access to your Personal Data, limited to the bare minimum needed to process your payment.{% endblocktrans %}</li>
 </ul>
 
 <p>{% blocktrans %}All Personal Data is stored in the European Union.{% endblocktrans %}</p>
 
-<h2>{% blocktrans %}Disclossure of the Personal Data{% endblocktrans %}</h2>
+<h2>{% blocktrans %}Disclosure of the Personal Data{% endblocktrans %}</h2>
 
 <p>{% blocktrans %}The Personal Data might be disclosed to third parties in limited circumstances when the Controller has a good faith belief it is required by law, such as under a subpoena or other judicial or administrative order.{% endblocktrans %}</p>
 
 <p>{% blocktrans %}In case the Controller is required by law to disclose the Personal Data, an attempt will be made to provide the User with prior notice by e-mail (unless the Controller is prohibited, or it would be futile) that a request for the Personal Data has been made to allow the User to object to the disclosure. If the User does not challenge the disclosure request, the Controller may be legally required to turn over the Personal Data.{% endblocktrans %}</p>
 
 <h2>{% blocktrans %}The Personal Data retention{% endblocktrans %}</h2>
```

#### html2text {}

```diff
@@ -47,19 +47,20 @@
 {% blocktrans %}The Controller has made all reasonable technical means to
 protect the Personal Data. Only authorized persons can access the Personal
 Data.{% endblocktrans %}
 {% blocktrans %}Third parties which can gain access to the Personal Data when
 necessary are:{% endblocktrans %}
     * {% blocktrans %}Persons which are contracted for technical assurance of
       the service.{% endblocktrans %}
-    * {% blocktrans %}Payment processors when purchasing a service from us.{%
-      endblocktrans %}
+    * {% blocktrans %}If you purchase a service from us, a payment processor
+      gets essential access to your Personal Data, limited to the bare minimum
+      needed to process your payment.{% endblocktrans %}
 {% blocktrans %}All Personal Data is stored in the European Union.{%
 endblocktrans %}
-***** {% blocktrans %}Disclossure of the Personal Data{% endblocktrans %} *****
+***** {% blocktrans %}Disclosure of the Personal Data{% endblocktrans %} *****
 {% blocktrans %}The Personal Data might be disclosed to third parties in
 limited circumstances when the Controller has a good faith belief it is
 required by law, such as under a subpoena or other judicial or administrative
 order.{% endblocktrans %}
 {% blocktrans %}In case the Controller is required by law to disclose the
 Personal Data, an attempt will be made to provide the User with prior notice by
 e-mail (unless the Controller is prohibited, or it would be futile) that a
```

### Comparing `wllegal-2023.3/wllegal/templates/legal/documents/summary.html` & `wllegal-2023.4/wllegal/templates/legal/documents/summary.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/wllegal/templates/legal/documents/tos.html` & `wllegal-2023.4/wllegal/templates/legal/documents/tos.html`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/wllegal/templates/security.txt` & `wllegal-2023.4/wllegal/templates/security.txt`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/wllegal/templates/weblate_503.html` & `wllegal-2023.4/wllegal/templates/weblate_503.html`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             </div>
 
             <div class="clear"></div>
             <div class="footer-center">
                 <a href="https://status.weblate.org/" class="service-status l10n">Service Status</a>
             </div>
 			<div class="footer-left">
-                Copyright © 2012–2021 <a href="https://cihar.com/">Michal Čihař</a> • <a href="https://docs.weblate.org/en/latest/license.html" class="l10n">Licensed GNU GPLv3+</a>
+                Copyright © <a href="https://cihar.com/">Michal Čihař</a> • <a href="https://docs.weblate.org/en/latest/license.html" class="l10n">Licensed GNU GPLv3+</a>
             </div>
             <div class="footer-right"><a href="https://weblate.org/terms/" class="l10n">Terms and Privacy</a> • Design by <a href="https://vitavalka.com/">Vita Valka</a></div>
 		</div>
     </footer>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -24,9 +24,9 @@
 
 ****** Rate limit ******
 You have made too many requests too quickly. Please try again later.
 
 weblate
 
 Service_Status
-Copyright Â© 2012â2021 Michal_ÄihaÅ â¢ Licensed_GNU_GPLv3+
+Copyright Â© Michal_ÄihaÅ â¢ Licensed_GNU_GPLv3+
 Terms_and_Privacy â¢ Design by Vita_Valka
```

### Comparing `wllegal-2023.3/wllegal/templates/weblate_50x.html` & `wllegal-2023.4/wllegal/templates/weblate_50x.html`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             </div>
 
             <div class="clear"></div>
             <div class="footer-center">
                 <a href="https://status.weblate.org/" class="service-status l10n">Service Status</a>
             </div>
 			<div class="footer-left">
-                Copyright © 2012–2021 <a href="https://cihar.com/">Michal Čihař</a> • <a href="https://docs.weblate.org/en/latest/license.html" class="l10n">Licensed GNU GPLv3+</a>
+                Copyright © <a href="https://cihar.com/">Michal Čihař</a> • <a href="https://docs.weblate.org/en/latest/license.html" class="l10n">Licensed GNU GPLv3+</a>
             </div>
             <div class="footer-right"><a href="https://weblate.org/terms/" class="l10n">Terms and Privacy</a> • Design by <a href="https://vitavalka.com/">Vita Valka</a></div>
 		</div>
     </footer>
 
   </body>
 </html>
```

#### html2text {}

```diff
@@ -24,9 +24,9 @@
 
 ****** Maintenance in progress ******
 This site is currently down for maintenance.
 
 weblate
 
 Service_Status
-Copyright Â© 2012â2021 Michal_ÄihaÅ â¢ Licensed_GNU_GPLv3+
+Copyright Â© Michal_ÄihaÅ â¢ Licensed_GNU_GPLv3+
 Terms_and_Privacy â¢ Design by Vita_Valka
```

### Comparing `wllegal-2023.3/wllegal/templatetags/lawlinks.py` & `wllegal-2023.4/wllegal/templatetags/lawlinks.py`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/wllegal/tests.py` & `wllegal-2023.4/wllegal/tests.py`

 * *Files identical despite different names*

### Comparing `wllegal-2023.3/wllegal.egg-info/PKG-INFO` & `wllegal-2023.4/wllegal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wllegal
-Version: 2023.3
+Version: 2023.4
 Summary: Hosted Weblate legal stuff
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/wllegal
 Author: Michal Čihař
 Author-email: michal@cihar.com
 License: GPL-3.0-or-later
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/wllegal/issues
```

### Comparing `wllegal-2023.3/wllegal.egg-info/SOURCES.txt` & `wllegal-2023.4/wllegal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

