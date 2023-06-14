# Comparing `tmp/odoo14-addon-energy_communities-14.0.1.1.1.tar.gz` & `tmp/odoo14-addon-energy_communities-14.0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo14-addon-energy_communities-14.0.1.1.1.tar", last modified: Fri Mar 31 12:18:45 2023, max compression
+gzip compressed data, was "odoo14-addon-energy_communities-14.0.1.1.2.tar", last modified: Mon Apr  3 14:16:47 2023, max compression
```

## Comparing `odoo14-addon-energy_communities-14.0.1.1.1.tar` & `odoo14-addon-energy_communities-14.0.1.1.2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.986492 odoo14-addon-energy_communities-14.0.1.1.1/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      462 2023-03-31 12:18:45.986492 odoo14-addon-energy_communities-14.0.1.1.1/PKG-INFO
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.974491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.974491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.974491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      145 2023-03-31 12:08:05.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1852 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/__manifest__.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.974491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/controllers/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      116 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/controllers/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      240 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/controllers/controllers.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    10862 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/controllers/website_subscription_main.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    12194 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.978491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1900 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1695 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/crm_lead_tag.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      830 2023-03-24 12:42:10.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/ir_cron.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    12993 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/mail_template_data.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    16958 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/mail_template_update_data.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1931 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/product_data.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      825 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/utm_data.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.978491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/demo/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2663 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/demo/demo_data.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      553 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/hooks.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.978491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    74932 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/ca_ES.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    54300 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/energy_communities.pot
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    75015 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/es.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    75025 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/eu_ES.po
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.978491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n_extra/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)   123966 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n_extra/ca_ES.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)   122892 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n_extra/es.po
--rw-rw-r--   0 daniil    (1000) daniil    (1000)   122896 2023-03-31 08:37:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n_extra/eu_ES.po
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.978491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      374 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      591 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/account_chart_template.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2397 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/account_move.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     4078 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/auth_oauth_provider.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    11809 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/crm_lead.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     5117 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/operation_request.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1489 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/product.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     7508 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/res_company.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1219 2023-03-30 14:28:26.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/res_partner.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     7365 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/res_users.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      139 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/res_users_role.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     4505 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/subscription_request.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      418 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/utm_source.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.982491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/security/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3002 2023-03-31 08:37:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/security/ir_rule_data.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3645 2023-03-27 09:26:17.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/security/res_users_role_data.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.982491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      160 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     5281 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/ce_community_service.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     8407 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/ce_member_profile_service.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     6696 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/ce_member_service.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     7655 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/crm_lead_service.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     6632 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/schemas.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.974491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/static/
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.982491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/static/description/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3721 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/static/description/icon.png
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.982491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       30 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      975 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/common.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      793 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/common_service.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1875 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/test_crm_lead_service.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3347 2023-03-31 11:02:04.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/test_res_company.py
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.982491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1322 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/auth_oauth_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3354 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/ce_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3734 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/crm_lead_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1889 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/menus.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     2307 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/res_company_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      798 2023-03-22 15:41:21.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/res_partner_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      630 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/res_users_role_view.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      656 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/res_users_view.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      607 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/subscription_request_view.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1510 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/utm_views.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      953 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/view_users_form.xml
--rw-rw-r--   0 daniil    (1000) daniil    (1000)    17283 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/website_subscription_template.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.982491 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/wizards/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       41 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/wizards/__init__.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     5119 2023-03-31 12:08:05.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     1598 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
-drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-03-31 12:18:45.986492 odoo14-addon-energy_communities-14.0.1.1.1/odoo14_addon_energy_communities.egg-info/
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      462 2023-03-31 12:18:45.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo14_addon_energy_communities.egg-info/PKG-INFO
--rw-rw-r--   0 daniil    (1000) daniil    (1000)     3921 2023-03-31 12:18:45.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo14_addon_energy_communities.egg-info/SOURCES.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-03-31 12:18:45.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo14_addon_energy_communities.egg-info/dependency_links.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-03-31 12:18:45.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo14_addon_energy_communities.egg-info/not-zip-safe
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      459 2023-03-31 12:18:45.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo14_addon_energy_communities.egg-info/requires.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)        5 2023-03-31 12:18:45.000000 odoo14-addon-energy_communities-14.0.1.1.1/odoo14_addon_energy_communities.egg-info/top_level.txt
--rw-rw-r--   0 daniil    (1000) daniil    (1000)       38 2023-03-31 12:18:45.986492 odoo14-addon-energy_communities-14.0.1.1.1/setup.cfg
--rw-rw-r--   0 daniil    (1000) daniil    (1000)      324 2023-03-31 08:37:08.000000 odoo14-addon-energy_communities-14.0.1.1.1/setup.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.187026 odoo14-addon-energy_communities-14.0.1.1.2/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      462 2023-04-03 14:16:47.187026 odoo14-addon-energy_communities-14.0.1.1.2/PKG-INFO
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.175026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.175026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.175026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      145 2023-03-31 12:08:05.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1852 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/__manifest__.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.175026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/controllers/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      116 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/controllers/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      240 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/controllers/controllers.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    10862 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/controllers/website_subscription_main.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    12263 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.179026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1900 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1695 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/crm_lead_tag.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      830 2023-03-24 12:42:10.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/ir_cron.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    12993 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/mail_template_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    16880 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/mail_template_update_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1931 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/product_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      825 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/utm_data.xml
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.179026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/demo/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2663 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/demo/demo_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      553 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/hooks.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.179026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    75721 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/ca_ES.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    56107 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/energy_communities.pot
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    76207 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/es.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    76207 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/eu_ES.po
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.179026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n_extra/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)   123966 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n_extra/ca_ES.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)   122892 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n_extra/es.po
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)   122896 2023-03-31 08:37:15.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n_extra/eu_ES.po
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.183026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      374 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      591 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/account_chart_template.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2397 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/account_move.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     4078 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/auth_oauth_provider.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    11809 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/crm_lead.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     5117 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/operation_request.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1489 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/product.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     7508 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/res_company.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1219 2023-03-30 14:28:26.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/res_partner.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     7365 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/res_users.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      139 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/res_users_role.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     4551 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/subscription_request.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      418 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/utm_source.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.183026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/security/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3002 2023-03-31 08:37:15.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/security/ir_rule_data.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3645 2023-03-27 09:26:17.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/security/res_users_role_data.xml
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.183026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      160 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     5281 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/ce_community_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     8407 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/ce_member_profile_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     6696 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/ce_member_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     7655 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/crm_lead_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     6632 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/schemas.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.175026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/static/
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.183026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/static/description/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3721 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/static/description/icon.png
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.183026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       30 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      975 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/common.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      793 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/common_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1875 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/test_crm_lead_service.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3347 2023-03-31 11:02:04.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/test_res_company.py
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.187026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1322 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/auth_oauth_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3354 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/ce_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3734 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/crm_lead_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1889 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/menus.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2307 2023-03-31 12:18:15.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/res_company_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      798 2023-03-22 15:41:21.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/res_partner_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      630 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/res_users_role_view.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      656 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/res_users_view.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     2103 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/subscription_request_view.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1510 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/utm_views.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      953 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/view_users_form.xml
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)    17308 2023-04-03 14:14:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/website_subscription_template.xml
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.187026 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/wizards/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       41 2023-03-16 14:10:34.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/wizards/__init__.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     5119 2023-03-31 12:08:05.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     1598 2023-03-22 14:44:43.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml
+drwxrwxr-x   0 daniil    (1000) daniil    (1000)        0 2023-04-03 14:16:47.187026 odoo14-addon-energy_communities-14.0.1.1.2/odoo14_addon_energy_communities.egg-info/
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      462 2023-04-03 14:16:46.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo14_addon_energy_communities.egg-info/PKG-INFO
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)     3921 2023-04-03 14:16:47.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo14_addon_energy_communities.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-04-03 14:16:46.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo14_addon_energy_communities.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        1 2023-04-03 14:16:46.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo14_addon_energy_communities.egg-info/not-zip-safe
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      459 2023-04-03 14:16:46.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo14_addon_energy_communities.egg-info/requires.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)        5 2023-04-03 14:16:46.000000 odoo14-addon-energy_communities-14.0.1.1.2/odoo14_addon_energy_communities.egg-info/top_level.txt
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)       38 2023-04-03 14:16:47.187026 odoo14-addon-energy_communities-14.0.1.1.2/setup.cfg
+-rw-rw-r--   0 daniil    (1000) daniil    (1000)      324 2023-03-31 08:37:08.000000 odoo14-addon-energy_communities-14.0.1.1.2/setup.py
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/__manifest__.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': "Energy Community",
-    'version': '14.0.1.1.1',
+    'version': '14.0.1.1.2',
     'depends': [
         'account',
         'account_payment_order',
         'cooperator',
         'base_technical_features',
         'base_user_role',
         'base_user_role_company',
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/controllers/website_subscription_main.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/controllers/website_subscription_main.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/controllers/website_subscription_voluntary_share.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,35 +253,32 @@
             values["generic_rules_approved"] = True
 
         values["source"] = "website"
         values["company_id"] = kwargs.get("company_id")
         company = request.env['res.company'].sudo().search([('id', '=', values["company_id"])])
 
         if partner:
-            values["email"] = partner.email
+            values["email"] = partner.email or _("Email not found")
             values["phone"] = partner.phone
-            values["lastname"] = partner.lastname
+            values["lastname"] = partner.lastname or ""
             values["firstname"] = partner.firstname or partner.name
-            values["address"] = partner.street
-            values["city"] = partner.city
-            values["zip_code"] = partner.zip
-            values["country_id"] = partner.country_id.id
-            values["lang"] = partner.lang
+            values["address"] = partner.street or _("Address not found")
+            values["city"] = partner.city or _("City not found")
+            values["zip_code"] = partner.zip or _("ZIP code not found")
+            values["country_id"] = partner.country_id.id or company.default_country_id.id
+            values["lang"] = partner.lang or company.default_lang_id.id
             values["birthdate"] = partner.birthdate_date
         else:
-            values["lastname"] = "Partner not found"
-            values["firstname"] = "Partner not found"
-            values["address"] = "Partner not found"
-            values["city"] = "Partner not found"
-            values["zip_code"] = "Partner not found"
+            values["lastname"] = _("Partner not found")
+            values["firstname"] = _("Partner not found")
+            values["address"] = _("Partner not found")
+            values["city"] = _("Partner not found")
+            values["zip_code"] = _("Partner not found")
             values["country_id"] = company.default_country_id.id
             values["lang"] = company.default_lang_id.code
-            values["birthdate"] = datetime.strptime(
-                '2000-01-01', "%Y-%m-%d"
-            ).date()
         values["share_product_id"] = company.voluntary_share_id.id
         subscription_id = sub_req_obj.sudo().create(values)
 
         if partner:
             if partner.email != kwargs.get('email') or partner.phone != kwargs.get('phone'):
                 subscription_id.message_post(**{
                     'subject': 'We found partner discrepancy in the form',
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/auth_oauth_provider_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/crm_lead_tag.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/crm_lead_tag.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/ir_cron.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/ir_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/mail_template_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/mail_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/mail_template_update_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/mail_template_update_data.xml`

 * *Files 1% similar despite different names*

#### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/mail_template_update_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/mail_template_update_data.xml`

```diff
@@ -12,15 +12,15 @@
       <field name="name">Confirmation Email for CE Subscription Request Receipt</field>
       <field name="email_from">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="subject">[Somcomunitats.coop] Application to become Community membership</field>
       <field name="email_to">${object.email}</field>
       <field name="email_cc">info+altausuari@somcomunitats.coop</field>
       <field name="reply_to">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="model_id" ref="model_subscription_request"/>
-      <field name="auto_delete" eval="True"/>
+      <field name="auto_delete" eval="False"/>
       <field name="lang">${(object.lang or object.company_id.default_lang_id.code or object.company_id.partner_id.lang)}</field>
       <field name="is_cooperator_template" eval="True"/>
       <field name="body_html"><![CDATA[
 <div style="font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; ">
 
     <p>Hello,</p>
     <p>Thank you for filling out the form and request to join the Community.</p>
@@ -69,15 +69,15 @@
       <field name="subject">[Somcomunitats.coop] Request to become member of Energy Community
                 ${object.company_id.name}</field>
       <field name="partner_to">${object.partner_id.id}</field>
       <field name="email_cc">info+altausuari@somcomunitats.coop</field>
       <!--<field name="email_bcc">${object.company_id.email}</field>-->
       <field name="reply_to">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="model_id" ref="account.model_account_move"/>
-      <field name="auto_delete" eval="True"/>
+      <field name="auto_delete" eval="False"/>
       <field name="report_template"/>
       <!--
             <field name="report_template" ref="action_cooperator_invoices" />
             <field
                 name="report_name"
             >${(object.name or "capital_release_request").replace("/", "_")}${object.state == "draft" and "_draft" or ""}</field>
              -->
@@ -147,15 +147,15 @@
       <field name="email_from">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="subject">Wellcome to the Energy Community ${object.env.company.name}!</field>
       <field name="partner_to">${object.id}</field>
       <field name="email_cc">info+altausuari@somcomunitats.coop</field>
       <!--<field name="email_bcc">${object.company_id.email}</field>-->
       <field name="reply_to">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="model_id" ref="model_res_partner"/>
-      <field name="auto_delete" eval="True"/>
+      <field name="auto_delete" eval="False"/>
       <field name="report_template"/>
       <!--
             <field name="report_template" ref="action_cooperator_report_certificat" />
             <field
                 name="report_name"
             >Certificate ${(object.cooperator_register_number or '')}</field>
             -->
@@ -215,15 +215,15 @@
       <field name="name">Confirmation Email for CE Subscription Request Receipt</field>
       <field name="email_from">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="subject">[Somcomunitats.coop] Application to become Community membership</field>
       <field name="email_to">${object.email}</field>
       <field name="email_cc">info+altausuari@somcomunitats.coop</field>
       <field name="reply_to">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="model_id" ref="model_subscription_request"/>
-      <field name="auto_delete" eval="True"/>
+      <field name="auto_delete" eval="False"/>
       <field name="lang">${(object.lang or object.company_id.default_lang_id.code or object.company_id.partner_id.lang)}</field>
       <field name="is_cooperator_template" eval="True"/>
       <field name="body_html"><![CDATA[
 <div style="font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; ">
 
     <p>Hello,</p>
     <p>Thank you for filling out the form and request to join the Community.</p>
@@ -260,19 +260,18 @@
       <field name="name">Confirmation Email for CE Voluntary Share Receipt</field>
       <field name="email_from">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="subject">Contribute to ${object.company_id.name} Ref. ACSV${object.id}</field>
       <field name="email_to">${object.email}</field>
       <field name="email_cc"/>
       <field name="reply_to">${(object.company_id.coop_email_contact or object.company_id.email)|safe}</field>
       <field name="model_id" ref="model_subscription_request"/>
-      <field name="auto_delete" eval="True"/>
+      <field name="auto_delete" eval="False"/>
       <field name="lang">${(object.lang or object.company_id.default_lang_id.code or object.company_id.partner_id.lang)}</field>
       <field name="is_cooperator_template" eval="True"/>
       <field name="body_html"><![CDATA[
-<img src="data:image/png;base64,${object.company_id.logo}" style="width: 150px;height: 80px;" />
     <p>Dear ${object.firstname},</p>
     <p>
         We confirm that we have correctly received your request to make a voluntary contribution to the capital
         social of <b>${object.company_id.name}</b>, with the following data:
     </p>
     <ul>
         <li>Partner VAT: <b>${object.vat}</b></li>
@@ -306,11 +305,12 @@
     </p>
     <p>
         Sincerely,
     </p>
     <p>
         ${object.company_id.name} team
     </p>
+    <img src="/web/image/res.company/${object.company_id.id}/logo" style="width: 150px;height: 80px;"/>
             ]]></field>
     </record>
   </data>
 </odoo>
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/product_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/product_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/data/utm_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/data/utm_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/demo/demo_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/demo/demo_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/hooks.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/hooks.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/ca_ES.po` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/ca_ES.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-31 08:40+0000\n"
-"PO-Revision-Date: 2023-03-31 10:56+0200\n"
+"POT-Creation-Date: 2023-04-03 13:22+0000\n"
+"PO-Revision-Date: 2023-04-03 15:43+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: ca_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: \n"
@@ -28,14 +28,123 @@
 msgstr ""
 "\n"
 "        El NIF/CIF. Completa aquest camp si el contacte està subjecte a\n"
 "        les taxes estatals. Es fa servir en alguns  informes legals.\"\n"
 "        "
 
 #. module: energy_communities
+#: model:mail.template,body_html:energy_communities.email_template_confirmation_voluntary_share
+msgid ""
+"\n"
+"    <p>Dear ${object.firstname},</p>\n"
+"    <p>\n"
+"        We confirm that we have correctly received your request to make a "
+"voluntary contribution to the capital\n"
+"        social of <b>${object.company_id.name}</b>, with the following "
+"data:\n"
+"    </p>\n"
+"    <ul>\n"
+"        <li>Partner VAT: <b>${object.vat}</b></li>\n"
+"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
+"li>\n"
+"        <li>Charging account: <b>${object.iban}</b></li>\n"
+"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
+"li>\n"
+"    </ul>\n"
+"    <p>\n"
+"        In the next few days you will receive the bank charge in this "
+"account, please verify that all the data\n"
+"        provided is correct and you have the money you want to invest, to "
+"avoid any incident in the\n"
+"        draft of the receipt.\n"
+"    </p>\n"
+"    <p>\n"
+"        Once the validity of the payment has been verified, you will "
+"receive a new notification confirming the\n"
+"        contribution\n"
+"        made and detailing the particular conditions of your contribution.\n"
+"    </p>\n"
+"    <p>\n"
+"        Thank you for your involvement with the cooperative and inform you "
+"that for any doubt or clarification you can\n"
+"        consult\n"
+"        our website:\n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
+"        or send us an email to\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
+"    </p>\n"
+"    <p>\n"
+"        Get the word out by explaining the project to family and friends. "
+"The more we are, the further we will go!\n"
+"    </p>\n"
+"    <p>\n"
+"        Thank you very much and good energy!\n"
+"    </p>\n"
+"    <p>\n"
+"        Sincerely,\n"
+"    </p>\n"
+"    <p>\n"
+"        ${object.company_id.name} team\n"
+"    </p>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
+"            "
+msgstr ""
+"\n"
+"    <p>Apreciat/ada ${object.firstname},</p>\n"
+"    <p>\n"
+"        Et confirmem que hem rebut correctament la teva sol·licitud per "
+"realitzar una aportació voluntària al capital social de <b>${object."
+"company_id.name}</b>, amb les següents dades:\n"
+"    </p>\n"
+"    <ul>\n"
+"        <li>Soci/sòcia NIF: <b>${object.vat}</b></li>\n"
+"        <li>Soci/sòcia: <b>${object.firstname} ${object.lastname}</b></li>\n"
+"        <li>Compte bancari: <b>${object.iban}</b></li>\n"
+"        <li>Import d'aportació: <b>${object.subscription_amount}€</b></li>\n"
+"    </ul>\n"
+"    <p>\n"
+"En els pròxims dies rebràs el càrrec bancari en aquest compte, si us plau "
+"verifica que totes les teves dades siguin correctes i disposis dels diners "
+"que vulguis invertir, per evitar qualsevol incidència en el gir del rebut.\n"
+"    </p>\n"
+"    <p>\n"
+"Una vegada verificat el pagament, rebràs una notificació confirmant "
+"l'aportació realitzada i detallant les condicions particulars de la teva "
+"aportació.\n"
+"    </p>\n"
+"    <p>\n"
+"Agraïm la teva implicació amb la cooperativa i t'informem que pots aclarir "
+"qualsevol dubte en la nostra pàgina web \n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
+"o enviar-nos un correu electrònic a\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
+"    </p>\n"
+"    <p>\n"
+"Fes que corri la veu explicant el nostre projecte a familiars i amics/"
+"amigues. Com més siguem, més lluny arribarem!\n"
+"    </p>\n"
+"    <p>\n"
+"Moltes gràcies i bona energia!\n"
+"    </p>\n"
+"    <p>\n"
+"        Atentament,\n"
+"    </p>\n"
+"    <p>\n"
+"        L'equip de ${object.company_id.name}\n"
+"    </p>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
+"            "
+
+#. module: energy_communities
 #: model:mail.template,body_html:energy_communities.email_templ_lead_request_contact_confirm_id
 msgid ""
 "\n"
 "<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
 "serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
 "\">\n"
 "\n"
@@ -589,151 +698,35 @@
 "    <p>Equip Somcomunitats.coop</p>\n"
 "    <p><a href=\"https://web-test.somcomunitats.coop/recursos/\">Resources "
 "and FAQs</a></p>\n"
 "</div>\n"
 "            "
 
 #. module: energy_communities
-#: model:mail.template,body_html:energy_communities.email_template_confirmation_voluntary_share
-msgid ""
-"\n"
-"<img src=\"data:image/png;base64,${object.company_id.logo}\" style=\"width: "
-"150px;height: 80px;\" />\n"
-"    <p>Dear ${object.firstname},</p>\n"
-"    <p>\n"
-"        We confirm that we have correctly received your request to make a "
-"voluntary contribution to the capital\n"
-"        social of <b>${object.company_id.name}</b>, with the following "
-"data:\n"
-"    </p>\n"
-"    <ul>\n"
-"        <li>Partner VAT: <b>${object.vat}</b></li>\n"
-"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
-"li>\n"
-"        <li>Charging account: <b>${object.iban}</b></li>\n"
-"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
-"li>\n"
-"    </ul>\n"
-"    <p>\n"
-"        In the next few days you will receive the bank charge in this "
-"account, please verify that all the data\n"
-"        provided is correct and you have the money you want to invest, to "
-"avoid any incident in the\n"
-"        draft of the receipt.\n"
-"    </p>\n"
-"    <p>\n"
-"        Once the validity of the payment has been verified, you will "
-"receive a new notification confirming the\n"
-"        contribution\n"
-"        made and detailing the particular conditions of your contribution.\n"
-"    </p>\n"
-"    <p>\n"
-"        Thank you for your involvement with the cooperative and inform you "
-"that for any doubt or clarification you can\n"
-"        consult\n"
-"        our website:\n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id."
-"website}</a>\n"
-"        or send us an email to\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
-"a>\n"
-"    </p>\n"
-"    <p>\n"
-"        Get the word out by explaining the project to family and friends. "
-"The more we are, the further we will go!\n"
-"    </p>\n"
-"    <p>\n"
-"        Thank you very much and good energy!\n"
-"    </p>\n"
-"    <p>\n"
-"        Sincerely,\n"
-"    </p>\n"
-"    <p>\n"
-"        ${object.company_id.name} team\n"
-"    </p>\n"
-"            "
-msgstr ""
-"\n"
-"<img src=\"data:image/png;base64,${object.company_id.logo}\" style=\"width: "
-"150px;height: 80px;\" />\n"
-"     <p>Benvolgut ${object.firstname},</p>\n"
-"     <p>\n"
-"         Confirmem que hem rebut correctament la vostra sol·licitud per fer "
-"una aportació voluntària al capital\n"
-"         social de <b>${object.company_id.name}</b>, amb les dades "
-"següents:\n"
-"     </p>\n"
-"     <ul>\n"
-"         <li>NIF del soci: <b>${object.vat}</b></li>\n"
-"         <li>Nom del soci: <b>${object.firstname} ${object.lastname}</b></"
-"li>\n"
-"         <li>Compte de càrrega: <b>${object.iban}</b></li>\n"
-"         <li>Import de la aportació: <b>${object.subscription_amount}â¬</"
-"b></li>\n"
-"     </ul>\n"
-"     <p>\n"
-"         En els dies vinents rebreu el càrrec bancari en aquest compte, si "
-"us plau, comproveu que totes les dades\n"
-"         proporcionat són correctes i tens els diners que vols aportar, per "
-"evitar qualsevol incidència en el\n"
-"         càrrec del rebut.\n"
-"     </p>\n"
-"     <p>\n"
-"         Un cop verificada la validesa del pagament, rebràs una nova "
-"notificació confirmant la\n"
-"         contribució\n"
-"         realitzada i detallant les condicions particulars de la seva "
-"aportació.\n"
-"     </p>\n"
-"     <p>\n"
-"         Agraïm la vostra implicació amb la cooperativa i us informem que "
-"per qualsevol dubte o aclariment podeu\n"
-"         consultar\n"
-"         el nostre lloc web:\n"
-"         <a href=\"${object.company_id.website}\"> ${object.company_id."
-"website}</a>\n"
-"         o envia'ns un correu electrònic a\n"
-"         <a href=\"${object.company_id.email}\">${object.company_id.email}</"
-"a>\n"
-"     </p>\n"
-"     <p>\n"
-"         Fes difusió explicant el projecte a familiars i amics. Com més "
-"siguem, més lluny anirem!\n"
-"     </p>\n"
-"     <p>\n"
-"         Moltes gràcies i molta energia!\n"
-"     </p>\n"
-"     <p>\n"
-"         Sincerament,\n"
-"     </p>\n"
-"     <p>\n"
-"         Equip de ${object.company_id.name}\n"
-"     </p>"
-
-#. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser_pwd
 msgid "\"Superuser\" user password"
 msgstr "Contrasenya del super-usuari"
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser
 msgid "A super power user that is able to CRUD users on KC."
 msgstr "Un super-usuari amb permisos pper CRUD en KC."
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
-msgid "Accept to make the payment via SEPA transfer."
-msgstr "Accepto rebre el pagament a partir de domiciliació SEPA."
-
-#. module: energy_communities
 #: model:ir.model,name:energy_communities.model_account_chart_template
 msgid "Account Chart Template"
 msgstr "Plantilla de gràfic de comptes"
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Address not found"
+msgstr "Adreça no trobada"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__is_admin_provider
 msgid "Admin provider"
 msgstr "ProveÏdor AUTH  taques administratives"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_admin
 msgid "Administrator"
@@ -830,14 +823,20 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__chart_template_id
 msgid "Chart Template"
 msgstr "Plantilla plan contable"
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "City not found"
+msgstr "Ciutat no trobada"
+
+#. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_utm_sources_action
 msgid "Click to define a new Source."
 msgstr "Clica per definir un nou Source."
 
 #. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_crm_lead_tags_action
 msgid "Click to define a new tag."
@@ -846,14 +845,15 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__code
 msgid "Code"
 msgstr "Codi"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__community
 #, python-format
 msgid "Community"
 msgstr "Comunitat"
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_crm_lead__community_company_id
 msgid "Community related to this Lead"
@@ -871,19 +871,14 @@
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_collective_purchases
 msgid "Compres col·lectives"
 msgstr "Compres col·lectives"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__community
-msgid "Comunidad"
-msgstr "Comunitat"
-
-#. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_config_menu
 msgid "Configuration"
 msgstr "Configuració"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Confirm Email"
@@ -920,15 +915,15 @@
 msgid "Contribution to Share Capital"
 msgstr "Aportació al Capital Social"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "Converting just part of the shares is not yet implemented"
-msgstr "Convertir només part de les aportacions no està encara implementat"
+msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.wizard_multicompany_easy_creation_form_inherit
 msgid "Cooperator"
 msgstr "Sòcia"
 
 #. module: energy_communities
@@ -938,20 +933,16 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__cooperator_journal
 msgid "Cooperator Journal"
 msgstr "Diari Sòcies"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
-msgid "Coordinadora"
-msgstr "Coordinadora"
-
-#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
 #, python-format
 msgid "Coordinator"
 msgstr "Coordinadora"
 
 #. module: energy_communities
 #: model:ir.actions.server,name:energy_communities.action_create_map_place_from_lead
 msgid "Create Map Place"
@@ -1021,15 +1012,21 @@
 msgstr "Email"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Email and confirmation email addresses don't match."
-msgstr "El correu i el correu de confirmació no coincideixen."
+msgstr "El correu de confirmació no coincideix amb l'email introduït."
+
+#. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Email not found"
+msgstr "Email no trobat"
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_thermal_energy
 msgid "Energia tèrmica i climatització"
 msgstr "Energia tèrmica i climatització"
 
 #. module: energy_communities
@@ -1093,20 +1090,20 @@
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__gender
 msgid "Gender"
 msgstr "Gènere"
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_common_generation
 msgid "Generació renovable comunitaria"
-msgstr "Generació renovable comunitaria"
+msgstr ""
 
 #. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_menu_general_settings
 msgid "General"
-msgstr "General"
+msgstr ""
 
 #. module: energy_communities
 #: model:ir.actions.act_window,name:energy_communities.ce_crm_leads_general_info_action
 #: model:ir.ui.menu,name:energy_communities.ce_crm_leads_general_info_menu
 msgid "General Information"
 msgstr "Informació general"
 
@@ -1117,14 +1114,19 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__hierarchy_level
 msgid "Hierarchy level"
 msgstr "Nivell jeràrquic"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
+msgid "I accept that the entity issues direct debit receipts to this account."
+msgstr "Accepto que l'entitat emeti rebuts domiciliats a aquest compte."
+
+#. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__gender__not_share
 #: model:ir.model.fields.selection,name:energy_communities.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
 msgstr "Prefereixo no compartir-ho"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_chart_template__id
@@ -1138,15 +1140,15 @@
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_partner__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_users__id
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__id
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__id
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source__id
 msgid "ID"
-msgstr "ID"
+msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_mailing_mailing__source_ext_id
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source__source_ext_id
 msgid "ID Ext Source"
 msgstr ""
 
@@ -1195,32 +1197,28 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__capital_share
 msgid "Initial capital share"
 msgstr "Quota inicial alta sòcia"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
 #, python-format
 msgid "Instance"
 msgstr "Instància"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
-msgid "Instancia"
-msgstr "Instància"
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__is_voluntary
 msgid "Is voluntary contribution"
 msgstr "És una aportació voluntària"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_account_move
 msgid "Journal Entry"
-msgstr "Assentament comptable"
+msgstr "Assentament"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__is_keycloak_provider
 msgid "Keycloak provider"
 msgstr "Proveïdor KeyCloak"
 
 #. module: energy_communities
@@ -1259,28 +1257,30 @@
 #. module: energy_communities
 #: model:auth.oauth.provider,body:energy_communities.keycloak_admin_provider
 #: model:auth.oauth.provider,body:energy_communities.keycloak_login_provider
 msgid "Login with Keycloak"
 msgstr "Registrar-se amb KeyCloak"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
+msgid "Mandatory Shares"
+msgstr "Aportacions obligatòries"
+
+#. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_sustainable_mobility
 msgid "Mobilitat sostenible"
 msgstr "Mobilitat sostenible"
 
 #. module: energy_communities
 #: model:ir.module.category,description:energy_communities.energy_communities_category
 msgid ""
 "Nivell d'Accés dels usuaris a la plataforma Odoo de les Comunitats "
 "Energètiques\n"
 "        "
 msgstr ""
-"Nivell d'Accés dels usuaris a la plataforma Odoo de les Comunitats "
-"Energètiques\n"
-"        "
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_community_service.py:0
 #, python-format
 msgid "No Odoo Company found for odoo_company_id %s"
 msgstr ""
 "No s'ha trobat cap companya al Odoo pel paràmetre: odoo_company_id= %s"
@@ -1391,14 +1391,20 @@
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "Parent company must be instance hierarchy level."
 msgstr "L'empresa principal ha de tenir nivell d'Instància."
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Partner not found"
+msgstr "Soci no trobat"
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Phone"
 msgstr "Telèfon"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_platform_manager
 msgid "Platform Manager"
@@ -1411,15 +1417,14 @@
 msgstr "Rol d'Administradora de Instància"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "Please upload a scan of your ID card."
 msgstr ""
-"Si us plau puja una imatge escanejada de la teva tarja d'identificació."
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__product_share_template
 msgid "Product Share Template"
 msgstr "Plantilla de producte aportació"
 
 #. module: energy_communities
@@ -1428,15 +1433,15 @@
 msgstr "Plantilla de producte"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Provided IBAN is not valid."
-msgstr "L'IBANproporcionat no és vàlid."
+msgstr "L'IBAN no és vàlid."
 
 #. module: energy_communities
 #: model:ir.actions.server,name:energy_communities.print_instance
 msgid "Push user to Keycloak"
 msgstr "Enviar usuari al KeyCloak"
 
 #. module: energy_communities
@@ -1459,15 +1464,15 @@
 msgid "Root URL"
 msgstr "URL arrel"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/account_chart_template.py:0
 #, python-format
 msgid "SUBJ"
-msgstr "SUBJ"
+msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Send"
 msgstr "Enviar"
 
 #. module: energy_communities
@@ -1480,15 +1485,15 @@
 msgid "Share type"
 msgstr "Tipus d'aportació"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "Some mandatory fields have not been filled."
-msgstr "Alguns camps obligatoris no han estat omplerts."
+msgstr "Alguns camps no s'han omplert."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_users.py:0
 #, python-format
 msgid "Something went wrong. Please check logs."
 msgstr "Quelcom ha anat malament. Si us plau revisa els LOGS."
 
@@ -1507,15 +1512,15 @@
 #: model:ir.actions.act_window,name:energy_communities.ce_utm_sources_action
 msgid "Sources"
 msgstr "Origens"
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_renewable_energy
 msgid "Subministrament d'energia 100% renovable"
-msgstr "Subministrament d'energia 100% renovable"
+msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/account_chart_template.py:0
 #, python-format
 msgid "Subscription Journal"
 msgstr "Diari de subscripcions"
 
@@ -1661,21 +1666,21 @@
 msgid "This language code %s is not active in Odoo. Active ones: %s"
 msgstr "Aquest codi d'idioma %s no està actiu a l'Odoo. Els actius són: %s"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "This operation is not yet implemented."
-msgstr "Aquesta operació encara no està implementada."
+msgstr "Aquesta funcionalitat encara no està implementada."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "This operation must be approved before to be executed"
-msgstr "Aquesta operació cal aprovar-la abans d'executar-se"
+msgstr "L'operació ha de ser aprovada abans d'executar-se"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid ""
 "To be a member you must fulfill this form and lateron proceed to pay the "
 "initial share of"
@@ -1814,14 +1819,19 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
 msgid "Voluntary Share of"
 msgstr "Aportació voluntaria de"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
+msgid "Voluntary Shares"
+msgstr "Aportacions voluntàries"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__voluntary_share_id
 msgid "Voluntary share to show on website"
 msgstr "Formulari d'aportació voluntària per ensenyar a la web"
 
 #. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_menu_webforms_settings
 msgid "Webforms"
@@ -1848,35 +1858,40 @@
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid ""
 "You can't subscribe for an amount that exceeds {amount}{currency_symbol}."
 msgstr ""
-"No pots subscriure't per un import superior a {amount}{currency_symbol}."
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "You can't subscribe to two different types of share."
-msgstr "No pots subscriure't a 2 tipus d'aportacions diferents."
+msgstr ""
+
+#. module: energy_communities
+#: code:addons/energy_communities/models/subscription_request.py:0
+#, python-format
+msgid "You can't validate a voluntary contribution in this versión."
+msgstr "No pots validar aportacions voluntàries en aquesta versió."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "You cannot create a instance company with a parent company."
 msgstr ""
 "Ho hi pot haver una empresa de nivell Instància que tingui una empresa "
 "principal assignada."
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "You must check the SEPA transference."
-msgstr ""
+msgstr "Has d'acceptar la transferència per SEPA."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/account_move.py:0
 #, python-format
 msgid ""
 "You must have a company specific sequence number for register.operation"
 msgstr ""
@@ -1896,14 +1911,20 @@
 #: code:addons/energy_communities/models/subscription_request.py:0
 #, python-format
 msgid "You must set a cooperator journal on you company."
 msgstr ""
 "Cal sel·leccionar un Diari específic per a Sòcies en aquesta companyia."
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "ZIP code not found"
+msgstr "Codi postal no trobat"
+
+#. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_template_confirmation_company
 msgid "[Somcomunitats.coop] Application to become Community membership"
 msgstr "[Somcomunitats.coop] Sol·licitud d'adhesió a Comunitat Energètica"
 
 #. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_templ_lead_request_contact_confirm_id
 msgid "[Somcomunitats.coop] Community Contact Request"
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/energy_communities.pot` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/energy_communities.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-31 08:38+0000\n"
-"PO-Revision-Date: 2023-03-31 08:38+0000\n"
+"POT-Creation-Date: 2023-04-03 13:21+0000\n"
+"PO-Revision-Date: 2023-04-03 13:21+0000\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Plural-Forms: \n"
 
@@ -21,14 +21,63 @@
 "\n"
 "        The Tax Identification Number. Complete it if the contact is subjected to\n"
 "        government taxes. Used in some legal statements.\"\n"
 "        "
 msgstr ""
 
 #. module: energy_communities
+#: model:mail.template,body_html:energy_communities.email_template_confirmation_voluntary_share
+msgid ""
+"\n"
+"    <p>Dear ${object.firstname},</p>\n"
+"    <p>\n"
+"        We confirm that we have correctly received your request to make a voluntary contribution to the capital\n"
+"        social of <b>${object.company_id.name}</b>, with the following data:\n"
+"    </p>\n"
+"    <ul>\n"
+"        <li>Partner VAT: <b>${object.vat}</b></li>\n"
+"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></li>\n"
+"        <li>Charging account: <b>${object.iban}</b></li>\n"
+"        <li>Subscription amount: <b>${object.subscription_amount}€</b></li>\n"
+"    </ul>\n"
+"    <p>\n"
+"        In the next few days you will receive the bank charge in this account, please verify that all the data\n"
+"        provided is correct and you have the money you want to invest, to avoid any incident in the\n"
+"        draft of the receipt.\n"
+"    </p>\n"
+"    <p>\n"
+"        Once the validity of the payment has been verified, you will receive a new notification confirming the\n"
+"        contribution\n"
+"        made and detailing the particular conditions of your contribution.\n"
+"    </p>\n"
+"    <p>\n"
+"        Thank you for your involvement with the cooperative and inform you that for any doubt or clarification you can\n"
+"        consult\n"
+"        our website:\n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>\n"
+"        or send us an email to\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a>\n"
+"    </p>\n"
+"    <p>\n"
+"        Get the word out by explaining the project to family and friends. The more we are, the further we will go!\n"
+"    </p>\n"
+"    <p>\n"
+"        Thank you very much and good energy!\n"
+"    </p>\n"
+"    <p>\n"
+"        Sincerely,\n"
+"    </p>\n"
+"    <p>\n"
+"        ${object.company_id.name} team\n"
+"    </p>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" style=\"width: 150px;height: 80px;\"/>\n"
+"            "
+msgstr ""
+
+#. module: energy_communities
 #: model:mail.template,body_html:energy_communities.email_templ_lead_request_contact_confirm_id
 msgid ""
 "\n"
 "<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; \">\n"
 "\n"
 "    <p>Hello,</p>\n"
 "\n"
@@ -271,80 +320,32 @@
 "    <p>Somcomunitats.coop team </p>\n"
 "    <p><a href=\"https://web-test.somcomunitats.coop/recursos/\">Resources and FAQs</a></p>\n"
 "</div>\n"
 "            "
 msgstr ""
 
 #. module: energy_communities
-#: model:mail.template,body_html:energy_communities.email_template_confirmation_voluntary_share
-msgid ""
-"\n"
-"<img src=\"data:image/png;base64,${object.company_id.logo}\" style=\"width: 150px;height: 80px;\" />\n"
-"    <p>Dear ${object.firstname},</p>\n"
-"    <p>\n"
-"        We confirm that we have correctly received your request to make a voluntary contribution to the capital\n"
-"        social of <b>${object.company_id.name}</b>, with the following data:\n"
-"    </p>\n"
-"    <ul>\n"
-"        <li>Partner VAT: <b>${object.vat}</b></li>\n"
-"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></li>\n"
-"        <li>Charging account: <b>${object.iban}</b></li>\n"
-"        <li>Subscription amount: <b>${object.subscription_amount}€</b></li>\n"
-"    </ul>\n"
-"    <p>\n"
-"        In the next few days you will receive the bank charge in this account, please verify that all the data\n"
-"        provided is correct and you have the money you want to invest, to avoid any incident in the\n"
-"        draft of the receipt.\n"
-"    </p>\n"
-"    <p>\n"
-"        Once the validity of the payment has been verified, you will receive a new notification confirming the\n"
-"        contribution\n"
-"        made and detailing the particular conditions of your contribution.\n"
-"    </p>\n"
-"    <p>\n"
-"        Thank you for your involvement with the cooperative and inform you that for any doubt or clarification you can\n"
-"        consult\n"
-"        our website:\n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id.website}</a>\n"
-"        or send us an email to\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</a>\n"
-"    </p>\n"
-"    <p>\n"
-"        Get the word out by explaining the project to family and friends. The more we are, the further we will go!\n"
-"    </p>\n"
-"    <p>\n"
-"        Thank you very much and good energy!\n"
-"    </p>\n"
-"    <p>\n"
-"        Sincerely,\n"
-"    </p>\n"
-"    <p>\n"
-"        ${object.company_id.name} team\n"
-"    </p>\n"
-"            "
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser_pwd
 msgid "\"Superuser\" user password"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser
 msgid "A super power user that is able to CRUD users on KC."
 msgstr ""
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
-msgid "Accept to make the payment via SEPA transfer."
+#: model:ir.model,name:energy_communities.model_account_chart_template
+msgid "Account Chart Template"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model,name:energy_communities.model_account_chart_template
-msgid "Account Chart Template"
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Address not found"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__is_admin_provider
 msgid "Admin provider"
 msgstr ""
 
@@ -361,14 +362,15 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__allow_new_members
 msgid "Allow new members"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "An instance company already exists"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__mandate_approved
 msgid "Approved SEPA"
@@ -445,14 +447,20 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__chart_template_id
 msgid "Chart Template"
 msgstr ""
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "City not found"
+msgstr ""
+
+#. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_utm_sources_action
 msgid "Click to define a new Source."
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_crm_lead_tags_action
 msgid "Click to define a new tag."
@@ -461,14 +469,15 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__code
 msgid "Code"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__community
 #, python-format
 msgid "Community"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_crm_lead__community_company_id
 msgid "Community related to this Lead"
@@ -486,19 +495,14 @@
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_collective_purchases
 msgid "Compres col·lectives"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__community
-msgid "Comunidad"
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_config_menu
 msgid "Configuration"
 msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Confirm Email"
@@ -550,20 +554,16 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__cooperator_journal
 msgid "Cooperator Journal"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
-msgid "Coordinadora"
-msgstr ""
-
-#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
 #, python-format
 msgid "Coordinator"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.actions.server,name:energy_communities.action_create_map_place_from_lead
 msgid "Create Map Place"
@@ -636,14 +636,20 @@
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Email and confirmation email addresses don't match."
 msgstr ""
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Email not found"
+msgstr ""
+
+#. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_thermal_energy
 msgid "Energia tèrmica i climatització"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.actions.act_window,name:energy_communities.ce_crm_lead_tags_action
 msgid "Energy Actions"
@@ -729,14 +735,19 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__hierarchy_level
 msgid "Hierarchy level"
 msgstr ""
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
+msgid "I accept that the entity issues direct debit receipts to this account."
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__gender__not_share
 #: model:ir.model.fields.selection,name:energy_communities.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_chart_template__id
@@ -807,24 +818,20 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__capital_share
 msgid "Initial capital share"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
 #, python-format
 msgid "Instance"
 msgstr ""
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
-msgid "Instancia"
-msgstr ""
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__is_voluntary
 msgid "Is voluntary contribution"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_account_move
 msgid "Journal Entry"
@@ -871,14 +878,19 @@
 #. module: energy_communities
 #: model:auth.oauth.provider,body:energy_communities.keycloak_admin_provider
 #: model:auth.oauth.provider,body:energy_communities.keycloak_login_provider
 msgid "Login with Keycloak"
 msgstr ""
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
+msgid "Mandatory Shares"
+msgstr ""
+
+#. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_sustainable_mobility
 msgid "Mobilitat sostenible"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.module.category,description:energy_communities.energy_communities_category
 msgid ""
@@ -978,25 +990,37 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__parent_id_filtered_ids
 msgid "Parent Id Filtered"
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "Parent company must be coordinator hierarchy level."
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "Parent company must be instance hierarchy level."
 msgstr ""
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Partner not found"
+msgstr ""
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Phone"
 msgstr ""
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_platform_manager
 msgid "Platform Manager"
@@ -1378,14 +1402,19 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
 msgid "Voluntary Share of"
 msgstr ""
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
+msgid "Voluntary Shares"
+msgstr ""
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__voluntary_share_id
 msgid "Voluntary share to show on website"
 msgstr ""
 
 #. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_menu_webforms_settings
 msgid "Webforms"
@@ -1420,14 +1449,21 @@
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "You can't subscribe to two different types of share."
 msgstr ""
 
 #. module: energy_communities
+#: code:addons/energy_communities/models/subscription_request.py:0
+#, python-format
+msgid "You can't validate a voluntary contribution in this versión."
+msgstr ""
+
+#. module: energy_communities
+#: code:addons/energy_communities/models/res_company.py:0
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "You cannot create a instance company with a parent company."
 msgstr ""
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
@@ -1452,14 +1488,20 @@
 #. module: energy_communities
 #: code:addons/energy_communities/models/subscription_request.py:0
 #, python-format
 msgid "You must set a cooperator journal on you company."
 msgstr ""
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "ZIP code not found"
+msgstr ""
+
+#. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_template_confirmation_company
 msgid "[Somcomunitats.coop] Application to become Community membership"
 msgstr ""
 
 #. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_templ_lead_request_contact_confirm_id
 msgid "[Somcomunitats.coop] Community Contact Request"
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/es.po` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/es.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-31 08:40+0000\n"
-"PO-Revision-Date: 2023-03-31 11:09+0200\n"
+"POT-Creation-Date: 2023-04-03 13:46+0000\n"
+"PO-Revision-Date: 2023-04-03 15:56+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: \n"
@@ -28,14 +28,124 @@
 msgstr ""
 "\n"
 "        El NIF/CIF. Completa este campo si el contacto está subjecto a\n"
 "        las tasas estatales. Se usa en algunos informes legales.\"\n"
 "        "
 
 #. module: energy_communities
+#: model:mail.template,body_html:energy_communities.email_template_confirmation_voluntary_share
+msgid ""
+"\n"
+"    <p>Dear ${object.firstname},</p>\n"
+"    <p>\n"
+"        We confirm that we have correctly received your request to make a "
+"voluntary contribution to the capital\n"
+"        social of <b>${object.company_id.name}</b>, with the following "
+"data:\n"
+"    </p>\n"
+"    <ul>\n"
+"        <li>Partner VAT: <b>${object.vat}</b></li>\n"
+"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
+"li>\n"
+"        <li>Charging account: <b>${object.iban}</b></li>\n"
+"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
+"li>\n"
+"    </ul>\n"
+"    <p>\n"
+"        In the next few days you will receive the bank charge in this "
+"account, please verify that all the data\n"
+"        provided is correct and you have the money you want to invest, to "
+"avoid any incident in the\n"
+"        draft of the receipt.\n"
+"    </p>\n"
+"    <p>\n"
+"        Once the validity of the payment has been verified, you will "
+"receive a new notification confirming the\n"
+"        contribution\n"
+"        made and detailing the particular conditions of your contribution.\n"
+"    </p>\n"
+"    <p>\n"
+"        Thank you for your involvement with the cooperative and inform you "
+"that for any doubt or clarification you can\n"
+"        consult\n"
+"        our website:\n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
+"        or send us an email to\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
+"    </p>\n"
+"    <p>\n"
+"        Get the word out by explaining the project to family and friends. "
+"The more we are, the further we will go!\n"
+"    </p>\n"
+"    <p>\n"
+"        Thank you very much and good energy!\n"
+"    </p>\n"
+"    <p>\n"
+"        Sincerely,\n"
+"    </p>\n"
+"    <p>\n"
+"        ${object.company_id.name} team\n"
+"    </p>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
+"            "
+msgstr ""
+"\n"
+"    <p>Apreciado/a ${object.firstname},</p>\n"
+"    <p>\n"
+"Te confirmamos que hemos recibido correctamente tu solicitud para realizar "
+"una aportación voluntaria al capital social de <b>${object.company_id.name}"
+"</b>, con los siguientes datos:\n"
+"    </p>\n"
+"    <ul>\n"
+"        <li>Socio/a NIF: <b>${object.vat}</b></li>\n"
+"        <li>Socio/a: <b>${object.firstname} ${object.lastname}</b></li>\n"
+"        <li>Cuenta de cargo: <b>${object.iban}</b></li>\n"
+"        <li>Importe aportación: <b>${object.subscription_amount}€</b></li>\n"
+"    </ul>\n"
+"    <p>\n"
+"En los próximos días recibirás el cargo bancario en esta cuenta, por favor "
+"verifica que todos los datos facilitados sean correctos y dispones del "
+"dinero que quieres invertir, para evitar cualquier incidencia en el giro "
+"del recibo.\n"
+"    </p>\n"
+"    <p>\n"
+"Una vez verificada la validez del pago realizado recibirás una nueva "
+"notificación confirmando la aportación realizada y detallando las "
+"condiciones particulares de tu aportación.\n"
+"    </p>\n"
+"    <p>\n"
+"Agradecer tu implicación con la cooperativa y informarte que para cualquier "
+"duda o aclaración puedes consultar nuestra web \n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
+"         o enviarnos un correo electrónico \n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
+"    </p>\n"
+"    <p>\n"
+"Haz que corra la voz explicando el proyecto a familiares y amigos/as. "
+"Cuantos más seamos, más lejos llegaremos!\n"
+"    </p>\n"
+"    <p>\n"
+"¡Muchas gracias y buena energía!\n"
+"    </p>\n"
+"    <p>\n"
+"        Atentamente,\n"
+"    </p>\n"
+"    <p>\n"
+"        El equipo de ${object.company_id.name}\n"
+"    </p>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
+"            "
+
+#. module: energy_communities
 #: model:mail.template,body_html:energy_communities.email_templ_lead_request_contact_confirm_id
 msgid ""
 "\n"
 "<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
 "serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
 "\">\n"
 "\n"
@@ -588,144 +698,35 @@
 "    <p>Equipo Somcomunitats.coop</p>\n"
 "    <p><a href=\"https://web-test.somcomunitats.coop/recursos/\">Resources "
 "and FAQs</a></p>\n"
 "</div>\n"
 "            "
 
 #. module: energy_communities
-#: model:mail.template,body_html:energy_communities.email_template_confirmation_voluntary_share
-msgid ""
-"\n"
-"<img src=\"data:image/png;base64,${object.company_id.logo}\" style=\"width: "
-"150px;height: 80px;\" />\n"
-"    <p>Dear ${object.firstname},</p>\n"
-"    <p>\n"
-"        We confirm that we have correctly received your request to make a "
-"voluntary contribution to the capital\n"
-"        social of <b>${object.company_id.name}</b>, with the following "
-"data:\n"
-"    </p>\n"
-"    <ul>\n"
-"        <li>Partner VAT: <b>${object.vat}</b></li>\n"
-"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
-"li>\n"
-"        <li>Charging account: <b>${object.iban}</b></li>\n"
-"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
-"li>\n"
-"    </ul>\n"
-"    <p>\n"
-"        In the next few days you will receive the bank charge in this "
-"account, please verify that all the data\n"
-"        provided is correct and you have the money you want to invest, to "
-"avoid any incident in the\n"
-"        draft of the receipt.\n"
-"    </p>\n"
-"    <p>\n"
-"        Once the validity of the payment has been verified, you will "
-"receive a new notification confirming the\n"
-"        contribution\n"
-"        made and detailing the particular conditions of your contribution.\n"
-"    </p>\n"
-"    <p>\n"
-"        Thank you for your involvement with the cooperative and inform you "
-"that for any doubt or clarification you can\n"
-"        consult\n"
-"        our website:\n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id."
-"website}</a>\n"
-"        or send us an email to\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
-"a>\n"
-"    </p>\n"
-"    <p>\n"
-"        Get the word out by explaining the project to family and friends. "
-"The more we are, the further we will go!\n"
-"    </p>\n"
-"    <p>\n"
-"        Thank you very much and good energy!\n"
-"    </p>\n"
-"    <p>\n"
-"        Sincerely,\n"
-"    </p>\n"
-"    <p>\n"
-"        ${object.company_id.name} team\n"
-"    </p>\n"
-"            "
-msgstr ""
-"\n"
-"<img src=\"data:image/png;base64,${object.company_id.logo}\" style=\"ancho: "
-"150px;alto: 80px;\" />\n"
-"     <p>Apreciado/a  ${object.firstname},</p>\n"
-"     <p>\n"
-"         Te confirmamos que hemos recibido correctamente tu solicitud para "
-"realizar una aportación voluntaria al capital social de <b>${object."
-"company_id.name}</b>, con los siguientes datos:\n"
-"     </p>\n"
-"     <ul>\n"
-"         <li>NIF: <b>${object.vat}</b></li>\n"
-"         <li>Socio/a:: <b>${object.firstname} ${object.lastname}</b></li>\n"
-"         <li>Cuenta de cargo: <b>${object.iban}</b></li>\n"
-"         <li>Importe aportación: <b>${object.subscription_amount}â¬</b></"
-"li>\n"
-"     </ul>\n"
-"     <p>\n"
-"En los próximos días recibirás el cargo bancario en esta cuenta, por favor "
-"verifica que todos los datos facilitados sean correctos y dispones del "
-"dinero que quieres invertir, para evitar cualquier incidencia en el giro "
-"del recibo.\n"
-"     </p>\n"
-"     <p>\n"
-"Una vez verificada la validez del pago realizado recibirás una nueva "
-"notificación confirmando la aportación realizada y detallando las "
-"condiciones particulares de tu aportación.\n"
-"     </p>\n"
-"     <p>\n"
-"Agradecer tu implicación con la cooperativa y informarte que para cualquier "
-"duda o aclaración puedes consultar nuestra web :\n"
-"         <a href=\"${objeto.id_empresa.sitio web}\"> ${objeto.id_empresa."
-"sitioweb}</a>\n"
-"         o enviarnos un correo electrónico \n"
-"         <a href=\"${object.company_id.email}\">${object.company_id.email}</"
-"a>\n"
-"     </p>\n"
-"     <p>\n"
-"         Haz que corra la voz explicando el proyecto a familiares y amigos/"
-"as. Cuantos más seamos, más lejos llegaremos!\n"
-"     </p>\n"
-"     <p>\n"
-"         ¡Muchas gracias y buena energía!\n"
-"     </p>\n"
-"     <p>\n"
-"         Atentamente,\n"
-"     </p>\n"
-"     <p>\n"
-"         El equipo de ${object.company_id.name}\n"
-"     </p>"
-
-#. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser_pwd
 msgid "\"Superuser\" user password"
 msgstr "Contraseña del super-usuario"
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser
 msgid "A super power user that is able to CRUD users on KC."
 msgstr "Un super-usuario con permisos para CRUD en KC."
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
-msgid "Accept to make the payment via SEPA transfer."
-msgstr "Acepta realizar el pago mediante transferencia SEPA."
-
-#. module: energy_communities
 #: model:ir.model,name:energy_communities.model_account_chart_template
 msgid "Account Chart Template"
 msgstr "Plantilla de gráfico de cuentas"
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Address not found"
+msgstr "Dirección no encontrada"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__is_admin_provider
 msgid "Admin provider"
 msgstr "Proveedor AUTH  tareas administrativas"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_admin
 msgid "Administrator"
@@ -746,15 +747,15 @@
 #, python-format
 msgid "An instance company already exists"
 msgstr "Ya existe una compañía con el rol de Instancia"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__mandate_approved
 msgid "Approved SEPA"
-msgstr "SEPA aprobado "
+msgstr "SEPA aprobado"
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_community_service.py:0
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #: code:addons/energy_communities/services/ce_member_service.py:0
 #, python-format
 msgid "Authorization token not found"
@@ -822,14 +823,20 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__chart_template_id
 msgid "Chart Template"
 msgstr "Plantilla plan contable"
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "City not found"
+msgstr "Ciudad no encontrada"
+
+#. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_utm_sources_action
 msgid "Click to define a new Source."
 msgstr "Haz clic para definir un nuevo Source."
 
 #. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_crm_lead_tags_action
 msgid "Click to define a new tag."
@@ -838,14 +845,15 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__code
 msgid "Code"
 msgstr "Código"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__community
 #, python-format
 msgid "Community"
 msgstr "Comunidad"
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_crm_lead__community_company_id
 msgid "Community related to this Lead"
@@ -863,19 +871,14 @@
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_collective_purchases
 msgid "Compres col·lectives"
 msgstr "Compras colectivas"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__community
-msgid "Comunidad"
-msgstr "Comunidad"
-
-#. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_config_menu
 msgid "Configuration"
 msgstr "Configuración"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Confirm Email"
@@ -911,15 +914,15 @@
 msgid "Contribution to Share Capital"
 msgstr "Aportación al Capital Social"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "Converting just part of the shares is not yet implemented"
-msgstr "Convertir solamente parte de las aportaciones no está aún contemplado"
+msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.wizard_multicompany_easy_creation_form_inherit
 msgid "Cooperator"
 msgstr "Socia"
 
 #. module: energy_communities
@@ -929,20 +932,16 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__cooperator_journal
 msgid "Cooperator Journal"
 msgstr "Diario Socias"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
-msgid "Coordinadora"
-msgstr "Coordinadora"
-
-#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
 #, python-format
 msgid "Coordinator"
 msgstr "Coordinadora"
 
 #. module: energy_communities
 #: model:ir.actions.server,name:energy_communities.action_create_map_place_from_lead
 msgid "Create Map Place"
@@ -1012,15 +1011,21 @@
 msgstr "Email"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Email and confirmation email addresses don't match."
-msgstr "El correo y el correo de confirmación no coinciden."
+msgstr "El email y el email de confirmación no concuerdan."
+
+#. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Email not found"
+msgstr "Email no encontrado"
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_thermal_energy
 msgid "Energia tèrmica i climatització"
 msgstr "Energía térmica y climatización"
 
 #. module: energy_communities
@@ -1108,14 +1113,19 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__hierarchy_level
 msgid "Hierarchy level"
 msgstr "Nivel jerárquico"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
+msgid "I accept that the entity issues direct debit receipts to this account."
+msgstr "Acepto que la entidad emita recibos domiciliados a esta cuenta."
+
+#. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__gender__not_share
 #: model:ir.model.fields.selection,name:energy_communities.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
 msgstr "Prefiero no compartirlo"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_chart_template__id
@@ -1186,24 +1196,20 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__capital_share
 msgid "Initial capital share"
 msgstr "Cuota inicial alta sòcia"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
 #, python-format
 msgid "Instance"
 msgstr "Instancia"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
-msgid "Instancia"
-msgstr "Instancia"
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__is_voluntary
 msgid "Is voluntary contribution"
 msgstr "Es aportación voluntaria"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_account_move
 msgid "Journal Entry"
@@ -1241,23 +1247,28 @@
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source____last_update
 msgid "Last Modified on"
 msgstr "Última modificación el"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_crm_lead
 msgid "Lead/Opportunity"
-msgstr "Iniciativa/Oportunidad"
+msgstr "Cliente potencial/Oportunidad"
 
 #. module: energy_communities
 #: model:auth.oauth.provider,body:energy_communities.keycloak_admin_provider
 #: model:auth.oauth.provider,body:energy_communities.keycloak_login_provider
 msgid "Login with Keycloak"
 msgstr "Registrarse con KeyCloak"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
+msgid "Mandatory Shares"
+msgstr "Aportaciones obligatorias"
+
+#. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_sustainable_mobility
 msgid "Mobilitat sostenible"
 msgstr "Movilidad sostenible"
 
 #. module: energy_communities
 #: model:ir.module.category,description:energy_communities.energy_communities_category
 msgid ""
@@ -1387,14 +1398,20 @@
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "Parent company must be instance hierarchy level."
 msgstr "La compañía matriz debe tener nivel de Instancia."
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Partner not found"
+msgstr "Socio no encontrado"
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Phone"
 msgstr "Teléfono"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_platform_manager
 msgid "Platform Manager"
@@ -1406,15 +1423,15 @@
 msgid "Platform admin role"
 msgstr "Rol de Administradora de Instancia"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "Please upload a scan of your ID card."
-msgstr "Por favor carga una imagen escaneada de tu tarjeta de identificación."
+msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__product_share_template
 msgid "Product Share Template"
 msgstr "Plantilla de producto aportación"
 
 #. module: energy_communities
@@ -1423,15 +1440,15 @@
 msgstr "Plantilla de producto"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Provided IBAN is not valid."
-msgstr "El IBAN proporcionado no es válido."
+msgstr "El IBAN no es válido."
 
 #. module: energy_communities
 #: model:ir.actions.server,name:energy_communities.print_instance
 msgid "Push user to Keycloak"
 msgstr "Enviar usuario al KeyCloak"
 
 #. module: energy_communities
@@ -1454,15 +1471,15 @@
 msgid "Root URL"
 msgstr "URL raíz"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/account_chart_template.py:0
 #, python-format
 msgid "SUBJ"
-msgstr "SUBJ"
+msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Send"
 msgstr "Enviar"
 
 #. module: energy_communities
@@ -1475,15 +1492,15 @@
 msgid "Share type"
 msgstr "Tipo de aportación"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "Some mandatory fields have not been filled."
-msgstr "Algunos campos obligatorios no se han rellenado."
+msgstr "Algunos campos del formulario no han sido rellenados."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_users.py:0
 #, python-format
 msgid "Something went wrong. Please check logs."
 msgstr "Algo fué mal. Por favor revisar los LOGS."
 
@@ -1513,15 +1530,15 @@
 #, python-format
 msgid "Subscription Journal"
 msgstr "Diario de subscripciones"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_subscription_request
 msgid "Subscription Request"
-msgstr "Solicitud de Suscripción"
+msgstr "Sol·licitud de Suscripción"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__superuser
 msgid "Superuser"
 msgstr "Super Usuario"
 
 #. module: energy_communities
@@ -1655,36 +1672,36 @@
 msgid "This language code %s is not active in Odoo. Active ones: %s"
 msgstr "Este código de idioma %s no está activo en Odoo. Los activos son: %s"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "This operation is not yet implemented."
-msgstr "Esta operación aún no está implementada."
+msgstr "Esta operación no está implementada todavía."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "This operation must be approved before to be executed"
-msgstr "Esta operación debe ser aprobada antes de ejecutarse"
+msgstr "Esta operación tiene que ser aprobada antes de ejecutarse"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid ""
 "To be a member you must fulfill this form and lateron proceed to pay the "
 "initial share of"
 msgstr ""
 "Para ser socio/a primero debes rellenar este cuestionario y después "
 "formalizar la aportación económica inicial de"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
 msgid "Total"
-msgstr "Total"
+msgstr ""
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_utm_source
 msgid "UTM Source"
 msgstr "Origen UTM"
 
 #. module: energy_communities
@@ -1808,14 +1825,19 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
 msgid "Voluntary Share of"
 msgstr "Aportación voluntaria de"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
+msgid "Voluntary Shares"
+msgstr "Aportaciones voluntarias"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__voluntary_share_id
 msgid "Voluntary share to show on website"
 msgstr "Aportación voluntaria para mostrar en el sitio web"
 
 #. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_menu_webforms_settings
 msgid "Webforms"
@@ -1842,21 +1864,27 @@
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid ""
 "You can't subscribe for an amount that exceeds {amount}{currency_symbol}."
 msgstr ""
-"No puedes suscribirte por un importe superior a {amount}{currency_symbol}."
+"No puedes aportar una aportación que exceda {amount}{currency_symbol}."
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "You can't subscribe to two different types of share."
-msgstr "No puedes suscribirte a 2 tipos distintos de aportación."
+msgstr ""
+
+#. module: energy_communities
+#: code:addons/energy_communities/models/subscription_request.py:0
+#, python-format
+msgid "You can't validate a voluntary contribution in this versión."
+msgstr "No puedes validar aportaciones voluntarias en esta versión."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "You cannot create a instance company with a parent company."
 msgstr ""
 "No puede haber una compañía de nivel Instancia con una empresa matriz "
@@ -1889,14 +1917,20 @@
 #. module: energy_communities
 #: code:addons/energy_communities/models/subscription_request.py:0
 #, python-format
 msgid "You must set a cooperator journal on you company."
 msgstr "Debe seleccionarse un Diario específico para Socias en esta compañía."
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "ZIP code not found"
+msgstr "Código postal no encontrado"
+
+#. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_template_confirmation_company
 msgid "[Somcomunitats.coop] Application to become Community membership"
 msgstr "[Somcomunitats.coop] Solicitud adhesión a Comunidad Energética"
 
 #. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_templ_lead_request_contact_confirm_id
 msgid "[Somcomunitats.coop] Community Contact Request"
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n/eu_ES.po` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n/eu_ES.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # This file contains the translation of the following modules:
 # 	* energy_communities
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 14.0\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-31 08:40+0000\n"
-"PO-Revision-Date: 2023-03-31 11:09+0200\n"
+"POT-Creation-Date: 2023-04-03 13:46+0000\n"
+"PO-Revision-Date: 2023-04-03 15:56+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: \n"
@@ -28,14 +28,124 @@
 msgstr ""
 "\n"
 "        El NIF/CIF. Completa este campo si el contacto está subjecto a\n"
 "        las tasas estatales. Se usa en algunos informes legales.\"\n"
 "        "
 
 #. module: energy_communities
+#: model:mail.template,body_html:energy_communities.email_template_confirmation_voluntary_share
+msgid ""
+"\n"
+"    <p>Dear ${object.firstname},</p>\n"
+"    <p>\n"
+"        We confirm that we have correctly received your request to make a "
+"voluntary contribution to the capital\n"
+"        social of <b>${object.company_id.name}</b>, with the following "
+"data:\n"
+"    </p>\n"
+"    <ul>\n"
+"        <li>Partner VAT: <b>${object.vat}</b></li>\n"
+"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
+"li>\n"
+"        <li>Charging account: <b>${object.iban}</b></li>\n"
+"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
+"li>\n"
+"    </ul>\n"
+"    <p>\n"
+"        In the next few days you will receive the bank charge in this "
+"account, please verify that all the data\n"
+"        provided is correct and you have the money you want to invest, to "
+"avoid any incident in the\n"
+"        draft of the receipt.\n"
+"    </p>\n"
+"    <p>\n"
+"        Once the validity of the payment has been verified, you will "
+"receive a new notification confirming the\n"
+"        contribution\n"
+"        made and detailing the particular conditions of your contribution.\n"
+"    </p>\n"
+"    <p>\n"
+"        Thank you for your involvement with the cooperative and inform you "
+"that for any doubt or clarification you can\n"
+"        consult\n"
+"        our website:\n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
+"        or send us an email to\n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
+"    </p>\n"
+"    <p>\n"
+"        Get the word out by explaining the project to family and friends. "
+"The more we are, the further we will go!\n"
+"    </p>\n"
+"    <p>\n"
+"        Thank you very much and good energy!\n"
+"    </p>\n"
+"    <p>\n"
+"        Sincerely,\n"
+"    </p>\n"
+"    <p>\n"
+"        ${object.company_id.name} team\n"
+"    </p>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
+"            "
+msgstr ""
+"\n"
+"    <p>Apreciado/a ${object.firstname},</p>\n"
+"    <p>\n"
+"Te confirmamos que hemos recibido correctamente tu solicitud para realizar "
+"una aportación voluntaria al capital social de <b>${object.company_id.name}"
+"</b>, con los siguientes datos:\n"
+"    </p>\n"
+"    <ul>\n"
+"        <li>Socio/a NIF: <b>${object.vat}</b></li>\n"
+"        <li>Socio/a: <b>${object.firstname} ${object.lastname}</b></li>\n"
+"        <li>Cuenta de cargo: <b>${object.iban}</b></li>\n"
+"        <li>Importe aportación: <b>${object.subscription_amount}€</b></li>\n"
+"    </ul>\n"
+"    <p>\n"
+"En los próximos días recibirás el cargo bancario en esta cuenta, por favor "
+"verifica que todos los datos facilitados sean correctos y dispones del "
+"dinero que quieres invertir, para evitar cualquier incidencia en el giro "
+"del recibo.\n"
+"    </p>\n"
+"    <p>\n"
+"Una vez verificada la validez del pago realizado recibirás una nueva "
+"notificación confirmando la aportación realizada y detallando las "
+"condiciones particulares de tu aportación.\n"
+"    </p>\n"
+"    <p>\n"
+"Agradecer tu implicación con la cooperativa y informarte que para cualquier "
+"duda o aclaración puedes consultar nuestra web \n"
+"        <a href=\"${object.company_id.website}\"> ${object.company_id."
+"website}</a>\n"
+"         o enviarnos un correo electrónico \n"
+"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
+"a>\n"
+"    </p>\n"
+"    <p>\n"
+"Haz que corra la voz explicando el proyecto a familiares y amigos/as. "
+"Cuantos más seamos, más lejos llegaremos!\n"
+"    </p>\n"
+"    <p>\n"
+"¡Muchas gracias y buena energía!\n"
+"    </p>\n"
+"    <p>\n"
+"        Atentamente,\n"
+"    </p>\n"
+"    <p>\n"
+"        El equipo de ${object.company_id.name}\n"
+"    </p>\n"
+"    <img src=\"/web/image/res.company/${object.company_id.id}/logo\" "
+"style=\"width: 150px;height: 80px;\"/>\n"
+"            "
+
+#. module: energy_communities
 #: model:mail.template,body_html:energy_communities.email_templ_lead_request_contact_confirm_id
 msgid ""
 "\n"
 "<div style=\"font-family: 'Lucica Grande', Ubuntu, Arial, Verdana, sans-"
 "serif; font-size: 12px; color: rgb(34, 34, 34); background-color: #FFF; "
 "\">\n"
 "\n"
@@ -588,144 +698,35 @@
 "    <p>Equipo Somcomunitats.coop</p>\n"
 "    <p><a href=\"https://web-test.somcomunitats.coop/recursos/\">Resources "
 "and FAQs</a></p>\n"
 "</div>\n"
 "            "
 
 #. module: energy_communities
-#: model:mail.template,body_html:energy_communities.email_template_confirmation_voluntary_share
-msgid ""
-"\n"
-"<img src=\"data:image/png;base64,${object.company_id.logo}\" style=\"width: "
-"150px;height: 80px;\" />\n"
-"    <p>Dear ${object.firstname},</p>\n"
-"    <p>\n"
-"        We confirm that we have correctly received your request to make a "
-"voluntary contribution to the capital\n"
-"        social of <b>${object.company_id.name}</b>, with the following "
-"data:\n"
-"    </p>\n"
-"    <ul>\n"
-"        <li>Partner VAT: <b>${object.vat}</b></li>\n"
-"        <li>Partner name: <b>${object.firstname} ${object.lastname}</b></"
-"li>\n"
-"        <li>Charging account: <b>${object.iban}</b></li>\n"
-"        <li>Subscription amount: <b>${object.subscription_amount}€</b></"
-"li>\n"
-"    </ul>\n"
-"    <p>\n"
-"        In the next few days you will receive the bank charge in this "
-"account, please verify that all the data\n"
-"        provided is correct and you have the money you want to invest, to "
-"avoid any incident in the\n"
-"        draft of the receipt.\n"
-"    </p>\n"
-"    <p>\n"
-"        Once the validity of the payment has been verified, you will "
-"receive a new notification confirming the\n"
-"        contribution\n"
-"        made and detailing the particular conditions of your contribution.\n"
-"    </p>\n"
-"    <p>\n"
-"        Thank you for your involvement with the cooperative and inform you "
-"that for any doubt or clarification you can\n"
-"        consult\n"
-"        our website:\n"
-"        <a href=\"${object.company_id.website}\"> ${object.company_id."
-"website}</a>\n"
-"        or send us an email to\n"
-"        <a href=\"${object.company_id.email}\">${object.company_id.email}</"
-"a>\n"
-"    </p>\n"
-"    <p>\n"
-"        Get the word out by explaining the project to family and friends. "
-"The more we are, the further we will go!\n"
-"    </p>\n"
-"    <p>\n"
-"        Thank you very much and good energy!\n"
-"    </p>\n"
-"    <p>\n"
-"        Sincerely,\n"
-"    </p>\n"
-"    <p>\n"
-"        ${object.company_id.name} team\n"
-"    </p>\n"
-"            "
-msgstr ""
-"\n"
-"<img src=\"data:image/png;base64,${object.company_id.logo}\" style=\"ancho: "
-"150px;alto: 80px;\" />\n"
-"     <p>Apreciado/a  ${object.firstname},</p>\n"
-"     <p>\n"
-"         Te confirmamos que hemos recibido correctamente tu solicitud para "
-"realizar una aportación voluntaria al capital social de <b>${object."
-"company_id.name}</b>, con los siguientes datos:\n"
-"     </p>\n"
-"     <ul>\n"
-"         <li>NIF: <b>${object.vat}</b></li>\n"
-"         <li>Socio/a:: <b>${object.firstname} ${object.lastname}</b></li>\n"
-"         <li>Cuenta de cargo: <b>${object.iban}</b></li>\n"
-"         <li>Importe aportación: <b>${object.subscription_amount}â¬</b></"
-"li>\n"
-"     </ul>\n"
-"     <p>\n"
-"En los próximos días recibirás el cargo bancario en esta cuenta, por favor "
-"verifica que todos los datos facilitados sean correctos y dispones del "
-"dinero que quieres invertir, para evitar cualquier incidencia en el giro "
-"del recibo.\n"
-"     </p>\n"
-"     <p>\n"
-"Una vez verificada la validez del pago realizado recibirás una nueva "
-"notificación confirmando la aportación realizada y detallando las "
-"condiciones particulares de tu aportación.\n"
-"     </p>\n"
-"     <p>\n"
-"Agradecer tu implicación con la cooperativa y informarte que para cualquier "
-"duda o aclaración puedes consultar nuestra web :\n"
-"         <a href=\"${objeto.id_empresa.sitio web}\"> ${objeto.id_empresa."
-"sitioweb}</a>\n"
-"         o enviarnos un correo electrónico \n"
-"         <a href=\"${object.company_id.email}\">${object.company_id.email}</"
-"a>\n"
-"     </p>\n"
-"     <p>\n"
-"         Haz que corra la voz explicando el proyecto a familiares y amigos/"
-"as. Cuantos más seamos, más lejos llegaremos!\n"
-"     </p>\n"
-"     <p>\n"
-"         ¡Muchas gracias y buena energía!\n"
-"     </p>\n"
-"     <p>\n"
-"         Atentamente,\n"
-"     </p>\n"
-"     <p>\n"
-"         El equipo de ${object.company_id.name}\n"
-"     </p>"
-
-#. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser_pwd
 msgid "\"Superuser\" user password"
 msgstr "Contraseña del super-usuario"
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_auth_oauth_provider__superuser
 msgid "A super power user that is able to CRUD users on KC."
 msgstr "Un super-usuario con permisos para CRUD en KC."
 
 #. module: energy_communities
-#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
-msgid "Accept to make the payment via SEPA transfer."
-msgstr "Acepta realizar el pago mediante transferencia SEPA."
-
-#. module: energy_communities
 #: model:ir.model,name:energy_communities.model_account_chart_template
 msgid "Account Chart Template"
 msgstr "Plantilla de gráfico de cuentas"
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Address not found"
+msgstr "Dirección no encontrada"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__is_admin_provider
 msgid "Admin provider"
 msgstr "Proveedor AUTH  tareas administrativas"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_admin
 msgid "Administrator"
@@ -746,15 +747,15 @@
 #, python-format
 msgid "An instance company already exists"
 msgstr "Ya existe una compañía con el rol de Instancia"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__mandate_approved
 msgid "Approved SEPA"
-msgstr "SEPA aprobado "
+msgstr "SEPA aprobado"
 
 #. module: energy_communities
 #: code:addons/energy_communities/services/ce_community_service.py:0
 #: code:addons/energy_communities/services/ce_member_profile_service.py:0
 #: code:addons/energy_communities/services/ce_member_service.py:0
 #, python-format
 msgid "Authorization token not found"
@@ -822,14 +823,20 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__chart_template_id
 msgid "Chart Template"
 msgstr "Plantilla plan contable"
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "City not found"
+msgstr "Ciudad no encontrada"
+
+#. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_utm_sources_action
 msgid "Click to define a new Source."
 msgstr "Haz clic para definir un nuevo Source."
 
 #. module: energy_communities
 #: model_terms:ir.actions.act_window,help:energy_communities.ce_crm_lead_tags_action
 msgid "Click to define a new tag."
@@ -838,14 +845,15 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_users_role__code
 msgid "Code"
 msgstr "Código"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__community
 #, python-format
 msgid "Community"
 msgstr "Comunidad"
 
 #. module: energy_communities
 #: model:ir.model.fields,help:energy_communities.field_crm_lead__community_company_id
 msgid "Community related to this Lead"
@@ -863,19 +871,14 @@
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_collective_purchases
 msgid "Compres col·lectives"
 msgstr "Compras colectivas"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__community
-msgid "Comunidad"
-msgstr "Comunidad"
-
-#. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_config_menu
 msgid "Configuration"
 msgstr "Configuración"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Confirm Email"
@@ -911,15 +914,15 @@
 msgid "Contribution to Share Capital"
 msgstr "Aportación al Capital Social"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "Converting just part of the shares is not yet implemented"
-msgstr "Convertir solamente parte de las aportaciones no está aún contemplado"
+msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.wizard_multicompany_easy_creation_form_inherit
 msgid "Cooperator"
 msgstr "Socia"
 
 #. module: energy_communities
@@ -929,20 +932,16 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__cooperator_journal
 msgid "Cooperator Journal"
 msgstr "Diario Socias"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
-msgid "Coordinadora"
-msgstr "Coordinadora"
-
-#. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__coordinator
 #, python-format
 msgid "Coordinator"
 msgstr "Coordinadora"
 
 #. module: energy_communities
 #: model:ir.actions.server,name:energy_communities.action_create_map_place_from_lead
 msgid "Create Map Place"
@@ -1012,15 +1011,21 @@
 msgstr "Email"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Email and confirmation email addresses don't match."
-msgstr "El correo y el correo de confirmación no coinciden."
+msgstr "El email y el email de confirmación no concuerdan."
+
+#. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Email not found"
+msgstr "Email no encontrado"
 
 #. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_thermal_energy
 msgid "Energia tèrmica i climatització"
 msgstr "Energía térmica y climatización"
 
 #. module: energy_communities
@@ -1108,14 +1113,19 @@
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__hierarchy_level
 msgid "Hierarchy level"
 msgstr "Nivel jerárquico"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
+msgid "I accept that the entity issues direct debit receipts to this account."
+msgstr "Acepto que la entidad emita recibos domiciliados a esta cuenta."
+
+#. module: energy_communities
 #: model:ir.model.fields.selection,name:energy_communities.selection__res_partner__gender__not_share
 #: model:ir.model.fields.selection,name:energy_communities.selection__subscription_request__gender__not_share
 msgid "I prefer to not share it"
 msgstr "Prefiero no compartirlo"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_chart_template__id
@@ -1186,24 +1196,20 @@
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__capital_share
 msgid "Initial capital share"
 msgstr "Cuota inicial alta sòcia"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
+#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
 #, python-format
 msgid "Instance"
 msgstr "Instancia"
 
 #. module: energy_communities
-#: model:ir.model.fields.selection,name:energy_communities.selection__res_company__hierarchy_level__instance
-msgid "Instancia"
-msgstr "Instancia"
-
-#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_subscription_request__is_voluntary
 msgid "Is voluntary contribution"
 msgstr "Es aportación voluntaria"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_account_move
 msgid "Journal Entry"
@@ -1241,23 +1247,28 @@
 #: model:ir.model.fields,field_description:energy_communities.field_utm_source____last_update
 msgid "Last Modified on"
 msgstr "Última modificación el"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_crm_lead
 msgid "Lead/Opportunity"
-msgstr "Iniciativa/Oportunidad"
+msgstr "Cliente potencial/Oportunidad"
 
 #. module: energy_communities
 #: model:auth.oauth.provider,body:energy_communities.keycloak_admin_provider
 #: model:auth.oauth.provider,body:energy_communities.keycloak_login_provider
 msgid "Login with Keycloak"
 msgstr "Registrarse con KeyCloak"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
+msgid "Mandatory Shares"
+msgstr "Aportaciones obligatorias"
+
+#. module: energy_communities
 #: model:crm.tag,name:energy_communities.ce_tag_sustainable_mobility
 msgid "Mobilitat sostenible"
 msgstr "Movilidad sostenible"
 
 #. module: energy_communities
 #: model:ir.module.category,description:energy_communities.energy_communities_category
 msgid ""
@@ -1387,14 +1398,20 @@
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "Parent company must be instance hierarchy level."
 msgstr "La compañía matriz debe tener nivel de Instancia."
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "Partner not found"
+msgstr "Socio no encontrado"
+
+#. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Phone"
 msgstr "Teléfono"
 
 #. module: energy_communities
 #: model:res.groups,name:energy_communities.group_platform_manager
 msgid "Platform Manager"
@@ -1406,15 +1423,15 @@
 msgid "Platform admin role"
 msgstr "Rol de Administradora de Instancia"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "Please upload a scan of your ID card."
-msgstr "Por favor carga una imagen escaneada de tu tarjeta de identificación."
+msgstr ""
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_account_multicompany_easy_creation_wiz__product_share_template
 msgid "Product Share Template"
 msgstr "Plantilla de producto aportación"
 
 #. module: energy_communities
@@ -1423,15 +1440,15 @@
 msgstr "Plantilla de producto"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
 #, python-format
 msgid "Provided IBAN is not valid."
-msgstr "El IBAN proporcionado no es válido."
+msgstr "El IBAN no es válido."
 
 #. module: energy_communities
 #: model:ir.actions.server,name:energy_communities.print_instance
 msgid "Push user to Keycloak"
 msgstr "Enviar usuario al KeyCloak"
 
 #. module: energy_communities
@@ -1454,36 +1471,36 @@
 msgid "Root URL"
 msgstr "URL raíz"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/account_chart_template.py:0
 #, python-format
 msgid "SUBJ"
-msgstr "SUBJ"
+msgstr ""
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share
 msgid "Send"
 msgstr "Enviar"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
 msgid "Share number"
-msgstr "Número de aportación"
+msgstr "Aportaciones"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
 msgid "Share type"
 msgstr "Tipo de aportación"
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "Some mandatory fields have not been filled."
-msgstr "Algunos campos obligatorios no se han rellenado."
+msgstr "Algunos campos del formulario no han sido rellenados."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_users.py:0
 #, python-format
 msgid "Something went wrong. Please check logs."
 msgstr "Algo fué mal. Por favor revisar los LOGS."
 
@@ -1513,15 +1530,15 @@
 #, python-format
 msgid "Subscription Journal"
 msgstr "Diario de subscripciones"
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_subscription_request
 msgid "Subscription Request"
-msgstr "Solicitud de Suscripción"
+msgstr "Sol·licitud de Suscripción"
 
 #. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_auth_oauth_provider__superuser
 msgid "Superuser"
 msgstr "Super Usuario"
 
 #. module: energy_communities
@@ -1655,36 +1672,36 @@
 msgid "This language code %s is not active in Odoo. Active ones: %s"
 msgstr "Este código de idioma %s no está activo en Odoo. Los activos son: %s"
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "This operation is not yet implemented."
-msgstr "Esta operación aún no está implementada."
+msgstr "Esta operación no está implementada todavía."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/operation_request.py:0
 #, python-format
 msgid "This operation must be approved before to be executed"
-msgstr "Esta operación debe ser aprobada antes de ejecutarse"
+msgstr "Esta operación tiene que ser aprobada antes de ejecutarse"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecompanycooperator
 #: model_terms:ir.ui.view,arch_db:energy_communities.becomecooperator_ccee
 msgid ""
 "To be a member you must fulfill this form and lateron proceed to pay the "
 "initial share of"
 msgstr ""
 "Para ser socio/a primero debes rellenar este cuestionario y después "
 "formalizar la aportación económica inicial de"
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_shares_template
 msgid "Total"
-msgstr "Total"
+msgstr ""
 
 #. module: energy_communities
 #: model:ir.model,name:energy_communities.model_utm_source
 msgid "UTM Source"
 msgstr "Origen UTM"
 
 #. module: energy_communities
@@ -1808,14 +1825,19 @@
 
 #. module: energy_communities
 #: model_terms:ir.ui.view,arch_db:energy_communities.voluntary_share_text_template
 msgid "Voluntary Share of"
 msgstr "Aportación voluntaria de"
 
 #. module: energy_communities
+#: model_terms:ir.ui.view,arch_db:energy_communities.view_subscription_request_filter_inherit
+msgid "Voluntary Shares"
+msgstr "Aportaciones voluntarias"
+
+#. module: energy_communities
 #: model:ir.model.fields,field_description:energy_communities.field_res_company__voluntary_share_id
 msgid "Voluntary share to show on website"
 msgstr "Aportación voluntaria para mostrar en el sitio web"
 
 #. module: energy_communities
 #: model:ir.ui.menu,name:energy_communities.ce_menu_webforms_settings
 msgid "Webforms"
@@ -1842,21 +1864,27 @@
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid ""
 "You can't subscribe for an amount that exceeds {amount}{currency_symbol}."
 msgstr ""
-"No puedes suscribirte por un importe superior a {amount}{currency_symbol}."
+"No puedes aportar una aportación que exceda {amount}{currency_symbol}."
 
 #. module: energy_communities
 #: code:addons/energy_communities/controllers/website_subscription_main.py:0
 #, python-format
 msgid "You can't subscribe to two different types of share."
-msgstr "No puedes suscribirte a 2 tipos distintos de aportación."
+msgstr ""
+
+#. module: energy_communities
+#: code:addons/energy_communities/models/subscription_request.py:0
+#, python-format
+msgid "You can't validate a voluntary contribution in this versión."
+msgstr "No puedes validar aportaciones voluntarias en esta versión."
 
 #. module: energy_communities
 #: code:addons/energy_communities/models/res_company.py:0
 #, python-format
 msgid "You cannot create a instance company with a parent company."
 msgstr ""
 "No puede haber una compañía de nivel Instancia con una empresa matriz "
@@ -1889,14 +1917,20 @@
 #. module: energy_communities
 #: code:addons/energy_communities/models/subscription_request.py:0
 #, python-format
 msgid "You must set a cooperator journal on you company."
 msgstr "Debe seleccionarse un Diario específico para Socias en esta compañía."
 
 #. module: energy_communities
+#: code:addons/energy_communities/controllers/website_subscription_voluntary_share.py:0
+#, python-format
+msgid "ZIP code not found"
+msgstr "Código postal no encontrado"
+
+#. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_template_confirmation_company
 msgid "[Somcomunitats.coop] Application to become Community membership"
 msgstr "[Somcomunitats.coop] Solicitud adhesión a Comunidad Energética"
 
 #. module: energy_communities
 #: model:mail.template,subject:energy_communities.email_templ_lead_request_contact_confirm_id
 msgid "[Somcomunitats.coop] Community Contact Request"
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n_extra/ca_ES.po` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n_extra/ca_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n_extra/es.po` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n_extra/es.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/i18n_extra/eu_ES.po` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/i18n_extra/eu_ES.po`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/account_chart_template.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/account_chart_template.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/account_move.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/account_move.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/auth_oauth_provider.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/auth_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/crm_lead.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/operation_request.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/operation_request.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/product.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/product.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/res_company.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/res_company.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/res_partner.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/res_users.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/res_users.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/models/subscription_request.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/models/subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
         for record in self:
             record.is_voluntary = record.share_product_id.categ_id == product_category_voluntary_share
 
     gender = fields.Selection(selection_add=[("not_binary", "Not binary"),
                                              ("not_share", "I prefer to not share it")])
     vat = fields.Char(required=True, readonly=True, states={"draft": [("readonly", False)]})
     mandate_approved = fields.Boolean(required=True, default=False, string="Approved SEPA")
-    is_voluntary = fields.Boolean(compute=_compute_is_voluntary, string="Is voluntary contribution", readonly=True)
+    is_voluntary = fields.Boolean(compute=_compute_is_voluntary, string="Is voluntary contribution", readonly=True,
+                                  store=True)
     def get_journal(self):
         """Need to override in order to use in multicompany enviroment"""
 
         j = super().get_journal()
 
         if self.company_id.id != 1:
             if self.company_id.cooperator_journal:
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/security/ir_rule_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/security/ir_rule_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/security/res_users_role_data.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/security/res_users_role_data.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/ce_community_service.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/ce_community_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/ce_member_profile_service.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/ce_member_profile_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/ce_member_service.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/ce_member_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/crm_lead_service.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/services/schemas.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/services/schemas.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/static/description/icon.png` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/static/description/icon.png`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/common.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/common.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/common_service.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/common_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/test_crm_lead_service.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/test_crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/tests/test_res_company.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/tests/test_res_company.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/auth_oauth_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/auth_oauth_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/ce_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/ce_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/crm_lead_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/crm_lead_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/menus.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/menus.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/res_company_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/res_company_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/res_partner_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/res_partner_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/res_users_role_view.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/res_users_role_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/res_users_view.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/res_users_view.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/utm_views.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/utm_views.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/view_users_form.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/view_users_form.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/website_subscription_template.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/website_subscription_template.xml`

 * *Files 0% similar despite different names*

#### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/views/website_subscription_template.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/views/website_subscription_template.xml`

```diff
@@ -113,15 +113,15 @@
         </div>
       </div>
       <div class="col-12" id="mandate_approved" name="mandate_approved_container">
         <div t-attf-class="form-group">
           <div class="form-check">
             <input type="checkbox" name="mandate_approved" class="form-check-input" t-att-required="1"/>
             <label>
-              <label for="mandate_approved">Accept to make the payment via SEPA transfer.</label>
+              <label for="mandate_approved">I accept that the entity issues direct debit receipts to this account.</label>
             </label>
           </div>
         </div>
       </div>
       <div class="col-md-5">
         <div class="form-group field-parts-type" t-attf-class="form-group #{error and 'share_product_id' in error and 'has-error' or ''}" name="share_product_container">
           <label for="share_product_id">Share type</label>
```

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/wizards/multicompany_easy_creation.py`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo/addons/energy_communities/wizards/multicompany_easy_creation.xml`

 * *Files identical despite different names*

### Comparing `odoo14-addon-energy_communities-14.0.1.1.1/odoo14_addon_energy_communities.egg-info/SOURCES.txt` & `odoo14-addon-energy_communities-14.0.1.1.2/odoo14_addon_energy_communities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

