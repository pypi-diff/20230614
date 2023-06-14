# Comparing `tmp/fyle-integrations-platform-connector-1.8.0.tar.gz` & `tmp/fyle-integrations-platform-connector-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyle-integrations-platform-connector-1.8.0.tar", last modified: Wed Mar 23 08:12:34 2022, max compression
+gzip compressed data, was "fyle-integrations-platform-connector-1.9.0.tar", last modified: Thu Mar 24 10:10:06 2022, max compression
```

## Comparing `fyle-integrations-platform-connector-1.8.0.tar` & `fyle-integrations-platform-connector-1.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:34.447372 fyle-integrations-platform-connector-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-03-23 08:12:34.443372 fyle-integrations-platform-connector-1.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:34.443372 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:34.443372 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/corporate_cards.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/cost_centers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/employees.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/expense_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     6914 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/expenses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/merchants.py
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/reimbursements.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/tax_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/fyle_integrations_platform_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:34.443372 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-03-23 08:12:34.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-03-23 08:12:34.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 08:12:34.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-03-23 08:12:34.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-03-23 08:12:34.000000 fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:34.443372 fyle-integrations-platform-connector-1.8.0/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 08:12:34.447372 fyle-integrations-platform-connector-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-03-23 08:12:21.000000 fyle-integrations-platform-connector-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:10:06.199545 fyle-integrations-platform-connector-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-03-24 10:10:06.199545 fyle-integrations-platform-connector-1.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:10:06.199545 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:10:06.199545 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3366 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/corporate_cards.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/cost_centers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/employees.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/expense_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6914 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/expenses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/merchants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/reimbursements.py
+-rw-r--r--   0 runner    (1001) docker     (121)      934 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/tax_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/fyle_integrations_platform_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:10:06.199545 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-03-24 10:10:06.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-03-24 10:10:06.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 10:10:06.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-03-24 10:10:06.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-03-24 10:10:06.000000 fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:10:06.199545 fyle-integrations-platform-connector-1.9.0/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-24 10:10:06.199545 fyle-integrations-platform-connector-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-03-24 10:09:53.000000 fyle-integrations-platform-connector-1.9.0/setup.py
```

### Comparing `fyle-integrations-platform-connector-1.8.0/PKG-INFO` & `fyle-integrations-platform-connector-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyle-integrations-platform-connector
-Version: 1.8.0
+Version: 1.9.0
 Summary: A common platform connector for all the Fyle Integrations to interact with Fyle Platform APIs
 Home-page: https://github.com/fylein/fyle-integrations-platform-connector
 Author: Shwetabh Kumar
 Author-email: shwetabh.kumar@fyle.in
 License: MIT
 Keywords: fyle,api,python,integration,platform,connector
 Platform: UNKNOWN
```

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/__init__.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/base.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/base.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/categories.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/categories.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/corporate_cards.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/corporate_cards.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/employees.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/employees.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/expense_custom_fields.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/expense_custom_fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,13 +22,14 @@
                 for option in row['options']:
                     attributes.append({
                         'attribute_type': attribute_type,
                         'display_name': row['field_name'],
                         'value': option,
                         'source_id': 'expense_custom_field.{}.{}'.format(row['field_name'].lower(), count),
                         'detail': {
-                            'custom_field_id': row['id']
+                            'custom_field_id': row['id'],
+                            'placeholder': row['placeholder']
                         }
                     })
                     count = count + 1
                 self.attribute_type = attribute_type
                 self.bulk_create_or_update_expense_attributes(attributes, True)
```

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/expenses.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/expenses.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/merchants.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/merchants.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/projects.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/projects.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/reimbursements.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/reimbursements.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/apis/tax_groups.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/apis/tax_groups.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector/fyle_integrations_platform_connector.py` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector/fyle_integrations_platform_connector.py`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector.egg-info/PKG-INFO` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyle-integrations-platform-connector
-Version: 1.8.0
+Version: 1.9.0
 Summary: A common platform connector for all the Fyle Integrations to interact with Fyle Platform APIs
 Home-page: https://github.com/fylein/fyle-integrations-platform-connector
 Author: Shwetabh Kumar
 Author-email: shwetabh.kumar@fyle.in
 License: MIT
 Keywords: fyle,api,python,integration,platform,connector
 Platform: UNKNOWN
```

### Comparing `fyle-integrations-platform-connector-1.8.0/fyle_integrations_platform_connector.egg-info/SOURCES.txt` & `fyle-integrations-platform-connector-1.9.0/fyle_integrations_platform_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fyle-integrations-platform-connector-1.8.0/setup.py` & `fyle-integrations-platform-connector-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('../README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='fyle-integrations-platform-connector',
-    version='1.8.0',
+    version='1.9.0',
     author='Shwetabh Kumar',
     author_email='shwetabh.kumar@fyle.in',
     description='A common platform connector for all the Fyle Integrations to interact with Fyle Platform APIs',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['fyle', 'api', 'python', 'integration', 'platform', 'connector'],
```

