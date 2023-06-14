# Comparing `tmp/design.plone.ioprenoto-1.0.3.tar.gz` & `tmp/design.plone.ioprenoto-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.ioprenoto-1.0.3.tar", last modified: Tue Jun 13 09:42:28 2023, max compression
+gzip compressed data, was "design.plone.ioprenoto-1.0.4.tar", last modified: Wed Jun 14 13:03:41 2023, max compression
```

## Comparing `design.plone.ioprenoto-1.0.3.tar` & `design.plone.ioprenoto-1.0.4.tar`

### file list

```diff
@@ -1,104 +1,108 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      464 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       58 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1338 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      662 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      116 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6063 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4344 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/README.rst
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7986 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-06-13 09:42:28.370688 design.plone.ioprenoto-1.0.3/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2799 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      139 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      562 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/adapters/stringinterp.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/behaviors/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/behaviors/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1392 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/behaviors/additional_fields.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      591 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/behaviors/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      628 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/browser/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/browser/overrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/browser/overrides/.gitkeep
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/browser/static/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/browser/static/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1530 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/events/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/events/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      431 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/events/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      136 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/events/on_create.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      270 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1520 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1754 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/update.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/permissions.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/metadata.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      180 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/registry/main.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/types/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      280 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      414 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1685 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2773 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/services/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/services/bookable_list/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6155 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      167 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/services/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      794 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1930 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/robot/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2019 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/robot/test_example.robot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1231 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2221 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2800 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7008 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2459 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4095 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-13 09:42:28.366688 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6063 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3553 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      127 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      281 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-13 09:42:28.000000 design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      555 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       58 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1338 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      662 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      116 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6154 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4344 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/README.rst
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7986 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2799 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.574432 design.plone.ioprenoto-1.0.4/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/src/design/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/src/design/plone/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      139 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      562 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/stringinterp.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1392 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/additional_fields.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      591 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      628 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/overrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/overrides/.gitkeep
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/static/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/static/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1530 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/events/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/events/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      431 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/events/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      136 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/events/on_create.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      270 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1520 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.574432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.574432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1754 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/update.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/permissions.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.574432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      180 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/registry/main.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      280 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      414 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1685 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2773 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookable_list/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6155 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.582432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      354 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      653 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookings/search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      201 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      794 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1930 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.586432 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/robot/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2019 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/robot/test_example.robot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1231 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2221 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2800 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7008 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2459 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4095 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-14 13:03:41.578432 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6154 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3749 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      127 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      281 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-06-14 13:03:41.000000 design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/top_level.txt
```

### Comparing `design.plone.ioprenoto-1.0.3/DEVELOP.rst` & `design.plone.ioprenoto-1.0.4/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/LICENSE.GPL` & `design.plone.ioprenoto-1.0.4/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/LICENSE.rst` & `design.plone.ioprenoto-1.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/PKG-INFO` & `design.plone.ioprenoto-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ioprenoto
-Version: 1.0.3
+Version: 1.0.4
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/design.plone.ioprenoto
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ioprenoto/
 Project-URL: Source, https://github.com/RedTurtle/design.plone.ioprenoto
@@ -196,14 +196,21 @@
 - RedTurtle, info@redturtle.it
 
 
 Changelog
 =========
 
 
+1.0.4 (2023-06-14)
+------------------
+
+- Overrides @bookings for booking urls
+  [mamico]
+
+
 1.0.3 (2023-06-13)
 ------------------
 
 - typo "corellati" vs. "correlati" (+ i18n)
   [mamico]
```

### Comparing `design.plone.ioprenoto-1.0.3/README.rst` & `design.plone.ioprenoto-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/docs/conf.py` & `design.plone.ioprenoto-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/setup.py` & `design.plone.ioprenoto-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.ioprenoto",
-    version="1.0.3",
+    version="1.0.4",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/adapters/configure.zcml` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/adapters/stringinterp.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/behaviors/additional_fields.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/additional_fields.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/behaviors/configure.zcml` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/browser/configure.zcml` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/configure.zcml` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/README.rst` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/locales/update.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/setuphandlers.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/testing.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/robot/test_example.robot` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_setup.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py` & `design.plone.ioprenoto-1.0.4/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/PKG-INFO` & `design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.ioprenoto
-Version: 1.0.3
+Version: 1.0.4
 Summary: An add-on for Plone
 Home-page: https://github.com/collective/design.plone.ioprenoto
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/design.plone.ioprenoto/
 Project-URL: Source, https://github.com/RedTurtle/design.plone.ioprenoto
@@ -196,14 +196,21 @@
 - RedTurtle, info@redturtle.it
 
 
 Changelog
 =========
 
 
+1.0.4 (2023-06-14)
+------------------
+
+- Overrides @bookings for booking urls
+  [mamico]
+
+
 1.0.3 (2023-06-13)
 ------------------
 
 - typo "corellati" vs. "correlati" (+ i18n)
   [mamico]
```

### Comparing `design.plone.ioprenoto-1.0.3/src/design.plone.ioprenoto.egg-info/SOURCES.txt` & `design.plone.ioprenoto-1.0.4/src/design.plone.ioprenoto.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
 src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
 src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
 src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
 src/design/plone/ioprenoto/restapi/services/configure.zcml
 src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
 src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
+src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
+src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
+src/design/plone/ioprenoto/restapi/services/bookings/search.py
 src/design/plone/ioprenoto/tests/__init__.py
 src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
 src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
 src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
 src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
 src/design/plone/ioprenoto/tests/test_setup.py
 src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
```

