# Comparing `tmp/collective.immediatecreate-1.0a3.tar.gz` & `tmp/collective.immediatecreate-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.immediatecreate-1.0a3.tar", last modified: Wed Nov  7 09:27:54 2018, max compression
+gzip compressed data, was "collective.immediatecreate-2.0.0.tar", last modified: Wed Jun 14 08:27:58 2023, max compression
```

## Comparing `collective.immediatecreate-1.0a3.tar` & `collective.immediatecreate-2.0.0.tar`

### file list

```diff
@@ -1,64 +1,57 @@
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/
--rw-r--r--   0 mhilbert (1824542945) 2074541850     1373 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/.gitlab-ci.yml
--rw-r--r--   0 mhilbert (1824542945) 2074541850     1242 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/.travis.yml
--rwxr-xr-x   0 mhilbert (1824542945) 2074541850      148 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/bootstrap.sh
--rw-r--r--   0 mhilbert (1824542945) 2074541850      291 2018-11-07 09:16:26.000000 collective.immediatecreate-1.0a3/CHANGES.rst
--rw-r--r--   0 mhilbert (1824542945) 2074541850      148 2018-11-07 09:24:22.000000 collective.immediatecreate-1.0a3/CONTRIBUTORS.rst
--rw-r--r--   0 mhilbert (1824542945) 2074541850      297 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/DEVELOP.rst
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/docs/
--rw-r--r--   0 mhilbert (1824542945) 2074541850       99 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/docs/index.rst
--rw-r--r--   0 mhilbert (1824542945) 2074541850    18092 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/LICENSE.GPL
--rw-r--r--   0 mhilbert (1824542945) 2074541850      670 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/LICENSE.rst
--rw-r--r--   0 mhilbert (1824542945) 2074541850      137 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/MANIFEST.in
--rw-r--r--   0 mhilbert (1824542945) 2074541850     7471 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/PKG-INFO
--rw-r--r--   0 mhilbert (1824542945) 2074541850       30 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/pyproject.toml
--rw-r--r--   0 mhilbert (1824542945) 2074541850     5001 2018-11-07 09:25:27.000000 collective.immediatecreate-1.0a3/README.rst
--rw-r--r--   0 mhilbert (1824542945) 2074541850       68 2018-11-06 14:52:52.000000 collective.immediatecreate-1.0a3/requirements.txt
--rw-r--r--   0 mhilbert (1824542945) 2074541850      314 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/setup.cfg
--rw-r--r--   0 mhilbert (1824542945) 2074541850     1641 2018-11-07 09:15:25.000000 collective.immediatecreate-1.0a3/setup.py
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective/
--rw-r--r--   0 mhilbert (1824542945) 2074541850       80 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/__init__.py
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/
--rw-r--r--   0 mhilbert (1824542945) 2074541850      143 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/__init__.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850     1853 2018-11-06 14:55:38.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/adding.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850      351 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/behaviors.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850     1244 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/cleanup.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850     2512 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/configure.zcml
--rw-r--r--   0 mhilbert (1824542945) 2074541850     4026 2018-09-12 10:00:22.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/editing.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850      441 2018-11-06 14:28:29.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/events.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850      292 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/indexer.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850      275 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/interfaces.py
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/locales/
--rw-r--r--   0 mhilbert (1824542945) 2074541850        0 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/locales/collective.immediatecreate.pot
--rwxr-xr-x   0 mhilbert (1824542945) 2074541850      515 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/locales/update.sh
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/profiles/
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/profiles/default/
--rw-r--r--   0 mhilbert (1824542945) 2074541850      204 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/profiles/default/browserlayer.xml
--rw-r--r--   0 mhilbert (1824542945) 2074541850      201 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/profiles/default/catalog.xml
--rw-r--r--   0 mhilbert (1824542945) 2074541850      195 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/profiles/default/metadata.xml
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/profiles/uninstall/
--rw-r--r--   0 mhilbert (1824542945) 2074541850      136 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 mhilbert (1824542945) 2074541850      170 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/profiles/uninstall/catalog.xml
--rw-r--r--   0 mhilbert (1824542945) 2074541850      603 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/setuphandlers.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850     1989 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/testing.py
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/
--rw-r--r--   0 mhilbert (1824542945) 2074541850        0 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/__init__.py
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/robot/
--rw-r--r--   0 mhilbert (1824542945) 2074541850   218068 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/robot/test_image.jpg
--rw-r--r--   0 mhilbert (1824542945) 2074541850     4229 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/robot/test_immediatecreate.robot
--rw-r--r--   0 mhilbert (1824542945) 2074541850     2661 2018-11-06 14:59:10.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/test_adding.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850      962 2018-11-06 14:59:42.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/test_robot.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850     2312 2018-11-06 15:00:14.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/test_setup.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850      195 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/upgrades.py
--rw-r--r--   0 mhilbert (1824542945) 2074541850      395 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/src/collective/immediatecreate/upgrades.zcml
-drwxr-xr-x   0 mhilbert (1824542945) 2074541850        0 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/
--rw-r--r--   0 mhilbert (1824542945) 2074541850        1 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/dependency_links.txt
--rw-r--r--   0 mhilbert (1824542945) 2074541850       53 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/entry_points.txt
--rw-r--r--   0 mhilbert (1824542945) 2074541850       11 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/namespace_packages.txt
--rw-r--r--   0 mhilbert (1824542945) 2074541850        1 2018-09-12 09:52:16.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/not-zip-safe
--rw-r--r--   0 mhilbert (1824542945) 2074541850     7471 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/PKG-INFO
--rw-r--r--   0 mhilbert (1824542945) 2074541850      113 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/requires.txt
--rw-r--r--   0 mhilbert (1824542945) 2074541850     2000 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/SOURCES.txt
--rw-r--r--   0 mhilbert (1824542945) 2074541850       11 2018-11-07 09:27:54.000000 collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/top_level.txt
--rwxr-xr-x   0 mhilbert (1824542945) 2074541850       36 2018-09-12 09:50:50.000000 collective.immediatecreate-1.0a3/style.sh
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      379 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/CHANGES.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      148 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/CONTRIBUTORS.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)    18092 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/LICENSE.GPL
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      670 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/LICENSE.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      137 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/MANIFEST.in
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     6456 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     5076 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/README.rst
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       55 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/constraints.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      123 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/requirements.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      245 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/setup.cfg
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1692 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/setup.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.309770 collective.immediatecreate-2.0.0/src/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       56 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/__init__.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      119 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/__init__.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1785 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/adding.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      327 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/behaviors.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1215 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/cleanup.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2393 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/configure.zcml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     3929 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/editing.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      417 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/events.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      268 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/indexer.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      251 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/interfaces.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/locales/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/locales/collective.immediatecreate.pot
+-rwxrwxr-x   0 jensens   (1000) jensens   (1000)      515 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/locales/update.sh
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.309770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/default/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      197 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/default/browserlayer.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      201 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/default/catalog.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      195 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/default/metadata.xml
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/uninstall/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      129 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      173 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/profiles/uninstall/catalog.xml
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      571 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/setuphandlers.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1965 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/testing.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/__init__.py
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.317770 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)   218068 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/test_image.jpg
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     4229 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/test_immediatecreate.robot
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2556 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_adding.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      934 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_robot.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     2302 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_setup.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      171 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/upgrades.py
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      404 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective/immediatecreate/upgrades.zcml
+drwxrwxr-x   0 jensens   (1000) jensens   (1000)        0 2023-06-14 08:27:58.313770 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     6456 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/PKG-INFO
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)     1925 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       40 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/entry_points.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/namespace_packages.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)        1 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/not-zip-safe
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)      117 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/requires.txt
+-rw-rw-r--   0 jensens   (1000) jensens   (1000)       11 2023-06-14 08:27:58.000000 collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.immediatecreate-1.0a3/LICENSE.GPL` & `collective.immediatecreate-2.0.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-1.0a3/LICENSE.rst` & `collective.immediatecreate-2.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-1.0a3/README.rst` & `collective.immediatecreate-2.0.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 collective.immediatecreate
 ==========================
 
 .. image:: https://img.shields.io/pypi/v/collective.immediatecreate.svg
     :target: https://pypi.org/project/collective.immediatecreate/
     :alt: Latest PyPI version
 
-.. image:: https://travis-ci.org/collective/collective.immediatecreate.svg?branch=master
-    :target: https://travis-ci.org/collective/collective.immediatecreate
+.. image:: https://github.com/collective/collective.immediatecreate/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/collective/collective.immediatecreate/actions/workflows/test.yml
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
 
 Folderish types are designed to be able to contain content.
-However, when you use ``collective.folderishtypes`` (or amy custom folderish types) in Plone and you simply add a folderish item and edit it immediately after adding you will see that all the assets you upload through the editor will be stored as siblings of the item you just created.
-This is due to the fact that the new item does not "exist" yet, that is, before it has been saved once.
+When you use ``collective.folderishtypes`` (or any custom folderish types) in Plone and you simply add a folderish item on edit (like an image in TinyMCE), then  after adding you will see that all the assets you upload through the editor will be stored as siblings of the item you just created.
+This is due to the fact that the new item does not "exist" yet - it is just an add-form - that is, before it has been saved once.
 
 This addon creates the object immediately, so items can be stored inside.
 
 Features
 --------
 
 ID/ Shortname
     A valid (and intermediate) ID will be generated after "add <Type>..." has been clicked, so the item can be persisted.
     However, the ID changes when the user saves the content for the first time so the Plone's default behavior is retained.
-    However, this feature might not be wanted by some users and is configureable (todo).
+    This feature might not be wanted by some users and is configureable (todo).
 
 Verification
     Additionally the drop-in-feature covers the usecase when an added type has mandatory fields or custom verification.
     All verification tasks are performed as usual when the user saves an item.
 
 Cancel becomes Delete
     When the user interacts with the item after it has been automatically created the "cancel" button is turned into a "delete" button.
@@ -42,66 +42,68 @@
     In order to get rid of initially created but never saved nor deleted items,
     a cleanup script is provided.
 
 
 Installation
 ------------
 
-Install ``collective.immediatecreate`` by adding it to your buildout::
+Install ``collective.immediatecreate`` by adding it to your buildout:
 
-    [buildout]
-
-    ...
+.. code-block:: INI
 
+    [buildout]
+    # ...
     eggs =
         collective.immediatecreate
 
 
 and then running ``bin/buildout``
 
 Restart Plone and install ``Immediate Create`` in control panel under addons.
 
 
 Activation
 ----------
 
 After installation nothing changed.
-The feature must be activated for a type first.
+The feature must be activated for a content-type first.
 To make a type available for immediate create, two changes need to be done:
 
 1. Add the behavior `collective.immediatecreate` to the type in the control panel under `Dexterity Content Types`
 
 2. Modify the Factory Type Information using the ZMI under `portal_types`.
    Change the value of  `Add view URL (Expression)` to `++addimmediate++TYPENAME`.
 
 Configuration using GenericSetup
 --------------------------------
 
-In a policy profile in filesystem the a Type Information under `profiles/default/types/TYPENAME.xml` can be edited to make a type aware of immediate create::
+In a policy profile in filesystem the a Type Information under `profiles/default/types/TYPENAME.xml` can be edited to make a type aware of immediate create:
+
+.. code-block:: XML
 
-    <?xml version="1.0"?>
-    <object
-        i18n:domain="plone"
-        meta_type="Dexterity FTI"
-        name="MyFolderishType"
-        xmlns:i18n="http://xml.zope.org/namespaces/i18n">
+   <?xml version="1.0"?>
+   <object
+     i18n:domain="plone"
+     meta_type="Dexterity FTI"
+     name="MyFolderishType"
+     xmlns:i18n="http://xml.zope.org/namespaces/i18n">
 
-        <!-- ... SNIP ... -->
+     <!-- ... SNIP ... -->
 
-        <property name="add_view_expr">string:${folder_url}/++addimmediate++MyFolderishType</property>
+     <property name="add_view_expr">string:${folder_url}/++addimmediate++MyFolderishType</property>
 
-        <!-- ... SNIP ... -->
+     <!-- ... SNIP ... -->
 
-        <!-- Enabled behaviors -->
-        <property name="behaviors" purge="False">
-          <element value="collective.immediatecreate" />
-        </property>
+     <!-- Enabled behaviors -->
+     <property name="behaviors" purge="False">
+       <element value="collective.immediatecreate" />
+     </property>
 
-        <!-- ... SNIP ... -->
-    </object>
+     <!-- ... SNIP ... -->
+   </object>
 
 Cleanup
 -------
 
 A cleanup script can be called as Manager user.
 It removes all stalled creations older than two hours.
 It is named ``@@immediatecreate-cleanup-leftovers``.
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/adding.py` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/adding.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from collective.immediatecreate.events import ImmediateAddedEvent
 from plone import api
 from plone.protect.interfaces import IDisableCSRFProtection
 from plone.protect.utils import addTokenToUrl
 from Products.Five.browser import BrowserView
 from zExceptions import Unauthorized
 from zope.event import notify
@@ -10,41 +9,40 @@
 from zope.interface import implementer
 from zope.location.interfaces import LocationError
 from zope.traversing.interfaces import ITraversable
 
 
 class ImmediateAddView(BrowserView):
     def __init__(self, context, request, fti):
-        super(ImmediateAddView, self).__init__(context, request)
+        super().__init__(context, request)
         self.fti = fti
 
     def __call__(self):
         # construct content
         if not self.fti.isConstructionAllowed(self.context):
             raise Unauthorized()
         newcontent = api.content.create(
             container=self.context,
             type=self.fti.getId(),
-            id="new-{0:s}".format(self.fti.getId()),
+            id=f"new-{self.fti.getId():s}",
             safe_id=True,
             collective_immediatecreate="initial",
         )
         notify(ImmediateAddedEvent(newcontent))
         newcontent.indexObject()
         alsoProvides(self.request, IDisableCSRFProtection)
         url = newcontent.absolute_url() + "/editimmediate"
         url = addTokenToUrl(url)
         self.request.response.redirect(url)
 
 
 @implementer(ITraversable)
-class ImmediateAddViewTraverser(object):
+class ImmediateAddViewTraverser:
 
-    """Immediate add view traverser.
-    """
+    """Immediate add view traverser."""
 
     def __init__(self, context, request):
         self.context = context
         self.request = request
 
     def traverse(self, name, ignored):
         ttool = api.portal.get_tool("portal_types")
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/cleanup.py` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/cleanup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from collective.immediatecreate import _
 from plone import api
 from Products.Five.browser import BrowserView
 
 import datetime
 
 
@@ -16,24 +15,24 @@
             in_immediate_creation=True,
             created={"query": two_hour_ago, "range": "max"},
         )
         objs = [b.getObject() for b in brains]
         count = len(objs)
         if count == 0:
             api.portal.show_message(
-                _(u"cleanup_delete_nothing", (u"Nothing to delete")),
+                _("cleanup_delete_nothing", ("Nothing to delete")),
                 request=self.request,
             )
             self.request.response.redirect(self.context.absolute_url())
         api.content.delete(objects=objs)
         api.portal.show_message(
             _(
-                u"cleanup_delete",
+                "cleanup_delete",
                 (
-                    u"${count} items left in creation state for more than two "
-                    u"hours deleted."
+                    "${count} items left in creation state for more than two "
+                    "hours deleted."
                 ),
                 mapping={"count": count},
             ),
             request=self.request,
         )
         self.request.response.redirect(self.context.absolute_url())
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/configure.zcml` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/configure.zcml`

 * *Files 7% similar despite different names*

```diff
@@ -1,80 +1,77 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:plone="http://namespaces.plone.org/plone"
     i18n_domain="collective.immediatecreate"
->
+    >
 
   <i18n:registerTranslations directory="locales" />
 
-  <!--
-    Be careful if you use general includeDependencies, it can have sideffects!
-    Better import explicite packages or configurations ;)
-  -->
-  <!--<includeDependencies package="." />-->
+  <include package="Products.CMFCore" />
 
   <include file="upgrades.zcml" />
 
   <genericsetup:registerProfile
       name="default"
       title="Immediate Create"
-      directory="profiles/default"
       description="Installs the collective.immediatecreate add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
       post_handler=".setuphandlers.post_install"
       />
 
   <genericsetup:registerProfile
       name="uninstall"
       title="Immediate Create (uninstall)"
-      directory="profiles/uninstall"
       description="Uninstalls the collective.immediatecreate add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/uninstall"
       post_handler=".setuphandlers.uninstall"
       />
 
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="collective.immediatecreate-hiddenprofiles"
       />
 
   <!-- behavior and indexer -->
   <plone:behavior
       name="collective.immediatecreate"
-      provides=".behaviors.ICollectiveImmediateCreate"
       title="Immediate Create"
       description="Creates item immediatly and skip add form. Needs changes in Factory Type Information (ZMI) for this type too!"
-  />
+      provides=".behaviors.ICollectiveImmediateCreate"
+      />
   <adapter
       factory=".indexer.index_in_immediate_creation"
       name="in_immediate_creation"
-  />
+      />
 
   <!-- traverser -->
   <adapter
-      name="addimmediate"
-      for="Products.CMFCore.interfaces.IFolderish .interfaces.ICollectiveImmediatecreateLayer"
       factory=".adding.ImmediateAddViewTraverser"
-  />
+      for="Products.CMFCore.interfaces.IFolderish
+           .interfaces.ICollectiveImmediatecreateLayer"
+      name="addimmediate"
+      />
 
   <!-- edit immediate -->
   <browser:page
-      for="plone.dexterity.interfaces.IDexterityContent"
-      layer=".interfaces.ICollectiveImmediatecreateLayer"
       name="editimmediate"
+      for="plone.dexterity.interfaces.IDexterityContent"
       class=".editing.ImmediateEditView"
       permission="cmf.AddPortalContent"
-  />
+      layer=".interfaces.ICollectiveImmediatecreateLayer"
+      />
 
   <!-- cleanup -->
   <browser:page
-      for="*"
-      layer=".interfaces.ICollectiveImmediatecreateLayer"
       name="immediatecreate-cleanup-leftovers"
+      for="*"
       class=".cleanup.CleanupImmediateLeftovers"
       permission="cmf.ManagePortal"
-  />
+      layer=".interfaces.ICollectiveImmediatecreateLayer"
+      />
 
 </configure>
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/editing.py` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/editing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from Acquisition import aq_parent
 from collective.immediatecreate import _
 from plone import api
 from plone.app.lockingbehavior.behaviors import ILocking
 from plone.dexterity.browser.base import DexterityExtensibleForm
 from plone.dexterity.events import EditBegunEvent
 from plone.dexterity.events import EditCancelledEvent
@@ -21,17 +20,17 @@
 from zope.container.interfaces import INameChooser
 from zope.event import notify
 from zope.interface import classImplements
 
 
 class ImmediateEditForm(DexterityExtensibleForm, form.EditForm):
 
-    success_message = _(u"New content saved")
+    success_message = _("New content saved")
 
-    @button.buttonAndHandler(_dx(u"Save"), name="save")
+    @button.buttonAndHandler(_dx("Save"), name="save")
     def handleApply(self, action):
         data, errors = self.extractData()
         if errors:
             self.status = self.formErrorsMessage
             return
         self.applyChanges(data)
         self.context.collective_immediatecreate = "created"
@@ -39,19 +38,17 @@
         chooser = INameChooser(aq_parent(self.context))
         new_id = chooser.chooseName(None, self.context)
         api.content.rename(obj=self.context, new_id=new_id)
         api.portal.show_message(self.success_message, self.request)
         self.request.response.redirect(self.nextURL())
         notify(EditFinishedEvent(self.context))
 
-    @button.buttonAndHandler(_dx(u"Cancel"), name="cancel")
+    @button.buttonAndHandler(_dx("Cancel"), name="cancel")
     def handleCancel(self, action):
-        api.portal.show_message(
-            _dx(u"Add New Item operation cancelled"), self.request
-        )
+        api.portal.show_message(_dx("Add New Item operation cancelled"), self.request)
         self.request.response.redirect(self.nextURL())
         notify(EditCancelledEvent(self.context))
         parent = aq_parent(self.context)
         api.content.delete(obj=self.context)
         self.context = parent
         self.request.response.redirect(self.nextURL())
 
@@ -78,34 +75,34 @@
         self.portal_type = self.context.portal_type
 
         if ILocking.providedBy(self.context):
             lockable = ILockable(self.context)
             if lockable.locked():
                 lockable.unlock()
 
-        super(ImmediateEditForm, self).update()
+        super().update()
 
         # fire the edit begun only if no action was executed
         if len(self.actions.executedActions) == 0:
             notify(EditBegunEvent(self.context))
 
     def updateActions(self):
-        super(ImmediateEditForm, self).updateActions()
+        super().updateActions()
 
         if "save" in self.actions:
             self.actions["save"].addClass("context")
 
         if "cancel" in self.actions:
             self.actions["cancel"].addClass("standalone")
 
     @property
     def fti(self):
         return getUtility(IDexterityFTI, name=self.portal_type)
 
     @property
     def label(self):
         type_name = self.fti.Title()
-        return _(u"Add ${name}", mapping={"name": type_name})
+        return _("Add ${name}", mapping={"name": type_name})
 
 
 ImmediateEditView = layout.wrap_form(ImmediateEditForm)
 classImplements(ImmediateEditView, IDexterityEditForm)
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/locales/update.sh` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/setuphandlers.py` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/setuphandlers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 from Products.CMFPlone.interfaces import INonInstallable
 from zope.interface import implementer
 
 
 @implementer(INonInstallable)
-class HiddenProfiles(object):
+class HiddenProfiles:
     def getNonInstallableProfiles(self):
         """Hide uninstall profile from site-creation and quickinstaller."""
         return ["collective.immediatecreate:uninstall"]
 
 
 def post_install(context):
     """Post install script"""
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/testing.py` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.robotframework.testing import REMOTE_LIBRARY_BUNDLE_FIXTURE
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneSandboxLayer
 from plone.testing import z2
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/robot/test_image.jpg` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/test_image.jpg`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/robot/test_immediatecreate.robot` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/robot/test_immediatecreate.robot`

 * *Files identical despite different names*

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/test_adding.py` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_adding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# -*- coding: utf-8 -*-
 """Setup tests for this package."""
 from collective.immediatecreate.events import IImmediateAddedEvent
 from collective.immediatecreate.events import ImmediateAddedEvent
-from collective.immediatecreate.testing import COLLECTIVE_IMMEDIATECREATE_INTEGRATION_TESTING  # noqa I001
+from collective.immediatecreate.testing import (
+    COLLECTIVE_IMMEDIATECREATE_INTEGRATION_TESTING,
+)
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from zope.component import getGlobalSiteManager
 
 import unittest
 
 
 class TestAdding(unittest.TestCase):
-    """Test that collective.immediatecreate adding traverse and view creates.
-    """
+    """Test that collective.immediatecreate adding traverse and view creates."""
 
     layer = COLLECTIVE_IMMEDIATECREATE_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         fti = self.portal.portal_types.Folder
         fti._updateProperty(
@@ -56,19 +56,14 @@
     def test_event_handler(self):
         sm = getGlobalSiteManager()
         firedEvents = []
 
         def recordEvent(event):
             firedEvents.append(event.__class__)
 
-        sm.registerHandler(recordEvent, (IImmediateAddedEvent, ))
+        sm.registerHandler(recordEvent, (IImmediateAddedEvent,))
 
         setRoles(self.portal, TEST_USER_ID, ["Contributor", "Editor"])
         view = self.portal.restrictedTraverse("++addimmediate++Folder")
         view()
 
-        self.assertItemsEqual(
-            firedEvents,
-            [
-                ImmediateAddedEvent,
-            ],
-        )
+        self.assertEqual(firedEvents, [ImmediateAddedEvent])
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/test_robot.py` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_robot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# -*- coding: utf-8 -*-
-from collective.immediatecreate.testing import COLLECTIVE_IMMEDIATECREATE_ACCEPTANCE_TESTING  # noqa I001
+from collective.immediatecreate.testing import (
+    COLLECTIVE_IMMEDIATECREATE_ACCEPTANCE_TESTING,
+)
 from plone.app.testing import ROBOT_TEST_LEVEL
 from plone.testing import layered
 
 import os
 import robotsuite
 import unittest
```

### Comparing `collective.immediatecreate-1.0a3/src/collective/immediatecreate/tests/test_setup.py` & `collective.immediatecreate-2.0.0/src/collective/immediatecreate/tests/test_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,64 @@
-# -*- coding: utf-8 -*-
 """Setup tests for this package."""
-from collective.immediatecreate.testing import COLLECTIVE_IMMEDIATECREATE_INTEGRATION_TESTING  # noqa I001
+from collective.immediatecreate.testing import (
+    COLLECTIVE_IMMEDIATECREATE_INTEGRATION_TESTING,
+)
 from plone import api
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
+from Products.CMFPlone.utils import get_installer
 
 import unittest
 
 
 class TestSetup(unittest.TestCase):
     """Test that collective.immediatecreate is properly installed."""
 
     layer = COLLECTIVE_IMMEDIATECREATE_INTEGRATION_TESTING
 
     def setUp(self):
         """Custom shared utility setup for tests."""
         self.portal = self.layer["portal"]
-        self.installer = api.portal.get_tool("portal_quickinstaller")
+        self.installer = get_installer(self.portal, self.layer["request"])
 
     def test_product_installed(self):
         """Test if collective.immediatecreate is installed."""
         self.assertTrue(
-            self.installer.isProductInstalled("collective.immediatecreate")
+            self.installer.is_product_installed("collective.immediatecreate")
         )
 
     def test_browserlayer(self):
         """Test that ICollectiveImmediatecreateLayer is registered."""
         from collective.immediatecreate.interfaces import (
             ICollectiveImmediatecreateLayer,
         )
         from plone.browserlayer import utils
 
-        self.assertIn(
-            ICollectiveImmediatecreateLayer, utils.registered_layers()
-        )
+        self.assertIn(ICollectiveImmediatecreateLayer, utils.registered_layers())
 
 
 class TestUninstall(unittest.TestCase):
 
     layer = COLLECTIVE_IMMEDIATECREATE_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
-        self.installer = api.portal.get_tool("portal_quickinstaller")
+        self.installer = get_installer(self.portal, self.layer["request"])
         roles_before = api.user.get_roles(TEST_USER_ID)
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
-        self.installer.uninstallProducts(["collective.immediatecreate"])
+        self.installer.uninstall_product("collective.immediatecreate")
         setRoles(self.portal, TEST_USER_ID, roles_before)
 
     def test_product_uninstalled(self):
         """Test if collective.immediatecreate is cleanly uninstalled."""
         self.assertFalse(
-            self.installer.isProductInstalled("collective.immediatecreate")
+            self.installer.is_product_installed("collective.immediatecreate")
         )
 
     def test_browserlayer_removed(self):
         """Test that ICollectiveImmediatecreateLayer is removed."""
         from collective.immediatecreate.interfaces import (
             ICollectiveImmediatecreateLayer,
         )
         from plone.browserlayer import utils
 
-        self.assertNotIn(
-            ICollectiveImmediatecreateLayer, utils.registered_layers()
-        )
+        self.assertNotIn(ICollectiveImmediatecreateLayer, utils.registered_layers())
```

### Comparing `collective.immediatecreate-1.0a3/src/collective.immediatecreate.egg-info/SOURCES.txt` & `collective.immediatecreate-2.0.0/src/collective.immediatecreate.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-.gitlab-ci.yml
-.travis.yml
 CHANGES.rst
 CONTRIBUTORS.rst
-DEVELOP.rst
 LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
-bootstrap.sh
-pyproject.toml
+constraints.txt
 requirements.txt
 setup.cfg
 setup.py
-style.sh
-docs/index.rst
 src/collective/__init__.py
 src/collective.immediatecreate.egg-info/PKG-INFO
 src/collective.immediatecreate.egg-info/SOURCES.txt
 src/collective.immediatecreate.egg-info/dependency_links.txt
 src/collective.immediatecreate.egg-info/entry_points.txt
 src/collective.immediatecreate.egg-info/namespace_packages.txt
 src/collective.immediatecreate.egg-info/not-zip-safe
```

