# Comparing `tmp/vesselapi-3.27.1.tar.gz` & `tmp/vesselapi-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vesselapi-3.27.1.tar", last modified: Wed Jun 14 00:08:57 2023, max compression
+gzip compressed data, was "vesselapi-3.5.2.tar", last modified: Tue Mar  7 22:17:16 2023, max compression
```

## Comparing `vesselapi-3.27.1.tar` & `vesselapi-3.5.2.tar`

### file list

```diff
@@ -1,171 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:57.397426 vesselapi-3.27.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-14 00:08:57.397426 vesselapi-3.27.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7350 2023-06-14 00:08:43.000000 vesselapi-3.27.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 00:08:57.397426 vesselapi-3.27.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-06-14 00:08:43.000000 vesselapi-3.27.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:57.349426 vesselapi-3.27.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:57.353426 vesselapi-3.27.1/src/vesselapi/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10492 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10131 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10358 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/calls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4414 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10454 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10238 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10396 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10279 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1633 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10324 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:57.353426 vesselapi-3.27.1/src/vesselapi/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:57.369426 vesselapi-3.27.1/src/vesselapi/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10779 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/delete_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/delete_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_calls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2208 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_event_attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2127 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2093 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2055 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2055 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2022 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2022 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2022 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2022 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2022 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1847 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2086 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1839 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1839 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1871 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1656 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2151 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1992 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1978 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1956 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1904 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1703 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/get_one_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1352 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1409 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1266 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1332 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1332 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1243 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1266 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3526 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_passthrough.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2115 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_link_exchange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_link_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1636 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/post_webhook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1402 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1431 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1240 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_event_attendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1428 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1475 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1428 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6237 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4684 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_calls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_contacts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5422 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_deals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6268 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_emails.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4412 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_event_attendees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5193 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5095 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_leads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4281 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4929 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4267 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:57.393426 vesselapi-3.27.1/src/vesselapi/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2864 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4889 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/accountcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2632 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/accountupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1208 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/address.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      684 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/booleanfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3376 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/callcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      704 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/callupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1763 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4324 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/contactcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2036 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/contactupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/datefilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5087 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/deal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2001 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/dealcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/dealupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5494 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/email.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5533 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/emailcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1592 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/emailupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4263 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3132 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/eventattendee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/eventattendeecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      519 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/eventattendeeupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/eventcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/eventupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3201 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/field.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4491 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/lead.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2342 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/leadcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2493 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/leadupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2721 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/note.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2445 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/notecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/noteupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1717 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/numberfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      341 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1846 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/stringfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1056 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/stringlistfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3639 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/task.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3386 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/taskcreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/taskupdate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3081 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1077 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/webhookmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      597 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/models/shared/webhookmetadatacreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10316 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/notes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2012 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/passthrough.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4045 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10366 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/tasks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/tokens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7340 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:57.397426 vesselapi-3.27.1/src/vesselapi/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4441 2023-06-14 00:08:43.000000 vesselapi-3.27.1/src/vesselapi/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 00:08:57.353426 vesselapi-3.27.1/src/vesselapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-14 00:08:57.000000 vesselapi-3.27.1/src/vesselapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-06-14 00:08:57.000000 vesselapi-3.27.1/src/vesselapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 00:08:57.000000 vesselapi-3.27.1/src/vesselapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-14 00:08:57.000000 vesselapi-3.27.1/src/vesselapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-14 00:08:57.000000 vesselapi-3.27.1/src/vesselapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-07 22:17:16.837517 vesselapi-3.5.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3842 2023-03-07 22:17:08.000000 vesselapi-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 22:17:16.837517 vesselapi-3.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-03-07 22:17:08.000000 vesselapi-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.821517 vesselapi-3.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8486 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8065 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3794 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8448 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8247 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8400 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8283 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8333 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.833517 vesselapi-3.5.2/src/vesselapi/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11828 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1209 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/delete_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/delete_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      913 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1836 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1957 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_event_attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1685 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1685 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1840 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1474 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1644 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1450 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1395 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/get_one_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1133 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2608 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_passthrough.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2275 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_link_exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1189 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_link_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1674 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/post_webhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event_attendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1452 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1508 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5923 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4618 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_contacts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_deals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5950 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_emails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_event_attendees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4875 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4775 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_leads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4609 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3947 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/src/vesselapi/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1979 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1915 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/accountcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1971 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/accountupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1129 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/address.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      605 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/booleanfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3304 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contactcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1583 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/contactupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/datefilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3632 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/deal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/dealcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/dealupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4129 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/email.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4053 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/emailcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/emailupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2195 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendeecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      440 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventattendeeupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2518 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1918 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/eventupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2634 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/field.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      971 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3485 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/lead.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/leadcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/leadupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2076 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/note.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1599 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/notecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/noteupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/numberfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/stringfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/stringlistfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2949 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/task.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/taskcreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1681 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/taskupdate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      531 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadatacreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8325 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/notes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2026 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/passthrough.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6878 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8375 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/tasks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1761 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/tokens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5961 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.837517 vesselapi-3.5.2/src/vesselapi/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23642 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3878 2023-03-07 22:17:08.000000 vesselapi-3.5.2/src/vesselapi/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:17:16.825517 vesselapi-3.5.2/src/vesselapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-07 22:17:16.000000 vesselapi-3.5.2/src/vesselapi.egg-info/top_level.txt
```

### Comparing `vesselapi-3.27.1/src/vesselapi/accounts.py` & `vesselapi-3.5.2/src/vesselapi/accounts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,206 +1,203 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
 class Accounts:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmAccountRequest) -> operations.GetBatchCrmAccountResponse:
         r"""Get Batch Accounts
         Retrieve Accounts by a set of Id's
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/account/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmAccountRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/account/batch'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmAccountRequestBody) -> operations.PostCrmAccountResponse:
+    def create(self, request: operations.PostCrmAccountRequest) -> operations.PostCrmAccountResponse:
         r"""Create Account
         Create a new Account
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/account'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/account'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmAccountRequest) -> operations.GetDetailsCrmAccountResponse:
         r"""Get Account Details
         Get details about all accounts. 
         Details include the type, possible values, and other meta data about the fields.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/account/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmAccountRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/account/details'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmAccountRequest) -> operations.GetOneCrmAccountResponse:
         r"""Get Account
         Retrieve a single Account by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/account'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmAccountRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/account'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmAccountResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmAccountsRequest) -> operations.GetAllCrmAccountsResponse:
         r"""Get All Accounts
         Retrieve all Accounts
         *CRM Caveats*:
         - Pipedrive: dealIds + contactIds not supported when querying for all accounts
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/accounts'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmAccountsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/accounts'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmAccountsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmAccountsRequest) -> operations.SearchCrmAccountsResponse:
         r"""Search Accounts
         Search all Accounts using filters
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/accounts/search'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/accounts/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmAccountsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmAccountsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmAccountsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmAccountRequestBody) -> operations.PutCrmAccountResponse:
+    def update(self, request: operations.PutCrmAccountRequest) -> operations.PutCrmAccountResponse:
         r"""Update Account
         Update an existing Account
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/account'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/account'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutCrmAccountResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `vesselapi-3.27.1/src/vesselapi/attendees.py` & `vesselapi-3.5.2/src/vesselapi/attendees.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,200 +1,195 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
 class Attendees:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmEventAttendeeRequest) -> operations.GetBatchCrmEventAttendeeResponse:
         r"""Get Batch Event Attendees
         Retrieve Event Attendees by a set of Id's
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/attendee/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmEventAttendeeRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
         
-        client = self.sdk_configuration.security_client
+        url = base_url.removesuffix('/') + '/crm/event/attendee/batch'
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        query_params = utils.get_query_params(request.query_params)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEventAttendeeResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def create(self) -> operations.PostCrmEventAttendeeResponse:
         r"""Create Event Attendee
         Add an Attendee to an Event
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/attendee'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
         
-        client = self.sdk_configuration.security_client
+        url = base_url.removesuffix('/') + '/crm/event/attendee'
         
-        http_res = client.request('POST', url, headers=headers)
+        
+        client = self._security_client
+        
+        http_res = client.request('POST', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEventAttendeeResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmEventAttendeeRequest) -> operations.GetDetailsCrmEventAttendeeResponse:
         r"""Get Event Attendee Details
         Get details about all event attendees. 
         Details include the type, possible values, and other meta data about the fields.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/attendee/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmEventAttendeeRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event/attendee/details'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEventAttendeeResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmEventAttendeeRequest) -> operations.GetOneCrmEventAttendeeResponse:
         r"""Get Event Attendee
         Retrieve a single Event Attendee by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/attendee'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmEventAttendeeRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event/attendee'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEventAttendeeResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmEventAttendeesRequest) -> operations.GetAllCrmEventAttendeesResponse:
         r"""Get All Event Attendees
         Retrieve all Attendees for all Events
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/attendees'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmEventAttendeesRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event/attendees'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmEventAttendeesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEventAttendeesResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmEventAttendeesRequest) -> operations.SearchCrmEventAttendeesResponse:
         r"""Search Event Attendees
         Search all Event Attendees using filters
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/attendees/search'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event/attendees/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmEventAttendeesRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmEventAttendeesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEventAttendeesResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def update(self) -> operations.PutCrmEventAttendeeResponse:
         r"""Update Event Attendee
         Update the status of an event attendee
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/attendee'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event/attendee'
+        
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('PATCH', url, headers=headers)
+        http_res = client.request('PATCH', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutCrmEventAttendeeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmEventAttendeeResponseBody])
```

### Comparing `vesselapi-3.27.1/src/vesselapi/calls.py` & `vesselapi-3.5.2/src/vesselapi/contacts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,213 +1,208 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
-class Calls:
-    sdk_configuration: SDKConfiguration
+class Contacts:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
 
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
-    def batch(self, request: operations.GetBatchCrmCallRequestBody) -> operations.GetBatchCrmCallResponse:
-        r"""Batch Calls
-        Retrieve Call by a set of Id's
+    def batch(self, request: operations.GetBatchCrmContactRequest) -> operations.GetBatchCrmContactResponse:
+        r"""Get Batch Contacts
+        Retrieve Contacts by a set of Id's
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/call/batch'
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
         
-        client = self.sdk_configuration.security_client
+        url = base_url.removesuffix('/') + '/crm/contact/batch'
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        query_params = utils.get_query_params(request.query_params)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetBatchCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmCallRequestBody) -> operations.PostCrmCallResponse:
-        r"""Create Call
-        Create a new Call.
+    def create(self, request: operations.PostCrmContactRequest) -> operations.PostCrmContactResponse:
+        r"""Create Contact
+        Create a new contact.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/call'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/contact'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmCallRequest) -> operations.GetDetailsCrmCallResponse:
-        r"""Get Call Details
-        Get details about all Calls. 
+    def details(self, request: operations.GetDetailsCrmContactRequest) -> operations.GetDetailsCrmContactResponse:
+        r"""Get Contact Details
+        Get details about all contacts. 
         Details include the type, possible values, and other meta data about the fields.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/call/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmCallRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/contact/details'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDetailsCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmCallRequest) -> operations.GetOneCrmCallResponse:
-        r"""Get Call
-        Retrieve a single Call by Id
+    def find(self, request: operations.GetOneCrmContactRequest) -> operations.GetOneCrmContactResponse:
+        r"""Get Contact
+        Retrieve a Contact by either Id or email. When both email and Id are included, Id will take priority.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/call'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmCallRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/contact'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmContactResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmCallsRequest) -> operations.GetAllCrmCallsResponse:
-        r"""Get All Calls
-        Retrieve all Calls
+    def list(self, request: operations.GetAllCrmContactsRequest) -> operations.GetAllCrmContactsResponse:
+        r"""Get All Contacts
+        Retrieve all Contacts
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/calls'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmCallsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/contacts'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmCallsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmContactsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmCallsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmContactsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmCallsRequest) -> operations.SearchCrmCallsResponse:
-        r"""Search Calls
-        Search all Calls using filters
+    def search(self, request: operations.SearchCrmContactsRequest) -> operations.SearchCrmContactsResponse:
+        r"""Search Contacts
+        Search all Contacts using filters
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/calls/search'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/contacts/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmCallsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmCallsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SearchCrmContactsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmCallsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmContactsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmCallRequestBody) -> operations.PutCrmCallResponse:
-        r"""Update Call
-        Update an Call by Id.
+    def update(self, request: operations.PutCrmContactRequest) -> operations.PutCrmContactResponse:
+        r"""Update Contact
+        Update an existing Contact.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/call'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/contact'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmCallResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PutCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmCallResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmContactResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.27.1/src/vesselapi/connections.py` & `vesselapi-3.5.2/src/vesselapi/webhooks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,101 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
-class Connections:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
-        
-    
-    def delete(self, request: operations.DeleteConnectionRequestBody, security: operations.DeleteConnectionSecurity) -> operations.DeleteConnectionResponse:
-        r"""Delete Connection
-        Remove a connection for a given `connectionId`. Removing a connection disconnects the user's CRM so they'll need to re-authenticate should they want to re-connect their CRM.
+class Webhooks:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
+        
+    def create(self, request: operations.PostWebhookRequest) -> operations.PostWebhookResponse:
+        r"""Create Webhook
+        Create a new webhook for a given connection
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/connection/connection'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/connection/webhook'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = utils.configure_security_client(self.sdk_configuration.client, security)
+        client = self._security_client
         
-        http_res = client.request('DELETE', url, data=data, files=form, headers=headers)
+        http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostWebhookResponseBody])
+                res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneConnectionRequest) -> operations.GetOneConnectionResponse:
-        r"""Get Connection
-        Get info about a connection for a given accessToken.
+    def delete(self, request: operations.DeleteWebhookRequest) -> operations.DeleteWebhookResponse:
+        r"""Remove Webhook
+        Removes a webhook for a given connection and id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/connection/connection'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/connection/webhook'
+        
         headers = {}
-        query_params = utils.get_query_params(operations.GetOneConnectionRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        req_content_type, data, form = utils.serialize_request_body(request)
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('DELETE', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneConnectionResponseBody])
-                res.response_body = out
+            pass
 
         return res
 
-    
-    def list(self) -> operations.GetAllCrmConnectionsResponse:
-        r"""Get All Connections
-        List all established connections for a workspace
+    def find(self, request: operations.GetOneWebhookRequest) -> operations.GetOneWebhookResponse:
+        r"""Get Webhook
+        Retrieve information about a webhook for a given connection and id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/connection/connections'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/connection/webhook'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmConnectionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmConnectionsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneWebhookResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.27.1/src/vesselapi/contacts.py` & `vesselapi-3.5.2/src/vesselapi/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,211 +1,210 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
-class Contacts:
-    sdk_configuration: SDKConfiguration
+class Tasks:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
 
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
-    def batch(self, request: operations.GetBatchCrmContactRequest) -> operations.GetBatchCrmContactResponse:
-        r"""Get Batch Contacts
-        Retrieve Contacts by a set of Id's
+    def batch(self, request: operations.GetBatchCrmTaskRequest) -> operations.GetBatchCrmTaskResponse:
+        r"""Get Batch Tasks
+        Retrieve Tasks by a set of Id's
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/contact/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmContactRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/task/batch'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetBatchCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmContactResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmContactRequestBody) -> operations.PostCrmContactResponse:
-        r"""Create Contact
-        Create a new contact.
+    def create(self, request: operations.PostCrmTaskRequest) -> operations.PostCrmTaskResponse:
+        r"""Create Task
+        Create a new Task.
+        *CRM Caveats*:
+        - Salesforce: You may only associate a Task with either a Lead or a Contact *and* either a Deal or an Account.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/contact'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/task'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmContactResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmContactRequest) -> operations.GetDetailsCrmContactResponse:
-        r"""Get Contact Details
-        Get details about all contacts. 
+    def details(self, request: operations.GetDetailsCrmTaskRequest) -> operations.GetDetailsCrmTaskResponse:
+        r"""Get Task Details
+        Get details about all tasks. 
         Details include the type, possible values, and other meta data about the fields.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/contact/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmContactRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/task/details'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDetailsCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmContactResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmContactRequest) -> operations.GetOneCrmContactResponse:
-        r"""Get Contact
-        Retrieve a Contact by either Id or email. When both email and Id are included, Id will take priority.
+    def find(self, request: operations.GetOneCrmTaskRequest) -> operations.GetOneCrmTaskResponse:
+        r"""Get Task
+        Retrieve a single Task by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/contact'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmContactRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
         
-        client = self.sdk_configuration.security_client
+        url = base_url.removesuffix('/') + '/crm/task'
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        query_params = utils.get_query_params(request.query_params)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmContactResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmTaskResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmContactsRequest) -> operations.GetAllCrmContactsResponse:
-        r"""Get All Contacts
-        Retrieve all Contacts
+    def list(self, request: operations.GetAllCrmTasksRequest) -> operations.GetAllCrmTasksResponse:
+        r"""Get All Tasks
+        Retrieve all Tasks
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/contacts'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmContactsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/tasks'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmContactsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmContactsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmTasksResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmContactsRequest) -> operations.SearchCrmContactsResponse:
-        r"""Search Contacts
-        Search all Contacts using filters
+    def search(self, request: operations.SearchCrmTasksRequest) -> operations.SearchCrmTasksResponse:
+        r"""Search Tasks
+        Search all Tasks using filters
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/contacts/search'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/tasks/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmContactsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmContactsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SearchCrmTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmContactsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmTasksResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmContactRequestBody) -> operations.PutCrmContactResponse:
-        r"""Update Contact
-        Update an existing Contact.
+    def update(self, request: operations.PutCrmTaskRequest) -> operations.PutCrmTaskResponse:
+        r"""Update Task
+        Update an existing Task by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/contact'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/task'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmContactResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PutCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmContactResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmTaskResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.27.1/src/vesselapi/deals.py` & `vesselapi-3.5.2/src/vesselapi/events.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,211 +1,208 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
-class Deals:
-    sdk_configuration: SDKConfiguration
+class Events:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
 
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
-    def batch(self, request: operations.GetBatchCrmDealRequest) -> operations.GetBatchCrmDealResponse:
-        r"""Get Batch Deals
-        Retrieve Deals by a set of Id's
+    def batch(self, request: operations.GetBatchCrmEventRequest) -> operations.GetBatchCrmEventResponse:
+        r"""Get Batch Events
+        Retrieve Events by a set of Id's
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/deal/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmDealRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event/batch'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetBatchCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmDealResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmDealRequestBody) -> operations.PostCrmDealResponse:
-        r"""Create Deal
-        Create a new Deal
+    def create(self, request: operations.PostCrmEventRequest) -> operations.PostCrmEventResponse:
+        r"""Create Event
+        Create a new Event.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/deal'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmDealResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmDealRequest) -> operations.GetDetailsCrmDealResponse:
-        r"""Get Deal Details
-        Get details about all deals or a particular deal. 
+    def details(self, request: operations.GetDetailsCrmEventRequest) -> operations.GetDetailsCrmEventResponse:
+        r"""Get Event Details
+        Get details about all events. 
         Details include the type, possible values, and other meta data about the fields.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/deal/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmDealRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event/details'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDetailsCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmDealResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmDealRequest) -> operations.GetOneCrmDealResponse:
-        r"""Get Deal
-        Retrieve a single Deal by Id
+    def find(self, request: operations.GetOneCrmEventRequest) -> operations.GetOneCrmEventResponse:
+        r"""Get Event
+        Retrieve a single Event by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/deal'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmDealRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
         
-        client = self.sdk_configuration.security_client
+        url = base_url.removesuffix('/') + '/crm/event'
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        query_params = utils.get_query_params(request.query_params)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmDealResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEventResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmDealsRequest) -> operations.GetAllCrmDealsResponse:
-        r"""Get All Deals
-        Retrieve all Deals
+    def list(self, request: operations.GetAllCrmEventsRequest) -> operations.GetAllCrmEventsResponse:
+        r"""Get All Events
+        Retrieve all Events
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/deals'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmDealsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/events'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmDealsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmDealsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEventsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmDealsRequest) -> operations.SearchCrmDealsResponse:
-        r"""Search Deals
-        Search all Deals using filters
+    def search(self, request: operations.SearchCrmEventsRequest) -> operations.SearchCrmEventsResponse:
+        r"""Search Events
+        Search all Events using filters
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/deals/search'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/events/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmDealsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmDealsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SearchCrmEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmDealsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEventsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmDealRequestBody) -> operations.PutCrmDealResponse:
-        r"""Update Deal
-        Update an existing Deal
+    def update(self, request: operations.PutCrmEventRequest) -> operations.PutCrmEventResponse:
+        r"""Update Event
+        Update an existing Event by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/deal'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/event'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PutCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmDealResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmEventResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.27.1/src/vesselapi/events.py` & `vesselapi-3.5.2/src/vesselapi/notes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,211 +1,210 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
-class Events:
-    sdk_configuration: SDKConfiguration
+class Notes:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
 
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
-    def batch(self, request: operations.GetBatchCrmEventRequest) -> operations.GetBatchCrmEventResponse:
-        r"""Get Batch Events
-        Retrieve Events by a set of Id's
+    def batch(self, request: operations.GetBatchCrmNoteRequest) -> operations.GetBatchCrmNoteResponse:
+        r"""Get Batch Notes
+        Retrieve Notes by a set of Id's
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmEventRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/note/batch'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetBatchCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmEventResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmNoteResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmEventRequestBody) -> operations.PostCrmEventResponse:
-        r"""Create Event
-        Create a new Event.
+    def create(self, request: operations.PostCrmNoteRequest) -> operations.PostCrmNoteResponse:
+        r"""Create Note
+        Create a new Note.
+        *CRM Caveats*:
+        - Salesforce: You may only associate a Note with one entity.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/note'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmEventResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmNoteResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmEventRequest) -> operations.GetDetailsCrmEventResponse:
-        r"""Get Event Details
-        Get details about all events. 
+    def details(self, request: operations.GetDetailsCrmNoteRequest) -> operations.GetDetailsCrmNoteResponse:
+        r"""Get Note Details
+        Get details about all notes. 
         Details include the type, possible values, and other meta data about the fields.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmEventRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/note/details'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDetailsCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmEventResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmNoteResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmEventRequest) -> operations.GetOneCrmEventResponse:
-        r"""Get Event
-        Retrieve a single Event by Id
+    def find(self, request: operations.GetOneCrmNoteRequest) -> operations.GetOneCrmNoteResponse:
+        r"""Get Note
+        Retrieve a single Note by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmEventRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
         
-        client = self.sdk_configuration.security_client
+        url = base_url.removesuffix('/') + '/crm/note'
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        query_params = utils.get_query_params(request.query_params)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmEventResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmNoteResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmEventsRequest) -> operations.GetAllCrmEventsResponse:
-        r"""Get All Events
-        Retrieve all Events
+    def list(self, request: operations.GetAllCrmNotesRequest) -> operations.GetAllCrmNotesResponse:
+        r"""Get All Notes
+        Retrieve all Notes
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/events'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmEventsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/notes'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmNotesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmEventsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmNotesResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmEventsRequest) -> operations.SearchCrmEventsResponse:
-        r"""Search Events
-        Search all Events using filters
+    def search(self, request: operations.SearchCrmNotesRequest) -> operations.SearchCrmNotesResponse:
+        r"""Search Notes
+        Search all Notes using filters
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/events/search'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/notes/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmEventsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SearchCrmNotesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmEventsResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmNotesResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmEventRequestBody) -> operations.PutCrmEventResponse:
-        r"""Update Event
-        Update an existing Event by Id
+    def update(self, request: operations.PutCrmNoteRequest) -> operations.PutCrmNoteResponse:
+        r"""Update Note
+        Update an existing Note by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/event'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/note'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PutCrmNoteResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmEventResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmNoteResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.27.1/src/vesselapi/integrations.py` & `vesselapi-3.5.2/src/vesselapi/integrations.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
 class Integrations:
-    sdk_configuration: SDKConfiguration
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
 
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
     def list(self) -> operations.GetAllCrmIntegrationsResponse:
         r"""Get CRM Integrations
         Return all of the CRM integrations supported by Vessel.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/connection/crm/integrations'
-        headers = {}
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/connection/crm/integrations'
+        
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, headers=headers)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmIntegrationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmIntegrationsResponseBody])
```

### Comparing `vesselapi-3.27.1/src/vesselapi/leads.py` & `vesselapi-3.5.2/src/vesselapi/leads.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,203 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
 class Leads:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
     def batch(self, request: operations.GetBatchCrmLeadRequest) -> operations.GetBatchCrmLeadResponse:
         r"""Get Batch Leads
         Retrieve Leads by a set of Id's
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/lead/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmLeadRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/lead/batch'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBatchCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmLeadRequestBody) -> operations.PostCrmLeadResponse:
+    def create(self, request: operations.PostCrmLeadRequest) -> operations.PostCrmLeadResponse:
         r"""Create Lead
         Create a new Lead
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/lead'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/lead'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def details(self, request: operations.GetDetailsCrmLeadRequest) -> operations.GetDetailsCrmLeadResponse:
         r"""Get Lead Details
         Get details about all leads. 
         Details include the type, possible values, and other meta data about the fields.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/lead/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmLeadRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/lead/details'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDetailsCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def find(self, request: operations.GetOneCrmLeadRequest) -> operations.GetOneCrmLeadResponse:
         r"""Get Lead
         Retrieve a single Lead by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/lead'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmLeadRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/lead'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetOneCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmLeadResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def list(self, request: operations.GetAllCrmLeadsRequest) -> operations.GetAllCrmLeadsResponse:
         r"""Get All Leads
         Retrieve all leads.
         *CRM Caveats*:
         - Pipedrive: Only `jobTitle` is returned when querying for all leads
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/leads'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmLeadsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/leads'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAllCrmLeadsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmLeadsResponseBody])
                 res.response_body = out
 
         return res
 
-    
     def search(self, request: operations.SearchCrmLeadsRequest) -> operations.SearchCrmLeadsResponse:
         r"""Search Leads
         Search all Leads using filters
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/leads/search'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/leads/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmLeadsRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.SearchCrmLeadsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmLeadsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmLeadRequestBody) -> operations.PutCrmLeadResponse:
+    def update(self, request: operations.PutCrmLeadRequest) -> operations.PutCrmLeadResponse:
         r"""Update Lead
         Update an existing Lead by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/lead'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/lead'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PutCrmLeadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
```

### Comparing `vesselapi-3.27.1/src/vesselapi/links.py` & `vesselapi-3.5.2/src/vesselapi/passthrough.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,50 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
-class Links:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+class Passthrough:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
-    def create(self, request: operations.PostLinkExchangeRequestBody, security: operations.PostLinkExchangeSecurity) -> operations.PostLinkExchangeResponse:
-        r"""Exchange Public Token for Access Token
-        Exchanges the public token for an access token used to interact with the account. Store the access token in a secure location.
+    def create(self, request: operations.PostCrmPassthroughRequest) -> operations.PostCrmPassthroughResponse:
+        r"""Passthrough Request
+        Send an authenticated passthrough request to the downstream CRM. This is useful for making requests to endpoints that are not yet supported by Vessel.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/link/exchange'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/passthrough'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = utils.configure_security_client(self.sdk_configuration.client, security)
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostLinkExchangeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmPassthroughResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostLinkExchangeResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmPassthroughResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/__init__.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,80 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from .delete_connection import *
 from .delete_webhook import *
 from .get_all_crm_accounts import *
-from .get_all_crm_calls import *
 from .get_all_crm_connections import *
 from .get_all_crm_contacts import *
 from .get_all_crm_deals import *
 from .get_all_crm_emails import *
 from .get_all_crm_event_attendees import *
 from .get_all_crm_events import *
 from .get_all_crm_integrations import *
 from .get_all_crm_leads import *
 from .get_all_crm_notes import *
 from .get_all_crm_tasks import *
 from .get_all_crm_users import *
 from .get_batch_crm_account import *
-from .get_batch_crm_call import *
 from .get_batch_crm_contact import *
 from .get_batch_crm_deal import *
 from .get_batch_crm_email import *
 from .get_batch_crm_event import *
 from .get_batch_crm_event_attendee import *
 from .get_batch_crm_lead import *
 from .get_batch_crm_note import *
 from .get_batch_crm_task import *
 from .get_batch_crm_user import *
 from .get_details_crm_account import *
-from .get_details_crm_call import *
 from .get_details_crm_contact import *
 from .get_details_crm_deal import *
 from .get_details_crm_email import *
 from .get_details_crm_event import *
 from .get_details_crm_event_attendee import *
 from .get_details_crm_lead import *
 from .get_details_crm_note import *
 from .get_details_crm_task import *
 from .get_details_crm_user import *
 from .get_one_connection import *
 from .get_one_crm_account import *
-from .get_one_crm_call import *
 from .get_one_crm_contact import *
 from .get_one_crm_deal import *
 from .get_one_crm_email import *
 from .get_one_crm_event import *
 from .get_one_crm_event_attendee import *
 from .get_one_crm_lead import *
 from .get_one_crm_note import *
 from .get_one_crm_task import *
 from .get_one_crm_user import *
 from .get_one_webhook import *
 from .post_crm_account import *
-from .post_crm_call import *
 from .post_crm_contact import *
 from .post_crm_deal import *
 from .post_crm_email import *
 from .post_crm_event import *
 from .post_crm_event_attendee import *
 from .post_crm_lead import *
 from .post_crm_note import *
 from .post_crm_passthrough import *
 from .post_crm_task import *
 from .post_link_exchange import *
 from .post_link_token import *
 from .post_webhook import *
 from .put_crm_account import *
-from .put_crm_call import *
 from .put_crm_contact import *
 from .put_crm_deal import *
 from .put_crm_email import *
 from .put_crm_event import *
 from .put_crm_event_attendee import *
 from .put_crm_lead import *
 from .put_crm_note import *
 from .put_crm_task import *
 from .search_crm_accounts import *
-from .search_crm_calls import *
 from .search_crm_contacts import *
 from .search_crm_deals import *
 from .search_crm_emails import *
 from .search_crm_event_attendees import *
 from .search_crm_events import *
 from .search_crm_leads import *
 from .search_crm_notes import *
 from .search_crm_tasks import *
 from .search_crm_users import *
 
-__all__ = ["DeleteConnectionRequestBody","DeleteConnectionResponse","DeleteConnectionSecurity","DeleteWebhookRequestBody","DeleteWebhookResponse","GetAllCrmAccountsRequest","GetAllCrmAccountsResponse","GetAllCrmAccountsResponseBody","GetAllCrmCallsRequest","GetAllCrmCallsResponse","GetAllCrmCallsResponseBody","GetAllCrmConnectionsResponse","GetAllCrmConnectionsResponseBody","GetAllCrmContactsRequest","GetAllCrmContactsResponse","GetAllCrmContactsResponseBody","GetAllCrmDealsRequest","GetAllCrmDealsResponse","GetAllCrmDealsResponseBody","GetAllCrmEmailsRequest","GetAllCrmEmailsResponse","GetAllCrmEmailsResponseBody","GetAllCrmEventAttendeesRequest","GetAllCrmEventAttendeesResponse","GetAllCrmEventAttendeesResponseBody","GetAllCrmEventsRequest","GetAllCrmEventsResponse","GetAllCrmEventsResponseBody","GetAllCrmIntegrationsResponse","GetAllCrmIntegrationsResponseBody","GetAllCrmLeadsRequest","GetAllCrmLeadsResponse","GetAllCrmLeadsResponseBody","GetAllCrmNotesRequest","GetAllCrmNotesResponse","GetAllCrmNotesResponseBody","GetAllCrmTasksRequest","GetAllCrmTasksResponse","GetAllCrmTasksResponseBody","GetAllCrmUsersRequest","GetAllCrmUsersResponse","GetAllCrmUsersResponseBody","GetBatchCrmAccountRequest","GetBatchCrmAccountResponse","GetBatchCrmAccountResponseBody","GetBatchCrmCallRequestBody","GetBatchCrmCallResponse","GetBatchCrmCallResponseBody","GetBatchCrmContactRequest","GetBatchCrmContactResponse","GetBatchCrmContactResponseBody","GetBatchCrmDealRequest","GetBatchCrmDealResponse","GetBatchCrmDealResponseBody","GetBatchCrmEmailRequest","GetBatchCrmEmailResponse","GetBatchCrmEmailResponseBody","GetBatchCrmEventAttendeeRequest","GetBatchCrmEventAttendeeResponse","GetBatchCrmEventAttendeeResponseBody","GetBatchCrmEventRequest","GetBatchCrmEventResponse","GetBatchCrmEventResponseBody","GetBatchCrmLeadRequest","GetBatchCrmLeadResponse","GetBatchCrmLeadResponseBody","GetBatchCrmNoteRequest","GetBatchCrmNoteResponse","GetBatchCrmNoteResponseBody","GetBatchCrmTaskRequest","GetBatchCrmTaskResponse","GetBatchCrmTaskResponseBody","GetBatchCrmUserRequest","GetBatchCrmUserResponse","GetBatchCrmUserResponseBody","GetDetailsCrmAccountRequest","GetDetailsCrmAccountResponse","GetDetailsCrmAccountResponseBody","GetDetailsCrmCallRequest","GetDetailsCrmCallResponse","GetDetailsCrmCallResponseBody","GetDetailsCrmContactRequest","GetDetailsCrmContactResponse","GetDetailsCrmContactResponseBody","GetDetailsCrmDealRequest","GetDetailsCrmDealResponse","GetDetailsCrmDealResponseBody","GetDetailsCrmEmailRequest","GetDetailsCrmEmailResponse","GetDetailsCrmEmailResponseBody","GetDetailsCrmEventAttendeeRequest","GetDetailsCrmEventAttendeeResponse","GetDetailsCrmEventAttendeeResponseBody","GetDetailsCrmEventRequest","GetDetailsCrmEventResponse","GetDetailsCrmEventResponseBody","GetDetailsCrmLeadRequest","GetDetailsCrmLeadResponse","GetDetailsCrmLeadResponseBody","GetDetailsCrmNoteRequest","GetDetailsCrmNoteResponse","GetDetailsCrmNoteResponseBody","GetDetailsCrmTaskRequest","GetDetailsCrmTaskResponse","GetDetailsCrmTaskResponseBody","GetDetailsCrmUserRequest","GetDetailsCrmUserResponse","GetDetailsCrmUserResponseBody","GetOneConnectionRequest","GetOneConnectionResponse","GetOneConnectionResponseBody","GetOneCrmAccountRequest","GetOneCrmAccountResponse","GetOneCrmAccountResponseBody","GetOneCrmCallRequest","GetOneCrmCallResponse","GetOneCrmCallResponseBody","GetOneCrmContactRequest","GetOneCrmContactResponse","GetOneCrmContactResponseBody","GetOneCrmDealRequest","GetOneCrmDealResponse","GetOneCrmDealResponseBody","GetOneCrmEmailRequest","GetOneCrmEmailResponse","GetOneCrmEmailResponseBody","GetOneCrmEventAttendeeRequest","GetOneCrmEventAttendeeResponse","GetOneCrmEventAttendeeResponseBody","GetOneCrmEventRequest","GetOneCrmEventResponse","GetOneCrmEventResponseBody","GetOneCrmLeadRequest","GetOneCrmLeadResponse","GetOneCrmLeadResponseBody","GetOneCrmNoteRequest","GetOneCrmNoteResponse","GetOneCrmNoteResponseBody","GetOneCrmTaskRequest","GetOneCrmTaskResponse","GetOneCrmTaskResponseBody","GetOneCrmUserRequest","GetOneCrmUserResponse","GetOneCrmUserResponseBody","GetOneWebhookRequest","GetOneWebhookResponse","GetOneWebhookResponseBody","PostCrmAccountRequestBody","PostCrmAccountResponse","PostCrmAccountResponseBody","PostCrmCallRequestBody","PostCrmCallResponse","PostCrmCallResponseBody","PostCrmContactRequestBody","PostCrmContactResponse","PostCrmContactResponseBody","PostCrmDealRequestBody","PostCrmDealResponse","PostCrmDealResponseBody","PostCrmEmailRequestBody","PostCrmEmailResponse","PostCrmEmailResponseBody","PostCrmEventAttendeeResponse","PostCrmEventAttendeeResponseBody","PostCrmEventRequestBody","PostCrmEventResponse","PostCrmEventResponseBody","PostCrmLeadRequestBody","PostCrmLeadResponse","PostCrmLeadResponseBody","PostCrmNoteRequestBody","PostCrmNoteResponse","PostCrmNoteResponseBody","PostCrmPassthroughRequestBody","PostCrmPassthroughRequestBodyBody","PostCrmPassthroughRequestBodyMethod","PostCrmPassthroughRequestBodyQuery","PostCrmPassthroughResponse","PostCrmPassthroughResponseBody","PostCrmPassthroughResponseBodyHeaders","PostCrmTaskRequestBody","PostCrmTaskResponse","PostCrmTaskResponseBody","PostLinkExchangeRequestBody","PostLinkExchangeResponse","PostLinkExchangeResponseBody","PostLinkExchangeResponseBodyIntegrationID","PostLinkExchangeSecurity","PostLinkTokenResponse","PostLinkTokenResponseBody","PostLinkTokenSecurity","PostWebhookRequestBody","PostWebhookResponse","PostWebhookResponseBody","PutCrmAccountRequestBody","PutCrmAccountResponse","PutCrmAccountResponseBody","PutCrmCallRequestBody","PutCrmCallResponse","PutCrmCallResponseBody","PutCrmContactRequestBody","PutCrmContactResponse","PutCrmContactResponseBody","PutCrmDealRequestBody","PutCrmDealResponse","PutCrmDealResponseBody","PutCrmEmailRequestBody","PutCrmEmailResponse","PutCrmEmailResponseBody","PutCrmEventAttendeeResponse","PutCrmEventAttendeeResponseBody","PutCrmEventRequestBody","PutCrmEventResponse","PutCrmEventResponseBody","PutCrmLeadRequestBody","PutCrmLeadResponse","PutCrmLeadResponseBody","PutCrmNoteRequestBody","PutCrmNoteResponse","PutCrmNoteResponseBody","PutCrmTaskRequestBody","PutCrmTaskResponse","PutCrmTaskResponseBody","SearchCrmAccountsRequest","SearchCrmAccountsRequestBody","SearchCrmAccountsRequestBodyFilters","SearchCrmAccountsResponse","SearchCrmAccountsResponseBody","SearchCrmCallsRequest","SearchCrmCallsRequestBody","SearchCrmCallsRequestBodyFilters","SearchCrmCallsResponse","SearchCrmCallsResponseBody","SearchCrmContactsRequest","SearchCrmContactsRequestBody","SearchCrmContactsRequestBodyFilters","SearchCrmContactsResponse","SearchCrmContactsResponseBody","SearchCrmDealsRequest","SearchCrmDealsRequestBody","SearchCrmDealsRequestBodyFilters","SearchCrmDealsResponse","SearchCrmDealsResponseBody","SearchCrmEmailsRequest","SearchCrmEmailsRequestBody","SearchCrmEmailsRequestBodyFilters","SearchCrmEmailsResponse","SearchCrmEmailsResponseBody","SearchCrmEventAttendeesRequest","SearchCrmEventAttendeesRequestBody","SearchCrmEventAttendeesRequestBodyFilters","SearchCrmEventAttendeesResponse","SearchCrmEventAttendeesResponseBody","SearchCrmEventsRequest","SearchCrmEventsRequestBody","SearchCrmEventsRequestBodyFilters","SearchCrmEventsResponse","SearchCrmEventsResponseBody","SearchCrmLeadsRequest","SearchCrmLeadsRequestBody","SearchCrmLeadsRequestBodyFilters","SearchCrmLeadsResponse","SearchCrmLeadsResponseBody","SearchCrmNotesRequest","SearchCrmNotesRequestBody","SearchCrmNotesRequestBodyFilters","SearchCrmNotesResponse","SearchCrmNotesResponseBody","SearchCrmTasksRequest","SearchCrmTasksRequestBody","SearchCrmTasksRequestBodyFilters","SearchCrmTasksResponse","SearchCrmTasksResponseBody","SearchCrmUsersRequest","SearchCrmUsersRequestBody","SearchCrmUsersRequestBodyFilters","SearchCrmUsersResponse","SearchCrmUsersResponseBody"]
+__all__ = ["DeleteConnectionRequest","DeleteConnectionRequestBody","DeleteConnectionResponse","DeleteConnectionSecurity","DeleteWebhookRequest","DeleteWebhookRequestBody","DeleteWebhookResponse","GetAllCrmAccountsQueryParams","GetAllCrmAccountsRequest","GetAllCrmAccountsResponse","GetAllCrmAccountsResponseBody","GetAllCrmConnectionsResponse","GetAllCrmConnectionsResponseBody","GetAllCrmContactsQueryParams","GetAllCrmContactsRequest","GetAllCrmContactsResponse","GetAllCrmContactsResponseBody","GetAllCrmDealsQueryParams","GetAllCrmDealsRequest","GetAllCrmDealsResponse","GetAllCrmDealsResponseBody","GetAllCrmEmailsQueryParams","GetAllCrmEmailsRequest","GetAllCrmEmailsResponse","GetAllCrmEmailsResponseBody","GetAllCrmEventAttendeesQueryParams","GetAllCrmEventAttendeesRequest","GetAllCrmEventAttendeesResponse","GetAllCrmEventAttendeesResponseBody","GetAllCrmEventsQueryParams","GetAllCrmEventsRequest","GetAllCrmEventsResponse","GetAllCrmEventsResponseBody","GetAllCrmIntegrationsResponse","GetAllCrmIntegrationsResponseBody","GetAllCrmLeadsQueryParams","GetAllCrmLeadsRequest","GetAllCrmLeadsResponse","GetAllCrmLeadsResponseBody","GetAllCrmNotesQueryParams","GetAllCrmNotesRequest","GetAllCrmNotesResponse","GetAllCrmNotesResponseBody","GetAllCrmTasksQueryParams","GetAllCrmTasksRequest","GetAllCrmTasksResponse","GetAllCrmTasksResponseBody","GetAllCrmUsersQueryParams","GetAllCrmUsersRequest","GetAllCrmUsersResponse","GetAllCrmUsersResponseBody","GetBatchCrmAccountQueryParams","GetBatchCrmAccountRequest","GetBatchCrmAccountResponse","GetBatchCrmAccountResponseBody","GetBatchCrmContactQueryParams","GetBatchCrmContactRequest","GetBatchCrmContactResponse","GetBatchCrmContactResponseBody","GetBatchCrmDealQueryParams","GetBatchCrmDealRequest","GetBatchCrmDealResponse","GetBatchCrmDealResponseBody","GetBatchCrmEmailQueryParams","GetBatchCrmEmailRequest","GetBatchCrmEmailResponse","GetBatchCrmEmailResponseBody","GetBatchCrmEventAttendeeQueryParams","GetBatchCrmEventAttendeeRequest","GetBatchCrmEventAttendeeResponse","GetBatchCrmEventAttendeeResponseBody","GetBatchCrmEventQueryParams","GetBatchCrmEventRequest","GetBatchCrmEventResponse","GetBatchCrmEventResponseBody","GetBatchCrmLeadQueryParams","GetBatchCrmLeadRequest","GetBatchCrmLeadResponse","GetBatchCrmLeadResponseBody","GetBatchCrmNoteQueryParams","GetBatchCrmNoteRequest","GetBatchCrmNoteResponse","GetBatchCrmNoteResponseBody","GetBatchCrmTaskQueryParams","GetBatchCrmTaskRequest","GetBatchCrmTaskResponse","GetBatchCrmTaskResponseBody","GetBatchCrmUserQueryParams","GetBatchCrmUserRequest","GetBatchCrmUserResponse","GetBatchCrmUserResponseBody","GetDetailsCrmAccountQueryParams","GetDetailsCrmAccountRequest","GetDetailsCrmAccountResponse","GetDetailsCrmAccountResponseBody","GetDetailsCrmContactQueryParams","GetDetailsCrmContactRequest","GetDetailsCrmContactResponse","GetDetailsCrmContactResponseBody","GetDetailsCrmDealQueryParams","GetDetailsCrmDealRequest","GetDetailsCrmDealResponse","GetDetailsCrmDealResponseBody","GetDetailsCrmEmailQueryParams","GetDetailsCrmEmailRequest","GetDetailsCrmEmailResponse","GetDetailsCrmEmailResponseBody","GetDetailsCrmEventAttendeeQueryParams","GetDetailsCrmEventAttendeeRequest","GetDetailsCrmEventAttendeeResponse","GetDetailsCrmEventAttendeeResponseBody","GetDetailsCrmEventQueryParams","GetDetailsCrmEventRequest","GetDetailsCrmEventResponse","GetDetailsCrmEventResponseBody","GetDetailsCrmLeadQueryParams","GetDetailsCrmLeadRequest","GetDetailsCrmLeadResponse","GetDetailsCrmLeadResponseBody","GetDetailsCrmNoteQueryParams","GetDetailsCrmNoteRequest","GetDetailsCrmNoteResponse","GetDetailsCrmNoteResponseBody","GetDetailsCrmTaskQueryParams","GetDetailsCrmTaskRequest","GetDetailsCrmTaskResponse","GetDetailsCrmTaskResponseBody","GetDetailsCrmUserQueryParams","GetDetailsCrmUserRequest","GetDetailsCrmUserResponse","GetDetailsCrmUserResponseBody","GetOneConnectionQueryParams","GetOneConnectionRequest","GetOneConnectionResponse","GetOneConnectionResponseBody","GetOneCrmAccountQueryParams","GetOneCrmAccountRequest","GetOneCrmAccountResponse","GetOneCrmAccountResponseBody","GetOneCrmContactQueryParams","GetOneCrmContactRequest","GetOneCrmContactResponse","GetOneCrmContactResponseBody","GetOneCrmDealQueryParams","GetOneCrmDealRequest","GetOneCrmDealResponse","GetOneCrmDealResponseBody","GetOneCrmEmailQueryParams","GetOneCrmEmailRequest","GetOneCrmEmailResponse","GetOneCrmEmailResponseBody","GetOneCrmEventAttendeeQueryParams","GetOneCrmEventAttendeeRequest","GetOneCrmEventAttendeeResponse","GetOneCrmEventAttendeeResponseBody","GetOneCrmEventQueryParams","GetOneCrmEventRequest","GetOneCrmEventResponse","GetOneCrmEventResponseBody","GetOneCrmLeadQueryParams","GetOneCrmLeadRequest","GetOneCrmLeadResponse","GetOneCrmLeadResponseBody","GetOneCrmNoteQueryParams","GetOneCrmNoteRequest","GetOneCrmNoteResponse","GetOneCrmNoteResponseBody","GetOneCrmTaskQueryParams","GetOneCrmTaskRequest","GetOneCrmTaskResponse","GetOneCrmTaskResponseBody","GetOneCrmUserQueryParams","GetOneCrmUserRequest","GetOneCrmUserResponse","GetOneCrmUserResponseBody","GetOneWebhookQueryParams","GetOneWebhookRequest","GetOneWebhookResponse","GetOneWebhookResponseBody","PostCrmAccountRequest","PostCrmAccountRequestBody","PostCrmAccountResponse","PostCrmAccountResponseBody","PostCrmContactRequest","PostCrmContactRequestBody","PostCrmContactResponse","PostCrmContactResponseBody","PostCrmDealRequest","PostCrmDealRequestBody","PostCrmDealResponse","PostCrmDealResponseBody","PostCrmEmailRequest","PostCrmEmailRequestBody","PostCrmEmailResponse","PostCrmEmailResponseBody","PostCrmEventAttendeeResponse","PostCrmEventAttendeeResponseBody","PostCrmEventRequest","PostCrmEventRequestBody","PostCrmEventResponse","PostCrmEventResponseBody","PostCrmLeadRequest","PostCrmLeadRequestBody","PostCrmLeadResponse","PostCrmLeadResponseBody","PostCrmNoteRequest","PostCrmNoteRequestBody","PostCrmNoteResponse","PostCrmNoteResponseBody","PostCrmPassthroughRequest","PostCrmPassthroughRequestBody","PostCrmPassthroughRequestBodyMethodEnum","PostCrmPassthroughResponse","PostCrmPassthroughResponseBody","PostCrmTaskRequest","PostCrmTaskRequestBody","PostCrmTaskResponse","PostCrmTaskResponseBody","PostLinkExchangeRequest","PostLinkExchangeRequestBody","PostLinkExchangeResponse","PostLinkExchangeResponseBody","PostLinkExchangeResponseBodyIntegrationIDEnum","PostLinkExchangeSecurity","PostLinkTokenRequest","PostLinkTokenResponse","PostLinkTokenResponseBody","PostLinkTokenSecurity","PostWebhookRequest","PostWebhookRequestBody","PostWebhookResponse","PostWebhookResponseBody","PutCrmAccountRequest","PutCrmAccountRequestBody","PutCrmAccountResponse","PutCrmAccountResponseBody","PutCrmContactRequest","PutCrmContactRequestBody","PutCrmContactResponse","PutCrmContactResponseBody","PutCrmDealRequest","PutCrmDealRequestBody","PutCrmDealResponse","PutCrmDealResponseBody","PutCrmEmailRequest","PutCrmEmailRequestBody","PutCrmEmailResponse","PutCrmEmailResponseBody","PutCrmEventAttendeeResponse","PutCrmEventAttendeeResponseBody","PutCrmEventRequest","PutCrmEventRequestBody","PutCrmEventResponse","PutCrmEventResponseBody","PutCrmLeadRequest","PutCrmLeadRequestBody","PutCrmLeadResponse","PutCrmLeadResponseBody","PutCrmNoteRequest","PutCrmNoteRequestBody","PutCrmNoteResponse","PutCrmNoteResponseBody","PutCrmTaskRequest","PutCrmTaskRequestBody","PutCrmTaskResponse","PutCrmTaskResponseBody","SearchCrmAccountsQueryParams","SearchCrmAccountsRequest","SearchCrmAccountsRequestBody","SearchCrmAccountsRequestBodyFilters","SearchCrmAccountsResponse","SearchCrmAccountsResponseBody","SearchCrmContactsQueryParams","SearchCrmContactsRequest","SearchCrmContactsRequestBody","SearchCrmContactsRequestBodyFilters","SearchCrmContactsResponse","SearchCrmContactsResponseBody","SearchCrmDealsQueryParams","SearchCrmDealsRequest","SearchCrmDealsRequestBody","SearchCrmDealsRequestBodyFilters","SearchCrmDealsResponse","SearchCrmDealsResponseBody","SearchCrmEmailsQueryParams","SearchCrmEmailsRequest","SearchCrmEmailsRequestBody","SearchCrmEmailsRequestBodyFilters","SearchCrmEmailsResponse","SearchCrmEmailsResponseBody","SearchCrmEventAttendeesQueryParams","SearchCrmEventAttendeesRequest","SearchCrmEventAttendeesRequestBody","SearchCrmEventAttendeesRequestBodyFilters","SearchCrmEventAttendeesResponse","SearchCrmEventAttendeesResponseBody","SearchCrmEventsQueryParams","SearchCrmEventsRequest","SearchCrmEventsRequestBody","SearchCrmEventsRequestBodyFilters","SearchCrmEventsResponse","SearchCrmEventsResponseBody","SearchCrmLeadsQueryParams","SearchCrmLeadsRequest","SearchCrmLeadsRequestBody","SearchCrmLeadsRequestBodyFilters","SearchCrmLeadsResponse","SearchCrmLeadsResponseBody","SearchCrmNotesQueryParams","SearchCrmNotesRequest","SearchCrmNotesRequestBody","SearchCrmNotesRequestBodyFilters","SearchCrmNotesResponse","SearchCrmNotesResponseBody","SearchCrmTasksQueryParams","SearchCrmTasksRequest","SearchCrmTasksRequestBody","SearchCrmTasksRequestBodyFilters","SearchCrmTasksResponse","SearchCrmTasksResponseBody","SearchCrmUsersQueryParams","SearchCrmUsersRequest","SearchCrmUsersRequestBody","SearchCrmUsersRequestBodyFilters","SearchCrmUsersResponse","SearchCrmUsersResponseBody"]
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/delete_connection.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_deal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import dealcreate as shared_dealcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DeleteConnectionSecurity:
-    vessel_api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header', 'field_name': 'vessel-api-token' }})
+class PostCrmDealRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    deal: shared_dealcreate.DealCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
     
 
-
+@dataclasses.dataclass
+class PostCrmDealRequest:
+    request: Optional[PostCrmDealRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class DeleteConnectionRequestBody:
-    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
+class PostCrmDealResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class DeleteConnectionResponse:
+class PostCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+    response_body: Optional[PostCrmDealResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/delete_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/delete_webhook.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class DeleteWebhookRequestBody:
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
     webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
     
 
-
-
+@dataclasses.dataclass
+class DeleteWebhookRequest:
+    request: Optional[DeleteWebhookRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclasses.dataclass
 class DeleteWebhookResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_accounts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_users.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import account as shared_account
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmAccountsRequest:
+class GetAllCrmUsersQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetAllCrmUsersRequest:
+    query_params: GetAllCrmUsersQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmAccountsResponseBody:
-    r"""OK"""
-    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+class GetAllCrmUsersResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmAccountsResponse:
+class GetAllCrmUsersResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmAccountsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmUsersResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_calls.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import call as shared_call
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmCallsRequest:
+class GetDetailsCrmEventQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmEventRequest:
+    query_params: GetDetailsCrmEventQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmCallsResponseBody:
-    r"""OK"""
-    calls: Optional[list[shared_call.Call]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('calls'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmEventResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmCallsResponse:
+class GetDetailsCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmCallsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmEventResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_connections.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_note.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import connection as shared_connection
+from ..shared import notecreate as shared_notecreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmConnectionsResponseBody:
-    r"""OK"""
-    connections: Optional[list[shared_connection.Connection]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connections'), 'exclude': lambda f: f is None }})
+class PostCrmNoteRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    note: shared_notecreate.NoteCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
     
 
+@dataclasses.dataclass
+class PostCrmNoteRequest:
+    request: Optional[PostCrmNoteRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PostCrmNoteResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    
 
 @dataclasses.dataclass
-class GetAllCrmConnectionsResponse:
+class PostCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmConnectionsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostCrmNoteResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_contacts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import contact as shared_contact
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmContactsRequest:
+class GetAllCrmTasksQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetAllCrmTasksRequest:
+    query_params: GetAllCrmTasksQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmContactsResponseBody:
-    r"""OK"""
-    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
+class GetAllCrmTasksResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmContactsResponse:
+class GetAllCrmTasksResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmContactsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmTasksResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_deals.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_deals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import deal as shared_deal
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmDealsRequest:
+class GetAllCrmDealsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetAllCrmDealsRequest:
+    query_params: GetAllCrmDealsQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetAllCrmDealsResponseBody:
-    r"""OK"""
     deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class GetAllCrmDealsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmDealsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_emails.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_event_attendees.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import email as shared_email
+from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmEmailsRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
+class GetAllCrmEventAttendeesQueryParams:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetAllCrmEventAttendeesRequest:
+    query_params: GetAllCrmEventAttendeesQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmEmailsResponseBody:
-    r"""OK"""
-    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+class GetAllCrmEventAttendeesResponseBody:
+    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmEmailsResponse:
+class GetAllCrmEventAttendeesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmEmailsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmEventAttendeesResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_event_attendees.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_event_attendee.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventattendee as shared_eventattendee
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmEventAttendeesRequest:
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
+class GetDetailsCrmEventAttendeeQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmEventAttendeeRequest:
+    query_params: GetDetailsCrmEventAttendeeQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmEventAttendeesResponseBody:
-    r"""OK"""
-    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmEventAttendeeResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmEventAttendeesResponse:
+class GetDetailsCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmEventAttendeesResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_events.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/datefilter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class GetAllCrmEventsRequest:
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmEventsResponseBody:
-    r"""OK"""
-    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    
-
-
-
-
-@dataclasses.dataclass
-class GetAllCrmEventsResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmEventsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+class DateFilter:
+    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    gt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
+    gte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
+    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
+    lt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
+    lte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
+    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_integrations.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_integrations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import integration as shared_integration
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetAllCrmIntegrationsResponseBody:
-    r"""OK"""
     integrations: Optional[list[shared_integration.Integration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrations'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class GetAllCrmIntegrationsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetAllCrmIntegrationsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_leads.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_note.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import lead as shared_lead
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmLeadsRequest:
+class GetDetailsCrmNoteQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmNoteRequest:
+    query_params: GetDetailsCrmNoteQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmLeadsResponseBody:
-    r"""OK"""
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmNoteResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmLeadsResponse:
+class GetDetailsCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmLeadsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmNoteResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_notes.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_leads.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import note as shared_note
+from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmNotesRequest:
+class GetAllCrmLeadsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetAllCrmLeadsRequest:
+    query_params: GetAllCrmLeadsQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmNotesResponseBody:
-    r"""OK"""
+class GetAllCrmLeadsResponseBody:
+    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmNotesResponse:
+class GetAllCrmLeadsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmNotesResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmLeadsResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_tasks.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_notes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import task as shared_task
+from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmTasksRequest:
+class GetAllCrmNotesQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetAllCrmNotesRequest:
+    query_params: GetAllCrmNotesQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmTasksResponseBody:
-    r"""OK"""
+class GetAllCrmNotesResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
+    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmTasksResponse:
+class GetAllCrmNotesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmTasksResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmNotesResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_all_crm_users.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import user as shared_user
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetAllCrmUsersRequest:
+class GetDetailsCrmUserQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmUserRequest:
+    query_params: GetDetailsCrmUserQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetAllCrmUsersResponseBody:
-    r"""OK"""
+class GetDetailsCrmUserResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetAllCrmUsersResponse:
+class GetDetailsCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetAllCrmUsersResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmUserResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_contact.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import account as shared_account
+from ..shared import contact as shared_contact
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetBatchCrmAccountRequest:
+class GetBatchCrmContactQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Account Id's."""
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmContactRequest:
+    query_params: GetBatchCrmContactQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmAccountResponseBody:
-    r"""OK"""
-    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+class GetBatchCrmContactResponseBody:
+    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
     invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
     
 
-
-
-
 @dataclasses.dataclass
-class GetBatchCrmAccountResponse:
+class GetBatchCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmContactResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/note.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,32 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import call as shared_call
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmCallRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ids') }})
-    r"""List of call Ids."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('allFields'), 'exclude': lambda f: f is None }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+class NoteAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
-@dataclasses.dataclass
-class GetBatchCrmCallResponseBody:
-    r"""OK"""
-    calls: Optional[list[shared_call.Call]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('calls'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    
-
-
-
-
 @dataclasses.dataclass
-class GetBatchCrmCallResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
+class Note:
+    r"""Note
+    A Note attached to some CRM Object. 
+    """
     
-
+    associations: NoteAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_deal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import contact as shared_contact
+from ..shared import deal as shared_deal
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetBatchCrmContactRequest:
+class GetBatchCrmDealQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Contact Id's."""
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmDealRequest:
+    query_params: GetBatchCrmDealQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmContactResponseBody:
-    r"""OK"""
-    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
+class GetBatchCrmDealResponseBody:
+    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
     invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
     
 
-
-
-
 @dataclasses.dataclass
-class GetBatchCrmContactResponse:
+class GetBatchCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmContactResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmDealResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_emails.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import deal as shared_deal
+from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetBatchCrmDealRequest:
+class GetAllCrmEmailsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Deal Id's."""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetAllCrmEmailsRequest:
+    query_params: GetAllCrmEmailsQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmDealResponseBody:
-    r"""OK"""
-    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
+class GetAllCrmEmailsResponseBody:
+    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetBatchCrmDealResponse:
+class GetAllCrmEmailsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmEmailsResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_lead.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import email as shared_email
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetBatchCrmEmailRequest:
+class GetDetailsCrmLeadQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Email Id's."""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmLeadRequest:
+    query_params: GetDetailsCrmLeadQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmEmailResponseBody:
-    r"""OK"""
-    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
+class GetDetailsCrmLeadResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetBatchCrmEmailResponse:
+class GetDetailsCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmEmailResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmLeadResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventupdate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,20 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class GetBatchCrmEventAttendeeRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Event Attendee Id's."""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmEventAttendeeResponseBody:
-    r"""OK"""
-    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    
-
-
-
-
-@dataclasses.dataclass
-class GetBatchCrmEventAttendeeResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+class EventUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_task.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import lead as shared_lead
+from ..shared import taskupdate as shared_taskupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBatchCrmLeadRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Lead Id's."""
+class PutCrmTaskRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    task: Optional[shared_taskupdate.TaskUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PutCrmTaskRequest:
+    request: Optional[PutCrmTaskRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmLeadResponseBody:
-    r"""OK"""
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
+class PutCrmTaskResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetBatchCrmLeadResponse:
+class PutCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PutCrmTaskResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_email.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import note as shared_note
+from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetBatchCrmNoteRequest:
+class GetDetailsCrmEmailQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Note Id's."""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmEmailRequest:
+    query_params: GetDetailsCrmEmailQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmNoteResponseBody:
-    r"""OK"""
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmEmailResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetBatchCrmNoteResponse:
+class GetDetailsCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmEmailResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetBatchCrmTaskRequest:
+class GetBatchCrmTaskQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of Task Id's."""
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmTaskRequest:
+    query_params: GetBatchCrmTaskQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetBatchCrmTaskResponseBody:
-    r"""OK"""
     invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
     tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class GetBatchCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetBatchCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_batch_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_contacts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import user as shared_user
+from ..shared import contact as shared_contact
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetBatchCrmUserRequest:
+class GetAllCrmContactsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
-    r"""Comma separated list of User Id's."""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetAllCrmContactsRequest:
+    query_params: GetAllCrmContactsQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetBatchCrmUserResponseBody:
-    r"""OK"""
-    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
-    r"""Ids that didn't return anything. Will be an empty array if all Ids are valid."""
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
+class GetAllCrmContactsResponseBody:
+    contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetBatchCrmUserResponse:
+class GetAllCrmContactsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetBatchCrmUserResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmContactsResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmAccountRequest:
+class GetDetailsCrmTaskQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmTaskRequest:
+    query_params: GetDetailsCrmTaskQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmAccountResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmTaskResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmAccountResponse:
+class GetDetailsCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmTaskResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_contact.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmCallRequest:
+class GetDetailsCrmContactQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmContactRequest:
+    query_params: GetDetailsCrmContactQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmCallResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmContactResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmCallResponse:
+class GetDetailsCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmContactResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_account.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmContactRequest:
+class GetDetailsCrmAccountQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmAccountRequest:
+    query_params: GetDetailsCrmAccountQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmContactResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+class GetDetailsCrmAccountResponseBody:
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmContactResponse:
+class GetDetailsCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmContactResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetDetailsCrmAccountResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_details_crm_deal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmDealRequest:
+class GetDetailsCrmDealQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
     cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    r"""If provided, get the details about a particular deal. If not provided, get details about all deals."""
     
 
-
+@dataclasses.dataclass
+class GetDetailsCrmDealRequest:
+    query_params: GetDetailsCrmDealQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetDetailsCrmDealResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
+    fields: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class GetDetailsCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetDetailsCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_lead.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmEmailRequest:
+class GetOneCrmLeadQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetOneCrmLeadRequest:
+    query_params: GetOneCrmLeadQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmEmailResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetOneCrmLeadResponseBody:
+    lead: Optional[shared_lead.Lead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmEmailResponse:
+class GetOneCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmEmailResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetOneCrmLeadResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_email.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmEventRequest:
+class GetBatchCrmEmailQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmEmailRequest:
+    query_params: GetBatchCrmEmailQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmEventResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetBatchCrmEmailResponseBody:
+    emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmEventResponse:
+class GetBatchCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmEmailResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/leadupdate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import field as shared_field
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class GetDetailsCrmEventAttendeeRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmEventAttendeeResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    
-
-
-
-
-@dataclasses.dataclass
-class GetDetailsCrmEventAttendeeResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+class LeadUpdate:
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event_attendee.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmLeadRequest:
+class GetBatchCrmEventAttendeeQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmEventAttendeeRequest:
+    query_params: GetBatchCrmEventAttendeeQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmLeadResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetBatchCrmEventAttendeeResponseBody:
+    event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmLeadResponse:
+class GetBatchCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_event.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmNoteRequest:
+class GetBatchCrmEventQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmEventRequest:
+    query_params: GetBatchCrmEventQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmNoteResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetBatchCrmEventResponseBody:
+    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmNoteResponse:
+class GetBatchCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmEventResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_contact.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import contact as shared_contact
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmTaskRequest:
+class GetOneCrmContactQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'email', 'style': 'form', 'explode': True }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetOneCrmContactRequest:
+    query_params: GetOneCrmContactQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmTaskResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetOneCrmContactResponseBody:
+    contact: Optional[shared_contact.Contact] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmTaskResponse:
+class GetOneCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetOneCrmContactResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_details_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_email.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import field as shared_field
+from ..shared import email as shared_email
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetDetailsCrmUserRequest:
+class GetOneCrmEmailQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns details about native fields."""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetOneCrmEmailRequest:
+    query_params: GetOneCrmEmailQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetDetailsCrmUserResponseBody:
-    r"""OK"""
-    fields_: Optional[list[shared_field.Field]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+class GetOneCrmEmailResponseBody:
+    email: Optional[shared_email.Email] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetDetailsCrmUserResponse:
+class GetOneCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetDetailsCrmUserResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetOneCrmEmailResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_connection.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import connection as shared_connection
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetOneConnectionRequest:
-    connection_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'connectionId', 'style': 'form', 'explode': True }})
-    r"""The ID of the connection for the customer's CRM account. This was generated when they connected their account."""
+class GetOneCrmUserQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetOneCrmUserRequest:
+    query_params: GetOneCrmUserQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetOneConnectionResponseBody:
-    r"""OK"""
-    connection: Optional[shared_connection.Connection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connection'), 'exclude': lambda f: f is None }})
+class GetOneCrmUserResponseBody:
+    user: Optional[shared_user.User] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetOneConnectionResponse:
+class GetOneCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneConnectionResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetOneCrmUserResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_task.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import account as shared_account
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetOneCrmAccountRequest:
+class GetOneCrmTaskQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     
 
-
+@dataclasses.dataclass
+class GetOneCrmTaskRequest:
+    query_params: GetOneCrmTaskQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetOneCrmAccountResponseBody:
-    r"""OK"""
-    account: Optional[shared_account.Account] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
-    r"""(Alias: company, organization) An organization involved with your business."""
+class GetOneCrmTaskResponseBody:
+    task: Optional[shared_task.Task] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetOneCrmAccountResponse:
+class GetOneCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetOneCrmTaskResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_webhook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,33 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import deal as shared_deal
+from ..shared import webhookmetadata as shared_webhookmetadata
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetOneCrmDealRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+class GetOneWebhookQueryParams:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'webhookId', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetOneWebhookRequest:
+    query_params: GetOneWebhookQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetOneCrmDealResponseBody:
-    r"""OK"""
-    deal: Optional[shared_deal.Deal] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal'), 'exclude': lambda f: f is None }})
-    r"""(Alias: Opportunity) An object representing either the opportunity to sell a product to an Account, or in the case of an `isWon` deal, a product sold to an Account.
-    *CRM Caveats*:
-    - Pipedrive: Users must have \"Deal probability\" turned on for the given pipeline for probability to be configurable and returned.
-    """
+class GetOneWebhookResponseBody:
+    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetOneCrmDealResponse:
+class GetOneWebhookResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetOneWebhookResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetOneCrmEventRequest:
+class GetOneCrmEventQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     
 
-
+@dataclasses.dataclass
+class GetOneCrmEventRequest:
+    query_params: GetOneCrmEventQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetOneCrmEventResponseBody:
-    r"""OK"""
     event: Optional[shared_event.Event] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
-    r"""Events are a type of activity that has attendees and takes place at a certain point in time (i.e., has a start and end date).
-    For the currently supported CRMs, these are the objects Events most closely maps to:
-    - Salesforce = Events
-    - HubSpot = Meetings
-    - Pipedrive = Activities
-    """
     
 
-
-
-
 @dataclasses.dataclass
 class GetOneCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetOneCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/eventcreate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,24 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class GetOneCrmEventAttendeeRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetOneCrmEventAttendeeResponseBody:
-    r"""OK"""
-    event_attendee: Optional[shared_eventattendee.EventAttendee] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
-    r"""Event Attendees hold information about someone who attendeed or was invited to an event. Attendees are always associated with some Event and another person object such as a Contact, Lead, or Other."""
-    
-
-
-
-
-@dataclasses.dataclass
-class GetOneCrmEventAttendeeResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+class EventCreate:
+    end_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime') }})
+    start_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
+    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/taskupdate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class GetOneCrmLeadRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetOneCrmLeadResponseBody:
-    r"""OK"""
-    lead: Optional[shared_lead.Lead] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
-    r"""A Lead represents an individual, or sometimes an organization, that is interested in purchasing your product (i.e., is a potential Deal).
-    *CRM Caveats*:
-    - HubSpot: we consider contacts with the `leadStatus` set to be leads.
-    """
-    
-
-
-
-
-@dataclasses.dataclass
-class GetOneCrmLeadResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+class TaskUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_note.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetOneCrmNoteRequest:
+class GetOneCrmNoteQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
     id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
     
 
-
+@dataclasses.dataclass
+class GetOneCrmNoteRequest:
+    query_params: GetOneCrmNoteQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class GetOneCrmNoteResponseBody:
-    r"""OK"""
     note: Optional[shared_note.Note] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note'), 'exclude': lambda f: f is None }})
-    r"""A Note attached to some CRM Object."""
     
 
-
-
-
 @dataclasses.dataclass
 class GetOneCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[GetOneCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_events.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import task as shared_task
+from ..shared import event as shared_event
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetOneCrmTaskRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+class GetAllCrmEventsQueryParams:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetAllCrmEventsRequest:
+    query_params: GetAllCrmEventsQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetOneCrmTaskResponseBody:
-    r"""OK"""
-    task: Optional[shared_task.Task] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
-    r"""A task attached to some CRM object"""
+class GetAllCrmEventsResponseBody:
+    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetOneCrmTaskResponse:
+class GetAllCrmEventsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmEventsResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_crm_user.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_all_crm_accounts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import user as shared_user
+from ..shared import account as shared_account
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetOneCrmUserRequest:
+class GetAllCrmAccountsQueryParams:
     access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
     all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetAllCrmAccountsRequest:
+    query_params: GetAllCrmAccountsQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetOneCrmUserResponseBody:
-    r"""OK"""
-    user: Optional[shared_user.User] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user'), 'exclude': lambda f: f is None }})
-    r"""Users of the connected CRM platform. These are *not* the contacts or leads, but rather the user accounts from the connected CRM."""
+class GetAllCrmAccountsResponseBody:
+    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetOneCrmUserResponse:
+class GetAllCrmAccountsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneCrmUserResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetAllCrmAccountsResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/get_one_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_event_attendee.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import webhookmetadata as shared_webhookmetadata
+from ..shared import eventattendee as shared_eventattendee
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class GetOneWebhookRequest:
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's CRM account. This was generated when they connected their account."""
-    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'webhookId', 'style': 'form', 'explode': True }})
+class GetOneCrmEventAttendeeQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetOneCrmEventAttendeeRequest:
+    query_params: GetOneCrmEventAttendeeQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class GetOneWebhookResponseBody:
-    r"""OK"""
-    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
+class GetOneCrmEventAttendeeResponseBody:
+    event_attendee: Optional[shared_eventattendee.EventAttendee] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class GetOneWebhookResponse:
+class GetOneCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[GetOneWebhookResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetOneCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_webhook.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import accountcreate as shared_accountcreate
+from ..shared import webhookmetadata as shared_webhookmetadata
+from ..shared import webhookmetadatacreate as shared_webhookmetadatacreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmAccountRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    account: shared_accountcreate.AccountCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
+class PostWebhookRequestBody:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    webhook: Optional[shared_webhookmetadatacreate.WebhookMetadataCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PostWebhookRequest:
+    request: Optional[PostWebhookRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmAccountResponseBody:
-    r"""OK"""
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class PostWebhookResponseBody:
+    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmAccountResponse:
+class PostWebhookResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostWebhookResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_user.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import callcreate as shared_callcreate
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmCallRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    call: Optional[shared_callcreate.CallCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('call'), 'exclude': lambda f: f is None }})
+class GetBatchCrmUserQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmUserRequest:
+    query_params: GetBatchCrmUserQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmCallResponseBody:
-    r"""OK"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class GetBatchCrmUserResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmCallResponse:
+class GetBatchCrmUserResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmUserResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_note.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import contactcreate as shared_contactcreate
+from ..shared import noteupdate as shared_noteupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmContactRequestBody:
+class PutCrmNoteRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    contact: shared_contactcreate.ContactCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
-    r"""Properties that a contact can be created with"""
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    note: shared_noteupdate.NoteUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
     
 
-
+@dataclasses.dataclass
+class PutCrmNoteRequest:
+    request: Optional[PutCrmNoteRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmContactResponseBody:
-    r"""OK"""
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+class PutCrmNoteResponseBody:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmContactResponse:
+class PutCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmContactResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PutCrmNoteResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_email.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import dealcreate as shared_dealcreate
+from ..shared import emailcreate as shared_emailcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmDealRequestBody:
+class PostCrmEmailRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    deal: shared_dealcreate.DealCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
+    email: Optional[shared_emailcreate.EmailCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PostCrmEmailRequest:
+    request: Optional[PostCrmEmailRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmDealResponseBody:
-    r"""OK"""
+class PostCrmEmailResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmDealResponse:
+class PostCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostCrmEmailResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_note.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import emailcreate as shared_emailcreate
+from ..shared import note as shared_note
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmEmailRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    email: Optional[shared_emailcreate.EmailCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+class GetBatchCrmNoteQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmNoteRequest:
+    query_params: GetBatchCrmNoteQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmEmailResponseBody:
-    r"""OK"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class GetBatchCrmNoteResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmEmailResponse:
+class GetBatchCrmNoteResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmEmailResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmNoteResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventcreate as shared_eventcreate
+from ..shared import eventupdate as shared_eventupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmEventRequestBody:
+class PutCrmEventRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    event: Optional[shared_eventcreate.EventCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    event: Optional[shared_eventupdate.EventUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PutCrmEventRequest:
+    request: Optional[PutCrmEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmEventResponseBody:
-    r"""OK"""
+class PutCrmEventResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmEventResponse:
+class PutCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PutCrmEventResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event_attendee.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,23 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import eventattendeecreate as shared_eventattendeecreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PostCrmEventAttendeeResponseBody:
-    r"""OK"""
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
     event_attendee: Optional[shared_eventattendeecreate.EventAttendeeCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class PostCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import leadcreate as shared_leadcreate
+from ..shared import accountcreate as shared_accountcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmLeadRequestBody:
+class PostCrmAccountRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    lead: shared_leadcreate.LeadCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead') }})
+    account: shared_accountcreate.AccountCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
     
 
-
+@dataclasses.dataclass
+class PostCrmAccountRequest:
+    request: Optional[PostCrmAccountRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmLeadResponseBody:
-    r"""OK"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class PostCrmAccountResponseBody:
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmLeadResponse:
+class PostCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostCrmAccountResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_task.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import notecreate as shared_notecreate
+from ..shared import taskcreate as shared_taskcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmNoteRequestBody:
+class PostCrmTaskRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    note: shared_notecreate.NoteCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
-    r"""Create a new Note. You may only associate a note with at most one entity of each type upon creation."""
+    task: Optional[shared_taskcreate.TaskCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PostCrmTaskRequest:
+    request: Optional[PostCrmTaskRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmNoteResponseBody:
-    r"""OK"""
+class PostCrmTaskResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmNoteResponse:
+class PostCrmTaskResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostCrmTaskResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_passthrough.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_users.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,57 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import datefilter as shared_datefilter
+from ..shared import stringfilter as shared_stringfilter
+from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from typing import Any, Optional
+from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
-class PostCrmPassthroughRequestBodyBody:
-    r"""The body of the request."""
+class SearchCrmUsersQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
     
 
-
-class PostCrmPassthroughRequestBodyMethod(str, Enum):
-    GET = 'GET'
-    POST = 'POST'
-    PUT = 'PUT'
-    PATCH = 'PATCH'
-    DELETE = 'DELETE'
-
-
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCrmPassthroughRequestBodyQuery:
-    r"""The query parameters to send with the request as key value pairs. These are appended to the URL when the request is sent to the CRM."""
+class SearchCrmUsersRequestBodyFilters:
+    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmPassthroughRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    method: PostCrmPassthroughRequestBodyMethod = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-    path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('path') }})
-    r"""The path to send the request to. Vessel handles the domain so for a request to Salesforce instead of using `https://mydomain.my.salesforce.com/services/data/v52.0/sobjects/Account` you would use `services/data/v52.0/sobjects/Account`."""
-    body: Optional[PostCrmPassthroughRequestBodyBody] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    r"""The body of the request."""
-    query: Optional[PostCrmPassthroughRequestBodyQuery] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
-    r"""The query parameters to send with the request as key value pairs. These are appended to the URL when the request is sent to the CRM."""
+class SearchCrmUsersRequestBody:
+    filters: Optional[SearchCrmUsersRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmPassthroughResponseBodyHeaders:
-    pass
-
+class SearchCrmUsersRequest:
+    query_params: SearchCrmUsersQueryParams = dataclasses.field()
+    request: Optional[SearchCrmUsersRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmPassthroughResponseBody:
-    r"""OK"""
-    body: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    headers: Optional[PostCrmPassthroughResponseBodyHeaders] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('headers'), 'exclude': lambda f: f is None }})
-    status_code: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
-    r"""The HTTP status code of the response from the downstream CRM."""
-    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
-    r"""The full URL that the request was sent to."""
+class SearchCrmUsersResponseBody:
+    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmPassthroughResponse:
+class SearchCrmUsersResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmPassthroughResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[SearchCrmUsersResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_lead.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import taskcreate as shared_taskcreate
+from ..shared import lead as shared_lead
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmTaskRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    task: Optional[shared_taskcreate.TaskCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
+class GetBatchCrmLeadQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmLeadRequest:
+    query_params: GetBatchCrmLeadQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostCrmTaskResponseBody:
-    r"""OK"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class GetBatchCrmLeadResponseBody:
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
+    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostCrmTaskResponse:
+class GetBatchCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmLeadResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_link_exchange.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_link_exchange.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,49 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import security as shared_security
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from vesselapi import utils
 
 
-
 @dataclasses.dataclass
 class PostLinkExchangeSecurity:
-    vessel_api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header', 'field_name': 'vessel-api-token' }})
+    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PostLinkExchangeRequestBody:
     public_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('publicToken') }})
     
 
-
-class PostLinkExchangeResponseBodyIntegrationID(str, Enum):
-    SALESFORCE = 'salesforce'
-    HUBSPOT = 'hubspot'
-    PIPEDRIVE = 'pipedrive'
+@dataclasses.dataclass
+class PostLinkExchangeRequest:
+    security: PostLinkExchangeSecurity = dataclasses.field()
+    request: Optional[PostLinkExchangeRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
+class PostLinkExchangeResponseBodyIntegrationIDEnum(str, Enum):
+    SALESFORCE = "salesforce"
+    HUBSPOT = "hubspot"
+    PIPEDRIVE = "pipedrive"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PostLinkExchangeResponseBody:
-    r"""Exchange for access token"""
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
     connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
-    integration_id: PostLinkExchangeResponseBodyIntegrationID = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
+    integration_id: PostLinkExchangeResponseBodyIntegrationIDEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId') }})
     native_org_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgId') }})
     native_org_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgURL') }})
     
 
-
-
-
 @dataclasses.dataclass
 class PostLinkExchangeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PostLinkExchangeResponseBody] = dataclasses.field(default=None)
-    r"""Exchange for access token"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_link_token.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_event_attendee.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,23 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import eventattendeeupdate as shared_eventattendeeupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class PostLinkTokenSecurity:
-    vessel_api_token: str = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header', 'field_name': 'vessel-api-token' }})
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostLinkTokenResponseBody:
-    r"""Create link token"""
-    link_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkToken'), 'exclude': lambda f: f is None }})
+class PutCrmEventAttendeeResponseBody:
+    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
+    event_attendee: Optional[shared_eventattendeeupdate.EventAttendeeUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostLinkTokenResponse:
+class PutCrmEventAttendeeResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostLinkTokenResponseBody] = dataclasses.field(default=None)
-    r"""Create link token"""
-    
-
+    response_body: Optional[PutCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/post_webhook.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_batch_crm_account.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import webhookmetadata as shared_webhookmetadata
-from ..shared import webhookmetadatacreate as shared_webhookmetadatacreate
+from ..shared import account as shared_account
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostWebhookRequestBody:
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
-    webhook: Optional[shared_webhookmetadatacreate.WebhookMetadataCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
-    r"""Information describing a webhook"""
+class GetBatchCrmAccountQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    ids: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'ids', 'style': 'form', 'explode': True }})
     
 
-
+@dataclasses.dataclass
+class GetBatchCrmAccountRequest:
+    query_params: GetBatchCrmAccountQueryParams = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PostWebhookResponseBody:
-    r"""OK"""
-    webhook: Optional[shared_webhookmetadata.WebhookMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhook'), 'exclude': lambda f: f is None }})
+class GetBatchCrmAccountResponseBody:
+    accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
+    invalid_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invalidIds'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PostWebhookResponse:
+class GetBatchCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PostWebhookResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetBatchCrmAccountResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_account.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_account.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import accountupdate as shared_accountupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PutCrmAccountRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
     account: shared_accountupdate.AccountUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
+@dataclasses.dataclass
+class PutCrmAccountRequest:
+    request: Optional[PutCrmAccountRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PutCrmAccountResponseBody:
-    r"""OK"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
 class PutCrmAccountResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PutCrmAccountResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_call.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import callupdate as shared_callupdate
+from ..shared import eventcreate as shared_eventcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmCallRequestBody:
+class PostCrmEventRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    call: shared_callupdate.CallUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('call') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    event: Optional[shared_eventcreate.EventCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PostCrmEventRequest:
+    request: Optional[PostCrmEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmCallResponseBody:
-    r"""OK"""
+class PostCrmEventResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class PutCrmCallResponse:
+class PostCrmEventResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmCallResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostCrmEventResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_contact.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/delete_connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,32 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import contactupdate as shared_contactupdate
+from ..shared import security as shared_security
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmContactRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    contact: shared_contactupdate.ContactUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
-    r"""Update a Contact."""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class DeleteConnectionSecurity:
+    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmContactResponseBody:
-    r"""OK"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class DeleteConnectionRequestBody:
+    connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
     
 
-
-
+@dataclasses.dataclass
+class DeleteConnectionRequest:
+    security: DeleteConnectionSecurity = dataclasses.field()
+    request: Optional[DeleteConnectionRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclasses.dataclass
-class PutCrmContactResponse:
+class DeleteConnectionResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmContactResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_deal.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_contact.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import dealupdate as shared_dealupdate
+from ..shared import contactcreate as shared_contactcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmDealRequestBody:
+class PostCrmContactRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    deal: shared_dealupdate.DealUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    contact: shared_contactcreate.ContactCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
     
 
-
+@dataclasses.dataclass
+class PostCrmContactRequest:
+    request: Optional[PostCrmContactRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmDealResponseBody:
-    r"""OK"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class PostCrmContactResponseBody:
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PutCrmDealResponse:
+class PostCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmDealResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostCrmContactResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_email.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_email.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import emailupdate as shared_emailupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PutCrmEmailRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     email: Optional[shared_emailupdate.EmailUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PutCrmEmailRequest:
+    request: Optional[PutCrmEmailRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class PutCrmEmailResponseBody:
-    r"""OK"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
 class PutCrmEmailResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[PutCrmEmailResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_event.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_contact.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventupdate as shared_eventupdate
+from ..shared import contactupdate as shared_contactupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmEventRequestBody:
+class PutCrmContactRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    contact: shared_contactupdate.ContactUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contact') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    event: Optional[shared_eventupdate.EventUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PutCrmContactRequest:
+    request: Optional[PutCrmContactRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmEventResponseBody:
-    r"""OK"""
+class PutCrmContactResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class PutCrmEventResponse:
+class PutCrmContactResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmEventResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PutCrmContactResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_event_attendee.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/get_one_crm_deal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import eventattendeeupdate as shared_eventattendeeupdate
+from ..shared import deal as shared_deal
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmEventAttendeeResponseBody:
-    r"""OK"""
-    access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken'), 'exclude': lambda f: f is None }})
-    event_attendee: Optional[shared_eventattendeeupdate.EventAttendeeUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendee'), 'exclude': lambda f: f is None }})
+class GetOneCrmDealQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'id', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
     
 
+@dataclasses.dataclass
+class GetOneCrmDealRequest:
+    query_params: GetOneCrmDealQueryParams = dataclasses.field()
+    
 
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class GetOneCrmDealResponseBody:
+    deal: Optional[shared_deal.Deal] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal'), 'exclude': lambda f: f is None }})
+    
 
 @dataclasses.dataclass
-class PutCrmEventAttendeeResponse:
+class GetOneCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmEventAttendeeResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[GetOneCrmDealResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_lead.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_link_token.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,32 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import leadupdate as shared_leadupdate
+from ..shared import security as shared_security
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmLeadRequestBody:
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    lead: Optional[shared_leadupdate.LeadUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
+class PostLinkTokenSecurity:
+    vessel_api_token: shared_security.SchemeVesselAPIToken = dataclasses.field(metadata={'security': { 'scheme': True, 'type': 'apiKey', 'sub_type': 'header' }})
     
 
-
+@dataclasses.dataclass
+class PostLinkTokenRequest:
+    security: PostLinkTokenSecurity = dataclasses.field()
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmLeadResponseBody:
-    r"""OK"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class PostLinkTokenResponseBody:
+    link_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linkToken'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class PutCrmLeadResponse:
+class PostLinkTokenResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmLeadResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostLinkTokenResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_note.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_lead.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,34 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import noteupdate as shared_noteupdate
+from ..shared import leadcreate as shared_leadcreate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmNoteRequestBody:
+class PostCrmLeadRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    note: shared_noteupdate.NoteUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('note') }})
-    r"""Update an existing Note. Please note that updating associations is not currently supported."""
+    lead: shared_leadcreate.LeadCreate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead') }})
     
 
-
+@dataclasses.dataclass
+class PostCrmLeadRequest:
+    request: Optional[PostCrmLeadRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmNoteResponseBody:
-    r"""OK"""
+class PostCrmLeadResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class PutCrmNoteResponse:
+class PostCrmLeadResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmNoteResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PostCrmLeadResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/put_crm_task.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_deal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import taskupdate as shared_taskupdate
+from ..shared import dealupdate as shared_dealupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmTaskRequestBody:
+class PutCrmDealRequestBody:
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    deal: shared_dealupdate.DealUpdate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deal') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    task: Optional[shared_taskupdate.TaskUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('task'), 'exclude': lambda f: f is None }})
     
 
-
+@dataclasses.dataclass
+class PutCrmDealRequest:
+    request: Optional[PutCrmDealRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class PutCrmTaskResponseBody:
-    r"""OK"""
+class PutCrmDealResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     
 
-
-
-
 @dataclasses.dataclass
-class PutCrmTaskResponse:
+class PutCrmDealResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[PutCrmTaskResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[PutCrmDealResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_accounts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import account as shared_account
 from ..shared import datefilter as shared_datefilter
 from ..shared import numberfilter as shared_numberfilter
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmAccountsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmAccountsRequestBodyFilters:
     annual_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
     city: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
     country: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
@@ -30,55 +35,33 @@
     phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
     postal_code: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
     state: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
     street: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('street'), 'exclude': lambda f: f is None }})
     website: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmAccountsRequestBody:
     filters: Optional[SearchCrmAccountsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmAccountsRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmAccountsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmAccountsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmAccountsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmAccountsResponseBody:
-    r"""OK"""
     accounts: Optional[list[shared_account.Account]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmAccountsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmAccountsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_calls.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,62 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import call as shared_call
+from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
+from ..shared import event as shared_event
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmEventsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmCallsRequestBodyFilters:
+class SearchCrmEventsRequestBodyFilters:
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    date_: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'exclude': lambda f: f is None }})
     description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    direction: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('direction'), 'exclude': lambda f: f is None }})
-    disposition: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disposition'), 'exclude': lambda f: f is None }})
+    end_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    location: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+    start_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
     subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmCallsRequestBody:
-    filters: Optional[SearchCrmCallsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmEventsRequestBody:
+    filters: Optional[SearchCrmEventsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class SearchCrmCallsRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmCallsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmEventsRequest:
+    query_params: SearchCrmEventsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmEventsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmCallsResponseBody:
-    r"""OK"""
-    calls: Optional[list[shared_call.Call]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('calls'), 'exclude': lambda f: f is None }})
+class SearchCrmEventsResponseBody:
+    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class SearchCrmCallsResponse:
+class SearchCrmEventsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmCallsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[SearchCrmEventsResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_contacts.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_contacts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,60 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import contact as shared_contact
 from ..shared import datefilter as shared_datefilter
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmContactsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmContactsRequestBodyFilters:
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
     last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
     mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmContactsRequestBody:
     filters: Optional[SearchCrmContactsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmContactsRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmContactsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmContactsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmContactsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmContactsResponseBody:
-    r"""OK"""
     contacts: Optional[list[shared_contact.Contact]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contacts'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmContactsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmContactsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_deals.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_leads.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,81 +1,61 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
-from ..shared import deal as shared_deal
-from ..shared import numberfilter as shared_numberfilter
+from ..shared import lead as shared_lead
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmLeadsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmDealsRequestBodyFilters:
-    amount: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    close_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate'), 'exclude': lambda f: f is None }})
+class SearchCrmLeadsRequestBodyFilters:
+    account: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    expected_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expectedRevenue'), 'exclude': lambda f: f is None }})
+    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    is_closed: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isClosed'), 'exclude': lambda f: f is None }})
-    is_won: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isWon'), 'exclude': lambda f: f is None }})
+    job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    probability: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
-    stage: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
+    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmDealsRequestBody:
-    filters: Optional[SearchCrmDealsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmLeadsRequestBody:
+    filters: Optional[SearchCrmLeadsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class SearchCrmDealsRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmDealsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmLeadsRequest:
+    query_params: SearchCrmLeadsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmLeadsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmDealsResponseBody:
-    r"""OK"""
-    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
+class SearchCrmLeadsResponseBody:
+    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class SearchCrmDealsResponse:
+class SearchCrmLeadsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmDealsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[SearchCrmLeadsResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_emails.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_emails.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
 from ..shared import email as shared_email
 from ..shared import stringfilter as shared_stringfilter
 from ..shared import stringlistfilter as shared_stringlistfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmEmailsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEmailsRequestBodyFilters:
     bcc: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
     body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
     body_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
     cc: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
@@ -31,55 +36,33 @@
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
     to: Optional[shared_stringlistfilter.StringListFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmEmailsRequestBody:
     filters: Optional[SearchCrmEmailsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmEmailsRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmEmailsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmEmailsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmEmailsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmEmailsResponseBody:
-    r"""OK"""
     emails: Optional[list[shared_email.Email]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emails'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmEmailsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmEmailsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_event_attendees.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_event_attendees.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,57 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import datefilter as shared_datefilter
 from ..shared import eventattendee as shared_eventattendee
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmEventAttendeesQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequestBodyFilters:
     associated_object_type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associatedObjectType'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequestBody:
     filters: Optional[SearchCrmEventAttendeesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmEventAttendeesRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmEventAttendeesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmEventAttendeesQueryParams = dataclasses.field()
+    request: Optional[SearchCrmEventAttendeesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmEventAttendeesResponseBody:
-    r"""OK"""
     event_attendees: Optional[list[shared_eventattendee.EventAttendee]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendees'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmEventAttendeesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmEventAttendeesResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_events.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_tasks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,61 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
-from ..shared import event as shared_event
 from ..shared import stringfilter as shared_stringfilter
+from ..shared import task as shared_task
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmTasksQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmEventsRequestBodyFilters:
+class SearchCrmTasksRequestBodyFilters:
+    body: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    description: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    end_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
+    due_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    is_all_day_event: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    location: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    is_done: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    start_date_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
+    priority: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     subject: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
-    type: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmEventsRequestBody:
-    filters: Optional[SearchCrmEventsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmTasksRequestBody:
+    filters: Optional[SearchCrmTasksRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class SearchCrmEventsRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmEventsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmTasksRequest:
+    query_params: SearchCrmTasksQueryParams = dataclasses.field()
+    request: Optional[SearchCrmTasksRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmEventsResponseBody:
-    r"""OK"""
-    events: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events'), 'exclude': lambda f: f is None }})
+class SearchCrmTasksResponseBody:
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
+    tasks: Optional[list[shared_task.Task]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tasks'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class SearchCrmEventsResponse:
+class SearchCrmTasksResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmEventsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[SearchCrmTasksResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_leads.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_deals.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,64 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import booleanfilter as shared_booleanfilter
 from ..shared import datefilter as shared_datefilter
-from ..shared import lead as shared_lead
+from ..shared import deal as shared_deal
+from ..shared import numberfilter as shared_numberfilter
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmDealsQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SearchCrmLeadsRequestBodyFilters:
-    account: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+class SearchCrmDealsRequestBodyFilters:
+    amount: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    close_date: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    expected_revenue: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expectedRevenue'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    job_title: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    is_closed: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isClosed'), 'exclude': lambda f: f is None }})
+    is_won: Optional[shared_booleanfilter.BooleanFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isWon'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
+    name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    phone: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    probability: Optional[shared_numberfilter.NumberFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+    stage: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmLeadsRequestBody:
-    filters: Optional[SearchCrmLeadsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class SearchCrmDealsRequestBody:
+    filters: Optional[SearchCrmDealsRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class SearchCrmLeadsRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmLeadsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+class SearchCrmDealsRequest:
+    query_params: SearchCrmDealsQueryParams = dataclasses.field()
+    request: Optional[SearchCrmDealsRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmLeadsResponseBody:
-    r"""OK"""
-    leads: Optional[list[shared_lead.Lead]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leads'), 'exclude': lambda f: f is None }})
+class SearchCrmDealsResponseBody:
+    deals: Optional[list[shared_deal.Deal]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deals'), 'exclude': lambda f: f is None }})
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
-class SearchCrmLeadsResponse:
+class SearchCrmDealsResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmLeadsResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    response_body: Optional[SearchCrmDealsResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_notes.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/search_crm_notes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,57 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import datefilter as shared_datefilter
 from ..shared import note as shared_note
 from ..shared import stringfilter as shared_stringfilter
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SearchCrmNotesQueryParams:
+    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
+    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
+    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
+    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SearchCrmNotesRequestBodyFilters:
     content: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
     content_html: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentHtml'), 'exclude': lambda f: f is None }})
     content_text: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contentText'), 'exclude': lambda f: f is None }})
     created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
     id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
     modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
     native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmNotesRequestBody:
     filters: Optional[SearchCrmNotesRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmNotesRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmNotesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    query_params: SearchCrmNotesQueryParams = dataclasses.field()
+    request: Optional[SearchCrmNotesRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class SearchCrmNotesResponseBody:
-    r"""OK"""
     next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
     notes: Optional[list[shared_note.Note]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notes'), 'exclude': lambda f: f is None }})
     
 
-
-
-
 @dataclasses.dataclass
 class SearchCrmNotesResponse:
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
     response_body: Optional[SearchCrmNotesResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/operations/search_crm_users.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/email.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,43 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
-from ..shared import datefilter as shared_datefilter
-from ..shared import stringfilter as shared_stringfilter
-from ..shared import user as shared_user
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmUsersRequestBodyFilters:
-    created_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    email: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
-    id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    last_name: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
-    modified_time: Optional[shared_datefilter.DateFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    native_id: Optional[shared_stringfilter.StringFilter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
+class EmailAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class SearchCrmUsersRequestBody:
-    filters: Optional[SearchCrmUsersRequestBodyFilters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filters'), 'exclude': lambda f: f is None }})
+class Email:
+    r"""Email
+    An email is a message sent from one person to another through an email service. Emails involve participants - the person who the email was sent to, or the person that sent it. Participants are usually a Contact, Lead, or User but in certain CRMs, can be a person not yet associated with a CRM object.
+    """
     
-
-
-
-
-@dataclasses.dataclass
-class SearchCrmUsersRequest:
-    access_token: str = dataclasses.field(metadata={'query_param': { 'field_name': 'accessToken', 'style': 'form', 'explode': True }})
-    r"""The token for the customer's account. This was generated when they connected their account."""
-    all_fields: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'allFields', 'style': 'form', 'explode': True }})
-    r"""Returns all fields including non-unifiable and custom fields under the \\"additional\\" property in the response"""
-    cursor: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'cursor', 'style': 'form', 'explode': True }})
-    r"""The cursor to use for pagination"""
-    limit: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-    r"""The number of records to return per page."""
-    request_body: Optional[SearchCrmUsersRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
-@dataclasses.dataclass
-class SearchCrmUsersResponseBody:
-    r"""OK"""
-    next_page_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextPageCursor'), 'exclude': lambda f: f is None }})
-    users: Optional[list[shared_user.User]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('users'), 'exclude': lambda f: f is None }})
-    
-
-
-
-
-@dataclasses.dataclass
-class SearchCrmUsersResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    response_body: Optional[SearchCrmUsersResponseBody] = dataclasses.field(default=None)
-    r"""OK"""
-    
-
+    associations: EmailAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject') }})
+    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
+    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
+    has_attachment: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasAttachment'), 'exclude': lambda f: f is None }})
+    is_bounced: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBounced'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
+    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messageDate'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/accountcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/taskcreate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,23 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class AccountCreateAdditional:
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class AccountCreate:
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    additional: Optional[AccountCreateAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
-    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone | Not supported by Pipedrive"""
-    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    
-
+class TaskCreate:
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/accountupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
-from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class AccountUpdateAdditional:
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
+class TaskAssociations:
+    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class AccountUpdate:
-    additional: Optional[AccountUpdateAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
-    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone| Not supported by Pipedrive"""
-    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
+class Task:
+    r"""Task
+    A task attached to some CRM object
+    """
     
-
+    associations: TaskAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
+    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
+    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/address.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/dealupdate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Address:
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
-    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
-    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
-    street: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('street'), 'exclude': lambda f: f is None }})
-    
-
+class DealUpdate:
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    close_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/booleanfilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/stringlistfilter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class BooleanFilter:
-    equals: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
-    not_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
-    
-
+class StringListFilter:
+    has: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has'), 'exclude': lambda f: f is None }})
+    has_every: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasEvery'), 'exclude': lambda f: f is None }})
+    has_some: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasSome'), 'exclude': lambda f: f is None }})
+    is_empty: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isEmpty'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/call.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/event.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,43 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class CallAdditional:
-    pass
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CallAssociations:
+class EventAssociations:
     account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
     contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
+    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
+    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
     owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this call"""
     
 
-
-class CallDirection(str, Enum):
-    INBOUND = 'inbound'
-    OUTBOUND = 'outbound'
-    INTERNAL = 'internal'
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Call:
-    additional: Optional[CallAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    associations: Optional[CallAssociations] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations'), 'exclude': lambda f: f is None }})
-    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    r"""The timestamp that the call object was created"""
-    date_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'exclude': lambda f: f is None }})
-    r"""The date the call occurred"""
+class Event:
+    r"""Event
+    Events are a type of activity that has attendees and takes place at a certain point in time (i.e., has a start and end date).
+    For the currently supported CRMs, these are the objects Events most closely maps to:
+    - Salesforce = Events
+    - HubSpot = Meetings
+    - Pipedrive = Activities
+    """
+    
+    associations: EventAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
+    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    direction: Optional[CallDirection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('direction'), 'exclude': lambda f: f is None }})
-    disposition: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disposition'), 'exclude': lambda f: f is None }})
-    r"""Possibly an enum, See /details endpoint for values."""
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    r"""Unique Vessel Id."""
-    modified_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime'), 'exclude': lambda f: f is None }})
-    r"""The timestamp the call object was last modified"""
-    native_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId'), 'exclude': lambda f: f is None }})
-    r"""Id of the object in the connected CRM."""
+    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
+    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
+    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
     subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
-    
-
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/callcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from vesselapi import utils
 
-class CallCreateDirection(str, Enum):
-    INBOUND = 'inbound'
-    OUTBOUND = 'outbound'
-    INTERNAL = 'internal'
+class ConnectionIntegrationIDEnum(str, Enum):
+    SALESFORCE = "salesforce"
+    HUBSPOT = "hubspot"
+    PIPEDRIVE = "pipedrive"
+
+class ConnectionStatusEnum(str, Enum):
+    NEW_CONNECTION = "NEW_CONNECTION"
+    INITIAL_SYNC = "INITIAL_SYNC"
+    READY = "READY"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CallCreate:
-    direction: CallCreateDirection = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('direction') }})
-    disposition: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disposition') }})
-    r"""See /details endpoint for possible values."""
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    contact_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds'), 'exclude': lambda f: f is None }})
-    r"""The participants involved in this call. If this is an inbound call, this is the contacts that called, if this is an outbound call, this is the contacts that were called."""
-    date_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date'), 'exclude': lambda f: f is None }})
-    r"""The date the call occurred"""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
-    
-
+class Connection:
+    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
+    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    integration_id: Optional[ConnectionIntegrationIDEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
+    last_activity_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastActivityDate'), 'exclude': lambda f: f is None }})
+    native_org_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgURL'), 'exclude': lambda f: f is None }})
+    status: Optional[ConnectionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/callupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/emailupdate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class CallUpdate:
-    disposition: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('disposition') }})
-    r"""See /details endpoint for possible values."""
+class EmailUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
     owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    
-
+    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/connection.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/noteupdate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
-class ConnectionIntegrationID(str, Enum):
-    SALESFORCE = 'salesforce'
-    HUBSPOT = 'hubspot'
-    PIPEDRIVE = 'pipedrive'
-
-class ConnectionStatus(str, Enum):
-    NEW_CONNECTION = 'NEW_CONNECTION'
-    INITIAL_SYNC = 'INITIAL_SYNC'
-    READY = 'READY'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Connection:
-    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
-    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    integration_id: Optional[ConnectionIntegrationID] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
-    last_activity_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastActivityDate'), 'exclude': lambda f: f is None }})
-    native_org_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeOrgURL'), 'exclude': lambda f: f is None }})
-    status: Optional[ConnectionStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+class NoteUpdate:
+    r"""NoteUpdate
+    Update an existing Note. Please note that updating associations is not currently supported.
+    """
     
-
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/contact.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,42 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class ContactAdditional:
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ContactAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    call_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('callIds') }})
+class AccountAssociations:
+    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
     deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    email_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emailIds') }})
-    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
     event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
     lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
     note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
     task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Contact:
-    r"""Information about an individual affiliated with another CRM Object (e.g., a Lead, a Deal, etc)"""
-    associations: ContactAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+class Account:
+    r"""Account
+    (Alias: company, organization) An organization involved with your business.
+    """
+    
+    associations: AccountAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the contact was created"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the contact was last modified"""
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
-    additional: Optional[ContactAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    r"""The primary mobile phone number for this contact. Possibly the same as the phone number."""
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
     phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone number for this contact"""
-    
-
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/contactcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/accountupdate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class ContactCreateAdditional:
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ContactCreate:
-    r"""Properties that a contact can be created with"""
-    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName') }})
-    additional: Optional[ContactCreateAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
-    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+class AccountUpdate:
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
     phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone"""
-    
-
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/contactupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contactcreate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class ContactUpdateAdditional:
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class ContactUpdate:
-    r"""Update a Contact."""
-    additional: Optional[ContactUpdateAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
+class ContactCreate:
+    r"""ContactCreate
+    Properties that a contact can be created with
+    """
+    
+    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
     email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
     job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
     mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
     phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/datefilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/address.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class DateFilter:
-    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
-    gt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
-    gte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
-    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
-    lt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
-    lte: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
-    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
-    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
-    
-
+class Address:
+    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
+    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
+    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
+    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
+    street: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('street'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/dealupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/accountcreate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+from ..shared import address as shared_address
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class DealUpdateAdditional:
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class DealUpdate:
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    r"""Update the account this deal is associated with."""
-    additional: Optional[DealUpdateAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
-    close_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
-    r"""Decimal probability of closing the deal"""
-    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
-    r"""The stage the deal is in. See /deal/details for possible values"""
-    
-
+class AccountCreate:
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    address: Optional[shared_address.Address] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
+    annual_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('annualRevenue'), 'exclude': lambda f: f is None }})
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    industry: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('industry'), 'exclude': lambda f: f is None }})
+    number_of_employees: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numberOfEmployees'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+    website: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('website'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/email.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/deal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,42 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class EmailAdditional:
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class EmailAssociations:
+class DealAssociations:
     account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
     contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
     owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this email"""
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
+    event_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds'), 'exclude': lambda f: f is None }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Email:
-    r"""An email is a message sent from one person to another through an email service. Emails involve participants - the person who the email was sent to, or the person that sent it. Participants are usually a Contact, Lead, or User but in certain CRMs, can be a person not yet associated with a CRM object."""
-    associations: EmailAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+class Deal:
+    r"""Deal
+    (Alias: Opportunity) An object representing either the opportunity to sell a product to an Account, or in the case of an `isWon` deal, a product sold to an Account.
+    *CRM Caveats*:
+    - Pipedrive: Users must have \"Deal probability\" turned on for the given pipeline for probability to be configurable and returned.
+    """
+    
+    associations: DealAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+    close_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the email object was created"""
-    from_: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('from') }})
-    r"""The email address that sent the email"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the email object was last modified"""
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
-    subject: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject') }})
-    r"""The subject of the email"""
-    to: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('to') }})
-    r"""The email addresses that received the email"""
-    additional: Optional[EmailAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    bcc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bcc'), 'exclude': lambda f: f is None }})
-    r"""The email addresses that received a blind copy of the email"""
-    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    r"""The text formatted body of the email"""
-    body_html: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bodyHtml'), 'exclude': lambda f: f is None }})
-    r"""The html formatted body of the email"""
-    cc: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cc'), 'exclude': lambda f: f is None }})
-    r"""The email addresses that received a copy of the email"""
-    has_attachment: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasAttachment'), 'exclude': lambda f: f is None }})
-    r"""If this email has attachment(s)"""
-    is_bounced: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isBounced'), 'exclude': lambda f: f is None }})
-    r"""If this email was bounced"""
-    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
-    r"""If this email was sent to the user or sent by the user"""
-    message_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messageDate'), 'exclude': lambda f: f is None }})
-    r"""The date the email was created. This can be set when creating the email object and is not necessarily the same as the `createdTime` field."""
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""The status of the email (CRM specific, see /details)."""
-    
-
+    stage: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage') }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    expected_revenue: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expectedRevenue'), 'exclude': lambda f: f is None }})
+    is_closed: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isClosed'), 'exclude': lambda f: f is None }})
+    is_won: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isWon'), 'exclude': lambda f: f is None }})
+    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/emailupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/numberfilter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class EmailUpdateAdditional:
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class EmailUpdate:
-    additional: Optional[EmailUpdateAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    is_incoming: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isIncoming'), 'exclude': lambda f: f is None }})
-    r"""If this email was sent to the user or sent by the user"""
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    r"""The Id of the User that owns this email"""
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""The status of the email (CRM specific, see /details)."""
-    
-
+class NumberFilter:
+    equals: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    gt: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
+    gte: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
+    in_: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
+    lt: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
+    lte: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
+    not_: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+    not_in: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/eventcreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,53 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from enum import Enum
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class EventCreateAdditional:
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
+class FieldOptions:
+    key: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     
-
+class FieldTypeEnum(str, Enum):
+    STRING = "string"
+    NUMBER = "number"
+    DATETIME = "datetime"
+    DATE = "date"
+    BOOLEAN = "boolean"
+    REFERENCE = "reference"
+    PHONE = "phone"
+    URL = "url"
+    ID = "id"
+    EMAIL = "email"
+    PERCENT = "percent"
+    SINGLESELECT = "singleselect"
+    MULTISELECT = "multiselect"
+    ADDRESS = "address"
+    DECIMAL = "decimal"
+    TIME = "time"
+    DATERANGE = "daterange"
+    OBJECT = "object"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class EventCreate:
-    end_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime') }})
-    start_date_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime') }})
-    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
-    additional: Optional[EventCreateAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
-    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    r"""Not supported by HubSpot and Pipedrive"""
-    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
-    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+class Field:
+    r"""Field
+    (Alias: property) A field is a key-value pair on a CRM Object that provides information about that object.
+    """
     
-
+    creatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creatable') }})
+    custom: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom') }})
+    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})
+    type: FieldTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    universal: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('universal') }})
+    updatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatable') }})
+    is_array: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isArray'), 'exclude': lambda f: f is None }})
+    options: Optional[list[FieldOptions]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/eventupdate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contactupdate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class EventUpdateAdditional:
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class EventUpdate:
-    additional: Optional[EventUpdateAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Create any property in the downstream CRM, such as a custom or native property. For a list of all properties see /details."""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    end_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endDateTime'), 'exclude': lambda f: f is None }})
-    is_all_day_event: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isAllDayEvent'), 'exclude': lambda f: f is None }})
-    r"""Not supported by HubSpot and Pipedrive"""
-    location: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
-    owner_user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId'), 'exclude': lambda f: f is None }})
-    start_date_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startDateTime'), 'exclude': lambda f: f is None }})
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+class ContactUpdate:
+    r"""ContactUpdate
+    Update a Contact.
+    """
     
-
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/field.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/post_crm_passthrough.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,47 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Any, Optional
 from vesselapi import utils
 
+class PostCrmPassthroughRequestBodyMethodEnum(str, Enum):
+    GET = "GET"
+    POST = "POST"
+    PUT = "PUT"
+    PATCH = "PATCH"
+    DELETE = "DELETE"
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class FieldOptions:
-    key: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+class PostCrmPassthroughRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    method: PostCrmPassthroughRequestBodyMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
+    path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('path') }})
+    body: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    query: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
     
 
-
-class FieldType(str, Enum):
-    STRING = 'string'
-    NUMBER = 'number'
-    DATETIME = 'datetime'
-    DATE = 'date'
-    BOOLEAN = 'boolean'
-    REFERENCE = 'reference'
-    PHONE = 'phone'
-    URL = 'url'
-    ID = 'id'
-    EMAIL = 'email'
-    PERCENT = 'percent'
-    SINGLESELECT = 'singleselect'
-    MULTISELECT = 'multiselect'
-    ADDRESS = 'address'
-    DECIMAL = 'decimal'
-    TIME = 'time'
-    DATERANGE = 'daterange'
-    OBJECT = 'object'
-
+@dataclasses.dataclass
+class PostCrmPassthroughRequest:
+    request: Optional[PostCrmPassthroughRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Field:
-    r"""(Alias: property) A field is a key-value pair on a CRM Object that provides information about that object."""
-    creatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creatable') }})
-    r"""If this field can be used when creating the object"""
-    custom: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom') }})
-    r"""If this field is a custom field"""
-    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-    r"""The key in the CRM object (ex: annualRevenue, numberOfEmployees, etc)"""
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    r"""The display name of this field (ex: number of employees, annual revenue, etc)"""
-    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})
-    r"""If this field is required when creating the object"""
-    type: FieldType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    universal: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('universal') }})
-    r"""If this is a field we've unified across CRMs"""
-    updatable: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatable') }})
-    r"""If this field can be updated"""
-    is_array: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isArray'), 'exclude': lambda f: f is None }})
-    r"""If this field is an array"""
-    options: Optional[list[FieldOptions]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})
-    r"""Possible options for this field"""
+class PostCrmPassthroughResponseBody:
+    body: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
+    headers: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('headers'), 'exclude': lambda f: f is None }})
+    status_code: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusCode'), 'exclude': lambda f: f is None }})
+    url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url'), 'exclude': lambda f: f is None }})
     
 
+@dataclasses.dataclass
+class PostCrmPassthroughResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PostCrmPassthroughResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/integration.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 from vesselapi import utils
 
-class IntegrationIntegrationID(str, Enum):
-    SALESFORCE = 'salesforce'
-    HUBSPOT = 'hubspot'
-    PIPEDRIVE = 'pipedrive'
+class IntegrationIntegrationIDEnum(str, Enum):
+    SALESFORCE = "salesforce"
+    HUBSPOT = "hubspot"
+    PIPEDRIVE = "pipedrive"
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Integration:
     icon_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('iconURL'), 'exclude': lambda f: f is None }})
-    r"""Base 64 data URI"""
-    integration_id: Optional[IntegrationIntegrationID] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
+    integration_id: Optional[IntegrationIntegrationIDEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('integrationId'), 'exclude': lambda f: f is None }})
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/lead.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/lead.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,41 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class LeadAdditional:
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class LeadAssociations:
     account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    call_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('callIds') }})
     contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
-    email_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('emailIds') }})
     event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
     event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
     note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
     task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class Lead:
-    r"""A Lead represents an individual, or sometimes an organization, that is interested in purchasing your product (i.e., is a potential Deal).
+    r"""Lead
+    A Lead represents an individual, or sometimes an organization, that is interested in purchasing your product (i.e., is a potential Deal). 
     *CRM Caveats*:
     - HubSpot: we consider contacts with the `leadStatus` set to be leads.
     """
+    
     associations: LeadAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the lead was created"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the lead was last modified"""
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
     account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
-    r"""Name of the Account associated with this lead"""
-    additional: Optional[LeadAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
     email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
     job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
     last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
     mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
-    r"""The primary mobile phone number for this lead. Possibly the same as the phone number"""
     phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
-    r"""The primary phone"""
-    
-
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/note.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/dealcreate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class NoteAdditional:
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
-@dataclasses.dataclass
-class NoteAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this note"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Note:
-    r"""A Note attached to some CRM Object."""
-    associations: NoteAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the note was created"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the note was last modified"""
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
-    additional: Optional[NoteAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    content: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content'), 'exclude': lambda f: f is None }})
-    r"""The body of the note"""
-    
-
+class DealCreate:
+    close_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('closeDate') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    probability: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('probability'), 'exclude': lambda f: f is None }})
+    stage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stage'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/numberfilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/stringfilter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class NumberFilter:
-    equals: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
-    gt: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gt'), 'exclude': lambda f: f is None }})
-    gte: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gte'), 'exclude': lambda f: f is None }})
-    in_: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
-    lt: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lt'), 'exclude': lambda f: f is None }})
-    lte: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lte'), 'exclude': lambda f: f is None }})
-    not_: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
-    not_in: Optional[list[float]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
-    
-
+class StringFilter:
+    contains: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contains'), 'exclude': lambda f: f is None }})
+    ends_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endsWith'), 'exclude': lambda f: f is None }})
+    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
+    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
+    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
+    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
+    starts_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startsWith'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/stringfilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/leadcreate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,19 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
-class StringFilterMode(str, Enum):
-    INSENSITIVE = 'insensitive'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class StringFilter:
-    contains: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contains'), 'exclude': lambda f: f is None }})
-    ends_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endsWith'), 'exclude': lambda f: f is None }})
-    equals: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('equals'), 'exclude': lambda f: f is None }})
-    in_: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
-    mode: Optional[StringFilterMode] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode'), 'exclude': lambda f: f is None }})
-    not_: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('not'), 'exclude': lambda f: f is None }})
-    not_in: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('notIn'), 'exclude': lambda f: f is None }})
-    starts_with: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startsWith'), 'exclude': lambda f: f is None }})
-    
-
+class LeadCreate:
+    last_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName') }})
+    account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/stringlistfilter.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class StringListFilter:
-    has: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has'), 'exclude': lambda f: f is None }})
-    has_every: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasEvery'), 'exclude': lambda f: f is None }})
-    has_some: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasSome'), 'exclude': lambda f: f is None }})
-    is_empty: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isEmpty'), 'exclude': lambda f: f is None }})
-    
-
+class WebhookMetadata:
+    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
+    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
+    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
+    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/task.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/contact.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,39 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
-
-@dataclasses.dataclass
-class TaskAdditional:
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    
-
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class TaskAssociations:
+class ContactAssociations:
     account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    contact_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactIds') }})
     deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
+    event_attendee_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventAttendeeIds') }})
+    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
     lead_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadIds') }})
-    owner_user_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ownerUserId') }})
-    r"""The Id of the User that owns this Task"""
+    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
+    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class Task:
-    r"""A task attached to some CRM object"""
-    associations: TaskAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
+class Contact:
+    r"""Contact
+    Information about an individual affiliated with another CRM Object (e.g., a Lead, a Deal, etc)
+    """
+    
+    associations: ContactAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
     created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the task was created"""
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
     modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the task was last modified"""
     native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
-    additional: Optional[TaskAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    body: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('body'), 'exclude': lambda f: f is None }})
-    due_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dueDate'), 'exclude': lambda f: f is None }})
-    is_done: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isDone'), 'exclude': lambda f: f is None }})
-    priority: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('priority'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""Not supported by Pipedrive"""
-    subject: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subject'), 'exclude': lambda f: f is None }})
-    
-
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
+    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
+    job_title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobTitle'), 'exclude': lambda f: f is None }})
+    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
+    mobile_phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mobilePhone'), 'exclude': lambda f: f is None }})
+    phone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phone'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/user.py` & `vesselapi-3.5.2/src/vesselapi/models/operations/put_crm_lead.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,35 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
+from ..shared import leadupdate as shared_leadupdate
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
-
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UserAdditional:
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
+class PutCrmLeadRequestBody:
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessToken') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    lead: Optional[shared_leadupdate.LeadUpdate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lead'), 'exclude': lambda f: f is None }})
     
 
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class UserAssociations:
-    account_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountIds') }})
-    deal_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealIds') }})
-    event_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventIds') }})
-    note_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('noteIds') }})
-    task_ids: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taskIds') }})
+class PutCrmLeadRequest:
+    request: Optional[PutCrmLeadRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
-
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class User:
-    r"""Users of the connected CRM platform. These are *not* the contacts or leads, but rather the user accounts from the connected CRM."""
-    associations: UserAssociations = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('associations') }})
-    created_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime') }})
-    r"""The timestamp that the user was created"""
+class PutCrmLeadResponseBody:
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique Vessel Id."""
-    modified_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedTime') }})
-    r"""The timestamp the user was last modified"""
-    native_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nativeId') }})
-    r"""Id of the object in the connected CRM."""
-    additional: Optional[UserAdditional] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
-    r"""Returned when `allFields` is set in the query params. Includes all data, untransformed, we received from the downstream CRM"""
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    first_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('firstName'), 'exclude': lambda f: f is None }})
-    last_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastName'), 'exclude': lambda f: f is None }})
     
 
+@dataclasses.dataclass
+class PutCrmLeadResponse:
+    content_type: str = dataclasses.field()
+    status_code: int = dataclasses.field()
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    response_body: Optional[PutCrmLeadResponseBody] = dataclasses.field(default=None)
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/webhookmetadata.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/notecreate.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from typing import Any, Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
-class WebhookMetadata:
-    connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId'), 'exclude': lambda f: f is None }})
-    created_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdTime'), 'exclude': lambda f: f is None }})
-    webhook_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookId'), 'exclude': lambda f: f is None }})
-    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
+class NoteCreate:
+    r"""NoteCreate
+    Create a new Note. You may only associate a note with at most one entity of each type upon creation.
+    """
     
-
+    content: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content') }})
+    account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountId'), 'exclude': lambda f: f is None }})
+    additional: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional'), 'exclude': lambda f: f is None }})
+    contact_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contactId'), 'exclude': lambda f: f is None }})
+    deal_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealId'), 'exclude': lambda f: f is None }})
+    lead_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('leadId'), 'exclude': lambda f: f is None }})
+    user_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('userId'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/models/shared/webhookmetadatacreate.py` & `vesselapi-3.5.2/src/vesselapi/models/shared/webhookmetadatacreate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 from vesselapi import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
-
 @dataclasses.dataclass
 class WebhookMetadataCreate:
-    r"""Information describing a webhook"""
-    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
-    r"""a valid URL"""
+    r"""WebhookMetadataCreate
+    Information describing a webhook
+    """
     
-
+    webhook_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('webhookUrl'), 'exclude': lambda f: f is None }})
+
```

### Comparing `vesselapi-3.27.1/src/vesselapi/tasks.py` & `vesselapi-3.5.2/src/vesselapi/deals.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,208 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
-class Tasks:
-    sdk_configuration: SDKConfiguration
+class Deals:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
 
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
         
-    
-    def batch(self, request: operations.GetBatchCrmTaskRequest) -> operations.GetBatchCrmTaskResponse:
-        r"""Get Batch Tasks
-        Retrieve Tasks by a set of Id's
+    def batch(self, request: operations.GetBatchCrmDealRequest) -> operations.GetBatchCrmDealResponse:
+        r"""Get Batch Deals
+        Retrieve Deals by a set of Id's
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/task/batch'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetBatchCrmTaskRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/deal/batch'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBatchCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetBatchCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmTaskResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBatchCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def create(self, request: operations.PostCrmTaskRequestBody) -> operations.PostCrmTaskResponse:
-        r"""Create Task
-        Create a new Task.
-        *CRM Caveats*:
-        - Salesforce: You may only associate a Task with either a Lead or a Contact *and* either a Deal or an Account.
+    def create(self, request: operations.PostCrmDealRequest) -> operations.PostCrmDealResponse:
+        r"""Create Deal
+        Create a new Deal
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/task'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/deal'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmTaskResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def details(self, request: operations.GetDetailsCrmTaskRequest) -> operations.GetDetailsCrmTaskResponse:
-        r"""Get Task Details
-        Get details about all tasks. 
+    def details(self, request: operations.GetDetailsCrmDealRequest) -> operations.GetDetailsCrmDealResponse:
+        r"""Get Deal Details
+        Get details about all deals or a particular deal. 
         Details include the type, possible values, and other meta data about the fields.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/task/details'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetDetailsCrmTaskRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/deal/details'
         
-        client = self.sdk_configuration.security_client
+        query_params = utils.get_query_params(request.query_params)
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetDetailsCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetDetailsCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmTaskResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDetailsCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneCrmTaskRequest) -> operations.GetOneCrmTaskResponse:
-        r"""Get Task
-        Retrieve a single Task by Id
+    def find(self, request: operations.GetOneCrmDealRequest) -> operations.GetOneCrmDealResponse:
+        r"""Get Deal
+        Retrieve a single Deal by Id
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/task'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneCrmTaskRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
         
-        client = self.sdk_configuration.security_client
+        url = base_url.removesuffix('/') + '/crm/deal'
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        query_params = utils.get_query_params(request.query_params)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmTaskResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneCrmDealResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def list(self, request: operations.GetAllCrmTasksRequest) -> operations.GetAllCrmTasksResponse:
-        r"""Get All Tasks
-        Retrieve all Tasks
+    def list(self, request: operations.GetAllCrmDealsRequest) -> operations.GetAllCrmDealsResponse:
+        r"""Get All Deals
+        Retrieve all Deals
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/tasks'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetAllCrmTasksRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/deals'
+        
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAllCrmTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmDealsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmTasksResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmDealsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def search(self, request: operations.SearchCrmTasksRequest) -> operations.SearchCrmTasksResponse:
-        r"""Search Tasks
-        Search all Tasks using filters
+    def search(self, request: operations.SearchCrmDealsRequest) -> operations.SearchCrmDealsResponse:
+        r"""Search Deals
+        Search all Deals using filters
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/tasks/search'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/deals/search'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.SearchCrmTasksRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        query_params = utils.get_query_params(request.query_params)
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.SearchCrmTasksResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.SearchCrmDealsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmTasksResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.SearchCrmDealsResponseBody])
                 res.response_body = out
 
         return res
 
-    
-    def update(self, request: operations.PutCrmTaskRequestBody) -> operations.PutCrmTaskResponse:
-        r"""Update Task
-        Update an existing Task by Id
+    def update(self, request: operations.PutCrmDealRequest) -> operations.PutCrmDealResponse:
+        r"""Update Deal
+        Update an existing Deal
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/crm/task'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/crm/deal'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCrmTaskResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PutCrmDealResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmTaskResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PutCrmDealResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.27.1/src/vesselapi/utils/retries.py` & `vesselapi-3.5.2/src/vesselapi/utils/retries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import random
 import time
 
 import requests
 
 
 class BackoffStrategy:
@@ -20,17 +18,16 @@
 
 
 class RetryConfig:
     strategy: str
     backoff: BackoffStrategy
     retry_connection_errors: bool
 
-    def __init__(self, strategy: str, backoff: BackoffStrategy, retry_connection_errors: bool):
+    def __init__(self, strategy: str, retry_connection_errors: bool):
         self.strategy = strategy
-        self.backoff = backoff
         self.retry_connection_errors = retry_connection_errors
 
 
 class Retries:
     config: RetryConfig
     status_codes: list[str]
```

### Comparing `vesselapi-3.27.1/src/vesselapi/utils/utils.py` & `vesselapi-3.5.2/src/vesselapi/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
 import base64
 import json
 import re
 from dataclasses import Field, dataclass, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from email.message import Message
 from enum import Enum
-from typing import Any, Callable, Optional, Tuple, Union, get_args, get_origin
+from typing import Callable, Optional, Tuple, Union, get_args, get_origin
 from xmlrpc.client import boolean
 
 import dateutil.parser
 import requests
 from dataclasses_json import DataClassJsonMixin
 
 
@@ -28,17 +26,14 @@
 
         return self.client.request(method, url, **kwargs)
 
 
 def configure_security_client(client: requests.Session, security: dataclass):
     client = SecurityClient(client)
 
-    if security is None:
-        return client
-
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
         metadata = sec_field.metadata.get('security')
@@ -108,15 +103,15 @@
             raise Exception('not supported')
     elif scheme_type == "openIdConnect":
         client.client.headers[header_name] = value
     elif scheme_type == 'oauth2':
         client.client.headers[header_name] = value
     elif scheme_type == 'http':
         if sub_type == 'bearer':
-            client.client.headers[header_name] = value.lower().startswith('bearer ') and value or f'Bearer {value}'
+            client.client.headers[header_name] = value
         else:
             raise Exception('not supported')
     else:
         raise Exception('not supported')
 
 
 def _parse_basic_auth_scheme(client: SecurityClient, scheme: dataclass):
@@ -137,91 +132,72 @@
         if field_name == 'password':
             password = value
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
-                 gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(server_url: str, path: str, path_params: dataclass) -> str:
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
-            continue
-
         param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
+        if param_metadata.get('style', 'simple') == 'simple':
+            param = getattr(path_params, field.name)
+            if param is None:
+                continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+            if isinstance(param, list):
+                pp_vals: list[str] = []
+                for pp_val in param:
+                    if pp_val is None:
+                        continue
+                    pp_vals.append(_val_to_string(pp_val))
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            elif isinstance(param, dict):
+                pp_vals: list[str] = []
+                for pp_key in param:
+                    if param[pp_key] is None:
+                        continue
+                    if param_metadata.get('explode'):
+                        pp_vals.append(
+                            f"{pp_key}={_val_to_string(param[pp_key])}")
+                    else:
+                        pp_vals.append(
+                            f"{pp_key},{_val_to_string(param[pp_key])}")
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            elif not isinstance(param, (str, int, float, complex, bool)):
+                pp_vals: list[str] = []
+                param_fields: Tuple[Field, ...] = fields(param)
+                for param_field in param_fields:
+                    param_value_metadata = param_field.metadata.get(
+                        'path_param')
+                    if not param_value_metadata:
+                        continue
 
-        if param is None:
-            continue
+                    parm_name = param_value_metadata.get(
+                        'field_name', field.name)
 
-        f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
-            serialized_params = _get_serialized_params(
-                param_metadata, f_name, param)
-            for key, value in serialized_params.items():
+                    param_field_val = getattr(param, param_field.name)
+                    if param_field_val is None:
+                        continue
+                    if param_metadata.get('explode'):
+                        pp_vals.append(
+                            f"{parm_name}={_val_to_string(param_field_val)}")
+                    else:
+                        pp_vals.append(
+                            f"{parm_name},{_val_to_string(param_field_val)}")
                 path = path.replace(
-                    '{' + key + '}', value, 1)
-        else:
-            if param_metadata.get('style', 'simple') == 'simple':
-                if isinstance(param, list):
-                    pp_vals: list[str] = []
-                    for pp_val in param:
-                        if pp_val is None:
-                            continue
-                        pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                elif isinstance(param, dict):
-                    pp_vals: list[str] = []
-                    for pp_key in param:
-                        if param[pp_key] is None:
-                            continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
-                        else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                elif not isinstance(param, (str, int, float, complex, bool)):
-                    pp_vals: list[str] = []
-                    param_fields: Tuple[Field, ...] = fields(param)
-                    for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
-                        if not param_value_metadata:
-                            continue
-
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
-
-                        param_field_val = getattr(param, param_field.name)
-                        if param_field_val is None:
-                            continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
-                        else:
-                            pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            else:
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
@@ -230,54 +206,40 @@
     for key, value in params.items():
         url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[
-    str, list[str]]:
+def get_query_params(query_params: dataclass) -> dict[str, list[str]]:
+    if query_params is None:
+        return {}
+
     params: dict[str, list[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
-            continue
-
         metadata = field.metadata.get('query_param')
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
-
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
-
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
-            serialized_parms = _get_serialized_params(metadata, f_name, value)
-            for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
-                else:
-                    params[key] = [value]
+            params = params | _get_serialized_query_params(
+                metadata, f_name, getattr(query_params, param_name))
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
-                    metadata, f_name, value)
+                    metadata, f_name, getattr(query_params, param_name))
             elif style == 'form':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, ",")
-            elif style == 'pipeDelimited':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, "|")
+                params = params | _get_form_query_params(
+                    metadata, f_name, getattr(query_params, param_name))
             else:
                 raise Exception('not yet implemented')
     return params
 
 
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
@@ -296,16 +258,16 @@
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
-def _get_serialized_params(metadata: dict, field_name: str, obj: any) -> dict[str, str]:
-    params: dict[str, str] = {}
+def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
+    params: dict[str, list[str]] = {}
 
     serialization = metadata.get('serialization', '')
     if serialization == 'json':
         params[metadata.get("field_name", field_name)] = marshal_json(obj)
 
     return params
 
@@ -328,23 +290,20 @@
                 continue
 
             if isinstance(obj_val, list):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
-                        params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                        params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                     _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
@@ -372,52 +331,50 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, delimiter: str) -> dict[
-    str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
-
-
-SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
-}
+def _get_form_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name)
 
 
-def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[
-    str, any, any]:
+def serialize_request_body(request: dataclass) -> Tuple[str, any, any]:
     if request is None:
         return None, None, None, None
 
-    if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request)
-
-    request_val = getattr(request, request_field_name)
+    request_val = getattr(request, "request")
+    if request_val is None:
+        raise Exception("request body not found")
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
-        if field.name == request_field_name:
+        if field.name == "request":
             request_metadata = field.metadata.get('request')
             break
 
-    if request_metadata is None:
-        raise Exception('invalid request type')
+    if request_metadata is not None:
+        # single request
+        return serialize_content_type('request', request_metadata.get('media_type', 'application/octet-stream'), request_val)
 
-    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    request_fields: Tuple[Field, ...] = fields(request_val)
+    for field in request_fields:
+        req = getattr(request_val, field.name)
+        if req is None:
+            continue
+
+        request_metadata = field.metadata.get('request')
+        if request_metadata is None:
+            raise Exception(
+                f'missing request tag on request body field {field.name}')
+
+        return serialize_content_type(field.name, request_metadata.get('media_type', 'application/octet-stream'), req)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
     if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
     if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
@@ -482,15 +439,15 @@
                         [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
-    str, list[str]]:
+        str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -522,15 +479,15 @@
             field_name = metadata.get('field_name', field.name)
 
             if metadata.get('json'):
                 form[field_name] = [marshal_json(val)]
             else:
                 if metadata.get('style', 'form') == 'form':
                     form = form | _populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")
+                        field_name, metadata.get('explode', True), val, _get_form_field_name)
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
@@ -544,16 +501,15 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, delimiter: str) -> \
-        dict[str, list[str]]:
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
@@ -568,31 +524,31 @@
             if val is None:
                 continue
 
             if explode:
                 params[obj_field_name] = [_val_to_string(val)]
             else:
                 items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                    f'{obj_field_name},{_val_to_string(val)}')
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            params[field_name] = [','.join(items)]
     elif isinstance(obj, dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
                 params[key] = _val_to_string(value)
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f'{key},{_val_to_string(value)}')
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            params[field_name] = [','.join(items)]
     elif isinstance(obj, list):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
@@ -600,15 +556,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join([str(item) for item in items])]
+            params[field_name] = [','.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
@@ -740,22 +696,10 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return str(val.value)
+        return val.value
 
     return str(val)
-
-
-def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
-
-    return value
```

### Comparing `vesselapi-3.27.1/src/vesselapi/webhooks.py` & `vesselapi-3.5.2/src/vesselapi/connections.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,97 @@
-"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
-
-from .sdkconfiguration import SDKConfiguration
+import requests as requests_http
+from . import utils
 from typing import Optional
-from vesselapi import utils
 from vesselapi.models import operations
 
-class Webhooks:
-    sdk_configuration: SDKConfiguration
-
-    def __init__(self, sdk_config: SDKConfiguration) -> None:
-        self.sdk_configuration = sdk_config
-        
-    
-    def create(self, request: operations.PostWebhookRequestBody) -> operations.PostWebhookResponse:
-        r"""Create Webhook
-        Create a new webhook for a given connection
+class Connections:
+    _client: requests_http.Session
+    _security_client: requests_http.Session
+    _server_url: str
+    _language: str
+    _sdk_version: str
+    _gen_version: str
+
+    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
+        self._client = client
+        self._security_client = security_client
+        self._server_url = server_url
+        self._language = language
+        self._sdk_version = sdk_version
+        self._gen_version = gen_version
+        
+    def delete(self, request: operations.DeleteConnectionRequest) -> operations.DeleteConnectionResponse:
+        r"""Delete Connection
+        Remove a connection for a given `connectionId`. Removing a connection disconnects the user's CRM so they'll need to re-authenticate should they want to re-connect their CRM.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/connection/webhook'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/connection/connection'
+        
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request)
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
         
-        client = self.sdk_configuration.security_client
+        client = utils.configure_security_client(self._client, request.security)
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        http_res = client.request('DELETE', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostWebhookResponseBody])
-                res.response_body = out
+            pass
 
         return res
 
-    
-    def delete(self, request: operations.DeleteWebhookRequestBody) -> operations.DeleteWebhookResponse:
-        r"""Remove Webhook
-        Removes a webhook for a given connection and id
+    def find(self, request: operations.GetOneConnectionRequest) -> operations.GetOneConnectionResponse:
+        r"""Get Connection
+        Get info about a connection for a given accessToken.
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/connection/webhook'
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = '*/*'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
         
-        client = self.sdk_configuration.security_client
+        url = base_url.removesuffix('/') + '/connection/connection'
         
-        http_res = client.request('DELETE', url, data=data, files=form, headers=headers)
+        query_params = utils.get_query_params(request.query_params)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.DeleteWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetOneConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneConnectionResponseBody])
+                res.response_body = out
 
         return res
 
-    
-    def find(self, request: operations.GetOneWebhookRequest) -> operations.GetOneWebhookResponse:
-        r"""Get Webhook
-        Retrieve information about a webhook for a given connection and id
+    def list(self) -> operations.GetAllCrmConnectionsResponse:
+        r"""Get All Connections
+        List all established connections for a workspace
         """
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/connection/webhook'
-        headers = {}
-        query_params = utils.get_query_params(operations.GetOneWebhookRequest, request)
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version} {self.sdk_configuration.openapi_doc_version}'
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/connection/connections'
+        
         
-        client = self.sdk_configuration.security_client
+        client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params, headers=headers)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetOneWebhookResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAllCrmConnectionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetOneWebhookResponseBody])
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAllCrmConnectionsResponseBody])
                 res.response_body = out
 
         return res
```

### Comparing `vesselapi-3.27.1/src/vesselapi.egg-info/SOURCES.txt` & `vesselapi-3.5.2/src/vesselapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,112 +1,103 @@
 README.md
 setup.py
 src/vesselapi/__init__.py
 src/vesselapi/accounts.py
 src/vesselapi/attendees.py
-src/vesselapi/calls.py
 src/vesselapi/connections.py
 src/vesselapi/contacts.py
 src/vesselapi/deals.py
 src/vesselapi/emails.py
 src/vesselapi/events.py
 src/vesselapi/integrations.py
 src/vesselapi/leads.py
 src/vesselapi/links.py
 src/vesselapi/notes.py
 src/vesselapi/passthrough.py
 src/vesselapi/sdk.py
-src/vesselapi/sdkconfiguration.py
 src/vesselapi/tasks.py
 src/vesselapi/tokens.py
 src/vesselapi/users.py
 src/vesselapi/webhooks.py
 src/vesselapi.egg-info/PKG-INFO
 src/vesselapi.egg-info/SOURCES.txt
 src/vesselapi.egg-info/dependency_links.txt
 src/vesselapi.egg-info/requires.txt
 src/vesselapi.egg-info/top_level.txt
 src/vesselapi/models/__init__.py
 src/vesselapi/models/operations/__init__.py
 src/vesselapi/models/operations/delete_connection.py
 src/vesselapi/models/operations/delete_webhook.py
 src/vesselapi/models/operations/get_all_crm_accounts.py
-src/vesselapi/models/operations/get_all_crm_calls.py
 src/vesselapi/models/operations/get_all_crm_connections.py
 src/vesselapi/models/operations/get_all_crm_contacts.py
 src/vesselapi/models/operations/get_all_crm_deals.py
 src/vesselapi/models/operations/get_all_crm_emails.py
 src/vesselapi/models/operations/get_all_crm_event_attendees.py
 src/vesselapi/models/operations/get_all_crm_events.py
 src/vesselapi/models/operations/get_all_crm_integrations.py
 src/vesselapi/models/operations/get_all_crm_leads.py
 src/vesselapi/models/operations/get_all_crm_notes.py
 src/vesselapi/models/operations/get_all_crm_tasks.py
 src/vesselapi/models/operations/get_all_crm_users.py
 src/vesselapi/models/operations/get_batch_crm_account.py
-src/vesselapi/models/operations/get_batch_crm_call.py
 src/vesselapi/models/operations/get_batch_crm_contact.py
 src/vesselapi/models/operations/get_batch_crm_deal.py
 src/vesselapi/models/operations/get_batch_crm_email.py
 src/vesselapi/models/operations/get_batch_crm_event.py
 src/vesselapi/models/operations/get_batch_crm_event_attendee.py
 src/vesselapi/models/operations/get_batch_crm_lead.py
 src/vesselapi/models/operations/get_batch_crm_note.py
 src/vesselapi/models/operations/get_batch_crm_task.py
 src/vesselapi/models/operations/get_batch_crm_user.py
 src/vesselapi/models/operations/get_details_crm_account.py
-src/vesselapi/models/operations/get_details_crm_call.py
 src/vesselapi/models/operations/get_details_crm_contact.py
 src/vesselapi/models/operations/get_details_crm_deal.py
 src/vesselapi/models/operations/get_details_crm_email.py
 src/vesselapi/models/operations/get_details_crm_event.py
 src/vesselapi/models/operations/get_details_crm_event_attendee.py
 src/vesselapi/models/operations/get_details_crm_lead.py
 src/vesselapi/models/operations/get_details_crm_note.py
 src/vesselapi/models/operations/get_details_crm_task.py
 src/vesselapi/models/operations/get_details_crm_user.py
 src/vesselapi/models/operations/get_one_connection.py
 src/vesselapi/models/operations/get_one_crm_account.py
-src/vesselapi/models/operations/get_one_crm_call.py
 src/vesselapi/models/operations/get_one_crm_contact.py
 src/vesselapi/models/operations/get_one_crm_deal.py
 src/vesselapi/models/operations/get_one_crm_email.py
 src/vesselapi/models/operations/get_one_crm_event.py
 src/vesselapi/models/operations/get_one_crm_event_attendee.py
 src/vesselapi/models/operations/get_one_crm_lead.py
 src/vesselapi/models/operations/get_one_crm_note.py
 src/vesselapi/models/operations/get_one_crm_task.py
 src/vesselapi/models/operations/get_one_crm_user.py
 src/vesselapi/models/operations/get_one_webhook.py
 src/vesselapi/models/operations/post_crm_account.py
-src/vesselapi/models/operations/post_crm_call.py
 src/vesselapi/models/operations/post_crm_contact.py
 src/vesselapi/models/operations/post_crm_deal.py
 src/vesselapi/models/operations/post_crm_email.py
 src/vesselapi/models/operations/post_crm_event.py
 src/vesselapi/models/operations/post_crm_event_attendee.py
 src/vesselapi/models/operations/post_crm_lead.py
 src/vesselapi/models/operations/post_crm_note.py
 src/vesselapi/models/operations/post_crm_passthrough.py
 src/vesselapi/models/operations/post_crm_task.py
 src/vesselapi/models/operations/post_link_exchange.py
 src/vesselapi/models/operations/post_link_token.py
 src/vesselapi/models/operations/post_webhook.py
 src/vesselapi/models/operations/put_crm_account.py
-src/vesselapi/models/operations/put_crm_call.py
 src/vesselapi/models/operations/put_crm_contact.py
 src/vesselapi/models/operations/put_crm_deal.py
 src/vesselapi/models/operations/put_crm_email.py
 src/vesselapi/models/operations/put_crm_event.py
 src/vesselapi/models/operations/put_crm_event_attendee.py
 src/vesselapi/models/operations/put_crm_lead.py
 src/vesselapi/models/operations/put_crm_note.py
 src/vesselapi/models/operations/put_crm_task.py
 src/vesselapi/models/operations/search_crm_accounts.py
-src/vesselapi/models/operations/search_crm_calls.py
 src/vesselapi/models/operations/search_crm_contacts.py
 src/vesselapi/models/operations/search_crm_deals.py
 src/vesselapi/models/operations/search_crm_emails.py
 src/vesselapi/models/operations/search_crm_event_attendees.py
 src/vesselapi/models/operations/search_crm_events.py
 src/vesselapi/models/operations/search_crm_leads.py
 src/vesselapi/models/operations/search_crm_notes.py
@@ -114,17 +105,14 @@
 src/vesselapi/models/operations/search_crm_users.py
 src/vesselapi/models/shared/__init__.py
 src/vesselapi/models/shared/account.py
 src/vesselapi/models/shared/accountcreate.py
 src/vesselapi/models/shared/accountupdate.py
 src/vesselapi/models/shared/address.py
 src/vesselapi/models/shared/booleanfilter.py
-src/vesselapi/models/shared/call.py
-src/vesselapi/models/shared/callcreate.py
-src/vesselapi/models/shared/callupdate.py
 src/vesselapi/models/shared/connection.py
 src/vesselapi/models/shared/contact.py
 src/vesselapi/models/shared/contactcreate.py
 src/vesselapi/models/shared/contactupdate.py
 src/vesselapi/models/shared/datefilter.py
 src/vesselapi/models/shared/deal.py
 src/vesselapi/models/shared/dealcreate.py
```

