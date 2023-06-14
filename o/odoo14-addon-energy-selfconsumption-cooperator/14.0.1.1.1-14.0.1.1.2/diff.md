# Comparing `tmp/odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1.tar.gz` & `tmp/odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1.tar", last modified: Wed Jun 14 09:53:27 2023, max compression
+gzip compressed data, was "odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2.tar", last modified: Wed Jun 14 10:57:28 2023, max compression
```

## Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1.tar` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      463 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/PKG-INFO
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.275430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.275430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       21 2023-05-16 12:14:37.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      611 2023-06-14 09:47:53.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/__manifest__.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2152 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/ca_ES.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1957 2023-05-16 16:06:50.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/energy_selfconsumption_cooperator.pot
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2159 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/es.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2160 2023-05-16 16:06:50.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/eu_ES.po
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/models/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       27 2023-05-23 12:34:38.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/models/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      402 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/models/supply_point.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.275430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/static/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/static/description/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3721 2023-05-16 12:14:37.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/static/description/icon.png
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/views/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1473 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/views/res_partner_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      826 2023-05-30 07:52:25.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/views/supply_point_views.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo14_addon_energy_selfconsumption_cooperator.egg-info/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      463 2023-06-14 09:53:27.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo14_addon_energy_selfconsumption_cooperator.egg-info/PKG-INFO
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1169 2023-06-14 09:53:27.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo14_addon_energy_selfconsumption_cooperator.egg-info/SOURCES.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 09:53:27.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo14_addon_energy_selfconsumption_cooperator.egg-info/dependency_links.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 09:53:27.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo14_addon_energy_selfconsumption_cooperator.egg-info/not-zip-safe
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       86 2023-06-14 09:53:27.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo14_addon_energy_selfconsumption_cooperator.egg-info/requires.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        5 2023-06-14 09:53:27.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo14_addon_energy_selfconsumption_cooperator.egg-info/top_level.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       38 2023-06-14 09:53:27.279430 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/setup.cfg
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      224 2023-06-14 09:46:49.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/setup.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.368710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      463 2023-06-14 10:57:28.368710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/PKG-INFO
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.364710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.364710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.364710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       21 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      611 2023-06-14 10:56:30.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/__manifest__.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.368710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2152 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/ca_ES.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1957 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/energy_selfconsumption_cooperator.pot
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2159 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/es.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2160 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/eu_ES.po
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.368710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/models/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       27 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/models/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      402 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/models/supply_point.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.364710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/static/
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.368710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/static/description/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3721 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/static/description/icon.png
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.368710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/views/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1473 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/views/res_partner_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      826 2023-06-14 10:42:12.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/views/supply_point_views.xml
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-06-14 10:57:28.368710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo14_addon_energy_selfconsumption_cooperator.egg-info/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      463 2023-06-14 10:57:28.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo14_addon_energy_selfconsumption_cooperator.egg-info/PKG-INFO
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1169 2023-06-14 10:57:28.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo14_addon_energy_selfconsumption_cooperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 10:57:28.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo14_addon_energy_selfconsumption_cooperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-06-14 10:57:28.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo14_addon_energy_selfconsumption_cooperator.egg-info/not-zip-safe
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       93 2023-06-14 10:57:28.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo14_addon_energy_selfconsumption_cooperator.egg-info/requires.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        5 2023-06-14 10:57:28.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo14_addon_energy_selfconsumption_cooperator.egg-info/top_level.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       38 2023-06-14 10:57:28.368710 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/setup.cfg
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      231 2023-06-14 10:50:25.000000 odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/setup.py
```

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/__manifest__.py` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         """,
     "description": """
             Module glue between Energy Self-consumption and Cooperator
     """,
     "author": "Coopdevs Treball SCCL & Som Energia SCCL",
     "website": "https://somcomunitats.coop/",
     "category": "Customizations",
-    "version": "14.0.1.1.1",
+    "version": "14.0.1.1.2",
     "depends": [
         "energy_selfconsumption",
         "cooperator",
     ],
     "data": [
         "views/supply_point_views.xml",
         "views/res_partner_views.xml",
```

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/ca_ES.po` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/ca_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/energy_selfconsumption_cooperator.pot` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/energy_selfconsumption_cooperator.pot`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/es.po` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/es.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/i18n/eu_ES.po` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/i18n/eu_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/static/description/icon.png` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/static/description/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/views/res_partner_views.xml` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/views/res_partner_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo/addons/energy_selfconsumption_cooperator/views/supply_point_views.xml` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo/addons/energy_selfconsumption_cooperator/views/supply_point_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.1/odoo14_addon_energy_selfconsumption_cooperator.egg-info/SOURCES.txt` & `odoo14-addon-energy_selfconsumption_cooperator-14.0.1.1.2/odoo14_addon_energy_selfconsumption_cooperator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

