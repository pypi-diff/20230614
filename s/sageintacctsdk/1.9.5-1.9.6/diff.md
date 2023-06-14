# Comparing `tmp/sageintacctsdk-1.9.5.tar.gz` & `tmp/sageintacctsdk-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageintacctsdk-1.9.5.tar", last modified: Fri Mar 11 06:57:28 2022, max compression
+gzip compressed data, was "sageintacctsdk-1.9.6.tar", last modified: Thu Apr  7 06:55:01 2022, max compression
```

## Comparing `sageintacctsdk-1.9.5.tar` & `sageintacctsdk-1.9.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 06:57:28.857851 sageintacctsdk-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-03-11 06:57:28.857851 sageintacctsdk-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4310 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 06:57:28.853851 sageintacctsdk-1.9.5/sageintacctsdk/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 06:57:28.857851 sageintacctsdk-1.9.5/sageintacctsdk/apis/
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/ap_payments.py
--rw-r--r--   0 runner    (1001) docker     (121)    16862 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/ar_invoices.py
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/attachments.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/bills.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/charge_card_accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/charge_card_transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/checking_accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    12477 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/contacts.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/customers.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/departments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/employees.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/expense_payment_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/expense_reports.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/expense_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/gl_detail.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/items.py
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/journal_entries.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/location_entities.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/locations.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/reimbursements.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/savings_accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/tax_details.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/apis/vendors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8778 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/sageintacctsdk/sageintacctsdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-11 06:57:28.853851 sageintacctsdk-1.9.5/sageintacctsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-03-11 06:57:28.000000 sageintacctsdk-1.9.5/sageintacctsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-03-11 06:57:28.000000 sageintacctsdk-1.9.5/sageintacctsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-11 06:57:28.000000 sageintacctsdk-1.9.5/sageintacctsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-03-11 06:57:28.000000 sageintacctsdk-1.9.5/sageintacctsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-11 06:57:28.000000 sageintacctsdk-1.9.5/sageintacctsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-11 06:57:28.857851 sageintacctsdk-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-03-11 06:57:17.000000 sageintacctsdk-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 06:55:01.942792 sageintacctsdk-1.9.6/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-04-07 06:55:01.942792 sageintacctsdk-1.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4310 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 06:55:01.938792 sageintacctsdk-1.9.6/sageintacctsdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 06:55:01.942792 sageintacctsdk-1.9.6/sageintacctsdk/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/ap_payments.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16878 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/ar_invoices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/bills.py
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/charge_card_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/charge_card_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/checking_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12477 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/customers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/departments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/employees.py
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/expense_payment_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      839 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/expense_reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/expense_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/gl_detail.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/items.py
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/journal_entries.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/location_entities.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/locations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/reimbursements.py
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/savings_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/tax_details.py
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/apis/vendors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8778 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/sageintacctsdk/sageintacctsdk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 06:55:01.938792 sageintacctsdk-1.9.6/sageintacctsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-04-07 06:55:01.000000 sageintacctsdk-1.9.6/sageintacctsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-04-07 06:55:01.000000 sageintacctsdk-1.9.6/sageintacctsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-07 06:55:01.000000 sageintacctsdk-1.9.6/sageintacctsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-04-07 06:55:01.000000 sageintacctsdk-1.9.6/sageintacctsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-07 06:55:01.000000 sageintacctsdk-1.9.6/sageintacctsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-07 06:55:01.942792 sageintacctsdk-1.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-04-07 06:54:54.000000 sageintacctsdk-1.9.6/setup.py
```

### Comparing `sageintacctsdk-1.9.5/LICENSE` & `sageintacctsdk-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/PKG-INFO` & `sageintacctsdk-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageintacctsdk
-Version: 1.9.5
+Version: 1.9.6
 Summary: Python SDK for accessing Sage Intacct APIs
 Home-page: https://github.com/fylein/sageintacct-sdk-py
 Author: Ashwin T
 Author-email: ashwin.t@fyle.in
 License: MIT
 Keywords: sage-intacct,sage,fyle,api,python,sdk
 Platform: UNKNOWN
```

### Comparing `sageintacctsdk-1.9.5/README.md` & `sageintacctsdk-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/__init__.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/ap_payments.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/ap_payments.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/api_base.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/api_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         """
 
         api_headers = {
             'content-type': 'application/xml'
         }
         body = xmltodict.unparse(dict_body)
 
-        response = requests.post(api_url, headers=api_headers, data=body)
+        response = requests.post(api_url, headers=api_headers, data=body.encode('utf-8'))
 
         parsed_xml = xmltodict.parse(response.text, force_list={self.__dimension})
         parsed_response = json.loads(json.dumps(parsed_xml))
 
         if response.status_code == 200:
             if parsed_response['response']['control']['status'] == 'success':
                 api_response = parsed_response['response']['operation']
```

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/attachments.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/attachments.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/bills.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/bills.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/charge_card_transactions.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/charge_card_transactions.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/constants.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/constants.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/dimension_values.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/dimension_values.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/expense_reports.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/expense_reports.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/reimbursements.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/reimbursements.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/apis/savings_accounts.py` & `sageintacctsdk-1.9.6/sageintacctsdk/apis/savings_accounts.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/exceptions.py` & `sageintacctsdk-1.9.6/sageintacctsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk/sageintacctsdk.py` & `sageintacctsdk-1.9.6/sageintacctsdk/sageintacctsdk.py`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk.egg-info/PKG-INFO` & `sageintacctsdk-1.9.6/sageintacctsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageintacctsdk
-Version: 1.9.5
+Version: 1.9.6
 Summary: Python SDK for accessing Sage Intacct APIs
 Home-page: https://github.com/fylein/sageintacct-sdk-py
 Author: Ashwin T
 Author-email: ashwin.t@fyle.in
 License: MIT
 Keywords: sage-intacct,sage,fyle,api,python,sdk
 Platform: UNKNOWN
```

### Comparing `sageintacctsdk-1.9.5/sageintacctsdk.egg-info/SOURCES.txt` & `sageintacctsdk-1.9.6/sageintacctsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sageintacctsdk-1.9.5/setup.py` & `sageintacctsdk-1.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='sageintacctsdk',
-    version='1.9.5',
+    version='1.9.6',
     author='Ashwin T',
     author_email='ashwin.t@fyle.in',
     description='Python SDK for accessing Sage Intacct APIs',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['sage-intacct', 'sage', 'fyle', 'api', 'python', 'sdk'],
```

