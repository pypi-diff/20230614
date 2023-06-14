# Comparing `tmp/honeybee-ph-1.9.0.tar.gz` & `tmp/honeybee-ph-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-ph-1.9.0.tar", last modified: Thu Mar 16 08:47:34 2023, max compression
+gzip compressed data, was "dist/honeybee-ph-1.9.1.tar", last modified: Fri Mar 17 10:46:29 2023, max compression
```

## Comparing `honeybee-ph-1.9.0.tar` & `honeybee-ph-1.9.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/_extend_honeybee_energy_ph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/construction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/construction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/construction/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/construction/thermal_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/construction/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/cooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/ducting.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/fuels.py
--rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/heating.py
--rw-r--r--   0 runner    (1001) docker     (123)    19616 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/hot_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/hvac/ventilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/library/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/library/programtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/load/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/load/__lighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/load/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/load/ph_equipment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/load/phius_mf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/construction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/construction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/construction/opaque.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/construction/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hot_water/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hot_water/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hot_water/hw_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hot_water/hw_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/allair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/doas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/heatcool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/idealair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/load/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/load/equipment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/load/lighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/load/people.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/materials/opaque.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/ruleset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_energy_ph/properties/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/_extend_honeybee_ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/bldg_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/phi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/phius.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/properties/shade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/properties/space.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18489 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/site.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph_standards/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph_standards/programtypes/
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/programtypes/PHIUS_programs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/programtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/programtypes/default_elec_equip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph_standards/sourcefactors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/sourcefactors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/sourcefactors/factors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/sourcefactors/phius_CO2_factors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_standards/sourcefactors/phius_source_energy_factors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/honeybee_ph_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/enumerables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/input_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/iso_10077_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/occupancy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/sky_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/honeybee_ph_utils/ventilation.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-16 08:47:34.000000 honeybee-ph-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-16 08:46:32.000000 honeybee-ph-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/_extend_honeybee_energy_ph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/construction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/construction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/construction/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/construction/thermal_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/construction/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/cooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/ducting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/fuels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/heating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19793 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/hot_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/hvac/ventilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/library/programtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/load/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/load/__lighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/load/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/load/ph_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/load/phius_mf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/construction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/construction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/construction/opaque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/construction/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hot_water/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hot_water/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hot_water/hw_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hot_water/hw_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/allair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/doas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/heatcool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/idealair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/load/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/load/equipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/load/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/load/people.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/materials/opaque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_energy_ph/properties/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/_extend_honeybee_ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/bldg_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/phi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/phius.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/properties/shade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/properties/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18489 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph_standards/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph_standards/programtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/programtypes/PHIUS_programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/programtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/programtypes/default_elec_equip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph_standards/sourcefactors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/sourcefactors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/sourcefactors/factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/sourcefactors/phius_CO2_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_standards/sourcefactors/phius_source_energy_factors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/honeybee_ph_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/enumerables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/input_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/iso_10077_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/occupancy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/sky_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/honeybee_ph_utils/ventilation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-17 10:46:29.000000 honeybee-ph-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-17 10:45:17.000000 honeybee-ph-1.9.1/setup.py
```

### Comparing `honeybee-ph-1.9.0/LICENSE` & `honeybee-ph-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/PKG-INFO` & `honeybee-ph-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-ph
-Version: 1.9.0
+Version: 1.9.1
 Summary: Plugin for Honeybee to enable Passive House modeling.
 Home-page: https://github.com/PH-Tools/honeybee_ph
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # Honeybee-PH:
         Honeybee-PH is a free plugin for [Ladybug Tools](https://www.ladybug.tools/) which enables users to add detailed "Passive House" style attributes to their models in addition to the normal Honeybee inputs. Both Passive House Institute (PHI) and Passive House Institute US (Phius) model data can be added to the Ladybug-Tools models using the plugin. Note that this plugin is in no way affiliated with or created by either the Passive House Institute (PHI) or the Passive House Institute US (Phius).
```

### Comparing `honeybee-ph-1.9.0/README.md` & `honeybee-ph-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/README.md` & `honeybee-ph-1.9.1/honeybee_energy_ph/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/_extend_honeybee_energy_ph.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/_extend_honeybee_energy_ph.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/construction/_base.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/construction/_base.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/construction/thermal_bridge.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/construction/thermal_bridge.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/construction/window.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/construction/window.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/hvac/_base.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/hvac/_base.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/hvac/cooling.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/hvac/cooling.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/hvac/ducting.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/hvac/ducting.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/hvac/fuels.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/hvac/fuels.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/hvac/heating.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/hvac/heating.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/hvac/hot_water.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/hvac/hot_water.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,36 +23,43 @@
 
 # -- Piping ---------------------------------------------------------------------
 
 
 class PhPipeSegment(_base._PhHVACBase):
     """A single pipe segment (linear) with geometry and a diameter"""
 
-    def __init__(self, _geom, _diameter=0.0127, _insul_thickness=0.0, _insul_conductivity=0.04, _insul_refl=True, _insul_quality=None, _daily_period=24.0):
+    def __init__(self, 
+                 _geom, 
+                 _diameter_m=0.0127, 
+                 _insul_thickness_m=0.0127, 
+                 _insul_conductivity=0.04, 
+                 _insul_refl=True, 
+                 _insul_quality=None, 
+                 _daily_period=24.0):
         # type: (LineSegment3D, float, float, float, bool, None, float) -> None
         super(PhPipeSegment, self).__init__()
         self.geometry = _geom
-        self.diameter = _diameter
-        self.insulation_thickness = _insul_thickness
+        self.diameter_m = _diameter_m
+        self.insulation_thickness_m = _insul_thickness_m
         self.insulation_conductivity = _insul_conductivity
         self.insulation_reflective = _insul_refl
         self.insulation_quality = _insul_quality
         self.daily_period = _daily_period
 
     @property
-    def length(self):
+    def length_m(self):
         # type: () -> float
         return self.geometry.length
 
     def __copy__(self):
         # type: () -> PhPipeSegment
         new_obj = PhPipeSegment(self.geometry)
 
-        new_obj.diameter = self.diameter
-        new_obj.insulation_thickness = self.insulation_thickness
+        new_obj.diameter_m = self.diameter_m
+        new_obj.insulation_thickness_m = self.insulation_thickness_m
         new_obj.insulation_conductivity = self.insulation_conductivity
         new_obj.insulation_reflective = self.insulation_reflective
         new_obj.insulation_quality = self.insulation_quality
         new_obj.daily_period = self.daily_period
         new_obj.identifier = self.identifier
         new_obj.display_name = self.display_name
         new_obj.user_data = self.user_data
@@ -64,16 +71,16 @@
         return self.__copy__()
 
     def to_dict(self):
         # type: () -> dict[str, Union[str, dict]]
         d = {}
 
         d['geometry'] = self.geometry.to_dict()
-        d['diameter'] = self.diameter
-        d['insulation_thickness'] = self.insulation_thickness
+        d['diameter_m'] = self.diameter_m
+        d['insulation_thickness_m'] = self.insulation_thickness_m
         d['insulation_conductivity'] = self.insulation_conductivity
         d['insulation_reflective'] = self.insulation_reflective
         d['insulation_quality'] = self.insulation_quality
         d['daily_period'] = self.daily_period
         d['identifier'] = self.identifier
         d['display_name'] = self.display_name
         d['user_data'] = self.user_data
@@ -82,28 +89,28 @@
 
     @classmethod
     def from_dict(cls, _input_dict):
         # type: (dict) -> PhPipeSegment
         new_obj = cls(
             _geom=LineSegment3D.from_dict(_input_dict['geometry'])
         )
-        new_obj.diameter = _input_dict['diameter']
-        new_obj.insulation_thickness = _input_dict['insulation_thickness']
+        new_obj.diameter_m = _input_dict['diameter_m']
+        new_obj.insulation_thickness_m = _input_dict['insulation_thickness_m']
         new_obj.insulation_conductivity = _input_dict['insulation_conductivity']
         new_obj.insulation_reflective = _input_dict['insulation_reflective']
         new_obj.insulation_quality = _input_dict['insulation_quality']
         new_obj.daily_period = _input_dict['daily_period']
         new_obj.identifier = _input_dict['identifier']
         new_obj.display_name = _input_dict['display_name']
         new_obj.user_data = _input_dict['user_data']
 
         return new_obj
 
     def __str__(self):
-        return "{}: diam={}, length={:.3f}".format(self.__class__.__name__, self.diameter, self.length)
+        return "{}: diam={}, length={:.3f}".format(self.__class__.__name__, self.diameter_m, self.length_m)
 
     def __repr__(self):
         return str(self)
 
     def ToString(self):
         return self.__repr__()
 
@@ -117,17 +124,17 @@
 
     @property
     def segments(self):
         # type: () -> List[PhPipeSegment]
         return list(self._segments.values())
 
     @property
-    def length(self):
+    def length_m(self):
         # type: () -> float
-        return sum(s.length for s in self.segments)
+        return sum(s.length_m for s in self.segments)
 
     def add_segment(self, _segment):
         # type: (PhPipeSegment) -> None
         self._segments[_segment.identifier] = _segment
 
     def __copy__(self):
         # type: () -> PhPipeElement
@@ -169,15 +176,15 @@
         new_obj.identifier = _input_dict['identifier']
         new_obj.display_name = _input_dict['display_name']
         new_obj.user_data = _input_dict['user_data']
 
         return new_obj
 
     def __str__(self):
-        return "{}: (display_name={}, identifier={} ) [{} segments, len={:.3f}]".format(self.__class__.__name__, self.display_name, self.identifier, len(self.segments), self.length)
+        return "{}: (display_name={}, identifier={} ) [{} segments, len={:.3f}]".format(self.__class__.__name__, self.display_name, self.identifier, len(self.segments), self.length_m)
 
     def __repr__(self):
         return str(self)
 
     def ToString(self):
         return self.__repr__()
```

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/hvac/ventilation.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/hvac/ventilation.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/library/programtypes.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/library/programtypes.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/load/__lighting.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/load/__lighting.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/load/_base.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/load/_base.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/load/ph_equipment.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/load/ph_equipment.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/load/phius_mf.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/load/phius_mf.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/construction/window.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/construction/window.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/hot_water/hw_program.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/hot_water/hw_program.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/hot_water/hw_system.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/hot_water/hw_system.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/allair.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/allair.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/doas.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/doas.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/heatcool.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/heatcool.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/hvac/idealair.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/hvac/idealair.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/load/equipment.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/load/equipment.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/load/lighting.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/load/lighting.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/load/people.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/load/people.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/materials/opaque.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/materials/opaque.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/ruleset.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/ruleset.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_energy_ph/properties/space.py` & `honeybee-ph-1.9.1/honeybee_energy_ph/properties/space.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/README.md` & `honeybee-ph-1.9.1/honeybee_ph/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/_base.py` & `honeybee-ph-1.9.1/honeybee_ph/_base.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/_extend_honeybee_ph.py` & `honeybee-ph-1.9.1/honeybee_ph/_extend_honeybee_ph.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/bldg_segment.py` & `honeybee-ph-1.9.1/honeybee_ph/bldg_segment.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/phi.py` & `honeybee-ph-1.9.1/honeybee_ph/phi.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/phius.py` & `honeybee-ph-1.9.1/honeybee_ph/phius.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/properties/aperture.py` & `honeybee-ph-1.9.1/honeybee_ph/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/properties/face.py` & `honeybee-ph-1.9.1/honeybee_ph/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/properties/model.py` & `honeybee-ph-1.9.1/honeybee_ph/properties/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/properties/room.py` & `honeybee-ph-1.9.1/honeybee_ph/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/properties/shade.py` & `honeybee-ph-1.9.1/honeybee_ph/properties/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/properties/space.py` & `honeybee-ph-1.9.1/honeybee_ph/properties/space.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/site.py` & `honeybee-ph-1.9.1/honeybee_ph/site.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph/space.py` & `honeybee-ph-1.9.1/honeybee_ph/space.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph.egg-info/PKG-INFO` & `honeybee-ph-1.9.1/honeybee_ph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-ph
-Version: 1.9.0
+Version: 1.9.1
 Summary: Plugin for Honeybee to enable Passive House modeling.
 Home-page: https://github.com/PH-Tools/honeybee_ph
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # Honeybee-PH:
         Honeybee-PH is a free plugin for [Ladybug Tools](https://www.ladybug.tools/) which enables users to add detailed "Passive House" style attributes to their models in addition to the normal Honeybee inputs. Both Passive House Institute (PHI) and Passive House Institute US (Phius) model data can be added to the Ladybug-Tools models using the plugin. Note that this plugin is in no way affiliated with or created by either the Passive House Institute (PHI) or the Passive House Institute US (Phius).
```

### Comparing `honeybee-ph-1.9.0/honeybee_ph.egg-info/SOURCES.txt` & `honeybee-ph-1.9.1/honeybee_ph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_standards/programtypes/PHIUS_programs.py` & `honeybee-ph-1.9.1/honeybee_ph_standards/programtypes/PHIUS_programs.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_standards/programtypes/default_elec_equip.py` & `honeybee-ph-1.9.1/honeybee_ph_standards/programtypes/default_elec_equip.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_standards/sourcefactors/factors.py` & `honeybee-ph-1.9.1/honeybee_ph_standards/sourcefactors/factors.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_standards/sourcefactors/phius_CO2_factors.py` & `honeybee-ph-1.9.1/honeybee_ph_standards/sourcefactors/phius_CO2_factors.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_standards/sourcefactors/phius_source_energy_factors.py` & `honeybee-ph-1.9.1/honeybee_ph_standards/sourcefactors/phius_source_energy_factors.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/enumerables.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/enumerables.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/histogram.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/histogram.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/input_tools.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/input_tools.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/iso_10077_1.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/iso_10077_1.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/occupancy.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/occupancy.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/preview.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/preview.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/schedules.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/sky_matrix.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/sky_matrix.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/honeybee_ph_utils/ventilation.py` & `honeybee-ph-1.9.1/honeybee_ph_utils/ventilation.py`

 * *Files identical despite different names*

### Comparing `honeybee-ph-1.9.0/setup.cfg` & `honeybee-ph-1.9.1/setup.cfg`

 * *Files identical despite different names*

