# Comparing `tmp/mercoa-0.1.0.tar.gz` & `tmp/mercoa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.1.0.tar", max compression
+gzip compressed data, was "mercoa-0.1.1.tar", max compression
```

## Comparing `mercoa-0.1.0.tar` & `mercoa-0.1.1.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0      410 2023-05-31 04:09:52.712105 mercoa-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6243 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/__init__.py
--rw-r--r--   0        0        0     5449 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      326 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/py.typed
--rw-r--r--   0        0        0     6430 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     2582 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      397 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      148 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      216 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      469 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      441 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/order_direction.py
--rw-r--r--   0        0        0      855 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      199 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4513 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/client.py
--rw-r--r--   0        0        0      256 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/types/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/types/counterparty_response.py
--rw-r--r--   0        0        0     1446 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/counterparty/types/find_counterparties_response.py
--rw-r--r--   0        0        0     1491 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    34975 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     2109 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/__init__.py
--rw-r--r--   0        0        0      487 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/account_type.py
--rw-r--r--   0        0        0      836 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/amount_trigger.py
--rw-r--r--   0        0        0     1075 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_request.py
--rw-r--r--   0        0        0     1003 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_response.py
--rw-r--r--   0        0        0     1059 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_update_request.py
--rw-r--r--   0        0        0      963 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/approver_rule.py
--rw-r--r--   0        0        0     1535 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/business_type.py
--rw-r--r--   0        0        0      741 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/ein.py
--rw-r--r--   0        0        0      914 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_add_payees_request.py
--rw-r--r--   0        0        0       80 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_id.py
--rw-r--r--   0        0        0     2432 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_request.py
--rw-r--r--   0        0        0     1814 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_status.py
--rw-r--r--   0        0        0     2084 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/entity_update_request.py
--rw-r--r--   0        0        0      727 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/identifier_list.py
--rw-r--r--   0        0        0     1372 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-05-31 04:09:52.712105 mercoa-0.1.0/src/mercoa/resources/entity/types/individual_profile_response.py
--rw-r--r--   0        0        0     1059 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/invoice_metrics_response.py
--rw-r--r--   0        0        0       80 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/policy_id.py
--rw-r--r--   0        0        0      974 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/profile_response.py
--rw-r--r--   0        0        0      428 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/rule.py
--rw-r--r--   0        0        0      761 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/tax_id.py
--rw-r--r--   0        0        0      594 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity/types/trigger.py
--rw-r--r--   0        0        0      207 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/__init__.py
--rw-r--r--   0        0        0     9662 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/client.py
--rw-r--r--   0        0        0      281 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/types/__init__.py
--rw-r--r--   0        0        0       84 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_response.py
--rw-r--r--   0        0        0      847 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    23201 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0     1253 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0      935 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/approval_request.py
--rw-r--r--   0        0        0      990 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/approver.py
--rw-r--r--   0        0        0      631 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/approver_action.py
--rw-r--r--   0        0        0      862 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/approver_response.py
--rw-r--r--   0        0        0       81 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/comment_id.py
--rw-r--r--   0        0        0      934 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/comment_request.py
--rw-r--r--   0        0        0     1128 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/comment_response.py
--rw-r--r--   0        0        0     1048 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/create_vendor_request.py
--rw-r--r--   0        0        0    22179 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/currency_code.py
--rw-r--r--   0        0        0      955 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/document_response.py
--rw-r--r--   0        0        0       81 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_id.py
--rw-r--r--   0        0        0     1302 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1229 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_line_item_response.py
--rw-r--r--   0        0        0      870 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_order_by_field.py
--rw-r--r--   0        0        0     4084 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_request.py
--rw-r--r--   0        0        0     4060 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_response.py
--rw-r--r--   0        0        0     1485 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_status.py
--rw-r--r--   0        0        0      213 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4443 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      298 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/attachments.py
--rw-r--r--   0        0        0     1969 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/email_ocr_request.py
--rw-r--r--   0        0        0      891 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/ocr_mailbox.py
--rw-r--r--   0        0        0     1234 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      983 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0     7449 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1466 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      948 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      656 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1463 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1579 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1145 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      797 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0     1087 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    14367 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/client.py
--rw-r--r--   0        0        0     1638 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/__init__.py
--rw-r--r--   0        0        0       85 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_id.py
--rw-r--r--   0        0        0     1297 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_request.py
--rw-r--r--   0        0        0     1318 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_brand.py
--rw-r--r--   0        0        0       78 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_id.py
--rw-r--r--   0        0        0     1120 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_request.py
--rw-r--r--   0        0        0     1217 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_response.py
--rw-r--r--   0        0        0      750 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_type.py
--rw-r--r--   0        0        0       79 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_id.py
--rw-r--r--   0        0        0     1152 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_request.py
--rw-r--r--   0        0        0     1327 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_response.py
--rw-r--r--   0        0        0       80 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_id.py
--rw-r--r--   0        0        0     1568 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1922 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
--rw-r--r--   0        0        0     1639 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py
--rw-r--r--   0        0        0       87 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_id.py
--rw-r--r--   0        0        0     1296 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_request.py
--rw-r--r--   0        0        0     1662 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_response.py
--rw-r--r--   0        0        0     1229 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_type.py
--rw-r--r--   0        0        0      893 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_update_request.py
--rw-r--r--   0        0        0      425 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0     7794 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0      589 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/__init__.py
--rw-r--r--   0        0        0     1984 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1597 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1709 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
--rw-r--r--   0        0        0      143 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/process_invoice/__init__.py
--rw-r--r--   0        0        0     2498 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/process_invoice/client.py
--rw-r--r--   0        0        0      161 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/process_invoice/types/__init__.py
--rw-r--r--   0        0        0      916 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/process_invoice/types/process_invoice_request.py
--rw-r--r--   0        0        0      269 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/__init__.py
--rw-r--r--   0        0        0     8182 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/client.py
--rw-r--r--   0        0        0      381 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/__init__.py
--rw-r--r--   0        0        0       88 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/representative/types/responsibilities.py
--rw-r--r--   0        0        0      271 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     4315 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      386 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1125 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1564 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_response_expanded.py
--rw-r--r--   0        0        0     1261 2023-05-31 04:09:52.716105 mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-06-14 06:27:11.377764 mercoa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6227 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     5449 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/py.typed
+-rw-r--r--   0        0        0     6414 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-06-14 06:27:11.377764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     2582 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      397 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      216 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      469 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0      855 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      199 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4513 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/client.py
+-rw-r--r--   0        0        0      256 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/types/__init__.py
+-rw-r--r--   0        0        0     1022 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/types/counterparty_response.py
+-rw-r--r--   0        0        0     1446 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/counterparty/types/find_counterparties_response.py
+-rw-r--r--   0        0        0     1491 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    34975 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0     2109 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/account_type.py
+-rw-r--r--   0        0        0      836 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/amount_trigger.py
+-rw-r--r--   0        0        0     1075 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1003 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1059 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0      963 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/approver_rule.py
+-rw-r--r--   0        0        0     1535 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/business_profile_request.py
+-rw-r--r--   0        0        0     1492 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/business_type.py
+-rw-r--r--   0        0        0      741 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/ein.py
+-rw-r--r--   0        0        0      914 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0       80 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_id.py
+-rw-r--r--   0        0        0     2432 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_request.py
+-rw-r--r--   0        0        0     1814 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/entity_update_request.py
+-rw-r--r--   0        0        0      727 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/identifier_list.py
+-rw-r--r--   0        0        0     1372 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/individual_profile_response.py
+-rw-r--r--   0        0        0     1059 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0       80 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/policy_id.py
+-rw-r--r--   0        0        0      974 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/profile_response.py
+-rw-r--r--   0        0        0      428 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/rule.py
+-rw-r--r--   0        0        0      761 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/tax_id.py
+-rw-r--r--   0        0        0      594 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity/types/trigger.py
+-rw-r--r--   0        0        0      207 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/__init__.py
+-rw-r--r--   0        0        0     9662 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/client.py
+-rw-r--r--   0        0        0      281 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/types/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_response.py
+-rw-r--r--   0        0        0      831 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    23201 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0     1228 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/approval_request.py
+-rw-r--r--   0        0        0      843 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/approver.py
+-rw-r--r--   0        0        0      631 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/approver_action.py
+-rw-r--r--   0        0        0      862 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/approver_response.py
+-rw-r--r--   0        0        0       81 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_id.py
+-rw-r--r--   0        0        0      934 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_request.py
+-rw-r--r--   0        0        0     1128 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_response.py
+-rw-r--r--   0        0        0    22179 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/currency_code.py
+-rw-r--r--   0        0        0      955 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/document_response.py
+-rw-r--r--   0        0        0       81 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_id.py
+-rw-r--r--   0        0        0     1302 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1229 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0      870 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     3437 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_request.py
+-rw-r--r--   0        0        0     4234 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_response.py
+-rw-r--r--   0        0        0     1485 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_status.py
+-rw-r--r--   0        0        0      922 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/invoice/types/set_approver.py
+-rw-r--r--   0        0        0      213 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4340 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      298 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1068 2023-06-14 06:27:11.381764 mercoa-0.1.1/src/mercoa/resources/ocr/types/attachments.py
+-rw-r--r--   0        0        0     1969 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/ocr/types/email_ocr_request.py
+-rw-r--r--   0        0        0      891 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/ocr/types/ocr_mailbox.py
+-rw-r--r--   0        0        0     1234 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      983 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0     7449 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1466 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      656 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1145 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      797 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0     1087 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    14367 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/client.py
+-rw-r--r--   0        0        0     1638 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_id.py
+-rw-r--r--   0        0        0     1297 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_request.py
+-rw-r--r--   0        0        0     1318 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_type.py
+-rw-r--r--   0        0        0      819 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_brand.py
+-rw-r--r--   0        0        0       78 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_id.py
+-rw-r--r--   0        0        0     1120 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_request.py
+-rw-r--r--   0        0        0     1217 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_type.py
+-rw-r--r--   0        0        0       79 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_id.py
+-rw-r--r--   0        0        0     1152 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_request.py
+-rw-r--r--   0        0        0     1327 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_response.py
+-rw-r--r--   0        0        0       80 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_id.py
+-rw-r--r--   0        0        0     1568 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1922 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1639 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0       87 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_id.py
+-rw-r--r--   0        0        0     1296 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_request.py
+-rw-r--r--   0        0        0     1662 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_response.py
+-rw-r--r--   0        0        0     1229 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_type.py
+-rw-r--r--   0        0        0      893 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_update_request.py
+-rw-r--r--   0        0        0      425 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0     7794 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0      589 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/__init__.py
+-rw-r--r--   0        0        0     1984 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1597 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1709 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0      143 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/process_invoice/__init__.py
+-rw-r--r--   0        0        0     2498 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/process_invoice/client.py
+-rw-r--r--   0        0        0      161 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/process_invoice/types/__init__.py
+-rw-r--r--   0        0        0      916 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/process_invoice/types/process_invoice_request.py
+-rw-r--r--   0        0        0      269 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/__init__.py
+-rw-r--r--   0        0        0     8182 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/client.py
+-rw-r--r--   0        0        0      381 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/representative/types/responsibilities.py
+-rw-r--r--   0        0        0      271 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     4315 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1125 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1564 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-06-14 06:27:11.385764 mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.1.1/PKG-INFO
```

### Comparing `mercoa-0.1.0/src/mercoa/__init__.py` & `mercoa-0.1.1/src/mercoa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     CheckResponse,
     ColorSchemeRequest,
     ColorSchemeResponse,
     CommentId,
     CommentRequest,
     CommentResponse,
     CounterpartyResponse,
-    CreateVendorRequest,
     CurrencyCode,
     CustomId,
     CustomPaymentMethodRequest,
     CustomPaymentMethodResponse,
     CustomPaymentMethodUpdateRequest,
     DocumentResponse,
     Ein,
@@ -110,14 +109,15 @@
     ProfileResponse,
     RepresentativeId,
     RepresentativeRequest,
     RepresentativeResponse,
     Responsibilities,
     Rule,
     Rule_Approver,
+    SetApprover,
     TaxID,
     TransactionId,
     TransactionResponse,
     TransactionResponseExpanded,
     TransactionStatus,
     Trigger,
     Trigger_All,
@@ -172,15 +172,14 @@
     "CheckResponse",
     "ColorSchemeRequest",
     "ColorSchemeResponse",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "CounterpartyResponse",
-    "CreateVendorRequest",
     "CurrencyCode",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "CustomPaymentMethodUpdateRequest",
     "DocumentResponse",
     "Ein",
@@ -248,14 +247,15 @@
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "Rule",
     "Rule_Approver",
     "SSN",
+    "SetApprover",
     "TaxID",
     "TransactionId",
     "TransactionResponse",
     "TransactionResponseExpanded",
     "TransactionStatus",
     "Trigger",
     "Trigger_All",
```

### Comparing `mercoa-0.1.0/src/mercoa/client.py` & `mercoa-0.1.1/src/mercoa/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/core/datetime_utils.py` & `mercoa-0.1.1/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.1.1/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,24 +66,24 @@
     ApprovalRequest,
     Approver,
     ApproverAction,
     ApproverResponse,
     CommentId,
     CommentRequest,
     CommentResponse,
-    CreateVendorRequest,
     CurrencyCode,
     DocumentResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
+    SetApprover,
 )
 from .ocr import Attachments, EmailOcrRequest, OcrMailbox, OCRResponse
 from .organization import (
     ColorSchemeRequest,
     ColorSchemeResponse,
     EmailLogResponse,
     EmailProviderRequest,
@@ -170,15 +170,14 @@
     "CheckResponse",
     "ColorSchemeRequest",
     "ColorSchemeResponse",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "CounterpartyResponse",
-    "CreateVendorRequest",
     "CurrencyCode",
     "CustomId",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
     "CustomPaymentMethodUpdateRequest",
     "DocumentResponse",
     "Ein",
@@ -245,14 +244,15 @@
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "Rule",
     "Rule_Approver",
     "SSN",
+    "SetApprover",
     "TaxID",
     "TransactionId",
     "TransactionResponse",
     "TransactionResponseExpanded",
     "TransactionStatus",
     "Trigger",
     "Trigger_All",
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.1.1/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.1.1/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/commons/types/address.py` & `mercoa-0.1.1/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.1.1/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.1.1/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.1.1/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.1.1/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.1.1/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.1.1/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/counterparty/client.py` & `mercoa-0.1.1/src/mercoa/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/counterparty/types/counterparty_response.py` & `mercoa-0.1.1/src/mercoa/resources/counterparty/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/counterparty/types/find_counterparties_response.py` & `mercoa-0.1.1/src/mercoa/resources/counterparty/types/find_counterparties_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/client.py` & `mercoa-0.1.1/src/mercoa/resources/entity/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/amount_trigger.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/amount_trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_response.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/approval_policy_update_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/approval_policy_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/approver_rule.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/approver_rule.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/business_profile_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/business_profile_response.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/business_type.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/ein.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_add_payees_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_add_payees_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_response.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_status.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/entity_update_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/identifier_list.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/identifier_list.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/individual_profile_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/individual_profile_response.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/invoice_metrics_response.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/invoice_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/profile_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/profile_response.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/tax_id.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity/types/trigger.py` & `mercoa-0.1.1/src/mercoa/resources/entity/types/trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity_users/client.py` & `mercoa-0.1.1/src/mercoa/resources/entity_users/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_request.py` & `mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/entity_users/types/entity_user_response.py` & `mercoa-0.1.1/src/mercoa/resources/entity_users/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,38 +4,38 @@
     ApprovalRequest,
     Approver,
     ApproverAction,
     ApproverResponse,
     CommentId,
     CommentRequest,
     CommentResponse,
-    CreateVendorRequest,
     CurrencyCode,
     DocumentResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
+    SetApprover,
 )
 
 __all__ = [
     "ApprovalRequest",
     "Approver",
     "ApproverAction",
     "ApproverResponse",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
-    "CreateVendorRequest",
     "CurrencyCode",
     "DocumentResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
+    "SetApprover",
 ]
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/client.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,46 +106,46 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> InvoiceResponse:
+    def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> CommentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/approve"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> InvoiceResponse:
+    def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> CommentResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/reject"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
             headers=remove_none_from_headers(
@@ -333,48 +333,48 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.List[DocumentResponse], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> InvoiceResponse:
+    async def approve(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> CommentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/approve"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> InvoiceResponse:
+    async def reject(self, invoice_id: InvoiceId, *, request: ApprovalRequest) -> CommentResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/reject"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InvoiceResponse, _response_json)  # type: ignore
+            return pydantic.parse_obj_as(CommentResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_comments(self, invoice_id: InvoiceId) -> typing.List[CommentResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"invoice/{invoice_id}/comments"),
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 from .approval_request import ApprovalRequest
 from .approver import Approver
 from .approver_action import ApproverAction
 from .approver_response import ApproverResponse
 from .comment_id import CommentId
 from .comment_request import CommentRequest
 from .comment_response import CommentResponse
-from .create_vendor_request import CreateVendorRequest
 from .currency_code import CurrencyCode
 from .document_response import DocumentResponse
 from .invoice_id import InvoiceId
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_order_by_field import InvoiceOrderByField
 from .invoice_request import InvoiceRequest
 from .invoice_response import InvoiceResponse
 from .invoice_status import InvoiceStatus
+from .set_approver import SetApprover
 
 __all__ = [
     "ApprovalRequest",
     "Approver",
     "ApproverAction",
     "ApproverResponse",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
-    "CreateVendorRequest",
     "CurrencyCode",
     "DocumentResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
+    "SetApprover",
 ]
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/approval_request.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/approval_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/approver.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/set_approver.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...entity_users.types.entity_user_id import EntityUserId
-from .approver_action import ApproverAction
 
 
-class Approver(pydantic.BaseModel):
+class SetApprover(pydantic.BaseModel):
     user_id: EntityUserId = pydantic.Field(alias="userId")
     date: dt.datetime
-    action: ApproverAction
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/approver_action.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/approver_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/approver_response.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/approver_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/comment_request.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/comment_response.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/create_vendor_request.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...entity.types.entity_request import EntityRequest
-from ...payment_method.types.payment_method_request import PaymentMethodRequest
+from .email_sender_request import EmailSenderRequest
 
 
-class CreateVendorRequest(pydantic.BaseModel):
-    vendor: EntityRequest
-    payment_method: typing.Optional[PaymentMethodRequest] = pydantic.Field(alias="paymentMethod")
+class EmailProviderRequest(pydantic.BaseModel):
+    sender: EmailSenderRequest
+    inbox_domain: str = pydantic.Field(alias="inboxDomain")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/currency_code.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/document_response.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_line_item_request.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_line_item_response.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_line_item_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_order_by_field.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_order_by_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_request.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from ...entity.types.entity_id import EntityId
 from ...entity_users.types.entity_user_id import EntityUserId
 from ...payment_method.types.payment_method_id import PaymentMethodId
-from .create_vendor_request import CreateVendorRequest
 from .currency_code import CurrencyCode
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_status import InvoiceStatus
+from .set_approver import SetApprover
 
 
 class InvoiceRequest(pydantic.BaseModel):
     status: typing.Optional[InvoiceStatus]
     amount: typing.Optional[float]
     currency: typing.Optional[CurrencyCode]
     invoice_date: typing.Optional[dt.datetime] = pydantic.Field(
@@ -31,28 +31,19 @@
     due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate", description=("Due date of invoice.\n"))
     invoice_number: typing.Optional[str] = pydantic.Field(alias="invoiceNumber")
     note_to_self: typing.Optional[str] = pydantic.Field(alias="noteToSelf")
     service_start_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceStartDate")
     service_end_date: typing.Optional[dt.datetime] = pydantic.Field(alias="serviceEndDate")
     payer_id: typing.Optional[EntityId] = pydantic.Field(alias="payerId")
     payment_source_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentSourceId")
+    approvers: typing.Optional[typing.List[SetApprover]] = pydantic.Field(
+        description=("Set approvers for this invoice.\n")
+    )
     vendor_id: typing.Optional[EntityId] = pydantic.Field(alias="vendorId")
     payment_destination_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentDestinationId")
-    create_vendor: typing.Optional[CreateVendorRequest] = pydantic.Field(
-        alias="createVendor",
-        description=(
-            "When paying to a new vendor, use the createVendor object. Mercoa will create the vendor entity and tie it to this invoice. This object is ignored when updating an invoice.\n"
-        ),
-    )
-    update_vendor: typing.Optional[CreateVendorRequest] = pydantic.Field(
-        alias="updateVendor",
-        description=(
-            "When paying to an existing vendor with an incomplete profile, use the updateVendor object. Mercoa will update the vendor entity tied to this invoice. This object is ignored if the vendor already has already been created with complete information and when creating a new invoice.\n"
-        ),
-    )
     line_items: typing.Optional[typing.List[InvoiceLineItemRequest]] = pydantic.Field(alias="lineItems")
     metadata: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
         description=(
             "Metadata associated with this invoice. You can specify up to 10 keys, with key names up to 40 characters long and values up to 200 characters long.\n"
         )
     )
     uploaded_image: typing.Optional[str] = pydantic.Field(
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_response.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...entity.types.approval_policy_response import ApprovalPolicyResponse
 from ...entity.types.entity_id import EntityId
 from ...entity.types.entity_response import EntityResponse
 from ...entity_users.types.entity_user_response import EntityUserResponse
 from ...payment_method.types.payment_method_id import PaymentMethodId
 from ...payment_method.types.payment_method_response import PaymentMethodResponse
 from ...transaction.types.transaction_response import TransactionResponse
 from .approver import Approver
@@ -49,14 +50,15 @@
     payment_destination_id: typing.Optional[PaymentMethodId] = pydantic.Field(alias="paymentDestinationId")
     payment_destination_confirmed: bool = pydantic.Field(alias="paymentDestinationConfirmed")
     has_documents: bool = pydantic.Field(alias="hasDocuments")
     comments: typing.Optional[typing.List[CommentResponse]]
     transactions: typing.Optional[typing.List[TransactionResponse]]
     line_items: typing.Optional[typing.List[InvoiceLineItemResponse]] = pydantic.Field(alias="lineItems")
     approvers: typing.List[Approver]
+    approval_policy: typing.List[ApprovalPolicyResponse] = pydantic.Field(alias="approvalPolicy")
     metadata: typing.Dict[str, str] = pydantic.Field(description=("Metadata associated with this invoice.\n"))
     created_by: typing.Optional[EntityUserResponse] = pydantic.Field(
         alias="createdBy", description=("Entity user who created this invoice.\n")
     )
     processed_at: typing.Optional[dt.datetime] = pydantic.Field(alias="processedAt")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/invoice/types/invoice_status.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/ocr/client.py` & `mercoa-0.1.1/src/mercoa/resources/ocr/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..organization.types.organization_id import OrganizationId
-from .types.email_ocr_request import EmailOcrRequest
 from .types.ocr_response import OCRResponse
 
 
 class OcrClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
@@ -36,20 +35,20 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OCRResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def email_inbox(self, *, org: OrganizationId, items: typing.List[EmailOcrRequest]) -> None:
+    def email_inbox(self, *, org: OrganizationId, request: typing.Any) -> None:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "emailOcr"),
             params={"org": org},
-            json=jsonable_encoder({"items": items}),
+            json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         if 200 <= _response.status_code < 300:
             return
         try:
@@ -80,21 +79,21 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(OCRResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def email_inbox(self, *, org: OrganizationId, items: typing.List[EmailOcrRequest]) -> None:
+    async def email_inbox(self, *, org: OrganizationId, request: typing.Any) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "emailOcr"),
                 params={"org": org},
-                json=jsonable_encoder({"items": items}),
+                json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         if 200 <= _response.status_code < 300:
             return
         try:
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/ocr/types/attachments.py` & `mercoa-0.1.1/src/mercoa/resources/ocr/types/attachments.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/ocr/types/email_ocr_request.py` & `mercoa-0.1.1/src/mercoa/resources/ocr/types/email_ocr_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/ocr/types/ocr_mailbox.py` & `mercoa-0.1.1/src/mercoa/resources/ocr/types/ocr_mailbox.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.1.1/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/client.py` & `mercoa-0.1.1/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/color_scheme_request.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/color_scheme_response.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_sender_request import EmailSenderRequest
+from .email_sender_response import EmailSenderResponse
 
 
-class EmailProviderRequest(pydantic.BaseModel):
-    sender: EmailSenderRequest
+class EmailProviderResponse(pydantic.BaseModel):
+    sender: EmailSenderResponse
     inbox_domain: str = pydantic.Field(alias="inboxDomain")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.1.1/src/mercoa/resources/process_invoice/types/process_invoice_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_sender_response import EmailSenderResponse
+from ...invoice.types.invoice_id import InvoiceId
 
 
-class EmailProviderResponse(pydantic.BaseModel):
-    sender: EmailSenderResponse
-    inbox_domain: str = pydantic.Field(alias="inboxDomain")
+class ProcessInvoiceRequest(pydantic.BaseModel):
+    invoice_ids: typing.List[InvoiceId] = pydantic.Field(alias="invoiceIds")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.1.1/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/client.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_request.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_account_response.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_status.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/bank_type.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_brand.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_request.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_response.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/card_type.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_request.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/check_response.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_request.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_response.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_request.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_response.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_type.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method/types/payment_method_update_request.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method/types/payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/__init__.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py` & `mercoa-0.1.1/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/process_invoice/client.py` & `mercoa-0.1.1/src/mercoa/resources/process_invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/process_invoice/types/process_invoice_request.py` & `mercoa-0.1.1/src/mercoa/resources/invoice/types/approver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import pydantic
-
 from ....core.datetime_utils import serialize_datetime
-from ...invoice.types.invoice_id import InvoiceId
+from .approver_action import ApproverAction
+from .set_approver import SetApprover
 
 
-class ProcessInvoiceRequest(pydantic.BaseModel):
-    invoice_ids: typing.List[InvoiceId] = pydantic.Field(alias="invoiceIds")
+class Approver(SetApprover):
+    roles: typing.List[str]
+    action: ApproverAction
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.1.0/src/mercoa/resources/representative/client.py` & `mercoa-0.1.1/src/mercoa/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/representative/types/representative_request.py` & `mercoa-0.1.1/src/mercoa/resources/representative/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/representative/types/representative_response.py` & `mercoa-0.1.1/src/mercoa/resources/representative/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/representative/types/responsibilities.py` & `mercoa-0.1.1/src/mercoa/resources/representative/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/transaction/client.py` & `mercoa-0.1.1/src/mercoa/resources/transaction/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_response.py` & `mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_response_expanded.py` & `mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.1.1/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.1.0/PKG-INFO` & `mercoa-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

