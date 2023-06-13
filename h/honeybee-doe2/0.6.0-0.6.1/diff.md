# Comparing `tmp/honeybee-doe2-0.6.0.tar.gz` & `tmp/honeybee-doe2-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.6.0.tar", last modified: Mon Jun  5 14:46:37 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.6.1.tar", last modified: Tue Jun 13 23:52:13 2023, max compression
```

## Comparing `honeybee-doe2-0.6.0.tar` & `honeybee-doe2-0.6.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/interiorfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 14:46:36.000000 honeybee-doe2-0.6.0/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:46:36.000000 honeybee-doe2-0.6.0/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 14:46:36.000000 honeybee-doe2-0.6.0/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 14:46:36.000000 honeybee-doe2-0.6.0/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 14:46:36.000000 honeybee-doe2-0.6.0/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-05 14:46:37.000000 honeybee-doe2-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-05 14:45:20.000000 honeybee-doe2-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/interiorfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/setup.py
```

### Comparing `honeybee-doe2-0.6.0/LICENSE` & `honeybee-doe2-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/PKG-INFO` & `honeybee-doe2-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.6.0
+Version: 0.6.1
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.6.0/README.md` & `honeybee-doe2-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.6.1/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.6.1/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.6.1/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/groundcontact.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 class GroundFloor:
     def __init__(self, face):
         self.face = face
         self.polygon = DoePolygon.from_face(face, flip=True)
 
     def to_inp(self, space_origin):
-
-        azimuth = 180 if self.face.azimuth == 0 else self.face.azimuth
+        azimuth = 180
         origin_pt = self.face.geometry.lower_left_corner - space_origin
 
         # create a unique polygon for ground floor faces
         polygon_name = f'{self.face.display_name}_ug Plg'
         polygon = self.polygon.to_inp(name=polygon_name) + '\n'
         obj_lines = [polygon]
         obj_lines.append(
```

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/interiorfloor.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/interiorfloor.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         self.polygon = DoePolygon.from_face(face, flip=True)
 
     def to_inp(self, space_origin):
         p_name = short_name(self.face.display_name)
 
         constr = self.face.properties.energy.construction.display_name
         tilt = 90 - self.face.altitude
-        azimuth = 180 if self.face.azimuth == 0 else self.face.azimuth
+        azimuth = 180 if abs(180 - tilt) <= 0.01 else self.face.azimuth
         origin_pt = self.face.geometry.lower_left_corner - space_origin
 
         # create a unique polygon for exposed floor faces
         polygon_name = f'{self.face.display_name}_ef Plg'
         polygon = self.polygon.to_inp(name=polygon_name) + '\n'
         obj_lines = [polygon]
```

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/roof.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     def to_inp(self, space_origin):
 
         p_name = short_name(self.face.display_name)
 
         constr = self.face.properties.energy.construction.display_name
         tilt = 90 - self.face.altitude
-        azimuth = 180 if self.face.azimuth == 0 and tilt == 0 else self.face.azimuth
+        azimuth = 180 if abs(tilt) <= 0.01 else self.face.azimuth
         origin_pt = self.face.geometry.lower_left_corner - space_origin
 
         spc = ''
         obj_lines = []
 
         obj_lines.append('"{}" = ROOF'.format(p_name))
         obj_lines.append('\n   POLYGON           = "{}"'.format(p_name+' Plg'))
```

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/room.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from honeybee.boundarycondition import Ground, Outdoors, Surface
 from honeybee.facetype import Wall, Floor, RoofCeiling
 from honeybee.face import Face
 from honeybee.room import Room, Point3D
 from typing import List
 
 from ..utils.doe_formatters import short_name
-from ..utils.geometry import get_floor_boundary, get_room_rep_poly
+from ..utils.geometry import get_room_rep_poly
 from .wall import DoeWall
 from .roof import DoeRoof
 from .groundcontact import GroundFloor
 from .exposedfloor import ExposedFloor
 from .interiorfloor import InteriorFloor
 
 
@@ -106,17 +106,16 @@
 
     @property
     def activity_disc(self):
         pass
     # TODO add activity disc // loads support etc
 
     def space(self, floor_origin):
-
-        floor_face = self.boundary
-        azimuth = floor_face.azimuth
+        # chances that a space is defined by a different azimuth than 0 is very low
+        azimuth = 0
         # this value should be set in relation to the Floor object
         origin_pt = self.origin - floor_origin
         obj_lines = []
         obj_lines.append('"{}" = SPACE\n'.format(short_name(self.host.display_name)))
         obj_lines.append('   SHAPE           = POLYGON\n')
         obj_lines.append('   POLYGON         = "{} Plg"\n'.format(
             self.boundary.display_name))
```

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.6.1/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.6.1/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.6.1/honeybee_doe2/utils/geometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,40 @@
+from typing import List
+from uuid import uuid4
+
 from ladybug_geometry.geometry3d import Point3D, Face3D
 from ladybug_geometry.geometry2d import Polygon2D, Point2D
 from honeybee.face import Face
+from honeybee.room import Room
 from honeybee.facetype import Floor
-from uuid import uuid4
+
+
+def _try_get_boundary(in_boundaries: List[Polygon2D], small_to_large=False):
+    """Try to get union boundaries from boundaries."""
+    tolerances = [0.01, 0.1, 0.2, 0.5, 1.0, 1.5, 2.0]
+
+    if not small_to_large:
+        tolerances = list(reversed(tolerances))
+
+    for tolerance in tolerances:
+        try:
+            boundaries = Polygon2D.boolean_union_all(in_boundaries, tolerance=tolerance)
+            if not boundaries and tolerance != tolerances[-1]:
+                raise ValueError
+        except Exception as e:
+            if tolerance != tolerances[-1]:
+                continue
+            else:
+                raise ValueError(
+                    f'Failed to merge the floors:\n{str(e)}'
+                )
+        else:
+            break
+
+    return boundaries
 
 
 def get_floor_boundary(rooms):
     """Get a list of vertices for floor boundary for a list of rooms.
 
     This function joins all the floor faces and returns a list of Point3D that define the
     border of the floor in counter clockwise order starting from the lower left corner.
@@ -18,59 +46,55 @@
     for room in rooms:
         for face in room.faces:
             if isinstance(face.type, Floor):
                 floor_geom.append(face.geometry)
 
     # get the minimum z and use it for all the floors
     z = min(geo.plane.o.z for geo in floor_geom)
-    boundaries = []
+    in_boundaries = []
     # floors are most likely horizontal - let's make them 2D polygons
     for floor in floor_geom:
         boundary = Polygon2D(
             [
                 Point2D(v.x, v.y) for v in floor.lower_left_counter_clockwise_vertices
             ]
         )
-        boundaries.append(boundary)
+        in_boundaries.append(boundary)
 
     # find the union of the boundary polygons
-    boundaries = Polygon2D.boolean_union_all(boundaries, tolerance=0.01)
-
-    # ? I don't know if this is the right assumption
-    # * assert len(boundaries) == 1, \
-    # *    'Input story generates more than one polygon ' \
-    # *    f'[{len(boundaries)}]. Not in DOE2!'
+    boundaries = _try_get_boundary(in_boundaries, small_to_large=False)
 
     boundary = [
         Point3D(point.x, point.y, z) for point in boundaries[0].vertices
     ]
 
     vertices = Face3D(
         boundary,
         plane=floor_geom[0].plane
     ).lower_left_counter_clockwise_vertices
 
     return vertices
 
 
-def get_room_rep_poly(room):
+def get_room_rep_poly(room: Room):
     floors = [face for face in room.faces if str(face.type) == 'Floor']
     z = min(geo.geometry.plane.o.z for geo in floors)
 
     boundaries = []
 
     for floor in floors:
         boundaries.append(
             Polygon2D(
                 [Point2D(v.x, v.y)
                  for v in
                  floor.geometry.lower_left_counter_clockwise_vertices]))
 
-    boundaries = Polygon2D.boolean_union_all(boundaries, tolerance=0.01)
-
+    boundaries = _try_get_boundary(boundaries, small_to_large=True)
+    assert len(boundaries) == 1, \
+        f'Failed to find a single boundary for {room.display_name} [{room.identifier}]'
     boundary = [
         Point3D(point.x, point.y, z) for point in boundaries[0].vertices
     ]
 
     new_face = Face3D(
         boundary,
         plane=floors[0].geometry.plane
```

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2/writer.py` & `honeybee-doe2-0.6.1/honeybee_doe2/writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,22 +20,42 @@
     rp = RunPeriod()
     comp_data = ComplianceData()
     sb_data = sbd()
 
     hb_model.convert_to_units(units='Feet')
 
     room_names = {}
+    face_names = {}
     for room in hb_model.rooms:
+        room.display_name = room.display_name.replace('..', '_')
         if room.display_name in room_names:
             original_name = room.display_name
             room.display_name = f'{original_name}_{room_names[original_name]}'
             room_names[original_name] += 1
         else:
             room_names[room.display_name] = 1
 
+        for face in room.faces:
+            face.display_name = face.display_name.replace('..', '_')
+            if face.display_name in face_names:
+                original_name = face.display_name
+                face.display_name = f'{original_name}_{face_names[original_name]}'
+                face_names[original_name] += 1
+            else:
+                face_names[face.display_name] = 1
+
+            for apt in face.apertures:
+                apt.display_name = apt.display_name.replace('..', '_')
+                if apt.display_name in face_names:
+                    original_name = apt.display_name
+                    apt.display_name = f'{original_name}_{face_names[original_name]}'
+                    face_names[original_name] += 1
+                else:
+                    face_names[face.display_name] = 1
+
     room_mapper = {
         r.identifier: r.display_name for r in hb_model.rooms
     }
     for i, shade in enumerate(hb_model.shades):
         shade.display_name = f'shade_{i}'
     for face in hb_model.faces:
         if isinstance(face.boundary_condition, Surface):
```

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.6.1/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.6.0
+Version: 0.6.1
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.6.0/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.6.1/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.0/setup.py` & `honeybee-doe2-0.6.1/setup.py`

 * *Files identical despite different names*

