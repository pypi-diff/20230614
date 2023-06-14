# Comparing `tmp/ms_salesforce_api-1.0.0.tar.gz` & `tmp/ms_salesforce_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-1.0.0.tar", max compression
+gzip compressed data, was "ms_salesforce_api-1.0.1.tar", max compression
```

## Comparing `ms_salesforce_api-1.0.0.tar` & `ms_salesforce_api-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/LICENSE
--rw-r--r--   0        0        0     5631 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0      982 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2712 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2395 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3347 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15406 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     7675 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    19543 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    20551 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0     8894 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    17755 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13717 2023-06-12 12:27:36.529168 ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0     1055 2023-06-12 12:27:36.533168 ms_salesforce_api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 ms_salesforce_api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5631 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2713 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2395 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3347 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15402 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     7675 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    20445 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    22589 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0     8894 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    17755 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13717 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/helpers.py
+-rw-r--r--   0        0        0     1055 2023-06-14 12:14:01.853654 ms_salesforce_api-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 ms_salesforce_api-1.0.1/PKG-INFO
```

### Comparing `ms_salesforce_api-1.0.0/LICENSE` & `ms_salesforce_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/README.md` & `ms_salesforce_api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             logging.error("Authentication failed, cannot fetch data")
             return None
 
         headers = {"Authorization": f"Bearer {self.access_token}"}
 
         all_records = []
         next_url = f"{self.endpoint}?q={query}"
+
         while next_url:
             response = self._make_request(next_url, headers, 0)
             if response:
                 data = response.json()
                 all_records.extend(data.get("records", []))
                 nextRecordsUrl = data.get("nextRecordsUrl", None)
                 if nextRecordsUrl:
```

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
             "jhon.doe@ext.makingscience.com",
         )
         self.assertIsNone(opportunity["profit_center"])
         self.assertIsNone(opportunity["cost_center"])
         self.assertEqual(opportunity["project_tier"], "Unkown")
         self.assertEqual(
             opportunity["jira_task_url"],
-            '<a href="https://makingscience.atlassian.net/browse/ESMSBD0001-11848" target="_blank">View Jira Task</a>',  # noqa: E501
+            "<a href=https://makingscience.atlassian.net/browse/ESMSBD0001-11848 target=_blank>View Jira Task</a>",  # noqa: E501
         )
         self.assertEqual(opportunity["opportunity_percentage"], 10.0)
         self.assertEqual(len(opportunity["billing_lines"]), 1)
         billing_line = opportunity["billing_lines"][0]
 
         self.assertEqual(billing_line["id"], "a0sAa0000004Lx7IAE")
         self.assertEqual(billing_line["name"], "BL-000320965")
```

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     billing_postal_code  VARCHAR(255) DEFAULT NULL,
     billing_street  VARCHAR(255) DEFAULT NULL,
     company_invoicing  VARCHAR(255) DEFAULT NULL,
     office  VARCHAR(255) DEFAULT NULL,
     payment_terms  VARCHAR(255) DEFAULT NULL,
     billing_state_code  VARCHAR(255) DEFAULT NULL,
     mail_invoicing  VARCHAR(255) DEFAULT NULL,
-    invoicing_email  VARCHAR(255) DEFAULT NULL,
+    invoicing_email  VARCHAR(500) DEFAULT NULL,
     FOREIGN KEY (project_id) REFERENCES Opportunities(project_id)
 );
 """
 
 DEFAULT_POSTGRES_DATABASE_SCHEMAS_MAP = {
     "Opportunities": DEFAULT_OPPORTUNITIES_CREATE_TABLE_QUERY,
     "ProjectLine": DEFAULT_PROJECTLINE_CREATE_TABLE_QUERY,
```

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ms_salesforce_api.salesforce.project.dto.ProjectLineItemDTO import (  # noqa: E501
     ProjectLineItemDTO,
 )
+from ms_salesforce_api.salesforce.project.helpers import normalize_value
 
 
 class OpportunityDTO(object):
     def __init__(
         self,
         account_business_name,
         account_name,
@@ -108,31 +109,25 @@
         self.account_payment_terms = account_payment_terms
         self.account_billing_state_code = account_billing_state_code
         self.account_mail_invoicing = account_mail_invoicing
         self.account_invoicing_email = account_invoicing_email
 
     @staticmethod
     def from_salesforce_record(record):
-        def _normalize_str(text):
-            try:
-                return (
-                    text.replace("\n", "").replace("\r", "").replace("'", "")
-                )
-            except AttributeError:
-                return text
-
         def _get_account_business_name():
             try:
-                return record["Project_Account__r"]["Business_Name__c"]
+                return normalize_value(
+                    record["Project_Account__r"]["Business_Name__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_name():
             try:
-                return record["Project_Account__r"]["Name"]
+                return normalize_value(record["Project_Account__r"]["Name"])
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_id():
             try:
                 return record["Project_Account__r"]["Id"]
             except (TypeError, KeyError):
@@ -142,45 +137,53 @@
             try:
                 return record["Project_Account__r"]["BillingCountryCode"]
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_assigment_group():
             try:
-                return record["Project_Account__r"][
-                    "MS_Customer_Account_Assigment_Group__c"
-                ]
+                return normalize_value(
+                    record["Project_Account__r"][
+                        "MS_Customer_Account_Assigment_Group__c"
+                    ]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_tax_category():
             try:
-                return record["Project_Account__r"][
-                    "MS_Customer_Tax_Category__c"
-                ]
+                return normalize_value(
+                    record["Project_Account__r"]["MS_Customer_Tax_Category__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_tax_classification():
             try:
-                return record["Project_Account__r"][
-                    "MS_Customer_Tax_Classification__c"
-                ]
+                return normalize_value(
+                    record["Project_Account__r"][
+                        "MS_Customer_Tax_Classification__c"
+                    ]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_sap_id():
             try:
-                return record["Project_Account__r"]["TXT_SAPId__c"]
+                return normalize_value(
+                    record["Project_Account__r"]["TXT_SAPId__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_business_function():
             try:
-                return record["Project_Account__r"]["ms_Business_Function__c"]
+                return normalize_value(
+                    record["Project_Account__r"]["ms_Business_Function__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_tax_id_type():
             try:
                 return record["Project_Account__r"]["ms_TAX_id_Type__c"]
             except (TypeError, KeyError):
@@ -196,45 +199,47 @@
             try:
                 return record["Project_Account__r"]["CreatedDate"]
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_tier():
             try:
-                return record["Project_Account__r"]["Tier__c"]
+                return normalize_value(record["Project_Account__r"]["Tier__c"])
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_pec_email():
             try:
-                return record["Project_Account__r"]["PEC_Email__c"]
+                return normalize_value(
+                    record["Project_Account__r"]["PEC_Email__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_phone():
             try:
-                return record["Project_Account__r"]["Phone"]
+                return normalize_value(record["Project_Account__r"]["Phone"])
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_fax():
             try:
-                return record["Project_Account__r"]["Fax"]
+                return normalize_value(record["Project_Account__r"]["Fax"])
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_website():
             try:
-                return record["Project_Account__r"]["Website"]
+                return normalize_value(record["Project_Account__r"]["Website"])
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_cif():
             try:
-                return record["Project_Account__r"]["CIF__c"]
+                return normalize_value(record["Project_Account__r"]["CIF__c"])
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_billing_address():
             def build_address(location_dict):
                 """
                 Construct a string representation of an address from a
@@ -254,15 +259,15 @@
                     "country",
                 ]:
                     if field in location_dict and location_dict.get(field, ""):
                         address_components.append(location_dict[field])
 
                 address = ", ".join(address_components)
 
-                return _normalize_str(address)
+                return normalize_value(address)
 
             try:
                 return build_address(
                     record["Project_Account__r"]["BillingAddress"]
                 )
             except (TypeError, KeyError):
                 return ""
@@ -277,117 +282,137 @@
             try:
                 return record["Project_Account__r"]["BillingPostalCode"]
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_billing_street():
             try:
-                return _normalize_str(
+                return normalize_value(
                     record["Project_Account__r"]["BillingStreet"]
                 )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_company_invoicing():
             try:
-                return record["Project_Account__r"]["MS_Company_Invoicing__c"]
+                return normalize_value(
+                    record["Project_Account__r"]["MS_Company_Invoicing__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_office():
             try:
-                return record["Project_Account__r"]["MS_Office__c"]
+                return normalize_value(
+                    record["Project_Account__r"]["MS_Office__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_payment_terms():
             try:
-                return record["Project_Account__r"]["Payment_Terms__c"]
+                return normalize_value(
+                    record["Project_Account__r"]["Payment_Terms__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_billing_state_code():
             try:
                 return record["Project_Account__r"]["BillingStateCode"]
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_mail_invoicing():
             try:
-                return record["Project_Account__r"]["MAIL_Invoicing__c"]
+                return normalize_value(
+                    record["Project_Account__r"]["MAIL_Invoicing__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_account_invoicing_email():
             try:
                 email = record["Project_Account__r"]["Invoicing_Email__c"]
                 if email:
-                    return email.replace("\n", ",").replace("\r", "")
+                    return normalize_value(email)
             except (TypeError, KeyError):
                 return ""
 
         def _get_operation_coordinator_email():
             try:
-                return record["Operation_Coordinator__r"]["Name"]
+                return normalize_value(
+                    record["Operation_Coordinator__r"]["Name"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_operation_coordinator_sub_email():
             try:
-                return record["Operation_Coordinator_Sub__r"]["Name"]
+                return normalize_value(
+                    record["Operation_Coordinator_Sub__r"]["Name"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_opportunity_name():
             try:
-                return record["Opportunity__r"]["Opportunity_Name_Short__c"]
+                return normalize_value(
+                    record["Opportunity__r"]["Opportunity_Name_Short__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_stage():
             try:
-                return record["Opportunity__r"]["StageName"]
+                return normalize_value(record["Opportunity__r"]["StageName"])
             except (TypeError, KeyError):
                 return ""
 
         def _get_lead_source():
             try:
-                return record["Opportunity__r"]["LeadSource"]
+                return normalize_value(record["Opportunity__r"]["LeadSource"])
             except (TypeError, KeyError):
                 return ""
 
         def _get_controller_email():
             try:
-                return record["Operation_Coordinator__r"]["Controller__c"]
+                return normalize_value(
+                    record["Operation_Coordinator__r"]["Controller__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_controller_sub_email():
             try:
-                return record["Operation_Coordinator_Sub__r"][
-                    "Controller_SUB__c"
-                ]
+                return normalize_value(
+                    record["Operation_Coordinator_Sub__r"]["Controller_SUB__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_project_tier():
             try:
-                return record["Opportunity__r"]["Tier_Short__c"]
+                return normalize_value(
+                    record["Opportunity__r"]["Tier_Short__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_jira_task_url():
             try:
-                return record["Opportunity__r"]["JiraComponentURL__c"]
+                return normalize_value(
+                    record["Opportunity__r"]["JiraComponentURL__c"]
+                )
             except (TypeError, KeyError):
                 return ""
 
         def _get_opportunity_percentage():
             try:
-                return record["Opportunity__r"]["Probability"]
+                return normalize_value(record["Opportunity__r"]["Probability"])
             except (TypeError, KeyError):
                 return ""
 
         project_line_items = (
             [
                 ProjectLineItemDTO.from_salesforce_record(item)
                 for item in record.get("Project_Line_Items__r", {}).get(
```

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from itertools import islice
 from urllib.parse import quote
 
 from gc_google_services_api.bigquery import BigQueryManager
 
 
 class BigQueryExporter:
     def __init__(self, project_id, dataset_id):
@@ -169,74 +170,106 @@
                     profit_center,
                     cost_center,
                     project_tier,
                     jira_task_url,
                     opportunity_percentage
                 ) VALUES {', '.join(opportunities_values)};
             """
+
+            insert_opportunities_query = (
+                insert_opportunities_query.replace("\n", "")
+                .replace("    ", "")
+                .replace("  ", "")
+            )
+
             self.client.execute_query(insert_opportunities_query, None)
 
     def _export_billing_lines(self, opportunities):
-        billing_lines_values = []
-        for opp in opportunities:
-            for bl in opp["billing_lines"]:
-                billing_date = (
-                    f'DATE "{bl["billing_date"]}"'
-                    if bl["billing_date"]
-                    else "NULL"
-                )
-                billing_period_ending_date = (
-                    f'DATE "{bl["billing_period_ending_date"]}"'
-                    if bl["billing_period_ending_date"]
-                    else "NULL"
-                )
-                billing_period_starting_date = (
-                    f'DATE "{bl["billing_period_starting_date"]}"'
-                    if bl["billing_period_starting_date"]
-                    else "NULL"
-                )
-                billing_plan_billing_date = (
-                    f'DATE "{bl["billing_plan_billing_date"]}"'
-                    if bl["billing_plan_billing_date"]
-                    else "NULL"
-                )
-                billing_plan_service_end_date = (
-                    f'DATE "{bl["billing_plan_service_end_date"]}"'
-                    if bl["billing_plan_service_end_date"]
-                    else "NULL"
-                )
-                billing_plan_service_start_date = (
-                    f'DATE "{bl["billing_plan_service_start_date"]}"'
-                    if bl["billing_plan_service_start_date"]
-                    else "NULL"
+        total_billing_lines = sum(
+            len(opp["billing_lines"]) for opp in opportunities
+        )
+
+        for i in range(0, total_billing_lines, self.batch_size):
+            batch_opportunities = []
+            batch_billing_lines = []
+
+            for opp in opportunities:
+                remaining_lines = islice(
+                    opp["billing_lines"], i, i + self.batch_size
                 )
+                batch_opportunities.append(opp)
+                batch_billing_lines.extend(remaining_lines)
 
-                billing_lines_values.append(
-                    f"""
-                    (
-                        "{bl['id']}",
-                        "{bl['project_id']}",
-                        "{bl['name']}",
-                        "{bl['currency']}",
-                        TIMESTAMP "{bl['created_date']}",
-                        TIMESTAMP "{bl['last_modified_date']}",
-                        {bl['billing_amount']},
-                        {billing_date},
-                        {billing_period_ending_date},
-                        {billing_period_starting_date},
-                        {bl['hourly_price'] if bl['hourly_price'] else 'NULL'},
-                        {bl['revenue_dedication'] if bl['revenue_dedication'] else 'NULL'},
-                        "{bl['billing_plan_amount']}",
-                        {billing_plan_billing_date},
-                        "{bl['billing_plan_item']}",
-                        {billing_plan_service_end_date},
-                        {billing_plan_service_start_date}
-                    )
-                    """
+                if len(batch_billing_lines) >= self.batch_size:
+                    self._process_billing_lines_batch(batch_billing_lines)
+
+                    batch_opportunities = []
+                    batch_billing_lines = []
+
+            if batch_billing_lines:
+                self._process_billing_lines_batch(batch_billing_lines)
+
+    def _process_billing_lines_batch(self, billing_lines):
+        billing_lines_values = []
+        for bl in billing_lines:
+            billing_date = (
+                f'DATE "{bl["billing_date"]}"'
+                if bl["billing_date"]
+                else "NULL"
+            )
+            billing_period_ending_date = (
+                f'DATE "{bl["billing_period_ending_date"]}"'
+                if bl["billing_period_ending_date"]
+                else "NULL"
+            )
+            billing_period_starting_date = (
+                f'DATE "{bl["billing_period_starting_date"]}"'
+                if bl["billing_period_starting_date"]
+                else "NULL"
+            )
+            billing_plan_billing_date = (
+                f'DATE "{bl["billing_plan_billing_date"]}"'
+                if bl["billing_plan_billing_date"]
+                else "NULL"
+            )
+            billing_plan_service_end_date = (
+                f'DATE "{bl["billing_plan_service_end_date"]}"'
+                if bl["billing_plan_service_end_date"]
+                else "NULL"
+            )
+            billing_plan_service_start_date = (
+                f'DATE "{bl["billing_plan_service_start_date"]}"'
+                if bl["billing_plan_service_start_date"]
+                else "NULL"
+            )
+
+            billing_lines_values.append(
+                f"""
+                (
+                    "{bl['id']}",
+                    "{bl['project_id']}",
+                    "{bl['name']}",
+                    "{bl['currency']}",
+                    TIMESTAMP "{bl['created_date']}",
+                    TIMESTAMP "{bl['last_modified_date']}",
+                    {bl['billing_amount'] if bl['billing_amount'] else 0.0},
+                    {billing_date},
+                    {billing_period_ending_date},
+                    {billing_period_starting_date},
+                    {bl['hourly_price'] if bl['hourly_price'] else 'NULL'},
+                    {bl['revenue_dedication'] if bl['revenue_dedication'] else 'NULL'},
+                    "{bl['billing_plan_amount']}",
+                    {billing_plan_billing_date},
+                    "{bl['billing_plan_item']}",
+                    {billing_plan_service_end_date},
+                    {billing_plan_service_start_date}
                 )
+                """
+            )
+
         if billing_lines_values:
             insert_billing_lines_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.billing_lines` (
                     id,
                     project_id,
                     name,
                     currency,
@@ -251,79 +284,118 @@
                     billing_plan_amount,
                     billing_plan_billing_date,
                     billing_plan_item,
                     billing_plan_service_end_date,
                     billing_plan_service_start_date
                 ) VALUES {', '.join(billing_lines_values)};
             """
+            insert_billing_lines_query = (
+                insert_billing_lines_query.replace("\n", "")
+                .replace("    ", "")
+                .replace("  ", "")
+            )
 
             self.client.execute_query(insert_billing_lines_query, None)
 
     def _export_PLIs(self, opportunities):
-        project_line_items_values = []
-        for opp in opportunities:
-            project_id = opp["project_id"]
-            for pli in opp["project_line_items"]:
-                effort = f"{pli['effort']}" if pli["effort"] else "NULL"
-                total_price = (
-                    f"{pli['total_price']}" if pli["total_price"] else "NULL"
-                )
-                unit_price = (
-                    f"{pli['unit_price']}" if pli["unit_price"] else "NULL"
-                )
-                ending_date = (
-                    f'DATE "{pli["ending_date"]}"'
-                    if pli["ending_date"]
-                    else "NULL"
-                )
-                starting_date = (
-                    f'DATE "{pli["starting_date"]}"'
-                    if pli["starting_date"]
-                    else "NULL"
+        total_plis = sum(
+            len(opp["project_line_items"]) for opp in opportunities
+        )
+
+        for i in range(0, total_plis, self.batch_size):
+            batch_opportunities = []
+            batch_plis = []
+
+            for opp in opportunities:
+                remaining_plis = islice(
+                    opp["project_line_items"], i, i + self.batch_size
                 )
+                batch_opportunities.append(opp)
+                batch_plis.extend(remaining_plis)
+                project_id = opp["project_id"]
+
+                if len(batch_plis) >= self.batch_size:
+                    self._process_plis_batch(batch_plis, project_id)
+
+                    batch_opportunities = []
+                    batch_plis = []
+
+            if batch_plis:
+                self._process_plis_batch(batch_plis, project_id)
+
+    def _process_plis_batch(self, plis, project_id):
+        plis_values = []
+        for pli in plis:
+            effort = f"{pli['effort']}" if pli["effort"] else "NULL"
+            total_price = (
+                f"{pli['total_price']}" if pli["total_price"] else "NULL"
+            )
+
+            unit_price = (
+                f"{pli['unit_price']}" if pli["unit_price"] else "NULL"
+            )
+
+            ending_date = (
+                f'DATE "{pli["ending_date"]}"'
+                if pli["ending_date"]
+                else "NULL"
+            )
 
-                project_line_items_values.append(
-                    f"""
-                    (
-                        "{pli['country']}",
-                        TIMESTAMP "{pli['created_date']}",
-                        "{effort}",
-                        {ending_date},
-                        "{pli['id']}",
-                        TIMESTAMP "{pli['last_modified_date']}",
-                        "{pli['ms_pli_name']}",
-                        "{pli['product_name']}",
-                        {pli['quantity'] if pli['quantity'] else 0.0},
-                        {starting_date},
-                        "{total_price}",
-                        "{unit_price}",
-                        "{project_id}"
-                    )
-                    """
+            starting_date = (
+                f'DATE "{pli["starting_date"]}"'
+                if pli["starting_date"]
+                else "NULL"
+            )
+
+            plis_values.append(
+                f"""
+                (
+                    "{pli['country']}",
+                    TIMESTAMP "{pli['created_date']}",
+                    "{effort}",
+                    {ending_date},
+                    "{pli['id']}",
+                    TIMESTAMP "{pli['last_modified_date']}",
+                    "{pli['ms_pli_name']}",
+                    "{pli['product_name']}",
+                    {pli['quantity'] if pli['quantity'] else 0.0},
+                    {starting_date},
+                    "{total_price}",
+                    "{unit_price}",
+                    "{project_id}"
                 )
+                """
+            )
 
-        if project_line_items_values:
-            insert_project_line_items_query = f"""
+        if plis_values:
+            insert_plis_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.project_line_items` (
                     country,
                     created_date,
                     effort,
                     ending_date,
                     id,
                     last_modified_date,
                     ms_pli_name,
                     product_name,
                     quantity,
                     starting_date,
                     total_price,
                     unit_price,
                     project_id
-                ) VALUES {', '.join(project_line_items_values)};
+                ) VALUES {', '.join(plis_values)};
             """
-            self.client.execute_query(insert_project_line_items_query, None)
+
+            insert_plis_query = (
+                insert_plis_query.replace("\n", "")
+                .replace("    ", "")
+                .replace("  ", "")
+            )
+
+            self.client.execute_query(insert_plis_query, None)
 
     def _export_accounts(self, opportunities):
         account_values = []
         for opp in opportunities:
             account_name = (
                 f'"{opp["account_name"]}"' if opp["account_name"] else "NULL"
             )
@@ -513,14 +585,20 @@
                     office,
                     payment_terms,
                     billing_state_code,
                     mail_invoicing,
                     invoicing_email
                 ) VALUES {', '.join(account_values)};
             """
+            insert_opportunities_query = (
+                insert_opportunities_query.replace("\n", "")
+                .replace("    ", "")
+                .replace("  ", "")
+            )
+
             self.client.execute_query(insert_opportunities_query, None)
 
     def export_data(self, opportunities):
         opportunities_batches = [
             opportunities[i : i + self.batch_size]  # noqa: E203
             for i in range(0, len(opportunities), self.batch_size)
         ]
```

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-1.0.1/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.0/pyproject.toml` & `ms_salesforce_api-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-1.0.0/PKG-INFO` & `ms_salesforce_api-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ms-salesforce-api Version: 1.0.0 Summary: Python
+Metadata-Version: 2.1 Name: ms-salesforce-api Version: 1.0.1 Summary: Python
 library used to extract data from Salesforce API and migrate it to Bigquery and
 Postgres. Author: Making Science Requires-Python: >=3.8.1,<4.0.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: gc-google-services-api (>=1.2.7,<2.0.0) Requires-Dist: isort
 (>=5.12.0,<6.0.0) Requires-Dist: pre-commit (>=3.1.1,<4.0.0) Requires-Dist:
```

