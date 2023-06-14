# Comparing `tmp/control_rod-2023.5.6.1.tar.gz` & `tmp/control_rod-2023.6.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control_rod-2023.5.6.1.tar", last modified: Sun May  7 03:50:37 2023, max compression
+gzip compressed data, was "control_rod-2023.6.13.0.tar", last modified: Wed Jun 14 00:39:34 2023, max compression
```

## Comparing `control_rod-2023.5.6.1.tar` & `control_rod-2023.6.13.0.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:50:37.086418 control_rod-2023.5.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-07 03:50:37.086418 control_rod-2023.5.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:50:37.082418 control_rod-2023.5.6.1/abobjs/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/auditable_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/auditable_entity_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/auditable_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/buisness_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/continuous_monitoring_monitor_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/continuous_monitoring_monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/continuous_monitoring_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/controlrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/controls_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/departments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/effectiveness_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/status_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/vendor_criticalities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/abobjs/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:50:37.082418 control_rod-2023.5.6.1/control_rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-07 03:50:37.000000 control_rod-2023.5.6.1/control_rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-07 03:50:37.000000 control_rod-2023.5.6.1/control_rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:50:37.000000 control_rod-2023.5.6.1/control_rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 03:50:37.000000 control_rod-2023.5.6.1/control_rod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-07 03:50:37.086418 control_rod-2023.5.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:50:37.086418 control_rod-2023.5.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_controlrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_controlsdatum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_effectivenessoption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_status_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_testsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_testtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-07 03:50:19.000000 control_rod-2023.5.6.1/tests/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:39:34.276726 control_rod-2023.6.13.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-14 00:39:34.276726 control_rod-2023.6.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:39:34.272726 control_rod-2023.6.13.0/abobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/auditable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/auditable_entity_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/auditable_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28364 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/buisness_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/continuous_monitoring_monitor_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/continuous_monitoring_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/continuous_monitoring_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/controls_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/departments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/effectiveness_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/fn_register_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/vendor_criticalities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/abobjs/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:39:34.272726 control_rod-2023.6.13.0/control_rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-14 00:39:34.000000 control_rod-2023.6.13.0/control_rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-14 00:39:34.000000 control_rod-2023.6.13.0/control_rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:39:34.000000 control_rod-2023.6.13.0/control_rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 00:39:34.000000 control_rod-2023.6.13.0/control_rod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 00:39:34.000000 control_rod-2023.6.13.0/control_rod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-14 00:39:34.276726 control_rod-2023.6.13.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:39:34.276726 control_rod-2023.6.13.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_controlsdatum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_effectivenessoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_testsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_testtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-14 00:39:13.000000 control_rod-2023.6.13.0/tests/test_workspace.py
```

### Comparing `control_rod-2023.5.6.1/abobjs/__init__.py` & `control_rod-2023.6.13.0/abobjs/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,29 +24,39 @@
 from .auditable_entity_regions import AB_Auditable_Entity_Regions
 from .auditable_entity_types import AB_Auditable_Entity_Types
 from .vendor_criticalities import AB_Vendor_Criticality
 
 from .buisness_units import AB_Business_Unit
 from .departments import AB_Departments
 
+from .custom_field import AB_Custom_Fields
+
+from .user import AB_User
+
 from .multi import AB_Multi
 
 SUBOBJ_LK = {"region_id": {"obj": AB_Region},
              "process_id": {"obj": AB_Process},
              "subprocess_id": {"obj": AB_SubProcess},
              "risk_id": {"obj": AB_Risk},
              "control_id": {"obj": AB_Control},
              "entity_id": {"obj": AB_Entity},
              "controls_datum_ids": {"obj": AB_Controls_Data},
              "test_ids": {"obj": AB_Test},
              "file_ids": {"obj": AB_File},
              "continuous_monitoring_system_id": {"obj": AB_Continous_Monitoring_Systems},
              "continuous_monitoring_monitor_id": {"obj": AB_Continous_Monitoring_Monitors},
+             "auditable_entity_type_id": {"obj": AB_Auditable_Entity_Types},
              "auditable_entity_id": {"obj": AB_Auditable_Entities},
+             "auditable_entity_reference_ids": {"obj": AB_Auditable_Entities}, # How AE's reference other AE's
              "auditable_entity_region_id": {"obj": AB_Auditable_Entity_Regions},
-             "vendor_criticalities_id": {"obj": AB_Vendor_Criticality}
+             "vendor_criticalities_id": {"obj": AB_Vendor_Criticality},
+             "department_ids": {"obj": AB_Departments},
+             "created_by_user_id": {"obj": AB_User},
+             "tprm_user_ids": {"obj": AB_User},
+             "owner_user_ids": {"obj": AB_User},
             }
 
-
+from .fn_register_cf import fn_register_custom_fields
 from .controlrod import AB_ControlRod
 
-USER_AGENT = "control_rod/0.0.0"
+USER_AGENT = "control_rod/2023.6.13.0"
```

### Comparing `control_rod-2023.5.6.1/abobjs/assertion.py` & `control_rod-2023.6.13.0/abobjs/assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/auditable_entity.py` & `control_rod-2023.6.13.0/abobjs/auditable_entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 class AB_Auditable_Entities(abobjs.AB_Base):
 
     _endpoint = "/api/v1/auditable_entities"
     _single = ".auditable_entities[0]"
     _name = "auditable_entity"
 
+    _get_params = {"include[]": "auditableEntityReferences"}
+
     def __init__(self, id=None, api_info=None, **kwargs):
 
         # Dunder Handling
         endpoint = kwargs.get("endpoint", self._endpoint)
         single = kwargs.get("single", self._single)
         name = kwargs.get("name", self._name)
```

### Comparing `control_rod-2023.5.6.1/abobjs/auditable_entity_regions.py` & `control_rod-2023.6.13.0/abobjs/auditable_entity_regions.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/auditable_entity_types.py` & `control_rod-2023.6.13.0/abobjs/auditable_entity_types.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/base.py` & `control_rod-2023.6.13.0/abobjs/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import pyjq
 import xmltodict
 
 import abobjs
 
 
 class AB_Base:
-
     '''
     Base Object for API Calls
     '''
 
     # People need to set these three
     _endpoint = None
     _single = None
@@ -43,14 +42,23 @@
 
     _strips = ["_permissions"]
 
     _upload_endpoint = "/api/v1/files/s3_upload_signature"
     _file_notify_endpoint = "/api/v1/files"
     _user_endpoint = "/api/v1/user_stats"
 
+    #
+    _post_upload_post_headers = {}
+    _upload_file_headers = {}
+    _get_params = {}
+    _create_params = {}
+    _search_params = {}
+
+    _stich_def = []
+
     def __init__(self, id=None, api_info=None, **kwargs):
 
         self.api_info = api_info
         self.id = id
         self.datum = kwargs.get("datum", dict())
 
         self.kwargs = kwargs
@@ -71,19 +79,26 @@
         self.read_args = self.kwargs.get("read_args", self._read_args)
         self.max_depth = self.kwargs.get("max_depth", self._max_depth)
         self.allow_full_update = self.kwargs.get("allow_full_update", self._allow_full_update)
         self.file_modal = self.kwargs.get("file_modal", self._file_modal)
         self.fileable_type = self.kwargs.get("fileable_type", self._fileable_type)
         self.user_endpoint = self.kwargs.get("user_endpoint", self._user_endpoint)
         self.file_notify_endpoint = self.kwargs.get("file_notify_endpoint", self._file_notify_endpoint)
+        self.stich_def = self.kwargs.get("stich_def", self._stich_def)
 
         self.headers = {"Authorization": self.api_info["ab_token"],
                         "User-Agent": self.kwargs.get("user_agent", abobjs.USER_AGENT),
                         **self.api_info.get("headers", {})}
 
+        # Custom Headers
+        self.custom_params = {"get_params": self.kwargs.get("get_params", self._get_params),
+                              "create_params": self.kwargs.get("create_params", self._create_params),
+                              "search_params": self.kwargs.get("search_params", self._search_params)
+                              }
+
         self.logger = logging.getLogger("AB:{}".format(self.name))
 
         self.my_user_id = self.user_id()
 
         ignore_read = False
         self.init_action_taken = "none"
 
@@ -97,15 +112,14 @@
                 # I searched for and found (or not) a result
                 try:
                     self.id = self.search()
                 except Exception as error_in_search:
                     self.logger.debug(error_in_search)
                     raise error_in_search
 
-
                 self.init_action_taken = "read"
 
                 self.logger.info("Found ID : {} on search.".format(self.id))
 
                 if self.kwargs.get("init_action", "read") == "readorcreate" and self.id is None:
                     # If I didn't find a result and it's requested, let's create based on the data.
                     self.id, self.datum = self.create()
@@ -186,15 +200,15 @@
         '''
 
         search_endpoint = urllib.parse.urljoin(self.api_info.get("base_domain", None),
                                                self.endpoint)
 
         try:
             data_request = requests.get(search_endpoint, headers=self.headers,
-                                        params=self.read_args)
+                                        params={**self.custom_params["search_params"], **self.read_args})
         except Exception as error:
             self.logger.error("Error when requesting update about Control: {}".format(self.id))
             self.logger.debug("Error Message: {}".format(error))
         else:
             if data_request.status_code != requests.codes.ok:
                 self.logger.error("Unable to Search {} for Data".format(self.name))
                 self.logger.debug(data_request.text)
@@ -348,33 +362,61 @@
 
         objectified = straight_data
 
         current_depth = self.kwargs.get("depth", 0)
 
         if self.kwargs.get("depth", 0) < self.max_depth:
             for key, desired_obj in abobjs.SUBOBJ_LK.items():
+                do_replace = False
+                subobj = None
+                compare_data = None
                 if key in straight_data.keys():
-                    if isinstance(straight_data[key], list):
+                    compare_data = straight_data[key]
+                    do_replace = True
+                    self.logger.debug("Found Key {} in Objectify Data.")
+                elif key in straight_data.get("field_data", {}).keys():
+                    compare_data = straight_data["field_data"][key]
+                    do_replace = True
+                    subobj = "field_data"
+                    self.logger.debug("Found Key {} in Objectify Data, field_data")
+
+
+                if do_replace:
+                    if isinstance(compare_data, list):
                         # Replace List of Items
                         replace_with = list()
-                        for x in straight_data[key]:
-                            replace_with.append(desired_obj["obj"](id=x, init_action="read",
-                                                                   api_info=self.api_info,
-                                                                   depth=current_depth + 1,
-                                                                   my_user_id=self.my_user_id))
-                    elif isinstance(straight_data[key], int):
+                        for x in compare_data:
+                            if "map" in desired_obj.keys():
+                                replace_with.append(desired_obj["map"].get(x, None))
+                            elif "obj" in desired_obj.keys():
+                                replace_with.append(desired_obj["obj"](id=x, init_action="read",
+                                                                       api_info=self.api_info,
+                                                                       depth=current_depth + 1,
+                                                                       my_user_id=self.my_user_id))
+                            else:
+                                replace_with.append(x)
+                    elif isinstance(compare_data, int):
                         # Replace Single Item
-                        replace_with = desired_obj["obj"](id=straight_data[key], init_action="read",
+                        if "map" in desired_obj.keys():
+                            replace_with = desired_obj["map"].get(compare_data, None)
+                        elif "obj" in desired_obj.keys():
+                            replace_with = desired_obj["obj"](id=straight_data[key], init_action="read",
                                                           api_info=self.api_info,
                                                           depth=current_depth + 1,
                                                           my_user_id=self.my_user_id)
+                        else:
+                            replace_with = compare_data
+                    else:
+                        replace_with = compare_data
+
+                    if subobj is None:
+                        objectified[key] = replace_with
                     else:
-                        replace_with = straight_data[key]
+                        objectified[subobj][key] = replace_with
 
-                    objectified[key] = replace_with
         else:
             self.logger.debug("Because of Depth {}, not Enumerating type : {}".format(current_depth, self.name))
 
         for key in self.date_keys:
             if key in objectified.keys():
                 if objectified[key] is not None:
                     objectified[key] = self.dateread(straight_data[key])
@@ -390,32 +432,58 @@
 
         control_endpoint = urllib.parse.urljoin(self.api_info.get("base_domain", None),
                                                 "{}/{}".format(self.endpoint, self.id))
 
         self.logger.debug(control_endpoint)
 
         try:
-            data_request = requests.get(control_endpoint, headers=self.headers,
-                                        params=self.read_args)
+            data_request = requests.get(control_endpoint,
+                                        headers=self.headers,
+                                        params={**self.custom_params["get_params"], **self.read_args})
         except Exception as error:
             self.logger.error("Error when requesting data about Control: {}".format(self.id))
             raise error
         else:
             self.logger.debug(data_request.status_code)
             if data_request.status_code != requests.codes.ok:
                 self.logger.error("Unable to Get Data for {} {}".format(self.name, self.id))
-                self.logger.info("Error: {}".format(data_request.json()))
+                self.logger.info("Error: {}".format(data_request.text))
                 raise ValueError()
             else:
+                f_req_data = data_request.json()
                 self.logger.debug("Verbose Data {}".format(data_request.json()))
                 self.kwargs["full_single"] = data_request.json()
                 control_data = pyjq.first(self.single, data_request.json())
 
+                for stich_cfg in self.stich_def:
+                    source = stich_cfg["source"]
+                    idfield = stich_cfg["idfield"]
+                    val = stich_cfg["val"]
+                    isjqval = stich_cfg.get("isjqval", False)
+
+                    map = dict()
+
+                    if isinstance(f_req_data, dict):
+                        if source in f_req_data.keys() and isinstance(f_req_data[source], (list,tuple)):
+                            for x in f_req_data[source]:
+                                self.logger.debug(x)
+                                if isjqval is True:
+                                    map[x[idfield]] = pyjq.one(val, x)
+                                elif isinstance(x, dict):
+                                    map[x[idfield]] = x.get(val, None)
+                                else:
+                                    map[x[idfield]] = None
+
+                    control_data["{}_map".format(source)] = map
+
                 obj_cont_data = self.objectify_datum(control_data)
 
+                # Add Stiches Here
+                self.logger.debug(data_request.json())
+
         return self.id, obj_cont_data
 
     def dateread(self, datestring):
 
         """
         Reads AB Datestring with miliseconds and converts it to datetime object
```

### Comparing `control_rod-2023.5.6.1/abobjs/buisness_units.py` & `control_rod-2023.6.13.0/abobjs/buisness_units.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/continuous_monitoring_monitor_results.py` & `control_rod-2023.6.13.0/abobjs/continuous_monitoring_monitor_results.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/continuous_monitoring_monitors.py` & `control_rod-2023.6.13.0/abobjs/continuous_monitoring_monitors.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/continuous_monitoring_systems.py` & `control_rod-2023.6.13.0/abobjs/continuous_monitoring_systems.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/control.py` & `control_rod-2023.6.13.0/abobjs/control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/controlrod.py` & `control_rod-2023.6.13.0/abobjs/controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/controls_data.py` & `control_rod-2023.6.13.0/abobjs/controls_data.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/departments.py` & `control_rod-2023.6.13.0/abobjs/departments.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/effectiveness_option.py` & `control_rod-2023.6.13.0/abobjs/effectiveness_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/entity.py` & `control_rod-2023.6.13.0/abobjs/entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/file.py` & `control_rod-2023.6.13.0/abobjs/file.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/multi.py` & `control_rod-2023.6.13.0/abobjs/multi.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/process.py` & `control_rod-2023.6.13.0/abobjs/process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/region.py` & `control_rod-2023.6.13.0/abobjs/region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/risk.py` & `control_rod-2023.6.13.0/abobjs/risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/status_option.py` & `control_rod-2023.6.13.0/abobjs/status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/subprocess.py` & `control_rod-2023.6.13.0/abobjs/subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/test.py` & `control_rod-2023.6.13.0/abobjs/test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/test_section.py` & `control_rod-2023.6.13.0/abobjs/test_section.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/test_type.py` & `control_rod-2023.6.13.0/abobjs/test_type.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/vendor_criticalities.py` & `control_rod-2023.6.13.0/abobjs/vendor_criticalities.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/abobjs/workspace.py` & `control_rod-2023.6.13.0/abobjs/workspace.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/control_rod.egg-info/SOURCES.txt` & `control_rod-2023.6.13.0/control_rod.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,32 +10,36 @@
 abobjs/buisness_units.py
 abobjs/continuous_monitoring_monitor_results.py
 abobjs/continuous_monitoring_monitors.py
 abobjs/continuous_monitoring_systems.py
 abobjs/control.py
 abobjs/controlrod.py
 abobjs/controls_data.py
+abobjs/custom_field.py
 abobjs/departments.py
 abobjs/effectiveness_option.py
 abobjs/entity.py
 abobjs/file.py
+abobjs/fn_register_cf.py
 abobjs/multi.py
 abobjs/process.py
 abobjs/region.py
 abobjs/risk.py
 abobjs/status_option.py
 abobjs/subprocess.py
 abobjs/test.py
 abobjs/test_section.py
 abobjs/test_type.py
+abobjs/user.py
 abobjs/vendor_criticalities.py
 abobjs/workspace.py
 control_rod.egg-info/PKG-INFO
 control_rod.egg-info/SOURCES.txt
 control_rod.egg-info/dependency_links.txt
+control_rod.egg-info/requires.txt
 control_rod.egg-info/top_level.txt
 tests/test_assertion.py
 tests/test_control.py
 tests/test_controlrod.py
 tests/test_controlsdatum.py
 tests/test_effectivenessoption.py
 tests/test_entity.py
```

### Comparing `control_rod-2023.5.6.1/tests/test_assertion.py` & `control_rod-2023.6.13.0/tests/test_assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_control.py` & `control_rod-2023.6.13.0/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_controlrod.py` & `control_rod-2023.6.13.0/tests/test_controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_controlsdatum.py` & `control_rod-2023.6.13.0/tests/test_controlsdatum.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_effectivenessoption.py` & `control_rod-2023.6.13.0/tests/test_effectivenessoption.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_entity.py` & `control_rod-2023.6.13.0/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_files.py` & `control_rod-2023.6.13.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_process.py` & `control_rod-2023.6.13.0/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_region.py` & `control_rod-2023.6.13.0/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_risk.py` & `control_rod-2023.6.13.0/tests/test_risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_status_option.py` & `control_rod-2023.6.13.0/tests/test_status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_subprocess.py` & `control_rod-2023.6.13.0/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_test.py` & `control_rod-2023.6.13.0/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_testsection.py` & `control_rod-2023.6.13.0/tests/test_testsection.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_testtypes.py` & `control_rod-2023.6.13.0/tests/test_testtypes.py`

 * *Files identical despite different names*

### Comparing `control_rod-2023.5.6.1/tests/test_workspace.py` & `control_rod-2023.6.13.0/tests/test_workspace.py`

 * *Files identical despite different names*

