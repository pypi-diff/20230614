# Comparing `tmp/odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2.tar.gz` & `tmp/odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2.tar", last modified: Wed Jun  7 18:49:42 2023, max compression
+gzip compressed data, was "odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3.tar", last modified: Tue Jun 13 22:12:38 2023, max compression
```

## Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2.tar` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-07 18:49:42.487867 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      607 2023-06-07 18:49:42.487867 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/PKG-INFO
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-07 18:49:42.484534 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-07 18:49:42.484534 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-07 18:49:42.484534 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       21 2023-05-22 18:09:17.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      871 2023-06-07 18:49:15.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/__manifest__.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-07 18:49:42.487867 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/models/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-05-22 18:09:56.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/models/__init__.py
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)     2891 2023-06-07 18:48:42.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/models/hr_attendance_mitxelena.py
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-07 18:49:42.487867 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/security/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      177 2023-05-22 18:13:22.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/security/ir.model.access.csv
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-07 18:49:42.487867 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/views/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      622 2023-05-22 18:40:13.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/views/hr_attendance_views.xml
-drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-07 18:49:42.487867 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      607 2023-06-07 18:49:42.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/PKG-INFO
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      722 2023-06-07 18:49:42.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/SOURCES.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-06-07 18:49:42.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/dependency_links.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-05-22 19:54:48.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/not-zip-safe
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       53 2023-06-07 18:49:42.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/requires.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-06-07 18:49:42.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/top_level.txt
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-06-07 18:49:42.487867 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/setup.cfg
--rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-05-22 19:53:12.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/setup.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      607 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/PKG-INFO
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       21 2023-05-22 18:09:17.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      871 2023-06-13 22:12:14.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/__manifest__.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/models/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-05-22 18:09:56.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/models/__init__.py
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)     4481 2023-06-13 22:10:17.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/models/hr_attendance_mitxelena.py
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/security/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      177 2023-05-22 18:13:22.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/security/ir.model.access.csv
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/views/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      622 2023-05-22 18:40:13.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/views/hr_attendance_views.xml
+drwxr-xr-x   0 pelayo    (1000) pelayo    (1000)        0 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      607 2023-06-13 22:12:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/PKG-INFO
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      722 2023-06-13 22:12:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/SOURCES.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-06-13 22:12:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/dependency_links.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        1 2023-05-22 19:54:48.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/not-zip-safe
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       53 2023-06-13 22:12:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/requires.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)        5 2023-06-13 22:12:38.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/top_level.txt
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)       38 2023-06-13 22:12:38.823335 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/setup.cfg
+-rw-r--r--   0 pelayo    (1000) pelayo    (1000)      100 2023-06-13 21:48:11.000000 odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/setup.py
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/PKG-INFO` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-hr_attendance_mitxelena
-Version: 14.0.1.0.2
+Version: 14.0.1.0.3
 Summary: Employee Attendances Customizations for Mitxelena
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Requires-Python: >=3.6
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/__manifest__.py` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'HR Attendance Mitxelena',
-    'version': '14.0.1.0.2',
+    'version': '14.0.1.0.3',
     'category': 'Human Resources',
     'sequence': 20,
     'summary': 'Employee Attendances Customizations for Mitxelena',
     'description': """
 Customizations of Employee Attendances for Mitxelena
 ====================================================
 This module includes customizations for handling employee attendances at Mitxelena,
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo/addons/hr_attendance_mitxelena/views/hr_attendance_views.xml` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo/addons/hr_attendance_mitxelena/views/hr_attendance_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/PKG-INFO` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-hr-attendance-mitxelena
-Version: 14.0.1.0.2
+Version: 14.0.1.0.3
 Summary: Employee Attendances Customizations for Mitxelena
 Home-page: https://www.coopdevs.org
 Author: Coopdevs
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Requires-Python: >=3.6
```

### Comparing `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.2/odoo14_addon_hr_attendance_mitxelena.egg-info/SOURCES.txt` & `odoo14-addon-hr_attendance_mitxelena-14.0.1.0.3/odoo14_addon_hr_attendance_mitxelena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

