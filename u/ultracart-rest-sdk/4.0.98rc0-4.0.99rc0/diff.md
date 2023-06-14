# Comparing `tmp/ultracart_rest_sdk-4.0.98rc0.tar.gz` & `tmp/ultracart_rest_sdk-4.0.99rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultracart_rest_sdk-4.0.98rc0.tar", last modified: Thu Dec 15 16:42:24 2022, max compression
+gzip compressed data, was "ultracart_rest_sdk-4.0.99rc0.tar", last modified: Thu Dec 15 21:42:39 2022, max compression
```

## Comparing `ultracart_rest_sdk-4.0.98rc0.tar` & `ultracart_rest_sdk-4.0.99rc0.tar`

### file list

```diff
@@ -1,755 +1,756 @@
-drwxrwxrwx   0        0        0        0 2022-12-15 16:42:24.884703 ultracart_rest_sdk-4.0.98rc0/
--rw-rw-rw-   0        0        0    11558 2022-06-20 12:32:36.000000 ultracart_rest_sdk-4.0.98rc0/LICENSE
--rw-rw-rw-   0        0        0      380 2022-12-15 16:42:24.884703 ultracart_rest_sdk-4.0.98rc0/PKG-INFO
--rw-rw-rw-   0        0        0   141971 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/README.md
--rw-rw-rw-   0        0        0       76 2022-12-15 16:42:24.884703 ultracart_rest_sdk-4.0.98rc0/setup.cfg
--rw-rw-rw-   0        0        0      999 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-15 16:42:13.665553 ultracart_rest_sdk-4.0.98rc0/ultracart/
--rw-rw-rw-   0        0        0      701 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 16:42:14.134202 ultracart_rest_sdk-4.0.98rc0/ultracart/api/
--rw-rw-rw-   0        0        0      215 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/__init__.py
--rw-rw-rw-   0        0        0    14519 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/affiliate_api.py
--rw-rw-rw-   0        0        0    53810 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/auto_order_api.py
--rw-rw-rw-   0        0        0    28545 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/channel_partner_api.py
--rw-rw-rw-   0        0        0    32295 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/chargeback_api.py
--rw-rw-rw-   0        0        0   105889 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/checkout_api.py
--rw-rw-rw-   0        0        0   135593 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/conversation_api.py
--rw-rw-rw-   0        0        0   109039 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/coupon_api.py
--rw-rw-rw-   0        0        0   117148 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/customer_api.py
--rw-rw-rw-   0        0        0    35183 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/fulfillment_api.py
--rw-rw-rw-   0        0        0    46858 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/gift_certificate_api.py
--rw-rw-rw-   0        0        0    30164 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/integration_log_api.py
--rw-rw-rw-   0        0        0    95979 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/item_api.py
--rw-rw-rw-   0        0        0    13636 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/oauth_api.py
--rw-rw-rw-   0        0        0   143832 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/order_api.py
--rw-rw-rw-   0        0        0    21632 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/sso_api.py
--rw-rw-rw-   0        0        0   982262 2022-12-15 16:42:07.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/storefront_api.py
--rw-rw-rw-   0        0        0   148671 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/tax_api.py
--rw-rw-rw-   0        0        0    56627 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/user_api.py
--rw-rw-rw-   0        0        0    46761 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api/webhook_api.py
--rw-rw-rw-   0        0        0    39074 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/api_client.py
-drwxrwxrwx   0        0        0        0 2022-12-15 16:42:14.134202 ultracart_rest_sdk-4.0.98rc0/ultracart/apis/
--rw-rw-rw-   0        0        0     1409 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/apis/__init__.py
--rw-rw-rw-   0        0        0    17844 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/configuration.py
--rw-rw-rw-   0        0        0     5069 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-12-15 16:42:24.822222 ultracart_rest_sdk-4.0.98rc0/ultracart/model/
--rw-rw-rw-   0        0        0      343 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/__init__.py
--rw-rw-rw-   0        0        0    17598 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_config.py
--rw-rw-rw-   0        0        0    13641 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_config_response.py
--rw-rw-rw-   0        0        0    12310 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_day_activity.py
--rw-rw-rw-   0        0        0    12850 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_stat_account.py
--rw-rw-rw-   0        0        0    13774 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_stat_metrics.py
--rw-rw-rw-   0        0        0    11655 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_stat_revenue.py
--rw-rw-rw-   0        0        0    13337 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_stats_response.py
--rw-rw-rw-   0        0        0    12709 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/activity.py
--rw-rw-rw-   0        0        0    16337 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/add_library_item_request.py
--rw-rw-rw-   0        0        0    13275 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/adjust_internal_certificate_request.py
--rw-rw-rw-   0        0        0    13144 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/adjust_internal_certificate_response.py
--rw-rw-rw-   0        0        0    15397 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_click.py
--rw-rw-rw-   0        0        0    13069 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_click_query.py
--rw-rw-rw-   0        0        0    12840 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_clicks_response.py
--rw-rw-rw-   0        0        0    17778 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_ledger.py
--rw-rw-rw-   0        0        0    13089 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_ledger_query.py
--rw-rw-rw-   0        0        0    12857 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_ledgers_response.py
--rw-rw-rw-   0        0        0    16127 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_link.py
--rw-rw-rw-   0        0        0    12706 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/api_user_application_profile.py
--rw-rw-rw-   0        0        0    12987 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/apply_library_item_request.py
--rw-rw-rw-   0        0        0    15428 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/apply_library_item_response.py
--rw-rw-rw-   0        0        0    19519 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order.py
--rw-rw-rw-   0        0        0    21602 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_item.py
--rw-rw-rw-   0        0        0    12406 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_item_future_schedule.py
--rw-rw-rw-   0        0        0    11750 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_item_option.py
--rw-rw-rw-   0        0        0    12723 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_item_simple_schedule.py
--rw-rw-rw-   0        0        0    11723 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_log.py
--rw-rw-rw-   0        0        0    11612 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_management.py
--rw-rw-rw-   0        0        0    17247 2022-12-15 16:41:53.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_query.py
--rw-rw-rw-   0        0        0    11501 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_query_batch.py
--rw-rw-rw-   0        0        0    12785 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_response.py
--rw-rw-rw-   0        0        0    11640 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_orders_request.py
--rw-rw-rw-   0        0        0    12799 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_orders_response.py
--rw-rw-rw-   0        0        0    15408 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/avalara_config.py
--rw-rw-rw-   0        0        0    12452 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/base_response.py
--rw-rw-rw-   0        0        0    12228 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/browser.py
--rw-rw-rw-   0        0        0    11398 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/browser_device.py
--rw-rw-rw-   0        0        0    12148 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/browser_os.py
--rw-rw-rw-   0        0        0    11956 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/browser_user_agent.py
--rw-rw-rw-   0        0        0    20508 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart.py
--rw-rw-rw-   0        0        0    11904 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_affiliate.py
--rw-rw-rw-   0        0        0    11808 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_affirm_checkout_response.py
--rw-rw-rw-   0        0        0    16564 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_billing.py
--rw-rw-rw-   0        0        0    13145 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_buysafe.py
--rw-rw-rw-   0        0        0    16032 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_checkout.py
--rw-rw-rw-   0        0        0    11440 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_coupon.py
--rw-rw-rw-   0        0        0    12087 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_currency_conversion.py
--rw-rw-rw-   0        0        0    19383 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_customer_profile.py
--rw-rw-rw-   0        0        0    14610 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_customer_profile_address.py
--rw-rw-rw-   0        0        0    13299 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_customer_profile_credit_card.py
--rw-rw-rw-   0        0        0    12019 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_finalize_order_request.py
--rw-rw-rw-   0        0        0    16957 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_finalize_order_request_options.py
--rw-rw-rw-   0        0        0    12736 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_finalize_order_response.py
--rw-rw-rw-   0        0        0    13134 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_gift.py
--rw-rw-rw-   0        0        0    12379 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_gift_certificate.py
--rw-rw-rw-   0        0        0    20348 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item.py
--rw-rw-rw-   0        0        0    11893 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_attribute.py
--rw-rw-rw-   0        0        0    14070 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_multimedia.py
--rw-rw-rw-   0        0        0    12445 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_multimedia_thumbnail.py
--rw-rw-rw-   0        0        0    15203 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_option.py
--rw-rw-rw-   0        0        0    12820 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_option_value.py
--rw-rw-rw-   0        0        0    12250 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_physical.py
--rw-rw-rw-   0        0        0    11776 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_variation_selection.py
--rw-rw-rw-   0        0        0    15756 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_kit_component_option.py
--rw-rw-rw-   0        0        0    12302 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_marketing.py
--rw-rw-rw-   0        0        0    13703 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment.py
--rw-rw-rw-   0        0        0    11531 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_affirm.py
--rw-rw-rw-   0        0        0    11559 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_amazon.py
--rw-rw-rw-   0        0        0    11507 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_check.py
--rw-rw-rw-   0        0        0    14285 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_credit_card.py
--rw-rw-rw-   0        0        0    11552 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_purchase_order.py
--rw-rw-rw-   0        0        0    12256 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_profile_login_request.py
--rw-rw-rw-   0        0        0    11915 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_profile_login_response.py
--rw-rw-rw-   0        0        0    11815 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_profile_register_request.py
--rw-rw-rw-   0        0        0    11924 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_profile_register_response.py
--rw-rw-rw-   0        0        0    12362 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_property.py
--rw-rw-rw-   0        0        0    11815 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_response.py
--rw-rw-rw-   0        0        0    13443 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings.py
--rw-rw-rw-   0        0        0    11711 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_billing.py
--rw-rw-rw-   0        0        0    12789 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_gift.py
--rw-rw-rw-   0        0        0    12053 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_gift_wrap.py
--rw-rw-rw-   0        0        0    16192 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_payment.py
--rw-rw-rw-   0        0        0    12096 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_payment_amazon.py
--rw-rw-rw-   0        0        0    12542 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_payment_credit_card.py
--rw-rw-rw-   0        0        0    12861 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_payment_pay_pal.py
--rw-rw-rw-   0        0        0    11607 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_province.py
--rw-rw-rw-   0        0        0    13285 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_shipping.py
--rw-rw-rw-   0        0        0    12908 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_shipping_calendar.py
--rw-rw-rw-   0        0        0    15468 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_shipping_estimate.py
--rw-rw-rw-   0        0        0    11426 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_taxes.py
--rw-rw-rw-   0        0        0    11688 2022-12-15 16:41:54.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_terms.py
--rw-rw-rw-   0        0        0    17806 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_shipping.py
--rw-rw-rw-   0        0        0    15618 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_summary.py
--rw-rw-rw-   0        0        0    11961 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_taxes.py
--rw-rw-rw-   0        0        0    12497 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_upsell_after.py
--rw-rw-rw-   0        0        0    11782 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_validation_request.py
--rw-rw-rw-   0        0        0    11909 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_validation_response.py
--rw-rw-rw-   0        0        0    13335 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner.py
--rw-rw-rw-   0        0        0    12801 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_cancel_response.py
--rw-rw-rw-   0        0        0    13090 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_estimate_shipping_response.py
--rw-rw-rw-   0        0        0    12744 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_estimate_tax_response.py
--rw-rw-rw-   0        0        0    13430 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_import_response.py
--rw-rw-rw-   0        0        0    41481 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order.py
--rw-rw-rw-   0        0        0    14458 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order_item.py
--rw-rw-rw-   0        0        0    11741 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order_item_option.py
--rw-rw-rw-   0        0        0    12195 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order_transaction.py
--rw-rw-rw-   0        0        0    11762 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order_transaction_detail.py
--rw-rw-rw-   0        0        0    11987 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_shipping_estimate.py
--rw-rw-rw-   0        0        0    18191 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/chargeback_dispute.py
--rw-rw-rw-   0        0        0    12865 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/chargeback_dispute_response.py
--rw-rw-rw-   0        0        0    12879 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/chargeback_disputes_response.py
--rw-rw-rw-   0        0        0    11635 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_allowed_countries_response.py
--rw-rw-rw-   0        0        0    14935 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_handoff_request.py
--rw-rw-rw-   0        0        0    12297 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_handoff_response.py
--rw-rw-rw-   0        0        0    11748 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_setup_browser_key_request.py
--rw-rw-rw-   0        0        0    11633 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_setup_browser_key_response.py
--rw-rw-rw-   0        0        0    11698 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_state_province_response.py
--rw-rw-rw-   0        0        0    12129 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/city_state_zip.py
--rw-rw-rw-   0        0        0    16816 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation.py
--rw-rw-rw-   0        0        0    12970 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_agent_auth.py
--rw-rw-rw-   0        0        0    12906 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_agent_auth_response.py
--rw-rw-rw-   0        0        0    11625 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_autocomplete_request.py
--rw-rw-rw-   0        0        0    13072 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_autocomplete_response.py
--rw-rw-rw-   0        0        0    12299 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_canned_message.py
--rw-rw-rw-   0        0        0    13031 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_canned_message_response.py
--rw-rw-rw-   0        0        0    13045 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_canned_messages_response.py
--rw-rw-rw-   0        0        0    11688 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_canned_messages_search.py
--rw-rw-rw-   0        0        0    12551 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_department.py
--rw-rw-rw-   0        0        0    12980 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_department_response.py
--rw-rw-rw-   0        0        0    12994 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_departments_response.py
--rw-rw-rw-   0        0        0    13050 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_engagement.py
--rw-rw-rw-   0        0        0    12980 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_engagement_response.py
--rw-rw-rw-   0        0        0    12994 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_engagements_response.py
--rw-rw-rw-   0        0        0    11873 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_add_coupon.py
--rw-rw-rw-   0        0        0    12010 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_add_item.py
--rw-rw-rw-   0        0        0    11905 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_queue_position.py
--rw-rw-rw-   0        0        0    12012 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_read_message.py
--rw-rw-rw-   0        0        0    12825 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_rr_web.py
--rw-rw-rw-   0        0        0    12094 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_typing.py
--rw-rw-rw-   0        0        0    11818 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_webchat_context.py
--rw-rw-rw-   0        0        0    11543 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_join_request.py
--rw-rw-rw-   0        0        0    15734 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_message.py
--rw-rw-rw-   0        0        0    11682 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_message_translation.py
--rw-rw-rw-   0        0        0    12327 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_message_transport_status.py
--rw-rw-rw-   0        0        0    12949 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_messages_response.py
--rw-rw-rw-   0        0        0    11610 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_multimedia_upload_url.py
--rw-rw-rw-   0        0        0    13127 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_multimedia_upload_url_response.py
--rw-rw-rw-   0        0        0    14482 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_participant.py
--rw-rw-rw-   0        0        0    12824 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_response.py
--rw-rw-rw-   0        0        0    13525 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_search_request.py
--rw-rw-rw-   0        0        0    11848 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_search_response.py
--rw-rw-rw-   0        0        0    12123 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_start_request.py
--rw-rw-rw-   0        0        0    11658 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_start_response.py
--rw-rw-rw-   0        0        0    16021 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_summary.py
--rw-rw-rw-   0        0        0    11723 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_twilio_account.py
--rw-rw-rw-   0        0        0    13789 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_context.py
--rw-rw-rw-   0        0        0    16005 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_status.py
--rw-rw-rw-   0        0        0    13126 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_status_agent.py
--rw-rw-rw-   0        0        0    13169 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_status_queue_entry.py
--rw-rw-rw-   0        0        0    11708 2022-12-15 16:41:55.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_status_update_request.py
--rw-rw-rw-   0        0        0    13029 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_statuses_response.py
--rw-rw-rw-   0        0        0    18978 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_websocket_message.py
--rw-rw-rw-   0        0        0    12888 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversations_response.py
--rw-rw-rw-   0        0        0    11590 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/countries_response.py
--rw-rw-rw-   0        0        0    11743 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/country.py
--rw-rw-rw-   0        0        0    42889 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon.py
--rw-rw-rw-   0        0        0    12601 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_items.py
--rw-rw-rw-   0        0        0    12360 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_shipping.py
--rw-rw-rw-   0        0        0    12756 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_shipping_with_items_purchase.py
--rw-rw-rw-   0        0        0    11988 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal.py
--rw-rw-rw-   0        0        0    12021 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_and_shipping.py
--rw-rw-rw-   0        0        0    12781 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_free_shipping_with_purchase.py
--rw-rw-rw-   0        0        0    12935 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_with_block_purchase.py
--rw-rw-rw-   0        0        0    12860 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_with_items_purchase.py
--rw-rw-rw-   0        0        0    12407 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_with_purchase.py
--rw-rw-rw-   0        0        0    12894 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_shipping_with_subtotal.py
--rw-rw-rw-   0        0        0    12434 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_auto_apply_condition.py
--rw-rw-rw-   0        0        0    13244 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_auto_apply_conditions.py
--rw-rw-rw-   0        0        0    11634 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_automatically_apply_coupon_codes.py
--rw-rw-rw-   0        0        0    11968 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_buy_one_get_one_limit.py
--rw-rw-rw-   0        0        0    13238 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_codes_request.py
--rw-rw-rw-   0        0        0    12987 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_codes_response.py
--rw-rw-rw-   0        0        0    11728 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_deletes_request.py
--rw-rw-rw-   0        0        0    13180 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_discount_item_with_item_purchase.py
--rw-rw-rw-   0        0        0    12597 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_discount_items.py
--rw-rw-rw-   0        0        0    14374 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_editor_values.py
--rw-rw-rw-   0        0        0    12922 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_exists_response.py
--rw-rw-rw-   0        0        0    13078 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_item_and_shipping_with_subtotal.py
--rw-rw-rw-   0        0        0    12926 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_item_with_item_purchase.py
--rw-rw-rw-   0        0        0    12707 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_item_with_subtotal.py
--rw-rw-rw-   0        0        0    13219 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_items_with_item_purchase.py
--rw-rw-rw-   0        0        0    13376 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_items_with_mix_match_purchase.py
--rw-rw-rw-   0        0        0    11597 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_shipping.py
--rw-rw-rw-   0        0        0    11615 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_shipping_specific_items.py
--rw-rw-rw-   0        0        0    11993 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_shipping_with_items_purchase.py
--rw-rw-rw-   0        0        0    12459 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_shipping_with_subtotal.py
--rw-rw-rw-   0        0        0    13900 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_item_search_result.py
--rw-rw-rw-   0        0        0    12978 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_item_search_results_response.py
--rw-rw-rw-   0        0        0    12113 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_multiple_amounts_off_items.py
--rw-rw-rw-   0        0        0    11708 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_no_discount.py
--rw-rw-rw-   0        0        0    13207 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_item_with_items_quantity_purchase.py
--rw-rw-rw-   0        0        0    12600 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_items.py
--rw-rw-rw-   0        0        0    12354 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_items_and_free_shipping.py
--rw-rw-rw-   0        0        0    12742 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_items_with_items_purchase.py
--rw-rw-rw-   0        0        0    13219 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_msrp_items.py
--rw-rw-rw-   0        0        0    12633 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_retail_price_items.py
--rw-rw-rw-   0        0        0    11933 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_shipping.py
--rw-rw-rw-   0        0        0    11561 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal.py
--rw-rw-rw-   0        0        0    11944 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal_and_free_shipping.py
--rw-rw-rw-   0        0        0    12328 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal_limit.py
--rw-rw-rw-   0        0        0    11963 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal_with_items_purchase.py
--rw-rw-rw-   0        0        0    12409 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal_with_subtotal.py
--rw-rw-rw-   0        0        0    14140 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_query.py
--rw-rw-rw-   0        0        0    13173 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_response.py
--rw-rw-rw-   0        0        0    12121 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_restriction.py
--rw-rw-rw-   0        0        0    12255 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_amount.py
--rw-rw-rw-   0        0        0    11833 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_item_discount.py
--rw-rw-rw-   0        0        0    12267 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_percent.py
--rw-rw-rw-   0        0        0    12223 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_quantity_amount.py
--rw-rw-rw-   0        0        0    12233 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_quantity_percent.py
--rw-rw-rw-   0        0        0    12321 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_amount_off_items.py
--rw-rw-rw-   0        0        0    12224 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_amount_off_subtotal.py
--rw-rw-rw-   0        0        0    12431 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_percent_off_items.py
--rw-rw-rw-   0        0        0    12465 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_percent_off_shipping.py
--rw-rw-rw-   0        0        0    12234 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_percent_off_subtotal.py
--rw-rw-rw-   0        0        0    12267 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_percent_off_subtotal_based_on_msrp.py
--rw-rw-rw-   0        0        0    11772 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_type.py
--rw-rw-rw-   0        0        0    11582 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupons_request.py
--rw-rw-rw-   0        0        0    12748 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupons_response.py
--rw-rw-rw-   0        0        0    12648 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/currency.py
--rw-rw-rw-   0        0        0    32102 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer.py
--rw-rw-rw-   0        0        0    13685 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_activity.py
--rw-rw-rw-   0        0        0    12157 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_affiliate.py
--rw-rw-rw-   0        0        0    12519 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_attachment.py
--rw-rw-rw-   0        0        0    16404 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_billing.py
--rw-rw-rw-   0        0        0    13673 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_card.py
--rw-rw-rw-   0        0        0    12359 2022-12-15 16:41:56.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_edi.py
--rw-rw-rw-   0        0        0    14976 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_editor_values.py
--rw-rw-rw-   0        0        0    13077 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_email.py
--rw-rw-rw-   0        0        0    11886 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_email_list_changes.py
--rw-rw-rw-   0        0        0    14106 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_loyalty.py
--rw-rw-rw-   0        0        0    14834 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_loyalty_ledger.py
--rw-rw-rw-   0        0        0    14828 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_loyalty_redemption.py
--rw-rw-rw-   0        0        0    12674 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_magic_link_response.py
--rw-rw-rw-   0        0        0    11814 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_merge_request.py
--rw-rw-rw-   0        0        0    12297 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_orders_summary.py
--rw-rw-rw-   0        0        0    11754 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_pricing_tier.py
--rw-rw-rw-   0        0        0    12397 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_privacy.py
--rw-rw-rw-   0        0        0    20888 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_query.py
--rw-rw-rw-   0        0        0    12295 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_quotes_summary.py
--rw-rw-rw-   0        0        0    12764 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_response.py
--rw-rw-rw-   0        0        0    14096 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_reviewer.py
--rw-rw-rw-   0        0        0    16421 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_shipping.py
--rw-rw-rw-   0        0        0    14418 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_software_entitlement.py
--rw-rw-rw-   0        0        0    13544 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_store_credit.py
--rw-rw-rw-   0        0        0    12542 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_store_credit_add_request.py
--rw-rw-rw-   0        0        0    13671 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_store_credit_ledger_entry.py
--rw-rw-rw-   0        0        0    12941 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_store_credit_response.py
--rw-rw-rw-   0        0        0    11497 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_tag.py
--rw-rw-rw-   0        0        0    12743 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_tax_codes.py
--rw-rw-rw-   0        0        0    12778 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/customers_response.py
--rw-rw-rw-   0        0        0    12242 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/data_tables_server_side_response.py
--rw-rw-rw-   0        0        0    11730 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/distance.py
--rw-rw-rw-   0        0        0    24060 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/distribution_center.py
--rw-rw-rw-   0        0        0    12934 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/distribution_centers_response.py
--rw-rw-rw-   0        0        0    11491 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_base_template_list_response.py
--rw-rw-rw-   0        0        0    20256 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign.py
--rw-rw-rw-   0        0        0    12655 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign_folder.py
--rw-rw-rw-   0        0        0    12911 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign_folder_response.py
--rw-rw-rw-   0        0        0    12925 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign_folders_response.py
--rw-rw-rw-   0        0        0    12815 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign_response.py
--rw-rw-rw-   0        0        0    12829 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaigns_response.py
--rw-rw-rw-   0        0        0    11623 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_click.py
--rw-rw-rw-   0        0        0    12784 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_clicks_response.py
--rw-rw-rw-   0        0        0    12659 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq.py
--rw-rw-rw-   0        0        0    20021 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_email.py
--rw-rw-rw-   0        0        0    12841 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_email_response.py
--rw-rw-rw-   0        0        0    13620 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_email_send_test_request.py
--rw-rw-rw-   0        0        0    12515 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_email_send_test_response.py
--rw-rw-rw-   0        0        0    12770 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_emails_request.py
--rw-rw-rw-   0        0        0    12855 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_emails_response.py
--rw-rw-rw-   0        0        0    15641 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcard.py
--rw-rw-rw-   0        0        0    12886 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcard_response.py
--rw-rw-rw-   0        0        0    14044 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcard_send_test_request.py
--rw-rw-rw-   0        0        0    13200 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcard_send_test_response.py
--rw-rw-rw-   0        0        0    11549 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcards_request.py
--rw-rw-rw-   0        0        0    12900 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcards_response.py
--rw-rw-rw-   0        0        0    12875 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_response.py
--rw-rw-rw-   0        0        0    14474 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_sequence_test_request.py
--rw-rw-rw-   0        0        0    12512 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_sequence_test_response.py
--rw-rw-rw-   0        0        0    12030 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_sms_send_test_request.py
--rw-rw-rw-   0        0        0    12901 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_sms_send_test_response.py
--rw-rw-rw-   0        0        0    22683 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_stat.py
--rw-rw-rw-   0        0        0    12831 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_stat_response.py
--rw-rw-rw-   0        0        0    15261 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_step.py
--rw-rw-rw-   0        0        0    11841 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_step_log.py
--rw-rw-rw-   0        0        0    12866 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_step_logs_response.py
--rw-rw-rw-   0        0        0    12755 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_webhook_send_test_request.py
--rw-rw-rw-   0        0        0    13219 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_webhook_send_test_response.py
--rw-rw-rw-   0        0        0    12889 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseqs_response.py
--rw-rw-rw-   0        0        0    13491 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_customer.py
--rw-rw-rw-   0        0        0    12714 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_customer_editor_url_response.py
--rw-rw-rw-   0        0        0    12756 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_customers_response.py
--rw-rw-rw-   0        0        0    13155 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_dashboard_activity.py
--rw-rw-rw-   0        0        0    12912 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_dashboard_activity_response.py
--rw-rw-rw-   0        0        0    12796 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_dashboard_stats_response.py
--rw-rw-rw-   0        0        0    14341 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_domain.py
--rw-rw-rw-   0        0        0    12671 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_editor_token_response.py
--rw-rw-rw-   0        0        0    21242 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow.py
--rw-rw-rw-   0        0        0    12051 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_back_populate_request.py
--rw-rw-rw-   0        0        0    12503 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_back_populate_response.py
--rw-rw-rw-   0        0        0    12607 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_folder.py
--rw-rw-rw-   0        0        0    12851 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_folder_response.py
--rw-rw-rw-   0        0        0    12865 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_folders_response.py
--rw-rw-rw-   0        0        0    12755 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_response.py
--rw-rw-rw-   0        0        0    12769 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flows_response.py
--rw-rw-rw-   0        0        0    11449 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_global_settings.py
--rw-rw-rw-   0        0        0    12911 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_global_settings_response.py
--rw-rw-rw-   0        0        0    11441 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_global_unsubscribe_request.py
--rw-rw-rw-   0        0        0    11508 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_global_unsubscribe_response.py
--rw-rw-rw-   0        0        0    11510 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_histogram_property_names_response.py
--rw-rw-rw-   0        0        0    11518 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_histogram_property_values_response.py
--rw-rw-rw-   0        0        0    14940 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list.py
--rw-rw-rw-   0        0        0    12704 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_archive_response.py
--rw-rw-rw-   0        0        0    12257 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_customer.py
--rw-rw-rw-   0        0        0    12797 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_customers_response.py
--rw-rw-rw-   0        0        0    12755 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_response.py
--rw-rw-rw-   0        0        0    12692 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_folder.py
--rw-rw-rw-   0        0        0    12962 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_folder_response.py
--rw-rw-rw-   0        0        0    12976 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_folders_response.py
--rw-rw-rw-   0        0        0    12568 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_membership.py
--rw-rw-rw-   0        0        0    12037 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_used_by.py
--rw-rw-rw-   0        0        0    11649 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_subscribe_response.py
--rw-rw-rw-   0        0        0    12769 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_lists_response.py
--rw-rw-rw-   0        0        0    12190 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_order.py
--rw-rw-rw-   0        0        0    12784 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_orders_response.py
--rw-rw-rw-   0        0        0    19999 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance.py
--rw-rw-rw-   0        0        0    11912 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance_customer_histogram.py
--rw-rw-rw-   0        0        0    12572 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance_customer_histogram_period.py
--rw-rw-rw-   0        0        0    13165 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance_daily.py
--rw-rw-rw-   0        0        0    12860 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance_response.py
--rw-rw-rw-   0        0        0    15537 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_plan.py
--rw-rw-rw-   0        0        0    13146 2022-12-15 16:41:57.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_plan_additional.py
--rw-rw-rw-   0        0        0    12755 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_plan_response.py
--rw-rw-rw-   0        0        0    20459 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_postcard_stat.py
--rw-rw-rw-   0        0        0    16866 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_postcard_tracking.py
--rw-rw-rw-   0        0        0    12896 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_postcard_tracking_response.py
--rw-rw-rw-   0        0        0    19182 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment.py
--rw-rw-rw-   0        0        0    12728 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_archive_response.py
--rw-rw-rw-   0        0        0    12287 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_customer.py
--rw-rw-rw-   0        0        0    12827 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_customers_response.py
--rw-rw-rw-   0        0        0    13512 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_download_prepare_response.py
--rw-rw-rw-   0        0        0    12800 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_response.py
--rw-rw-rw-   0        0        0    12814 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segments_response.py
--rw-rw-rw-   0        0        0    12806 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_sending_domain_response.py
--rw-rw-rw-   0        0        0    12820 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_sending_domains_response.py
--rw-rw-rw-   0        0        0    15413 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_settings.py
--rw-rw-rw-   0        0        0    12815 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_settings_response.py
--rw-rw-rw-   0        0        0    22364 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat.py
--rw-rw-rw-   0        0        0    11716 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat_postcard_summary_request.py
--rw-rw-rw-   0        0        0    12868 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat_postcard_summary_response.py
--rw-rw-rw-   0        0        0    11931 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat_summary_request.py
--rw-rw-rw-   0        0        0    12787 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat_summary_response.py
--rw-rw-rw-   0        0        0    21286 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_stat.py
--rw-rw-rw-   0        0        0    11663 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_stat_request.py
--rw-rw-rw-   0        0        0    12807 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_stat_response.py
--rw-rw-rw-   0        0        0    11494 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_waiting_request.py
--rw-rw-rw-   0        0        0    11660 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_waiting_response.py
--rw-rw-rw-   0        0        0    14489 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_template.py
--rw-rw-rw-   0        0        0    12829 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_templates_response.py
--rw-rw-rw-   0        0        0    11594 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_list.py
--rw-rw-rw-   0        0        0    11772 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_list_import_request.py
--rw-rw-rw-   0        0        0    14767 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_provider.py
--rw-rw-rw-   0        0        0    12931 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_providers_response.py
--rw-rw-rw-   0        0        0    11591 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_tag.py
--rw-rw-rw-   0        0        0    11655 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_verify_token_request.py
--rw-rw-rw-   0        0        0    12685 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_verify_token_response.py
--rw-rw-rw-   0        0        0    11461 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_verify_token_validate_request.py
--rw-rw-rw-   0        0        0    12512 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_verify_token_validate_response.py
--rw-rw-rw-   0        0        0    13258 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_webhook_editor_values_response.py
--rw-rw-rw-   0        0        0    12757 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/error.py
--rw-rw-rw-   0        0        0    12455 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/error_response.py
--rw-rw-rw-   0        0        0    16598 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiment.py
--rw-rw-rw-   0        0        0    12794 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiment_response.py
--rw-rw-rw-   0        0        0    18996 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiment_variation.py
--rw-rw-rw-   0        0        0    15007 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiment_variation_stat.py
--rw-rw-rw-   0        0        0    12808 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiments_response.py
--rw-rw-rw-   0        0        0    14237 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_directory.py
--rw-rw-rw-   0        0        0    16303 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_file.py
--rw-rw-rw-   0        0        0    13554 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_page.py
--rw-rw-rw-   0        0        0    12881 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_page_response.py
--rw-rw-rw-   0        0        0    11942 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_upload_request.py
--rw-rw-rw-   0        0        0    12846 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_upload_url_response.py
--rw-rw-rw-   0        0        0    11627 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/fulfillment_inventory.py
--rw-rw-rw-   0        0        0    12894 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/fulfillment_shipment.py
--rw-rw-rw-   0        0        0    11553 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/geo_point.py
--rw-rw-rw-   0        0        0    12296 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/geocode_request.py
--rw-rw-rw-   0        0        0    12874 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/geocode_response.py
--rw-rw-rw-   0        0        0    16714 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate.py
--rw-rw-rw-   0        0        0    12939 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate_create_request.py
--rw-rw-rw-   0        0        0    13303 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate_ledger_entry.py
--rw-rw-rw-   0        0        0    13908 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate_query.py
--rw-rw-rw-   0        0        0    12875 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate_response.py
--rw-rw-rw-   0        0        0    12889 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificates_response.py
--rw-rw-rw-   0        0        0    13201 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/group.py
--rw-rw-rw-   0        0        0    12719 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/group_response.py
--rw-rw-rw-   0        0        0    12530 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/group_user_membership.py
--rw-rw-rw-   0        0        0    12733 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/groups_response.py
--rw-rw-rw-   0        0        0    13608 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/hit_page_view.py
--rw-rw-rw-   0        0        0    11584 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/hit_page_view_meta_data.py
--rw-rw-rw-   0        0        0    15003 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/hit_session_start.py
--rw-rw-rw-   0        0        0    14175 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/hit_session_utm.py
--rw-rw-rw-   0        0        0    11664 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/http_header.py
--rw-rw-rw-   0        0        0    15289 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log.py
--rw-rw-rw-   0        0        0    11962 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_file.py
--rw-rw-rw-   0        0        0    11598 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_log.py
--rw-rw-rw-   0        0        0    13922 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_query_filter_values.py
--rw-rw-rw-   0        0        0    13975 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_query_request.py
--rw-rw-rw-   0        0        0    13376 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_query_response.py
--rw-rw-rw-   0        0        0    12860 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_response.py
--rw-rw-rw-   0        0        0    13001 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_summary.py
--rw-rw-rw-   0        0        0    11786 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_summary_query_request.py
--rw-rw-rw-   0        0        0    13002 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_summary_query_response.py
--rw-rw-rw-   0        0        0    30236 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item.py
--rw-rw-rw-   0        0        0    12033 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_accounting.py
--rw-rw-rw-   0        0        0    12125 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_amember.py
--rw-rw-rw-   0        0        0    18365 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_auto_order.py
--rw-rw-rw-   0        0        0    17558 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_auto_order_step.py
--rw-rw-rw-   0        0        0    11830 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_auto_order_step_arbitrary_unit_cost_schedule.py
--rw-rw-rw-   0        0        0    11788 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_auto_order_step_grandfather_pricing.py
--rw-rw-rw-   0        0        0    12987 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_cc_bill.py
--rw-rw-rw-   0        0        0    16646 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_channel_partner_mapping.py
--rw-rw-rw-   0        0        0    12277 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_chargeback.py
--rw-rw-rw-   0        0        0    12283 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_chargeback_addendum.py
--rw-rw-rw-   0        0        0    12163 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_chargeback_adjustment_request.py
--rw-rw-rw-   0        0        0    12603 2022-12-15 16:41:58.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_checkout.py
--rw-rw-rw-   0        0        0    16094 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content.py
--rw-rw-rw-   0        0        0    12933 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content_assignment.py
--rw-rw-rw-   0        0        0    12390 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content_attribute.py
--rw-rw-rw-   0        0        0    16332 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content_multimedia.py
--rw-rw-rw-   0        0        0    12785 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content_multimedia_thumbnail.py
--rw-rw-rw-   0        0        0    14016 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_delivery.py
--rw-rw-rw-   0        0        0    15198 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_item.py
--rw-rw-rw-   0        0        0    14650 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_item_pdf_meta.py
--rw-rw-rw-   0        0        0    12856 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_item_response.py
--rw-rw-rw-   0        0        0    12900 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_items_response.py
--rw-rw-rw-   0        0        0    35287 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_ebay.py
--rw-rw-rw-   0        0        0    11702 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_ebay_category_specific.py
--rw-rw-rw-   0        0        0    12300 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_ebay_market_listing.py
--rw-rw-rw-   0        0        0    14201 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_ebay_market_place_analysis.py
--rw-rw-rw-   0        0        0    11893 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_email_notifications.py
--rw-rw-rw-   0        0        0    11566 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_enrollment123.py
--rw-rw-rw-   0        0        0    12516 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_fulfillment_addon.py
--rw-rw-rw-   0        0        0    12053 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_gift_certificate.py
--rw-rw-rw-   0        0        0    26424 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_google_product_search.py
--rw-rw-rw-   0        0        0    12464 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_identifiers.py
--rw-rw-rw-   0        0        0    12222 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_instant_payment_notification.py
--rw-rw-rw-   0        0        0    11846 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_instant_payment_notifications.py
--rw-rw-rw-   0        0        0    11460 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_internal.py
--rw-rw-rw-   0        0        0    12719 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_kit_component.py
--rw-rw-rw-   0        0        0    11684 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_kit_definition.py
--rw-rw-rw-   0        0        0    15728 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_option.py
--rw-rw-rw-   0        0        0    16577 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_option_value.py
--rw-rw-rw-   0        0        0    11959 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_option_value_additional_item.py
--rw-rw-rw-   0        0        0    11832 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_option_value_digital_item.py
--rw-rw-rw-   0        0        0    13056 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_payment_processing.py
--rw-rw-rw-   0        0        0    12238 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_physical.py
--rw-rw-rw-   0        0        0    16963 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_pricing.py
--rw-rw-rw-   0        0        0    12900 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_pricing_tier.py
--rw-rw-rw-   0        0        0    11654 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_pricing_tier_discount.py
--rw-rw-rw-   0        0        0    12144 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_pricing_tier_limit.py
--rw-rw-rw-   0        0        0    12041 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_property.py
--rw-rw-rw-   0        0        0    12336 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_realtime_pricing.py
--rw-rw-rw-   0        0        0    12367 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_related.py
--rw-rw-rw-   0        0        0    12197 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_related_item.py
--rw-rw-rw-   0        0        0    11843 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_reporting.py
--rw-rw-rw-   0        0        0    12704 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_response.py
--rw-rw-rw-   0        0        0    13725 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_restriction.py
--rw-rw-rw-   0        0        0    12353 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_restriction_item.py
--rw-rw-rw-   0        0        0    13583 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_revguard.py
--rw-rw-rw-   0        0        0    19635 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_review.py
--rw-rw-rw-   0        0        0    14717 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_reviews.py
--rw-rw-rw-   0        0        0    11801 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_salesforce.py
--rw-rw-rw-   0        0        0    27671 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping.py
--rw-rw-rw-   0        0        0    12364 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_case.py
--rw-rw-rw-   0        0        0    12900 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_destination_markup.py
--rw-rw-rw-   0        0        0    12236 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_destination_restriction.py
--rw-rw-rw-   0        0        0    15701 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_distribution_center.py
--rw-rw-rw-   0        0        0    15931 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_method.py
--rw-rw-rw-   0        0        0    11774 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_package_requirement.py
--rw-rw-rw-   0        0        0    11829 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_tag.py
--rw-rw-rw-   0        0        0    11551 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_tags.py
--rw-rw-rw-   0        0        0    12652 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_tax.py
--rw-rw-rw-   0        0        0    12706 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_tax_exemption.py
--rw-rw-rw-   0        0        0    13056 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_third_party_email_marketing.py
--rw-rw-rw-   0        0        0    13067 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_variant_item.py
--rw-rw-rw-   0        0        0    13078 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_variation.py
--rw-rw-rw-   0        0        0    12481 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_variation_option.py
--rw-rw-rw-   0        0        0    12397 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_wishlist_member.py
--rw-rw-rw-   0        0        0    11548 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/items_request.py
--rw-rw-rw-   0        0        0    12732 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/items_response.py
--rw-rw-rw-   0        0        0    11984 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/key_value.py
--rw-rw-rw-   0        0        0    12039 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_filter_values.py
--rw-rw-rw-   0        0        0    12901 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_filter_values_response.py
--rw-rw-rw-   0        0        0    26505 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item.py
--rw-rw-rw-   0        0        0    11984 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_account.py
--rw-rw-rw-   0        0        0    11595 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_asset.py
--rw-rw-rw-   0        0        0    11592 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_attribute.py
--rw-rw-rw-   0        0        0    11908 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_email.py
--rw-rw-rw-   0        0        0    14805 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_published_meta.py
--rw-rw-rw-   0        0        0    12672 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_purchased_meta.py
--rw-rw-rw-   0        0        0    14637 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_query.py
--rw-rw-rw-   0        0        0    12815 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_response.py
--rw-rw-rw-   0        0        0    11678 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_screenshot.py
--rw-rw-rw-   0        0        0    12819 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_items_response.py
--rw-rw-rw-   0        0        0    12217 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/linked_account.py
--rw-rw-rw-   0        0        0    11768 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/list_segment_membership.py
--rw-rw-rw-   0        0        0    12240 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/lookup_request.py
--rw-rw-rw-   0        0        0    12755 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/lookup_response.py
--rw-rw-rw-   0        0        0    11385 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/mailgun.py
--rw-rw-rw-   0        0        0    12891 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/metric.py
--rw-rw-rw-   0        0        0    11571 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/model_property.py
--rw-rw-rw-   0        0        0    16098 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/notification.py
--rw-rw-rw-   0        0        0    11807 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/oauth_revoke_success_response.py
--rw-rw-rw-   0        0        0    13770 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/oauth_token_response.py
--rw-rw-rw-   0        0        0    24476 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order.py
--rw-rw-rw-   0        0        0    12446 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_affiliate.py
--rw-rw-rw-   0        0        0    14619 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_affiliate_ledger.py
--rw-rw-rw-   0        0        0    18519 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_auto_order.py
--rw-rw-rw-   0        0        0    16960 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_billing.py
--rw-rw-rw-   0        0        0    13383 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_buysafe.py
--rw-rw-rw-   0        0        0    11461 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_by_token_query.py
--rw-rw-rw-   0        0        0    16274 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_channel_partner.py
--rw-rw-rw-   0        0        0    16088 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_checkout.py
--rw-rw-rw-   0        0        0    13196 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_coupon.py
--rw-rw-rw-   0        0        0    13607 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_digital_item.py
--rw-rw-rw-   0        0        0    12968 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_digital_order.py
--rw-rw-rw-   0        0        0    12815 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_edi.py
--rw-rw-rw-   0        0        0    17003 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_format.py
--rw-rw-rw-   0        0        0    12041 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_format_response.py
--rw-rw-rw-   0        0        0    18057 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_fraud_score.py
--rw-rw-rw-   0        0        0    14445 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_gift.py
--rw-rw-rw-   0        0        0    12345 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_gift_certificate.py
--rw-rw-rw-   0        0        0    12999 2022-12-15 16:41:59.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_internal.py
--rw-rw-rw-   0        0        0    30809 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item.py
--rw-rw-rw-   0        0        0    12239 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_edi.py
--rw-rw-rw-   0        0        0    11803 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_edi_identification.py
--rw-rw-rw-   0        0        0    11954 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_edi_lot.py
--rw-rw-rw-   0        0        0    14939 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_option.py
--rw-rw-rw-   0        0        0    12170 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_option_file_attachment.py
--rw-rw-rw-   0        0        0    12377 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_property.py
--rw-rw-rw-   0        0        0    11500 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_tag.py
--rw-rw-rw-   0        0        0    13149 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_linked_shipment.py
--rw-rw-rw-   0        0        0    12596 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_marketing.py
--rw-rw-rw-   0        0        0    12719 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_packing_slip_response.py
--rw-rw-rw-   0        0        0    19148 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment.py
--rw-rw-rw-   0        0        0    11468 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_check.py
--rw-rw-rw-   0        0        0    15348 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_credit_card.py
--rw-rw-rw-   0        0        0    14976 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_e_check.py
--rw-rw-rw-   0        0        0    12239 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_insurance.py
--rw-rw-rw-   0        0        0    11555 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_purchase_order.py
--rw-rw-rw-   0        0        0    12668 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_transaction.py
--rw-rw-rw-   0        0        0    11835 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_transaction_detail.py
--rw-rw-rw-   0        0        0    12147 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_process_payment_request.py
--rw-rw-rw-   0        0        0    12959 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_process_payment_response.py
--rw-rw-rw-   0        0        0    12365 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_property.py
--rw-rw-rw-   0        0        0    24167 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_query.py
--rw-rw-rw-   0        0        0    11447 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_query_batch.py
--rw-rw-rw-   0        0        0    12012 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_quote.py
--rw-rw-rw-   0        0        0    12854 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_refundable_response.py
--rw-rw-rw-   0        0        0    16822 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_replacement.py
--rw-rw-rw-   0        0        0    12238 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_replacement_item.py
--rw-rw-rw-   0        0        0    12497 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_replacement_response.py
--rw-rw-rw-   0        0        0    12719 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_response.py
--rw-rw-rw-   0        0        0    11561 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_salesforce.py
--rw-rw-rw-   0        0        0    22057 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_shipping.py
--rw-rw-rw-   0        0        0    16793 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_summary.py
--rw-rw-rw-   0        0        0    11488 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_tag.py
--rw-rw-rw-   0        0        0    17986 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_taxes.py
--rw-rw-rw-   0        0        0    12789 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_token_response.py
--rw-rw-rw-   0        0        0    14014 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_tracking_number_detail.py
--rw-rw-rw-   0        0        0    16062 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_tracking_number_details.py
--rw-rw-rw-   0        0        0    12749 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/orders_response.py
--rw-rw-rw-   0        0        0    12199 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/permission.py
--rw-rw-rw-   0        0        0    20857 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/pricing_tier.py
--rw-rw-rw-   0        0        0    12053 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/pricing_tier_notification.py
--rw-rw-rw-   0        0        0    12858 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/pricing_tiers_response.py
--rw-rw-rw-   0        0        0    11551 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/publish_library_item_request.py
--rw-rw-rw-   0        0        0    13148 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/register_affiliate_click_request.py
--rw-rw-rw-   0        0        0    12481 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/register_affiliate_click_response.py
--rw-rw-rw-   0        0        0    11847 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/response_metadata.py
--rw-rw-rw-   0        0        0    13143 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/result_set.py
--rw-rw-rw-   0        0        0    11420 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/ruler_validation_request.py
--rw-rw-rw-   0        0        0    11649 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/ruler_validation_response.py
--rw-rw-rw-   0        0        0    25104 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording.py
--rw-rw-rw-   0        0        0    12969 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_ad_platform.py
--rw-rw-rw-   0        0        0    28573 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter.py
--rw-rw-rw-   0        0        0    12259 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_geo_distance.py
--rw-rw-rw-   0        0        0    12040 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_ip_search.py
--rw-rw-rw-   0        0        0    16989 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view.py
--rw-rw-rw-   0        0        0    12094 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view_event.py
--rw-rw-rw-   0        0        0    13215 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view_event_param.py
--rw-rw-rw-   0        0        0    11979 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view_param.py
--rw-rw-rw-   0        0        0    12003 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view_referrer_param.py
--rw-rw-rw-   0        0        0    12159 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_range_big_decimal.py
--rw-rw-rw-   0        0        0    11693 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_range_date.py
--rw-rw-rw-   0        0        0    12120 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_range_integer.py
--rw-rw-rw-   0        0        0    12265 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_string_search.py
--rw-rw-rw-   0        0        0    16948 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values.py
--rw-rw-rw-   0        0        0    12020 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values_event.py
--rw-rw-rw-   0        0        0    12333 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values_event_params.py
--rw-rw-rw-   0        0        0    11651 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values_page_param.py
--rw-rw-rw-   0        0        0    13189 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values_page_view.py
--rw-rw-rw-   0        0        0    17649 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap.py
--rw-rw-rw-   0        0        0    11491 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_index_request.py
--rw-rw-rw-   0        0        0    12969 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_index_response.py
--rw-rw-rw-   0        0        0    12162 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_request.py
--rw-rw-rw-   0        0        0    11425 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_reset.py
--rw-rw-rw-   0        0        0    12901 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_response.py
--rw-rw-rw-   0        0        0    12580 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_url.py
--rw-rw-rw-   0        0        0    11504 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_merchant_notes_request.py
--rw-rw-rw-   0        0        0    12130 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_multifield.py
--rw-rw-rw-   0        0        0    16484 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view.py
--rw-rw-rw-   0        0        0    12734 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view_data_response.py
--rw-rw-rw-   0        0        0    12854 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view_event.py
--rw-rw-rw-   0        0        0    11930 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view_event_parameter.py
--rw-rw-rw-   0        0        0    11628 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view_parameter.py
--rw-rw-rw-   0        0        0    11699 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_query_request.py
--rw-rw-rw-   0        0        0    14706 2022-12-15 16:42:00.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_query_response.py
--rw-rw-rw-   0        0        0    13101 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_response.py
--rw-rw-rw-   0        0        0    13842 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_segment.py
--rw-rw-rw-   0        0        0    12901 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_segment_response.py
--rw-rw-rw-   0        0        0    12915 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_segments_response.py
--rw-rw-rw-   0        0        0    13463 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_settings.py
--rw-rw-rw-   0        0        0    12916 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_settings_response.py
--rw-rw-rw-   0        0        0    11732 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_store_front.py
--rw-rw-rw-   0        0        0    11433 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_tags_request.py
--rw-rw-rw-   0        0        0    12681 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_tags_response.py
--rw-rw-rw-   0        0        0    12724 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_user_agent.py
--rw-rw-rw-   0        0        0    11439 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_user_agent_device.py
--rw-rw-rw-   0        0        0    11798 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_user_agent_os.py
--rw-rw-rw-   0        0        0    11900 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_user_property.py
--rw-rw-rw-   0        0        0    12862 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/screenshots_response.py
--rw-rw-rw-   0        0        0    11601 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/self_config.py
--rw-rw-rw-   0        0        0    11738 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/simple_value.py
--rw-rw-rw-   0        0        0    12238 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/single_sign_on_authorize_request.py
--rw-rw-rw-   0        0        0    12069 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/single_sign_on_authorize_response.py
--rw-rw-rw-   0        0        0    11911 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/single_sign_on_token_request.py
--rw-rw-rw-   0        0        0    12334 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/single_sign_on_token_response.py
--rw-rw-rw-   0        0        0    13504 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/sovos_config.py
--rw-rw-rw-   0        0        0    11708 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/state_province.py
--rw-rw-rw-   0        0        0    11675 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/step_waiting.py
--rw-rw-rw-   0        0        0    13575 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/store_front.py
--rw-rw-rw-   0        0        0    12813 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/store_fronts_response.py
--rw-rw-rw-   0        0        0    14145 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_city.py
--rw-rw-rw-   0        0        0    14249 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_country.py
--rw-rw-rw-   0        0        0    12576 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_country_code.py
--rw-rw-rw-   0        0        0    14483 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_county.py
--rw-rw-rw-   0        0        0    14138 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_jar_config.py
--rw-rw-rw-   0        0        0    13412 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_postal_code.py
--rw-rw-rw-   0        0        0    11713 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_activate_result.py
--rw-rw-rw-   0        0        0    12307 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_avalara.py
--rw-rw-rw-   0        0        0    11851 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_avalara_companies_result.py
--rw-rw-rw-   0        0        0    12395 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_avalara_company.py
--rw-rw-rw-   0        0        0    12671 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_self.py
--rw-rw-rw-   0        0        0    11708 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_self_countries_response.py
--rw-rw-rw-   0        0        0    11674 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_self_regions_response.py
--rw-rw-rw-   0        0        0    12287 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_sovos.py
--rw-rw-rw-   0        0        0    12298 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_tax_jar.py
--rw-rw-rw-   0        0        0    11701 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_test_result.py
--rw-rw-rw-   0        0        0    12853 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_ultra_cart.py
--rw-rw-rw-   0        0        0    14551 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_ultra_cart_state.py
--rw-rw-rw-   0        0        0    14269 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_providers_response.py
--rw-rw-rw-   0        0        0    17623 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_state.py
--rw-rw-rw-   0        0        0    12542 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_state_code.py
--rw-rw-rw-   0        0        0    13028 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/temp_multimedia.py
--rw-rw-rw-   0        0        0    12860 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/temp_multimedia_response.py
--rw-rw-rw-   0        0        0    12251 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/thumbnail_parameters_request.py
--rw-rw-rw-   0        0        0    12887 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/thumbnail_parameters_response.py
--rw-rw-rw-   0        0        0    18214 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/transaction_email.py
--rw-rw-rw-   0        0        0    12719 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/transaction_email_list_response.py
--rw-rw-rw-   0        0        0    13055 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/transaction_email_option.py
--rw-rw-rw-   0        0        0    12830 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/transaction_email_response.py
--rw-rw-rw-   0        0        0    12072 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/twilio.py
--rw-rw-rw-   0        0        0    12947 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/twilio_response.py
--rw-rw-rw-   0        0        0    12748 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/twilios_response.py
--rw-rw-rw-   0        0        0    11616 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/ultra_cart_config.py
--rw-rw-rw-   0        0        0    12740 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/upload_coupon_codes_request.py
--rw-rw-rw-   0        0        0    13296 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/upload_coupon_codes_response.py
--rw-rw-rw-   0        0        0    17784 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/user.py
--rw-rw-rw-   0        0        0    12062 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/user_group_membership.py
--rw-rw-rw-   0        0        0    12096 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/user_login.py
--rw-rw-rw-   0        0        0    12790 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/user_logins_response.py
--rw-rw-rw-   0        0        0    12704 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/user_response.py
--rw-rw-rw-   0        0        0    12718 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/users_response.py
--rw-rw-rw-   0        0        0    11764 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/verification_record.py
--rw-rw-rw-   0        0        0    11864 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/warning.py
--rw-rw-rw-   0        0        0    18572 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook.py
--rw-rw-rw-   0        0        0    13293 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_event_category.py
--rw-rw-rw-   0        0        0    14399 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_event_subscription.py
--rw-rw-rw-   0        0        0    14638 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_log.py
--rw-rw-rw-   0        0        0    12800 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_log_response.py
--rw-rw-rw-   0        0        0    12979 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_log_summaries_response.py
--rw-rw-rw-   0        0        0    12004 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_log_summary.py
--rw-rw-rw-   0        0        0    12749 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_response.py
--rw-rw-rw-   0        0        0    12349 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_sample_request.py
--rw-rw-rw-   0        0        0    12956 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_sample_request_response.py
--rw-rw-rw-   0        0        0    12763 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhooks_response.py
--rw-rw-rw-   0        0        0    11726 2022-12-15 16:42:01.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model/weight.py
--rw-rw-rw-   0        0        0    82574 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/model_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-15 16:42:24.837840 ultracart_rest_sdk-4.0.98rc0/ultracart/models/
--rw-rw-rw-   0        0        0    53811 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/models/__init__.py
--rw-rw-rw-   0        0        0    14268 2022-12-15 16:42:08.000000 ultracart_rest_sdk-4.0.98rc0/ultracart/rest.py
-drwxrwxrwx   0        0        0        0 2022-12-15 16:42:24.884703 ultracart_rest_sdk-4.0.98rc0/ultracart_rest_sdk.egg-info/
--rw-rw-rw-   0        0        0      380 2022-12-15 16:42:13.000000 ultracart_rest_sdk-4.0.98rc0/ultracart_rest_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    32194 2022-12-15 16:42:13.000000 ultracart_rest_sdk-4.0.98rc0/ultracart_rest_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-15 16:42:13.000000 ultracart_rest_sdk-4.0.98rc0/ultracart_rest_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2022-12-15 16:42:13.000000 ultracart_rest_sdk-4.0.98rc0/ultracart_rest_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-15 16:42:13.000000 ultracart_rest_sdk-4.0.98rc0/ultracart_rest_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-15 21:42:39.753251 ultracart_rest_sdk-4.0.99rc0/
+-rw-rw-rw-   0        0        0    11558 2022-06-20 12:32:36.000000 ultracart_rest_sdk-4.0.99rc0/LICENSE
+-rw-rw-rw-   0        0        0      380 2022-12-15 21:42:39.753251 ultracart_rest_sdk-4.0.99rc0/PKG-INFO
+-rw-rw-rw-   0        0        0   142124 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/README.md
+-rw-rw-rw-   0        0        0       76 2022-12-15 21:42:39.753251 ultracart_rest_sdk-4.0.99rc0/setup.cfg
+-rw-rw-rw-   0        0        0      999 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-15 21:42:29.003993 ultracart_rest_sdk-4.0.99rc0/ultracart/
+-rw-rw-rw-   0        0        0      701 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-15 21:42:29.482032 ultracart_rest_sdk-4.0.99rc0/ultracart/api/
+-rw-rw-rw-   0        0        0      215 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/__init__.py
+-rw-rw-rw-   0        0        0    14519 2022-12-15 21:42:22.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/affiliate_api.py
+-rw-rw-rw-   0        0        0    53810 2022-12-15 21:42:22.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/auto_order_api.py
+-rw-rw-rw-   0        0        0    28545 2022-12-15 21:42:22.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/channel_partner_api.py
+-rw-rw-rw-   0        0        0    32295 2022-12-15 21:42:22.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/chargeback_api.py
+-rw-rw-rw-   0        0        0   105889 2022-12-15 21:42:22.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/checkout_api.py
+-rw-rw-rw-   0        0        0   135593 2022-12-15 21:42:22.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/conversation_api.py
+-rw-rw-rw-   0        0        0   109039 2022-12-15 21:42:22.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/coupon_api.py
+-rw-rw-rw-   0        0        0   117148 2022-12-15 21:42:22.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/customer_api.py
+-rw-rw-rw-   0        0        0    35183 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/fulfillment_api.py
+-rw-rw-rw-   0        0        0    46858 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/gift_certificate_api.py
+-rw-rw-rw-   0        0        0    30164 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/integration_log_api.py
+-rw-rw-rw-   0        0        0    95979 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/item_api.py
+-rw-rw-rw-   0        0        0    13636 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/oauth_api.py
+-rw-rw-rw-   0        0        0   143832 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/order_api.py
+-rw-rw-rw-   0        0        0    21632 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/sso_api.py
+-rw-rw-rw-   0        0        0   982262 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/storefront_api.py
+-rw-rw-rw-   0        0        0   148671 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/tax_api.py
+-rw-rw-rw-   0        0        0    56627 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/user_api.py
+-rw-rw-rw-   0        0        0    46761 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api/webhook_api.py
+-rw-rw-rw-   0        0        0    39074 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/api_client.py
+drwxrwxrwx   0        0        0        0 2022-12-15 21:42:29.497583 ultracart_rest_sdk-4.0.99rc0/ultracart/apis/
+-rw-rw-rw-   0        0        0     1409 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/apis/__init__.py
+-rw-rw-rw-   0        0        0    17844 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/configuration.py
+-rw-rw-rw-   0        0        0     5069 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/exceptions.py
+drwxrwxrwx   0        0        0        0 2022-12-15 21:42:39.675155 ultracart_rest_sdk-4.0.99rc0/ultracart/model/
+-rw-rw-rw-   0        0        0      343 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/__init__.py
+-rw-rw-rw-   0        0        0    17598 2022-12-15 21:42:08.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_config.py
+-rw-rw-rw-   0        0        0    13641 2022-12-15 21:42:08.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_config_response.py
+-rw-rw-rw-   0        0        0    12310 2022-12-15 21:42:08.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_day_activity.py
+-rw-rw-rw-   0        0        0    12850 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_stat_account.py
+-rw-rw-rw-   0        0        0    13774 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_stat_metrics.py
+-rw-rw-rw-   0        0        0    11655 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_stat_revenue.py
+-rw-rw-rw-   0        0        0    13337 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_stats_response.py
+-rw-rw-rw-   0        0        0    12709 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/activity.py
+-rw-rw-rw-   0        0        0    16337 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/add_library_item_request.py
+-rw-rw-rw-   0        0        0    13275 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/adjust_internal_certificate_request.py
+-rw-rw-rw-   0        0        0    13144 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/adjust_internal_certificate_response.py
+-rw-rw-rw-   0        0        0    15397 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_click.py
+-rw-rw-rw-   0        0        0    13069 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_click_query.py
+-rw-rw-rw-   0        0        0    12840 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_clicks_response.py
+-rw-rw-rw-   0        0        0    17778 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_ledger.py
+-rw-rw-rw-   0        0        0    13089 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_ledger_query.py
+-rw-rw-rw-   0        0        0    12857 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_ledgers_response.py
+-rw-rw-rw-   0        0        0    16127 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_link.py
+-rw-rw-rw-   0        0        0    12706 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/api_user_application_profile.py
+-rw-rw-rw-   0        0        0    12987 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/apply_library_item_request.py
+-rw-rw-rw-   0        0        0    15428 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/apply_library_item_response.py
+-rw-rw-rw-   0        0        0    19519 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order.py
+-rw-rw-rw-   0        0        0    21602 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_item.py
+-rw-rw-rw-   0        0        0    12406 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_item_future_schedule.py
+-rw-rw-rw-   0        0        0    11750 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_item_option.py
+-rw-rw-rw-   0        0        0    12723 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_item_simple_schedule.py
+-rw-rw-rw-   0        0        0    11723 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_log.py
+-rw-rw-rw-   0        0        0    11612 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_management.py
+-rw-rw-rw-   0        0        0    17247 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_query.py
+-rw-rw-rw-   0        0        0    11501 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_query_batch.py
+-rw-rw-rw-   0        0        0    12785 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_response.py
+-rw-rw-rw-   0        0        0    11640 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_orders_request.py
+-rw-rw-rw-   0        0        0    12799 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_orders_response.py
+-rw-rw-rw-   0        0        0    15408 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/avalara_config.py
+-rw-rw-rw-   0        0        0    12452 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/base_response.py
+-rw-rw-rw-   0        0        0    12228 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/browser.py
+-rw-rw-rw-   0        0        0    11398 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/browser_device.py
+-rw-rw-rw-   0        0        0    12148 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/browser_os.py
+-rw-rw-rw-   0        0        0    11956 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/browser_user_agent.py
+-rw-rw-rw-   0        0        0    20508 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart.py
+-rw-rw-rw-   0        0        0    11904 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_affiliate.py
+-rw-rw-rw-   0        0        0    11808 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_affirm_checkout_response.py
+-rw-rw-rw-   0        0        0    16564 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_billing.py
+-rw-rw-rw-   0        0        0    13145 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_buysafe.py
+-rw-rw-rw-   0        0        0    16032 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_checkout.py
+-rw-rw-rw-   0        0        0    11440 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_coupon.py
+-rw-rw-rw-   0        0        0    12087 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_currency_conversion.py
+-rw-rw-rw-   0        0        0    19383 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_customer_profile.py
+-rw-rw-rw-   0        0        0    14610 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_customer_profile_address.py
+-rw-rw-rw-   0        0        0    13299 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_customer_profile_credit_card.py
+-rw-rw-rw-   0        0        0    12019 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_finalize_order_request.py
+-rw-rw-rw-   0        0        0    16957 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_finalize_order_request_options.py
+-rw-rw-rw-   0        0        0    12736 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_finalize_order_response.py
+-rw-rw-rw-   0        0        0    13134 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_gift.py
+-rw-rw-rw-   0        0        0    12379 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_gift_certificate.py
+-rw-rw-rw-   0        0        0    20348 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item.py
+-rw-rw-rw-   0        0        0    11893 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_attribute.py
+-rw-rw-rw-   0        0        0    14070 2022-12-15 21:42:09.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_multimedia.py
+-rw-rw-rw-   0        0        0    12445 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_multimedia_thumbnail.py
+-rw-rw-rw-   0        0        0    15203 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_option.py
+-rw-rw-rw-   0        0        0    12820 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_option_value.py
+-rw-rw-rw-   0        0        0    12250 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_physical.py
+-rw-rw-rw-   0        0        0    11776 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_variation_selection.py
+-rw-rw-rw-   0        0        0    15756 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_kit_component_option.py
+-rw-rw-rw-   0        0        0    12302 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_marketing.py
+-rw-rw-rw-   0        0        0    13703 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment.py
+-rw-rw-rw-   0        0        0    11531 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_affirm.py
+-rw-rw-rw-   0        0        0    11559 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_amazon.py
+-rw-rw-rw-   0        0        0    11507 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_check.py
+-rw-rw-rw-   0        0        0    14285 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_credit_card.py
+-rw-rw-rw-   0        0        0    11552 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_purchase_order.py
+-rw-rw-rw-   0        0        0    12256 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_profile_login_request.py
+-rw-rw-rw-   0        0        0    11915 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_profile_login_response.py
+-rw-rw-rw-   0        0        0    11815 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_profile_register_request.py
+-rw-rw-rw-   0        0        0    11924 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_profile_register_response.py
+-rw-rw-rw-   0        0        0    12362 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_property.py
+-rw-rw-rw-   0        0        0    11815 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_response.py
+-rw-rw-rw-   0        0        0    13443 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings.py
+-rw-rw-rw-   0        0        0    11711 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_billing.py
+-rw-rw-rw-   0        0        0    12789 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_gift.py
+-rw-rw-rw-   0        0        0    12053 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_gift_wrap.py
+-rw-rw-rw-   0        0        0    16192 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_payment.py
+-rw-rw-rw-   0        0        0    12096 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_payment_amazon.py
+-rw-rw-rw-   0        0        0    12542 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_payment_credit_card.py
+-rw-rw-rw-   0        0        0    12861 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_payment_pay_pal.py
+-rw-rw-rw-   0        0        0    11607 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_province.py
+-rw-rw-rw-   0        0        0    13285 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_shipping.py
+-rw-rw-rw-   0        0        0    12908 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_shipping_calendar.py
+-rw-rw-rw-   0        0        0    15468 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_shipping_estimate.py
+-rw-rw-rw-   0        0        0    11426 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_taxes.py
+-rw-rw-rw-   0        0        0    11688 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_terms.py
+-rw-rw-rw-   0        0        0    17806 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_shipping.py
+-rw-rw-rw-   0        0        0    15618 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_summary.py
+-rw-rw-rw-   0        0        0    11961 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_taxes.py
+-rw-rw-rw-   0        0        0    12497 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_upsell_after.py
+-rw-rw-rw-   0        0        0    11782 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_validation_request.py
+-rw-rw-rw-   0        0        0    11909 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_validation_response.py
+-rw-rw-rw-   0        0        0    13335 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner.py
+-rw-rw-rw-   0        0        0    12801 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_cancel_response.py
+-rw-rw-rw-   0        0        0    13090 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_estimate_shipping_response.py
+-rw-rw-rw-   0        0        0    12744 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_estimate_tax_response.py
+-rw-rw-rw-   0        0        0    13430 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_import_response.py
+-rw-rw-rw-   0        0        0    41481 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order.py
+-rw-rw-rw-   0        0        0    14458 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order_item.py
+-rw-rw-rw-   0        0        0    11741 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order_item_option.py
+-rw-rw-rw-   0        0        0    12195 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order_transaction.py
+-rw-rw-rw-   0        0        0    11762 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order_transaction_detail.py
+-rw-rw-rw-   0        0        0    11987 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_shipping_estimate.py
+-rw-rw-rw-   0        0        0    18191 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/chargeback_dispute.py
+-rw-rw-rw-   0        0        0    12865 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/chargeback_dispute_response.py
+-rw-rw-rw-   0        0        0    12879 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/chargeback_disputes_response.py
+-rw-rw-rw-   0        0        0    11635 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_allowed_countries_response.py
+-rw-rw-rw-   0        0        0    14935 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_handoff_request.py
+-rw-rw-rw-   0        0        0    12297 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_handoff_response.py
+-rw-rw-rw-   0        0        0    11748 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_setup_browser_key_request.py
+-rw-rw-rw-   0        0        0    11633 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_setup_browser_key_response.py
+-rw-rw-rw-   0        0        0    11698 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_state_province_response.py
+-rw-rw-rw-   0        0        0    12129 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/city_state_zip.py
+-rw-rw-rw-   0        0        0    16816 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation.py
+-rw-rw-rw-   0        0        0    12970 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_agent_auth.py
+-rw-rw-rw-   0        0        0    12906 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_agent_auth_response.py
+-rw-rw-rw-   0        0        0    11625 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_autocomplete_request.py
+-rw-rw-rw-   0        0        0    13323 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_autocomplete_response.py
+-rw-rw-rw-   0        0        0    11654 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_autocomplete_value.py
+-rw-rw-rw-   0        0        0    12299 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_canned_message.py
+-rw-rw-rw-   0        0        0    13031 2022-12-15 21:42:10.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_canned_message_response.py
+-rw-rw-rw-   0        0        0    13045 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_canned_messages_response.py
+-rw-rw-rw-   0        0        0    11688 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_canned_messages_search.py
+-rw-rw-rw-   0        0        0    12551 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_department.py
+-rw-rw-rw-   0        0        0    12980 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_department_response.py
+-rw-rw-rw-   0        0        0    12994 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_departments_response.py
+-rw-rw-rw-   0        0        0    13050 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_engagement.py
+-rw-rw-rw-   0        0        0    12980 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_engagement_response.py
+-rw-rw-rw-   0        0        0    12994 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_engagements_response.py
+-rw-rw-rw-   0        0        0    11873 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_add_coupon.py
+-rw-rw-rw-   0        0        0    12010 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_add_item.py
+-rw-rw-rw-   0        0        0    11905 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_queue_position.py
+-rw-rw-rw-   0        0        0    12012 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_read_message.py
+-rw-rw-rw-   0        0        0    12825 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_rr_web.py
+-rw-rw-rw-   0        0        0    12094 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_typing.py
+-rw-rw-rw-   0        0        0    11818 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_webchat_context.py
+-rw-rw-rw-   0        0        0    11543 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_join_request.py
+-rw-rw-rw-   0        0        0    15734 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_message.py
+-rw-rw-rw-   0        0        0    11682 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_message_translation.py
+-rw-rw-rw-   0        0        0    12327 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_message_transport_status.py
+-rw-rw-rw-   0        0        0    12949 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_messages_response.py
+-rw-rw-rw-   0        0        0    11610 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_multimedia_upload_url.py
+-rw-rw-rw-   0        0        0    13127 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_multimedia_upload_url_response.py
+-rw-rw-rw-   0        0        0    14482 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_participant.py
+-rw-rw-rw-   0        0        0    12824 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_response.py
+-rw-rw-rw-   0        0        0    14007 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_search_request.py
+-rw-rw-rw-   0        0        0    11848 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_search_response.py
+-rw-rw-rw-   0        0        0    12123 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_start_request.py
+-rw-rw-rw-   0        0        0    11658 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_start_response.py
+-rw-rw-rw-   0        0        0    16021 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_summary.py
+-rw-rw-rw-   0        0        0    11723 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_twilio_account.py
+-rw-rw-rw-   0        0        0    13789 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_context.py
+-rw-rw-rw-   0        0        0    16005 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_status.py
+-rw-rw-rw-   0        0        0    13126 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_status_agent.py
+-rw-rw-rw-   0        0        0    13169 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_status_queue_entry.py
+-rw-rw-rw-   0        0        0    11708 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_status_update_request.py
+-rw-rw-rw-   0        0        0    13029 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_statuses_response.py
+-rw-rw-rw-   0        0        0    18978 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_websocket_message.py
+-rw-rw-rw-   0        0        0    12888 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversations_response.py
+-rw-rw-rw-   0        0        0    11590 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/countries_response.py
+-rw-rw-rw-   0        0        0    11743 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/country.py
+-rw-rw-rw-   0        0        0    42889 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon.py
+-rw-rw-rw-   0        0        0    12601 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_items.py
+-rw-rw-rw-   0        0        0    12360 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_shipping.py
+-rw-rw-rw-   0        0        0    12756 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_shipping_with_items_purchase.py
+-rw-rw-rw-   0        0        0    11988 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal.py
+-rw-rw-rw-   0        0        0    12021 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_and_shipping.py
+-rw-rw-rw-   0        0        0    12781 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_free_shipping_with_purchase.py
+-rw-rw-rw-   0        0        0    12935 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_with_block_purchase.py
+-rw-rw-rw-   0        0        0    12860 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_with_items_purchase.py
+-rw-rw-rw-   0        0        0    12407 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_with_purchase.py
+-rw-rw-rw-   0        0        0    12894 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_shipping_with_subtotal.py
+-rw-rw-rw-   0        0        0    12434 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_auto_apply_condition.py
+-rw-rw-rw-   0        0        0    13244 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_auto_apply_conditions.py
+-rw-rw-rw-   0        0        0    11634 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_automatically_apply_coupon_codes.py
+-rw-rw-rw-   0        0        0    11968 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_buy_one_get_one_limit.py
+-rw-rw-rw-   0        0        0    13238 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_codes_request.py
+-rw-rw-rw-   0        0        0    12987 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_codes_response.py
+-rw-rw-rw-   0        0        0    11728 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_deletes_request.py
+-rw-rw-rw-   0        0        0    13180 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_discount_item_with_item_purchase.py
+-rw-rw-rw-   0        0        0    12597 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_discount_items.py
+-rw-rw-rw-   0        0        0    14374 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_editor_values.py
+-rw-rw-rw-   0        0        0    12922 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_exists_response.py
+-rw-rw-rw-   0        0        0    13078 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_item_and_shipping_with_subtotal.py
+-rw-rw-rw-   0        0        0    12926 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_item_with_item_purchase.py
+-rw-rw-rw-   0        0        0    12707 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_item_with_subtotal.py
+-rw-rw-rw-   0        0        0    13219 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_items_with_item_purchase.py
+-rw-rw-rw-   0        0        0    13376 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_items_with_mix_match_purchase.py
+-rw-rw-rw-   0        0        0    11597 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_shipping.py
+-rw-rw-rw-   0        0        0    11615 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_shipping_specific_items.py
+-rw-rw-rw-   0        0        0    11993 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_shipping_with_items_purchase.py
+-rw-rw-rw-   0        0        0    12459 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_shipping_with_subtotal.py
+-rw-rw-rw-   0        0        0    13900 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_item_search_result.py
+-rw-rw-rw-   0        0        0    12978 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_item_search_results_response.py
+-rw-rw-rw-   0        0        0    12113 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_multiple_amounts_off_items.py
+-rw-rw-rw-   0        0        0    11708 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_no_discount.py
+-rw-rw-rw-   0        0        0    13207 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_item_with_items_quantity_purchase.py
+-rw-rw-rw-   0        0        0    12600 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_items.py
+-rw-rw-rw-   0        0        0    12354 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_items_and_free_shipping.py
+-rw-rw-rw-   0        0        0    12742 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_items_with_items_purchase.py
+-rw-rw-rw-   0        0        0    13219 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_msrp_items.py
+-rw-rw-rw-   0        0        0    12633 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_retail_price_items.py
+-rw-rw-rw-   0        0        0    11933 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_shipping.py
+-rw-rw-rw-   0        0        0    11561 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal.py
+-rw-rw-rw-   0        0        0    11944 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal_and_free_shipping.py
+-rw-rw-rw-   0        0        0    12328 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal_limit.py
+-rw-rw-rw-   0        0        0    11963 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal_with_items_purchase.py
+-rw-rw-rw-   0        0        0    12409 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal_with_subtotal.py
+-rw-rw-rw-   0        0        0    14140 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_query.py
+-rw-rw-rw-   0        0        0    13173 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_response.py
+-rw-rw-rw-   0        0        0    12121 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_restriction.py
+-rw-rw-rw-   0        0        0    12255 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_amount.py
+-rw-rw-rw-   0        0        0    11833 2022-12-15 21:42:11.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_item_discount.py
+-rw-rw-rw-   0        0        0    12267 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_percent.py
+-rw-rw-rw-   0        0        0    12223 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_quantity_amount.py
+-rw-rw-rw-   0        0        0    12233 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_quantity_percent.py
+-rw-rw-rw-   0        0        0    12321 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_amount_off_items.py
+-rw-rw-rw-   0        0        0    12224 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_amount_off_subtotal.py
+-rw-rw-rw-   0        0        0    12431 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_percent_off_items.py
+-rw-rw-rw-   0        0        0    12465 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_percent_off_shipping.py
+-rw-rw-rw-   0        0        0    12234 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_percent_off_subtotal.py
+-rw-rw-rw-   0        0        0    12267 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_percent_off_subtotal_based_on_msrp.py
+-rw-rw-rw-   0        0        0    11772 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_type.py
+-rw-rw-rw-   0        0        0    11582 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupons_request.py
+-rw-rw-rw-   0        0        0    12748 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupons_response.py
+-rw-rw-rw-   0        0        0    12648 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/currency.py
+-rw-rw-rw-   0        0        0    32102 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer.py
+-rw-rw-rw-   0        0        0    13685 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_activity.py
+-rw-rw-rw-   0        0        0    12157 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_affiliate.py
+-rw-rw-rw-   0        0        0    12519 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_attachment.py
+-rw-rw-rw-   0        0        0    16404 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_billing.py
+-rw-rw-rw-   0        0        0    13673 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_card.py
+-rw-rw-rw-   0        0        0    12359 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_edi.py
+-rw-rw-rw-   0        0        0    14976 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_editor_values.py
+-rw-rw-rw-   0        0        0    13077 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_email.py
+-rw-rw-rw-   0        0        0    11886 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_email_list_changes.py
+-rw-rw-rw-   0        0        0    14106 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_loyalty.py
+-rw-rw-rw-   0        0        0    14834 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_loyalty_ledger.py
+-rw-rw-rw-   0        0        0    14828 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_loyalty_redemption.py
+-rw-rw-rw-   0        0        0    12674 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_magic_link_response.py
+-rw-rw-rw-   0        0        0    11814 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_merge_request.py
+-rw-rw-rw-   0        0        0    12297 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_orders_summary.py
+-rw-rw-rw-   0        0        0    11754 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_pricing_tier.py
+-rw-rw-rw-   0        0        0    12397 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_privacy.py
+-rw-rw-rw-   0        0        0    20888 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_query.py
+-rw-rw-rw-   0        0        0    12295 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_quotes_summary.py
+-rw-rw-rw-   0        0        0    12764 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_response.py
+-rw-rw-rw-   0        0        0    14096 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_reviewer.py
+-rw-rw-rw-   0        0        0    16421 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_shipping.py
+-rw-rw-rw-   0        0        0    14418 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_software_entitlement.py
+-rw-rw-rw-   0        0        0    13544 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_store_credit.py
+-rw-rw-rw-   0        0        0    12542 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_store_credit_add_request.py
+-rw-rw-rw-   0        0        0    13671 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_store_credit_ledger_entry.py
+-rw-rw-rw-   0        0        0    12941 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_store_credit_response.py
+-rw-rw-rw-   0        0        0    11497 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_tag.py
+-rw-rw-rw-   0        0        0    12743 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_tax_codes.py
+-rw-rw-rw-   0        0        0    12778 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/customers_response.py
+-rw-rw-rw-   0        0        0    12242 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/data_tables_server_side_response.py
+-rw-rw-rw-   0        0        0    11730 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/distance.py
+-rw-rw-rw-   0        0        0    24060 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/distribution_center.py
+-rw-rw-rw-   0        0        0    12934 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/distribution_centers_response.py
+-rw-rw-rw-   0        0        0    11491 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_base_template_list_response.py
+-rw-rw-rw-   0        0        0    20256 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign.py
+-rw-rw-rw-   0        0        0    12655 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign_folder.py
+-rw-rw-rw-   0        0        0    12911 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign_folder_response.py
+-rw-rw-rw-   0        0        0    12925 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign_folders_response.py
+-rw-rw-rw-   0        0        0    12815 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign_response.py
+-rw-rw-rw-   0        0        0    12829 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaigns_response.py
+-rw-rw-rw-   0        0        0    11623 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_click.py
+-rw-rw-rw-   0        0        0    12784 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_clicks_response.py
+-rw-rw-rw-   0        0        0    12659 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq.py
+-rw-rw-rw-   0        0        0    20021 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_email.py
+-rw-rw-rw-   0        0        0    12841 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_email_response.py
+-rw-rw-rw-   0        0        0    13620 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_email_send_test_request.py
+-rw-rw-rw-   0        0        0    12515 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_email_send_test_response.py
+-rw-rw-rw-   0        0        0    12770 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_emails_request.py
+-rw-rw-rw-   0        0        0    12855 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_emails_response.py
+-rw-rw-rw-   0        0        0    15641 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcard.py
+-rw-rw-rw-   0        0        0    12886 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcard_response.py
+-rw-rw-rw-   0        0        0    14044 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcard_send_test_request.py
+-rw-rw-rw-   0        0        0    13200 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcard_send_test_response.py
+-rw-rw-rw-   0        0        0    11549 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcards_request.py
+-rw-rw-rw-   0        0        0    12900 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcards_response.py
+-rw-rw-rw-   0        0        0    12875 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_response.py
+-rw-rw-rw-   0        0        0    14474 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_sequence_test_request.py
+-rw-rw-rw-   0        0        0    12512 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_sequence_test_response.py
+-rw-rw-rw-   0        0        0    12030 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_sms_send_test_request.py
+-rw-rw-rw-   0        0        0    12901 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_sms_send_test_response.py
+-rw-rw-rw-   0        0        0    22683 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_stat.py
+-rw-rw-rw-   0        0        0    12831 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_stat_response.py
+-rw-rw-rw-   0        0        0    15261 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_step.py
+-rw-rw-rw-   0        0        0    11841 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_step_log.py
+-rw-rw-rw-   0        0        0    12866 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_step_logs_response.py
+-rw-rw-rw-   0        0        0    12755 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_webhook_send_test_request.py
+-rw-rw-rw-   0        0        0    13219 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_webhook_send_test_response.py
+-rw-rw-rw-   0        0        0    12889 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseqs_response.py
+-rw-rw-rw-   0        0        0    13491 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_customer.py
+-rw-rw-rw-   0        0        0    12714 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_customer_editor_url_response.py
+-rw-rw-rw-   0        0        0    12756 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_customers_response.py
+-rw-rw-rw-   0        0        0    13155 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_dashboard_activity.py
+-rw-rw-rw-   0        0        0    12912 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_dashboard_activity_response.py
+-rw-rw-rw-   0        0        0    12796 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_dashboard_stats_response.py
+-rw-rw-rw-   0        0        0    14341 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_domain.py
+-rw-rw-rw-   0        0        0    12671 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_editor_token_response.py
+-rw-rw-rw-   0        0        0    21242 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow.py
+-rw-rw-rw-   0        0        0    12051 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_back_populate_request.py
+-rw-rw-rw-   0        0        0    12503 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_back_populate_response.py
+-rw-rw-rw-   0        0        0    12607 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_folder.py
+-rw-rw-rw-   0        0        0    12851 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_folder_response.py
+-rw-rw-rw-   0        0        0    12865 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_folders_response.py
+-rw-rw-rw-   0        0        0    12755 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_response.py
+-rw-rw-rw-   0        0        0    12769 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flows_response.py
+-rw-rw-rw-   0        0        0    11449 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_global_settings.py
+-rw-rw-rw-   0        0        0    12911 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_global_settings_response.py
+-rw-rw-rw-   0        0        0    11441 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_global_unsubscribe_request.py
+-rw-rw-rw-   0        0        0    11508 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_global_unsubscribe_response.py
+-rw-rw-rw-   0        0        0    11510 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_histogram_property_names_response.py
+-rw-rw-rw-   0        0        0    11518 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_histogram_property_values_response.py
+-rw-rw-rw-   0        0        0    14940 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list.py
+-rw-rw-rw-   0        0        0    12704 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_archive_response.py
+-rw-rw-rw-   0        0        0    12257 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_customer.py
+-rw-rw-rw-   0        0        0    12797 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_customers_response.py
+-rw-rw-rw-   0        0        0    12755 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_response.py
+-rw-rw-rw-   0        0        0    12692 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_folder.py
+-rw-rw-rw-   0        0        0    12962 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_folder_response.py
+-rw-rw-rw-   0        0        0    12976 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_folders_response.py
+-rw-rw-rw-   0        0        0    12568 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_membership.py
+-rw-rw-rw-   0        0        0    12037 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_used_by.py
+-rw-rw-rw-   0        0        0    11649 2022-12-15 21:42:12.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_subscribe_response.py
+-rw-rw-rw-   0        0        0    12769 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_lists_response.py
+-rw-rw-rw-   0        0        0    12190 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_order.py
+-rw-rw-rw-   0        0        0    12784 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_orders_response.py
+-rw-rw-rw-   0        0        0    19999 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance.py
+-rw-rw-rw-   0        0        0    11912 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance_customer_histogram.py
+-rw-rw-rw-   0        0        0    12572 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance_customer_histogram_period.py
+-rw-rw-rw-   0        0        0    13165 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance_daily.py
+-rw-rw-rw-   0        0        0    12860 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance_response.py
+-rw-rw-rw-   0        0        0    15537 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_plan.py
+-rw-rw-rw-   0        0        0    13146 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_plan_additional.py
+-rw-rw-rw-   0        0        0    12755 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_plan_response.py
+-rw-rw-rw-   0        0        0    20459 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_postcard_stat.py
+-rw-rw-rw-   0        0        0    16866 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_postcard_tracking.py
+-rw-rw-rw-   0        0        0    12896 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_postcard_tracking_response.py
+-rw-rw-rw-   0        0        0    19182 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment.py
+-rw-rw-rw-   0        0        0    12728 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_archive_response.py
+-rw-rw-rw-   0        0        0    12287 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_customer.py
+-rw-rw-rw-   0        0        0    12827 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_customers_response.py
+-rw-rw-rw-   0        0        0    13512 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_download_prepare_response.py
+-rw-rw-rw-   0        0        0    12800 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_response.py
+-rw-rw-rw-   0        0        0    12814 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segments_response.py
+-rw-rw-rw-   0        0        0    12806 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_sending_domain_response.py
+-rw-rw-rw-   0        0        0    12820 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_sending_domains_response.py
+-rw-rw-rw-   0        0        0    15413 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_settings.py
+-rw-rw-rw-   0        0        0    12815 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_settings_response.py
+-rw-rw-rw-   0        0        0    22364 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat.py
+-rw-rw-rw-   0        0        0    11716 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat_postcard_summary_request.py
+-rw-rw-rw-   0        0        0    12868 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat_postcard_summary_response.py
+-rw-rw-rw-   0        0        0    11931 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat_summary_request.py
+-rw-rw-rw-   0        0        0    12787 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat_summary_response.py
+-rw-rw-rw-   0        0        0    21286 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_stat.py
+-rw-rw-rw-   0        0        0    11663 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_stat_request.py
+-rw-rw-rw-   0        0        0    12807 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_stat_response.py
+-rw-rw-rw-   0        0        0    11494 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_waiting_request.py
+-rw-rw-rw-   0        0        0    11660 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_waiting_response.py
+-rw-rw-rw-   0        0        0    14489 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_template.py
+-rw-rw-rw-   0        0        0    12829 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_templates_response.py
+-rw-rw-rw-   0        0        0    11594 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_list.py
+-rw-rw-rw-   0        0        0    11772 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_list_import_request.py
+-rw-rw-rw-   0        0        0    14767 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_provider.py
+-rw-rw-rw-   0        0        0    12931 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_providers_response.py
+-rw-rw-rw-   0        0        0    11591 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_tag.py
+-rw-rw-rw-   0        0        0    11655 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_verify_token_request.py
+-rw-rw-rw-   0        0        0    12685 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_verify_token_response.py
+-rw-rw-rw-   0        0        0    11461 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_verify_token_validate_request.py
+-rw-rw-rw-   0        0        0    12512 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_verify_token_validate_response.py
+-rw-rw-rw-   0        0        0    13258 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_webhook_editor_values_response.py
+-rw-rw-rw-   0        0        0    12757 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/error.py
+-rw-rw-rw-   0        0        0    12455 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/error_response.py
+-rw-rw-rw-   0        0        0    16598 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiment.py
+-rw-rw-rw-   0        0        0    12794 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiment_response.py
+-rw-rw-rw-   0        0        0    18996 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiment_variation.py
+-rw-rw-rw-   0        0        0    15007 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiment_variation_stat.py
+-rw-rw-rw-   0        0        0    12808 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiments_response.py
+-rw-rw-rw-   0        0        0    14237 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_directory.py
+-rw-rw-rw-   0        0        0    16303 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_file.py
+-rw-rw-rw-   0        0        0    13554 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_page.py
+-rw-rw-rw-   0        0        0    12881 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_page_response.py
+-rw-rw-rw-   0        0        0    11942 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_upload_request.py
+-rw-rw-rw-   0        0        0    12846 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_upload_url_response.py
+-rw-rw-rw-   0        0        0    11627 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/fulfillment_inventory.py
+-rw-rw-rw-   0        0        0    12894 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/fulfillment_shipment.py
+-rw-rw-rw-   0        0        0    11553 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/geo_point.py
+-rw-rw-rw-   0        0        0    12296 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/geocode_request.py
+-rw-rw-rw-   0        0        0    12874 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/geocode_response.py
+-rw-rw-rw-   0        0        0    16714 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate.py
+-rw-rw-rw-   0        0        0    12939 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate_create_request.py
+-rw-rw-rw-   0        0        0    13303 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate_ledger_entry.py
+-rw-rw-rw-   0        0        0    13908 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate_query.py
+-rw-rw-rw-   0        0        0    12875 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate_response.py
+-rw-rw-rw-   0        0        0    12889 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificates_response.py
+-rw-rw-rw-   0        0        0    13201 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/group.py
+-rw-rw-rw-   0        0        0    12719 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/group_response.py
+-rw-rw-rw-   0        0        0    12530 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/group_user_membership.py
+-rw-rw-rw-   0        0        0    12733 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/groups_response.py
+-rw-rw-rw-   0        0        0    13608 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/hit_page_view.py
+-rw-rw-rw-   0        0        0    11584 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/hit_page_view_meta_data.py
+-rw-rw-rw-   0        0        0    15003 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/hit_session_start.py
+-rw-rw-rw-   0        0        0    14175 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/hit_session_utm.py
+-rw-rw-rw-   0        0        0    11664 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/http_header.py
+-rw-rw-rw-   0        0        0    15289 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log.py
+-rw-rw-rw-   0        0        0    11962 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_file.py
+-rw-rw-rw-   0        0        0    11598 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_log.py
+-rw-rw-rw-   0        0        0    13922 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_query_filter_values.py
+-rw-rw-rw-   0        0        0    13975 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_query_request.py
+-rw-rw-rw-   0        0        0    13376 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_query_response.py
+-rw-rw-rw-   0        0        0    12860 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_response.py
+-rw-rw-rw-   0        0        0    13001 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_summary.py
+-rw-rw-rw-   0        0        0    11786 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_summary_query_request.py
+-rw-rw-rw-   0        0        0    13002 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_summary_query_response.py
+-rw-rw-rw-   0        0        0    30236 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item.py
+-rw-rw-rw-   0        0        0    12033 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_accounting.py
+-rw-rw-rw-   0        0        0    12125 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_amember.py
+-rw-rw-rw-   0        0        0    18365 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_auto_order.py
+-rw-rw-rw-   0        0        0    17558 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_auto_order_step.py
+-rw-rw-rw-   0        0        0    11830 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_auto_order_step_arbitrary_unit_cost_schedule.py
+-rw-rw-rw-   0        0        0    11788 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_auto_order_step_grandfather_pricing.py
+-rw-rw-rw-   0        0        0    12987 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_cc_bill.py
+-rw-rw-rw-   0        0        0    16646 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_channel_partner_mapping.py
+-rw-rw-rw-   0        0        0    12277 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_chargeback.py
+-rw-rw-rw-   0        0        0    12283 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_chargeback_addendum.py
+-rw-rw-rw-   0        0        0    12163 2022-12-15 21:42:13.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_chargeback_adjustment_request.py
+-rw-rw-rw-   0        0        0    12603 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_checkout.py
+-rw-rw-rw-   0        0        0    16094 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content.py
+-rw-rw-rw-   0        0        0    12933 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content_assignment.py
+-rw-rw-rw-   0        0        0    12390 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content_attribute.py
+-rw-rw-rw-   0        0        0    16332 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content_multimedia.py
+-rw-rw-rw-   0        0        0    12785 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content_multimedia_thumbnail.py
+-rw-rw-rw-   0        0        0    14016 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_delivery.py
+-rw-rw-rw-   0        0        0    15198 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_item.py
+-rw-rw-rw-   0        0        0    14650 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_item_pdf_meta.py
+-rw-rw-rw-   0        0        0    12856 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_item_response.py
+-rw-rw-rw-   0        0        0    12900 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_items_response.py
+-rw-rw-rw-   0        0        0    35287 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_ebay.py
+-rw-rw-rw-   0        0        0    11702 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_ebay_category_specific.py
+-rw-rw-rw-   0        0        0    12300 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_ebay_market_listing.py
+-rw-rw-rw-   0        0        0    14201 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_ebay_market_place_analysis.py
+-rw-rw-rw-   0        0        0    11893 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_email_notifications.py
+-rw-rw-rw-   0        0        0    11566 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_enrollment123.py
+-rw-rw-rw-   0        0        0    12516 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_fulfillment_addon.py
+-rw-rw-rw-   0        0        0    12053 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_gift_certificate.py
+-rw-rw-rw-   0        0        0    26424 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_google_product_search.py
+-rw-rw-rw-   0        0        0    12464 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_identifiers.py
+-rw-rw-rw-   0        0        0    12222 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_instant_payment_notification.py
+-rw-rw-rw-   0        0        0    11846 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_instant_payment_notifications.py
+-rw-rw-rw-   0        0        0    11460 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_internal.py
+-rw-rw-rw-   0        0        0    12719 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_kit_component.py
+-rw-rw-rw-   0        0        0    11684 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_kit_definition.py
+-rw-rw-rw-   0        0        0    15728 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_option.py
+-rw-rw-rw-   0        0        0    16577 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_option_value.py
+-rw-rw-rw-   0        0        0    11959 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_option_value_additional_item.py
+-rw-rw-rw-   0        0        0    11832 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_option_value_digital_item.py
+-rw-rw-rw-   0        0        0    13056 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_payment_processing.py
+-rw-rw-rw-   0        0        0    12238 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_physical.py
+-rw-rw-rw-   0        0        0    16963 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_pricing.py
+-rw-rw-rw-   0        0        0    12900 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_pricing_tier.py
+-rw-rw-rw-   0        0        0    11654 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_pricing_tier_discount.py
+-rw-rw-rw-   0        0        0    12144 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_pricing_tier_limit.py
+-rw-rw-rw-   0        0        0    12041 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_property.py
+-rw-rw-rw-   0        0        0    12336 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_realtime_pricing.py
+-rw-rw-rw-   0        0        0    12367 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_related.py
+-rw-rw-rw-   0        0        0    12197 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_related_item.py
+-rw-rw-rw-   0        0        0    11843 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_reporting.py
+-rw-rw-rw-   0        0        0    12704 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_response.py
+-rw-rw-rw-   0        0        0    13725 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_restriction.py
+-rw-rw-rw-   0        0        0    12353 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_restriction_item.py
+-rw-rw-rw-   0        0        0    13583 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_revguard.py
+-rw-rw-rw-   0        0        0    19635 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_review.py
+-rw-rw-rw-   0        0        0    14717 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_reviews.py
+-rw-rw-rw-   0        0        0    11801 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_salesforce.py
+-rw-rw-rw-   0        0        0    27671 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping.py
+-rw-rw-rw-   0        0        0    12364 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_case.py
+-rw-rw-rw-   0        0        0    12900 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_destination_markup.py
+-rw-rw-rw-   0        0        0    12236 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_destination_restriction.py
+-rw-rw-rw-   0        0        0    15701 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_distribution_center.py
+-rw-rw-rw-   0        0        0    15931 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_method.py
+-rw-rw-rw-   0        0        0    11774 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_package_requirement.py
+-rw-rw-rw-   0        0        0    11829 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_tag.py
+-rw-rw-rw-   0        0        0    11551 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_tags.py
+-rw-rw-rw-   0        0        0    12652 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_tax.py
+-rw-rw-rw-   0        0        0    12706 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_tax_exemption.py
+-rw-rw-rw-   0        0        0    13056 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_third_party_email_marketing.py
+-rw-rw-rw-   0        0        0    13067 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_variant_item.py
+-rw-rw-rw-   0        0        0    13078 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_variation.py
+-rw-rw-rw-   0        0        0    12481 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_variation_option.py
+-rw-rw-rw-   0        0        0    12397 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_wishlist_member.py
+-rw-rw-rw-   0        0        0    11548 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/items_request.py
+-rw-rw-rw-   0        0        0    12732 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/items_response.py
+-rw-rw-rw-   0        0        0    11984 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/key_value.py
+-rw-rw-rw-   0        0        0    12039 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_filter_values.py
+-rw-rw-rw-   0        0        0    12901 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_filter_values_response.py
+-rw-rw-rw-   0        0        0    26505 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item.py
+-rw-rw-rw-   0        0        0    11984 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_account.py
+-rw-rw-rw-   0        0        0    11595 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_asset.py
+-rw-rw-rw-   0        0        0    11592 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_attribute.py
+-rw-rw-rw-   0        0        0    11908 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_email.py
+-rw-rw-rw-   0        0        0    14805 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_published_meta.py
+-rw-rw-rw-   0        0        0    12672 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_purchased_meta.py
+-rw-rw-rw-   0        0        0    14637 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_query.py
+-rw-rw-rw-   0        0        0    12815 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_response.py
+-rw-rw-rw-   0        0        0    11678 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_screenshot.py
+-rw-rw-rw-   0        0        0    12819 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_items_response.py
+-rw-rw-rw-   0        0        0    12217 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/linked_account.py
+-rw-rw-rw-   0        0        0    11768 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/list_segment_membership.py
+-rw-rw-rw-   0        0        0    12240 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/lookup_request.py
+-rw-rw-rw-   0        0        0    12755 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/lookup_response.py
+-rw-rw-rw-   0        0        0    11385 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/mailgun.py
+-rw-rw-rw-   0        0        0    12891 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/metric.py
+-rw-rw-rw-   0        0        0    11571 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/model_property.py
+-rw-rw-rw-   0        0        0    16098 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/notification.py
+-rw-rw-rw-   0        0        0    11807 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/oauth_revoke_success_response.py
+-rw-rw-rw-   0        0        0    13770 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/oauth_token_response.py
+-rw-rw-rw-   0        0        0    24476 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order.py
+-rw-rw-rw-   0        0        0    12446 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_affiliate.py
+-rw-rw-rw-   0        0        0    14619 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_affiliate_ledger.py
+-rw-rw-rw-   0        0        0    18519 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_auto_order.py
+-rw-rw-rw-   0        0        0    16960 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_billing.py
+-rw-rw-rw-   0        0        0    13383 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_buysafe.py
+-rw-rw-rw-   0        0        0    11461 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_by_token_query.py
+-rw-rw-rw-   0        0        0    16274 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_channel_partner.py
+-rw-rw-rw-   0        0        0    16088 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_checkout.py
+-rw-rw-rw-   0        0        0    13196 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_coupon.py
+-rw-rw-rw-   0        0        0    13607 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_digital_item.py
+-rw-rw-rw-   0        0        0    12968 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_digital_order.py
+-rw-rw-rw-   0        0        0    12815 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_edi.py
+-rw-rw-rw-   0        0        0    17003 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_format.py
+-rw-rw-rw-   0        0        0    12041 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_format_response.py
+-rw-rw-rw-   0        0        0    18057 2022-12-15 21:42:14.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_fraud_score.py
+-rw-rw-rw-   0        0        0    14445 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_gift.py
+-rw-rw-rw-   0        0        0    12345 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_gift_certificate.py
+-rw-rw-rw-   0        0        0    12999 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_internal.py
+-rw-rw-rw-   0        0        0    30809 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item.py
+-rw-rw-rw-   0        0        0    12239 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_edi.py
+-rw-rw-rw-   0        0        0    11803 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_edi_identification.py
+-rw-rw-rw-   0        0        0    11954 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_edi_lot.py
+-rw-rw-rw-   0        0        0    14939 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_option.py
+-rw-rw-rw-   0        0        0    12170 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_option_file_attachment.py
+-rw-rw-rw-   0        0        0    12377 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_property.py
+-rw-rw-rw-   0        0        0    11500 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_tag.py
+-rw-rw-rw-   0        0        0    13149 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_linked_shipment.py
+-rw-rw-rw-   0        0        0    12596 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_marketing.py
+-rw-rw-rw-   0        0        0    12719 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_packing_slip_response.py
+-rw-rw-rw-   0        0        0    19148 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment.py
+-rw-rw-rw-   0        0        0    11468 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_check.py
+-rw-rw-rw-   0        0        0    15348 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_credit_card.py
+-rw-rw-rw-   0        0        0    14976 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_e_check.py
+-rw-rw-rw-   0        0        0    12239 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_insurance.py
+-rw-rw-rw-   0        0        0    11555 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_purchase_order.py
+-rw-rw-rw-   0        0        0    12668 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_transaction.py
+-rw-rw-rw-   0        0        0    11835 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_transaction_detail.py
+-rw-rw-rw-   0        0        0    12147 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_process_payment_request.py
+-rw-rw-rw-   0        0        0    12959 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_process_payment_response.py
+-rw-rw-rw-   0        0        0    12365 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_property.py
+-rw-rw-rw-   0        0        0    24167 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_query.py
+-rw-rw-rw-   0        0        0    11447 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_query_batch.py
+-rw-rw-rw-   0        0        0    12012 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_quote.py
+-rw-rw-rw-   0        0        0    12854 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_refundable_response.py
+-rw-rw-rw-   0        0        0    16822 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_replacement.py
+-rw-rw-rw-   0        0        0    12238 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_replacement_item.py
+-rw-rw-rw-   0        0        0    12497 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_replacement_response.py
+-rw-rw-rw-   0        0        0    12719 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_response.py
+-rw-rw-rw-   0        0        0    11561 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_salesforce.py
+-rw-rw-rw-   0        0        0    22057 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_shipping.py
+-rw-rw-rw-   0        0        0    16793 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_summary.py
+-rw-rw-rw-   0        0        0    11488 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_tag.py
+-rw-rw-rw-   0        0        0    17986 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_taxes.py
+-rw-rw-rw-   0        0        0    12789 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_token_response.py
+-rw-rw-rw-   0        0        0    14014 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_tracking_number_detail.py
+-rw-rw-rw-   0        0        0    16062 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_tracking_number_details.py
+-rw-rw-rw-   0        0        0    12749 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/orders_response.py
+-rw-rw-rw-   0        0        0    12199 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/permission.py
+-rw-rw-rw-   0        0        0    20857 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/pricing_tier.py
+-rw-rw-rw-   0        0        0    12053 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/pricing_tier_notification.py
+-rw-rw-rw-   0        0        0    12858 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/pricing_tiers_response.py
+-rw-rw-rw-   0        0        0    11551 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/publish_library_item_request.py
+-rw-rw-rw-   0        0        0    13148 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/register_affiliate_click_request.py
+-rw-rw-rw-   0        0        0    12481 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/register_affiliate_click_response.py
+-rw-rw-rw-   0        0        0    11847 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/response_metadata.py
+-rw-rw-rw-   0        0        0    13143 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/result_set.py
+-rw-rw-rw-   0        0        0    11420 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/ruler_validation_request.py
+-rw-rw-rw-   0        0        0    11649 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/ruler_validation_response.py
+-rw-rw-rw-   0        0        0    25104 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording.py
+-rw-rw-rw-   0        0        0    12969 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_ad_platform.py
+-rw-rw-rw-   0        0        0    28573 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter.py
+-rw-rw-rw-   0        0        0    12259 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_geo_distance.py
+-rw-rw-rw-   0        0        0    12040 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_ip_search.py
+-rw-rw-rw-   0        0        0    16989 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view.py
+-rw-rw-rw-   0        0        0    12094 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view_event.py
+-rw-rw-rw-   0        0        0    13215 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view_event_param.py
+-rw-rw-rw-   0        0        0    11979 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view_param.py
+-rw-rw-rw-   0        0        0    12003 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view_referrer_param.py
+-rw-rw-rw-   0        0        0    12159 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_range_big_decimal.py
+-rw-rw-rw-   0        0        0    11693 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_range_date.py
+-rw-rw-rw-   0        0        0    12120 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_range_integer.py
+-rw-rw-rw-   0        0        0    12265 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_string_search.py
+-rw-rw-rw-   0        0        0    16948 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values.py
+-rw-rw-rw-   0        0        0    12020 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values_event.py
+-rw-rw-rw-   0        0        0    12333 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values_event_params.py
+-rw-rw-rw-   0        0        0    11651 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values_page_param.py
+-rw-rw-rw-   0        0        0    13189 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values_page_view.py
+-rw-rw-rw-   0        0        0    17649 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap.py
+-rw-rw-rw-   0        0        0    11491 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_index_request.py
+-rw-rw-rw-   0        0        0    12969 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_index_response.py
+-rw-rw-rw-   0        0        0    12162 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_request.py
+-rw-rw-rw-   0        0        0    11425 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_reset.py
+-rw-rw-rw-   0        0        0    12901 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_response.py
+-rw-rw-rw-   0        0        0    12580 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_url.py
+-rw-rw-rw-   0        0        0    11504 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_merchant_notes_request.py
+-rw-rw-rw-   0        0        0    12130 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_multifield.py
+-rw-rw-rw-   0        0        0    16484 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view.py
+-rw-rw-rw-   0        0        0    12734 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view_data_response.py
+-rw-rw-rw-   0        0        0    12854 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view_event.py
+-rw-rw-rw-   0        0        0    11930 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view_event_parameter.py
+-rw-rw-rw-   0        0        0    11628 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view_parameter.py
+-rw-rw-rw-   0        0        0    11699 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_query_request.py
+-rw-rw-rw-   0        0        0    14706 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_query_response.py
+-rw-rw-rw-   0        0        0    13101 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_response.py
+-rw-rw-rw-   0        0        0    13842 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_segment.py
+-rw-rw-rw-   0        0        0    12901 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_segment_response.py
+-rw-rw-rw-   0        0        0    12915 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_segments_response.py
+-rw-rw-rw-   0        0        0    13463 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_settings.py
+-rw-rw-rw-   0        0        0    12916 2022-12-15 21:42:15.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_settings_response.py
+-rw-rw-rw-   0        0        0    11732 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_store_front.py
+-rw-rw-rw-   0        0        0    11433 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_tags_request.py
+-rw-rw-rw-   0        0        0    12681 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_tags_response.py
+-rw-rw-rw-   0        0        0    12724 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_user_agent.py
+-rw-rw-rw-   0        0        0    11439 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_user_agent_device.py
+-rw-rw-rw-   0        0        0    11798 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_user_agent_os.py
+-rw-rw-rw-   0        0        0    11900 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_user_property.py
+-rw-rw-rw-   0        0        0    12862 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/screenshots_response.py
+-rw-rw-rw-   0        0        0    11601 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/self_config.py
+-rw-rw-rw-   0        0        0    11738 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/simple_value.py
+-rw-rw-rw-   0        0        0    12238 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/single_sign_on_authorize_request.py
+-rw-rw-rw-   0        0        0    12069 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/single_sign_on_authorize_response.py
+-rw-rw-rw-   0        0        0    11911 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/single_sign_on_token_request.py
+-rw-rw-rw-   0        0        0    12334 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/single_sign_on_token_response.py
+-rw-rw-rw-   0        0        0    13504 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/sovos_config.py
+-rw-rw-rw-   0        0        0    11708 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/state_province.py
+-rw-rw-rw-   0        0        0    11675 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/step_waiting.py
+-rw-rw-rw-   0        0        0    13575 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/store_front.py
+-rw-rw-rw-   0        0        0    12813 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/store_fronts_response.py
+-rw-rw-rw-   0        0        0    14145 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_city.py
+-rw-rw-rw-   0        0        0    14249 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_country.py
+-rw-rw-rw-   0        0        0    12576 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_country_code.py
+-rw-rw-rw-   0        0        0    14483 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_county.py
+-rw-rw-rw-   0        0        0    14138 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_jar_config.py
+-rw-rw-rw-   0        0        0    13412 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_postal_code.py
+-rw-rw-rw-   0        0        0    11713 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_activate_result.py
+-rw-rw-rw-   0        0        0    12307 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_avalara.py
+-rw-rw-rw-   0        0        0    11851 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_avalara_companies_result.py
+-rw-rw-rw-   0        0        0    12395 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_avalara_company.py
+-rw-rw-rw-   0        0        0    12671 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_self.py
+-rw-rw-rw-   0        0        0    11708 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_self_countries_response.py
+-rw-rw-rw-   0        0        0    11674 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_self_regions_response.py
+-rw-rw-rw-   0        0        0    12287 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_sovos.py
+-rw-rw-rw-   0        0        0    12298 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_tax_jar.py
+-rw-rw-rw-   0        0        0    11701 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_test_result.py
+-rw-rw-rw-   0        0        0    12853 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_ultra_cart.py
+-rw-rw-rw-   0        0        0    14551 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_ultra_cart_state.py
+-rw-rw-rw-   0        0        0    14269 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_providers_response.py
+-rw-rw-rw-   0        0        0    17623 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_state.py
+-rw-rw-rw-   0        0        0    12542 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_state_code.py
+-rw-rw-rw-   0        0        0    13028 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/temp_multimedia.py
+-rw-rw-rw-   0        0        0    12860 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/temp_multimedia_response.py
+-rw-rw-rw-   0        0        0    12251 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/thumbnail_parameters_request.py
+-rw-rw-rw-   0        0        0    12887 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/thumbnail_parameters_response.py
+-rw-rw-rw-   0        0        0    18214 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/transaction_email.py
+-rw-rw-rw-   0        0        0    12719 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/transaction_email_list_response.py
+-rw-rw-rw-   0        0        0    13055 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/transaction_email_option.py
+-rw-rw-rw-   0        0        0    12830 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/transaction_email_response.py
+-rw-rw-rw-   0        0        0    12072 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/twilio.py
+-rw-rw-rw-   0        0        0    12947 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/twilio_response.py
+-rw-rw-rw-   0        0        0    12748 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/twilios_response.py
+-rw-rw-rw-   0        0        0    11616 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/ultra_cart_config.py
+-rw-rw-rw-   0        0        0    12740 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/upload_coupon_codes_request.py
+-rw-rw-rw-   0        0        0    13296 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/upload_coupon_codes_response.py
+-rw-rw-rw-   0        0        0    17784 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/user.py
+-rw-rw-rw-   0        0        0    12062 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/user_group_membership.py
+-rw-rw-rw-   0        0        0    12096 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/user_login.py
+-rw-rw-rw-   0        0        0    12790 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/user_logins_response.py
+-rw-rw-rw-   0        0        0    12704 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/user_response.py
+-rw-rw-rw-   0        0        0    12718 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/users_response.py
+-rw-rw-rw-   0        0        0    11764 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/verification_record.py
+-rw-rw-rw-   0        0        0    11864 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/warning.py
+-rw-rw-rw-   0        0        0    18572 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook.py
+-rw-rw-rw-   0        0        0    13293 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_event_category.py
+-rw-rw-rw-   0        0        0    14399 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_event_subscription.py
+-rw-rw-rw-   0        0        0    14638 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_log.py
+-rw-rw-rw-   0        0        0    12800 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_log_response.py
+-rw-rw-rw-   0        0        0    12979 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_log_summaries_response.py
+-rw-rw-rw-   0        0        0    12004 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_log_summary.py
+-rw-rw-rw-   0        0        0    12749 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_response.py
+-rw-rw-rw-   0        0        0    12349 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_sample_request.py
+-rw-rw-rw-   0        0        0    12956 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_sample_request_response.py
+-rw-rw-rw-   0        0        0    12763 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhooks_response.py
+-rw-rw-rw-   0        0        0    11726 2022-12-15 21:42:16.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model/weight.py
+-rw-rw-rw-   0        0        0    82574 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/model_utils.py
+drwxrwxrwx   0        0        0        0 2022-12-15 21:42:39.690814 ultracart_rest_sdk-4.0.99rc0/ultracart/models/
+-rw-rw-rw-   0        0        0    53901 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/models/__init__.py
+-rw-rw-rw-   0        0        0    14268 2022-12-15 21:42:23.000000 ultracart_rest_sdk-4.0.99rc0/ultracart/rest.py
+drwxrwxrwx   0        0        0        0 2022-12-15 21:42:39.753251 ultracart_rest_sdk-4.0.99rc0/ultracart_rest_sdk.egg-info/
+-rw-rw-rw-   0        0        0      380 2022-12-15 21:42:28.000000 ultracart_rest_sdk-4.0.99rc0/ultracart_rest_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    32245 2022-12-15 21:42:28.000000 ultracart_rest_sdk-4.0.99rc0/ultracart_rest_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-15 21:42:28.000000 ultracart_rest_sdk-4.0.99rc0/ultracart_rest_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2022-12-15 21:42:28.000000 ultracart_rest_sdk-4.0.99rc0/ultracart_rest_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-12-15 21:42:28.000000 ultracart_rest_sdk-4.0.99rc0/ultracart_rest_sdk.egg-info/top_level.txt
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/LICENSE` & `ultracart_rest_sdk-4.0.99rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/README.md` & `ultracart_rest_sdk-4.0.99rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ultracart_rest_sdk
 UltraCart REST API Version 2
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 2.0.0
-- Package version: 4.0.98-RC
+- Package version: 4.0.99-RC
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [http://www.ultracart.com](http://www.ultracart.com)
 
 ## Requirements.
 
 Python >=3.6
 
@@ -619,14 +619,15 @@
  - [CheckoutStateProvinceResponse](docs/CheckoutStateProvinceResponse.md)
  - [CityStateZip](docs/CityStateZip.md)
  - [Conversation](docs/Conversation.md)
  - [ConversationAgentAuth](docs/ConversationAgentAuth.md)
  - [ConversationAgentAuthResponse](docs/ConversationAgentAuthResponse.md)
  - [ConversationAutocompleteRequest](docs/ConversationAutocompleteRequest.md)
  - [ConversationAutocompleteResponse](docs/ConversationAutocompleteResponse.md)
+ - [ConversationAutocompleteValue](docs/ConversationAutocompleteValue.md)
  - [ConversationCannedMessage](docs/ConversationCannedMessage.md)
  - [ConversationCannedMessageResponse](docs/ConversationCannedMessageResponse.md)
  - [ConversationCannedMessagesResponse](docs/ConversationCannedMessagesResponse.md)
  - [ConversationCannedMessagesSearch](docs/ConversationCannedMessagesSearch.md)
  - [ConversationDepartment](docs/ConversationDepartment.md)
  - [ConversationDepartmentResponse](docs/ConversationDepartmentResponse.md)
  - [ConversationDepartmentsResponse](docs/ConversationDepartmentsResponse.md)
@@ -1302,14 +1303,15 @@
 
 
 # CHANGE LOG
 Not every change is committed to every SDK.
 
 | Version | Date | Comments |
 | --: | :-: | --- |
+| 4.0.99-RC | 12/15/2022 | conversation search - added start date filtering |
 | 4.0.98-RC | 12/15/2022 | conversation searching |
 | 4.0.97-RC | 12/13/2022 | conversations - add email and sms_phone to participant object |
 | 4.0.96-RC | 12/09/2022 | conversations - message translation |
 | 4.0.95-RC | 12/08/2022 | conversation canned messages |
 | 4.0.94-RC | 12/08/2022 | communications - expose the rebuild percentage |
 | 4.0.93-RC | 12/06/2022 | convo - add session_start_dts to webchat context, cart - add customer_profile.signup_dts |
 | 4.0.92-RC | 12/06/2022 | customer api - expose edi information and editor values |
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/setup.py` & `ultracart_rest_sdk-4.0.99rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ultracart_rest_sdk"
-VERSION = "4.0.98-RC"
+VERSION = "4.0.99-RC"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/__init__.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 2.0.0
     Contact: support@ultracart.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "4.0.98-RC"
+__version__ = "4.0.99-RC"
 
 # import ApiClient
 from ultracart.api_client import ApiClient
 
 # import Configuration
 from ultracart.configuration import Configuration
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/affiliate_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/affiliate_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/auto_order_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/auto_order_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/channel_partner_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/channel_partner_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/chargeback_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/chargeback_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/checkout_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/checkout_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/conversation_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/conversation_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/coupon_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/coupon_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/customer_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/customer_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/fulfillment_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/fulfillment_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/gift_certificate_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/gift_certificate_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/integration_log_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/integration_log_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/item_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/item_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/oauth_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/oauth_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/order_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/order_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/sso_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/sso_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/storefront_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/storefront_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/tax_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/tax_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/user_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/user_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api/webhook_api.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api/webhook_api.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/api_client.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/4.0.98-RC/python'
+        self.user_agent = 'OpenAPI-Generator/4.0.99-RC/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/apis/__init__.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/configuration.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.0.0\n"\
-               "SDK Package Version: 4.0.98-RC".\
+               "SDK Package Version: 4.0.99-RC".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/exceptions.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/exceptions.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_config.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_config.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_config_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_config_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_day_activity.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_day_activity.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_stat_account.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_stat_account.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_stat_metrics.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_stat_metrics.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_stat_revenue.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_stat_revenue.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/accounts_receivable_retry_stats_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/accounts_receivable_retry_stats_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/activity.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/activity.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/add_library_item_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/add_library_item_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/adjust_internal_certificate_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/adjust_internal_certificate_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/adjust_internal_certificate_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/adjust_internal_certificate_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_click.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_click.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_click_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_click_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_clicks_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_clicks_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_ledger.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_ledger.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_ledger_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_ledger_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_ledgers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_ledgers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/affiliate_link.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/affiliate_link.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/api_user_application_profile.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/api_user_application_profile.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/apply_library_item_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/apply_library_item_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/apply_library_item_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/apply_library_item_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_item_future_schedule.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_item_future_schedule.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_item_option.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_item_option.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_item_simple_schedule.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_item_simple_schedule.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_log.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_log.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_management.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_management.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_query_batch.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_query_batch.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_order_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_order_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_orders_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_orders_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/auto_orders_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/auto_orders_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/avalara_config.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/avalara_config.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/base_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/base_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/browser.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/browser.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/browser_device.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/browser_device.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/browser_os.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/browser_os.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/browser_user_agent.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/browser_user_agent.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_affiliate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_affiliate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_affirm_checkout_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_affirm_checkout_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_billing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_billing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_buysafe.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_buysafe.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_checkout.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_checkout.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_coupon.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_coupon.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_currency_conversion.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_currency_conversion.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_customer_profile.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_customer_profile.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_customer_profile_address.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_customer_profile_address.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_customer_profile_credit_card.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_customer_profile_credit_card.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_finalize_order_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_finalize_order_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_finalize_order_request_options.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_finalize_order_request_options.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_finalize_order_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_finalize_order_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_gift.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_gift.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_gift_certificate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_gift_certificate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_attribute.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_attribute.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_multimedia.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_multimedia.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_multimedia_thumbnail.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_multimedia_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_option.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_option.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_option_value.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_option_value.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_physical.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_physical.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_item_variation_selection.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_item_variation_selection.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_kit_component_option.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_kit_component_option.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_marketing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_marketing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_affirm.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_affirm.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_amazon.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_amazon.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_check.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_check.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_credit_card.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_credit_card.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_payment_purchase_order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_payment_purchase_order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_profile_login_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_profile_login_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_profile_login_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_profile_login_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_profile_register_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_profile_register_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_profile_register_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_profile_register_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_property.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_property.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_billing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_billing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_gift.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_gift.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_gift_wrap.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_gift_wrap.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_payment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_payment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_payment_amazon.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_payment_amazon.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_payment_credit_card.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_payment_credit_card.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_payment_pay_pal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_payment_pay_pal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_province.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_province.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_shipping_calendar.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_shipping_calendar.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_shipping_estimate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_shipping_estimate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_taxes.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_taxes.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_settings_terms.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_settings_terms.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_summary.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_summary.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_taxes.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_taxes.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_upsell_after.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_upsell_after.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_validation_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_validation_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/cart_validation_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/cart_validation_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_cancel_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_cancel_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_estimate_shipping_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_estimate_shipping_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_estimate_tax_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_estimate_tax_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_import_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_import_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order_item_option.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order_item_option.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order_transaction.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order_transaction.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_order_transaction_detail.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_order_transaction_detail.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/channel_partner_shipping_estimate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/channel_partner_shipping_estimate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/chargeback_dispute.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/chargeback_dispute.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/chargeback_dispute_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/chargeback_dispute_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/chargeback_disputes_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/chargeback_disputes_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_allowed_countries_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_allowed_countries_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_handoff_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_handoff_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_handoff_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_handoff_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_setup_browser_key_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_setup_browser_key_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_setup_browser_key_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_setup_browser_key_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/checkout_state_province_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/checkout_state_province_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/city_state_zip.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/city_state_zip.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_agent_auth.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_agent_auth.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_agent_auth_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_agent_auth_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_autocomplete_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_autocomplete_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_autocomplete_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/twilio_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,23 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
+    from ultracart.model.twilio import Twilio
     from ultracart.model.warning import Warning
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
+    globals()['Twilio'] = Twilio
     globals()['Warning'] = Warning
 
 
-class ConversationAutocompleteResponse(ModelNormal):
+class TwilioResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,47 +90,45 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'diagnostics': (str,),  # noqa: E501
             'error': (Error,),  # noqa: E501
-            'field': (str,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
-            'results': ([str],),  # noqa: E501
             'success': (bool,),  # noqa: E501
-            'term': (str,),  # noqa: E501
+            'twilio': (Twilio,),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'diagnostics': 'diagnostics',  # noqa: E501
         'error': 'error',  # noqa: E501
-        'field': 'field',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
-        'results': 'results',  # noqa: E501
         'success': 'success',  # noqa: E501
-        'term': 'term',  # noqa: E501
+        'twilio': 'twilio',  # noqa: E501
         'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ConversationAutocompleteResponse - a model defined in OpenAPI
+        """TwilioResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,20 +153,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            diagnostics (str): [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
-            field (str): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
-            results ([str]): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            term (str): [optional]  # noqa: E501
+            twilio (Twilio): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -212,15 +211,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ConversationAutocompleteResponse - a model defined in OpenAPI
+        """TwilioResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,20 +244,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            diagnostics (str): [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
-            field (str): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
-            results ([str]): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            term (str): [optional]  # noqa: E501
+            twilio (Twilio): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_canned_message.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_canned_message.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_canned_message_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_canned_message_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_canned_messages_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_canned_messages_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_canned_messages_search.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_canned_messages_search.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_department.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_department.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_department_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_department_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_departments_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_departments_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_engagement.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_engagement.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_engagement_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_engagement_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_engagements_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_engagements_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_add_coupon.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_add_coupon.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_add_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_add_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_queue_position.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_queue_position.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_read_message.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_read_message.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_rr_web.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_rr_web.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_typing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_typing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_event_webchat_context.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_event_webchat_context.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_join_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_join_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_message.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_message.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_message_translation.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_message_translation.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_message_transport_status.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_message_transport_status.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_messages_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_messages_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_multimedia_upload_url.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_multimedia_upload_url.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_multimedia_upload_url_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_multimedia_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_participant.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_participant.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_search_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/hit_page_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from ultracart.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from ultracart.model.hit_page_view_meta_data import HitPageViewMetaData
+    globals()['HitPageViewMetaData'] = HitPageViewMetaData
 
-class ConversationSearchRequest(ModelNormal):
+
+class HitPageView(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,68 +67,72 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'email_filter': (str,),  # noqa: E501
-            'language_filter': (str,),  # noqa: E501
-            'medium_filter': (str,),  # noqa: E501
-            'order_by_newest': (bool,),  # noqa: E501
-            'order_by_oldest': (bool,),  # noqa: E501
-            'range_begin': (int,),  # noqa: E501
-            'range_end': (int,),  # noqa: E501
-            'sms_phone_number_filter': (str,),  # noqa: E501
-            'text_search': (str,),  # noqa: E501
-            'visible_filter': (bool,),  # noqa: E501
+            'bounce': (bool,),  # noqa: E501
+            'meta_data': ([HitPageViewMetaData],),  # noqa: E501
+            'method': (str,),  # noqa: E501
+            'prefetch': (bool,),  # noqa: E501
+            'query': (str,),  # noqa: E501
+            'recording': (bool,),  # noqa: E501
+            'redirect': (bool,),  # noqa: E501
+            'referrer': (str,),  # noqa: E501
+            'time_on_page': (float,),  # noqa: E501
+            'title': (str,),  # noqa: E501
+            'url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email_filter': 'email_filter',  # noqa: E501
-        'language_filter': 'language_filter',  # noqa: E501
-        'medium_filter': 'medium_filter',  # noqa: E501
-        'order_by_newest': 'order_by_newest',  # noqa: E501
-        'order_by_oldest': 'order_by_oldest',  # noqa: E501
-        'range_begin': 'range_begin',  # noqa: E501
-        'range_end': 'range_end',  # noqa: E501
-        'sms_phone_number_filter': 'sms_phone_number_filter',  # noqa: E501
-        'text_search': 'text_search',  # noqa: E501
-        'visible_filter': 'visible_filter',  # noqa: E501
+        'bounce': 'bounce',  # noqa: E501
+        'meta_data': 'meta_data',  # noqa: E501
+        'method': 'method',  # noqa: E501
+        'prefetch': 'prefetch',  # noqa: E501
+        'query': 'query',  # noqa: E501
+        'recording': 'recording',  # noqa: E501
+        'redirect': 'redirect',  # noqa: E501
+        'referrer': 'referrer',  # noqa: E501
+        'time_on_page': 'time_on_page',  # noqa: E501
+        'title': 'title',  # noqa: E501
+        'url': 'url',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ConversationSearchRequest - a model defined in OpenAPI
+        """HitPageView - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,24 +157,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email_filter (str): [optional]  # noqa: E501
-            language_filter (str): [optional]  # noqa: E501
-            medium_filter (str): [optional]  # noqa: E501
-            order_by_newest (bool): [optional]  # noqa: E501
-            order_by_oldest (bool): [optional]  # noqa: E501
-            range_begin (int): [optional]  # noqa: E501
-            range_end (int): [optional]  # noqa: E501
-            sms_phone_number_filter (str): [optional]  # noqa: E501
-            text_search (str): [optional]  # noqa: E501
-            visible_filter (bool): [optional]  # noqa: E501
+            bounce (bool): [optional]  # noqa: E501
+            meta_data ([HitPageViewMetaData]): [optional]  # noqa: E501
+            method (str): [optional]  # noqa: E501
+            prefetch (bool): [optional]  # noqa: E501
+            query (str): [optional]  # noqa: E501
+            recording (bool): [optional]  # noqa: E501
+            redirect (bool): [optional]  # noqa: E501
+            referrer (str): [optional]  # noqa: E501
+            time_on_page (float): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -211,15 +220,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ConversationSearchRequest - a model defined in OpenAPI
+        """HitPageView - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,24 +253,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email_filter (str): [optional]  # noqa: E501
-            language_filter (str): [optional]  # noqa: E501
-            medium_filter (str): [optional]  # noqa: E501
-            order_by_newest (bool): [optional]  # noqa: E501
-            order_by_oldest (bool): [optional]  # noqa: E501
-            range_begin (int): [optional]  # noqa: E501
-            range_end (int): [optional]  # noqa: E501
-            sms_phone_number_filter (str): [optional]  # noqa: E501
-            text_search (str): [optional]  # noqa: E501
-            visible_filter (bool): [optional]  # noqa: E501
+            bounce (bool): [optional]  # noqa: E501
+            meta_data ([HitPageViewMetaData]): [optional]  # noqa: E501
+            method (str): [optional]  # noqa: E501
+            prefetch (bool): [optional]  # noqa: E501
+            query (str): [optional]  # noqa: E501
+            recording (bool): [optional]  # noqa: E501
+            redirect (bool): [optional]  # noqa: E501
+            referrer (str): [optional]  # noqa: E501
+            time_on_page (float): [optional]  # noqa: E501
+            title (str): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_search_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_search_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_start_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_start_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_start_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_start_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_summary.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_summary.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_twilio_account.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_twilio_account.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_context.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_context.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_status.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_status.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_status_agent.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_status_agent.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_status_queue_entry.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_status_queue_entry.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_status_update_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_status_update_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_webchat_queue_statuses_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_webchat_queue_statuses_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversation_websocket_message.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_websocket_message.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/conversations_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversations_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/countries_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/countries_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/country.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/country.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_shipping_with_items_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_shipping_with_items_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_and_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_and_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_free_shipping_with_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_free_shipping_with_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_with_block_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_with_block_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_with_items_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_with_items_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_off_subtotal_with_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_off_subtotal_with_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_amount_shipping_with_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_amount_shipping_with_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_auto_apply_condition.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_auto_apply_condition.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_auto_apply_conditions.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_auto_apply_conditions.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_automatically_apply_coupon_codes.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_automatically_apply_coupon_codes.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_buy_one_get_one_limit.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_buy_one_get_one_limit.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_codes_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_codes_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_codes_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_codes_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_deletes_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_deletes_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_discount_item_with_item_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_discount_item_with_item_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_discount_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_discount_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_editor_values.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_editor_values.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_exists_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_exists_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_item_and_shipping_with_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_item_and_shipping_with_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_item_with_item_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_item_with_item_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_item_with_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_item_with_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_items_with_item_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_items_with_item_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_items_with_mix_match_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_items_with_mix_match_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_shipping_specific_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_shipping_specific_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_shipping_with_items_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_shipping_with_items_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_free_shipping_with_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_free_shipping_with_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_item_search_result.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_item_search_result.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_item_search_results_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_item_search_results_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_multiple_amounts_off_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_multiple_amounts_off_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_no_discount.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_no_discount.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_item_with_items_quantity_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_item_with_items_quantity_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_items_and_free_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_items_and_free_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_items_with_items_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_items_with_items_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_msrp_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_msrp_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_retail_price_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_retail_price_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal_and_free_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal_and_free_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal_limit.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal_limit.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal_with_items_purchase.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal_with_items_purchase.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_percent_off_subtotal_with_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_percent_off_subtotal_with_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_restriction.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_restriction.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_amount.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_amount.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_item_discount.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_item_discount.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_percent.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_percent.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_quantity_amount.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_quantity_amount.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tier_quantity_percent.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tier_quantity_percent.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_amount_off_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_amount_off_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_amount_off_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_amount_off_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_percent_off_items.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_percent_off_items.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_percent_off_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_percent_off_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_percent_off_subtotal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_percent_off_subtotal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_tiered_percent_off_subtotal_based_on_msrp.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_tiered_percent_off_subtotal_based_on_msrp.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupon_type.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupon_type.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupons_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupons_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/coupons_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/coupons_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/currency.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/currency.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_activity.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_activity.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_affiliate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_affiliate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_attachment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_attachment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_billing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_billing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_card.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_card.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_edi.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_edi.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_editor_values.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_editor_values.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_email.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_email.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_email_list_changes.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_email_list_changes.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_loyalty.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_loyalty.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_loyalty_ledger.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_loyalty_ledger.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_loyalty_redemption.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_loyalty_redemption.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_magic_link_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_magic_link_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_merge_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_merge_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_orders_summary.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_orders_summary.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_pricing_tier.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_pricing_tier.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_privacy.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_privacy.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_quotes_summary.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_quotes_summary.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_reviewer.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_reviewer.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_software_entitlement.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_software_entitlement.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_store_credit.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_store_credit.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_store_credit_add_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_store_credit_add_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_store_credit_ledger_entry.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_store_credit_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_store_credit_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_store_credit_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_tag.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_tag.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customer_tax_codes.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customer_tax_codes.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/customers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/customers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/data_tables_server_side_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/data_tables_server_side_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/distance.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/distance.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/distribution_center.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/distribution_center.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/distribution_centers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/distribution_centers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_base_template_list_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_base_template_list_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign_folder.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign_folder.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign_folder_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign_folder_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign_folders_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign_folders_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaign_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaign_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_campaigns_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_click.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_click.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_clicks_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_clicks_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_email.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_email.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_email_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_email_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_email_send_test_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_email_send_test_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_email_send_test_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_email_send_test_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_emails_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_emails_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_emails_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_emails_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcard.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcard.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcard_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcard_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcard_send_test_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcard_send_test_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcard_send_test_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcard_send_test_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcards_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcards_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_postcards_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_postcards_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_sequence_test_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_sequence_test_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_sequence_test_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_sequence_test_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_sms_send_test_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_sms_send_test_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_sms_send_test_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_sms_send_test_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_stat.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_stat.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_stat_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_stat_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_step.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_step.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_step_log.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_step_log.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_step_logs_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_step_logs_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_webhook_send_test_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_webhook_send_test_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseq_webhook_send_test_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseq_webhook_send_test_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_commseqs_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_commseqs_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_customer.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_customer.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_customer_editor_url_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_customer_editor_url_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_customers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_customers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_dashboard_activity.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_dashboard_activity.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_dashboard_activity_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_dashboard_activity_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_dashboard_stats_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_dashboard_stats_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_domain.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_domain.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_editor_token_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_editor_token_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_back_populate_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_back_populate_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_back_populate_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_back_populate_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_folder.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_folder.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_folder_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_folder_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_folders_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_folders_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flow_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flow_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_flows_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_flows_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_global_settings.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_global_settings.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_global_settings_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_global_settings_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_global_unsubscribe_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_global_unsubscribe_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_global_unsubscribe_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_global_unsubscribe_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_histogram_property_names_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_histogram_property_names_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_histogram_property_values_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_histogram_property_values_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_archive_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_archive_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_customer.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_customer.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_customers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_customers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_folder.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_folder.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_folder_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_folder_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_folders_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_folders_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_membership.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_membership.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_segment_used_by.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_segment_used_by.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_list_subscribe_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_list_subscribe_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_lists_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_lists_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_orders_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_orders_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance_customer_histogram.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance_customer_histogram.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance_customer_histogram_period.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance_customer_histogram_period.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance_daily.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance_daily.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_performance_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_performance_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_plan.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_plan.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_plan_additional.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_plan_additional.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_plan_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_plan_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_postcard_stat.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_postcard_stat.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_postcard_tracking.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_postcard_tracking.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_postcard_tracking_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_postcard_tracking_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_archive_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_archive_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_customer.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_customer.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_customers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_customers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_download_prepare_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_download_prepare_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segment_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segment_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_segments_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_segments_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_sending_domain_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_sending_domain_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_sending_domains_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_sending_domains_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_settings.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_settings.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_settings_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_settings_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat_postcard_summary_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat_postcard_summary_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat_postcard_summary_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat_postcard_summary_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat_summary_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat_summary_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_stat_summary_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_stat_summary_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_stat.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_stat.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_stat_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_stat_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_stat_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_stat_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_waiting_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_waiting_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_step_waiting_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_step_waiting_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_template.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_template.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_templates_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_templates_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_list.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_list.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_list_import_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_list_import_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_provider.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_provider.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_providers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_providers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_third_party_tag.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_third_party_tag.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_verify_token_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_verify_token_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_verify_token_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_verify_token_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_verify_token_validate_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_verify_token_validate_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_verify_token_validate_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_verify_token_validate_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/email_webhook_editor_values_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/email_webhook_editor_values_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/error.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/error.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/error_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/error_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiment_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiment_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiment_variation.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiment_variation.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiment_variation_stat.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiment_variation_stat.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/experiments_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/experiments_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_directory.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_directory.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_file.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_file.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_page.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_page.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_page_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_page_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_upload_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_upload_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/file_manager_upload_url_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/file_manager_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/fulfillment_inventory.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/fulfillment_inventory.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/fulfillment_shipment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/fulfillment_shipment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/geo_point.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/geo_point.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/geocode_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/geocode_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/geocode_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/geocode_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate_create_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate_create_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate_ledger_entry.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificate_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificate_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/gift_certificates_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/gift_certificates_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/group.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/group.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/group_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/group_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/group_user_membership.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/group_user_membership.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/groups_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/groups_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/hit_page_view.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_geo_distance.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from ultracart.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from ultracart.model.hit_page_view_meta_data import HitPageViewMetaData
-    globals()['HitPageViewMetaData'] = HitPageViewMetaData
 
-
-class HitPageView(ModelNormal):
+class ScreenRecordingFilterGeoDistance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -67,72 +63,58 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'bounce': (bool,),  # noqa: E501
-            'meta_data': ([HitPageViewMetaData],),  # noqa: E501
-            'method': (str,),  # noqa: E501
-            'prefetch': (bool,),  # noqa: E501
-            'query': (str,),  # noqa: E501
-            'recording': (bool,),  # noqa: E501
-            'redirect': (bool,),  # noqa: E501
-            'referrer': (str,),  # noqa: E501
-            'time_on_page': (float,),  # noqa: E501
-            'title': (str,),  # noqa: E501
-            'url': (str,),  # noqa: E501
+            'distance': (int,),  # noqa: E501
+            'distance_uom': (str,),  # noqa: E501
+            'from_address': (str,),  # noqa: E501
+            'lat': (float,),  # noqa: E501
+            'lon': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'bounce': 'bounce',  # noqa: E501
-        'meta_data': 'meta_data',  # noqa: E501
-        'method': 'method',  # noqa: E501
-        'prefetch': 'prefetch',  # noqa: E501
-        'query': 'query',  # noqa: E501
-        'recording': 'recording',  # noqa: E501
-        'redirect': 'redirect',  # noqa: E501
-        'referrer': 'referrer',  # noqa: E501
-        'time_on_page': 'time_on_page',  # noqa: E501
-        'title': 'title',  # noqa: E501
-        'url': 'url',  # noqa: E501
+        'distance': 'distance',  # noqa: E501
+        'distance_uom': 'distance_uom',  # noqa: E501
+        'from_address': 'from_address',  # noqa: E501
+        'lat': 'lat',  # noqa: E501
+        'lon': 'lon',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """HitPageView - a model defined in OpenAPI
+        """ScreenRecordingFilterGeoDistance - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -157,25 +139,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            bounce (bool): [optional]  # noqa: E501
-            meta_data ([HitPageViewMetaData]): [optional]  # noqa: E501
-            method (str): [optional]  # noqa: E501
-            prefetch (bool): [optional]  # noqa: E501
-            query (str): [optional]  # noqa: E501
-            recording (bool): [optional]  # noqa: E501
-            redirect (bool): [optional]  # noqa: E501
-            referrer (str): [optional]  # noqa: E501
-            time_on_page (float): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
+            distance (int): [optional]  # noqa: E501
+            distance_uom (str): [optional]  # noqa: E501
+            from_address (str): [optional]  # noqa: E501
+            lat (float): [optional]  # noqa: E501
+            lon (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,15 +196,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """HitPageView - a model defined in OpenAPI
+        """ScreenRecordingFilterGeoDistance - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,25 +229,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            bounce (bool): [optional]  # noqa: E501
-            meta_data ([HitPageViewMetaData]): [optional]  # noqa: E501
-            method (str): [optional]  # noqa: E501
-            prefetch (bool): [optional]  # noqa: E501
-            query (str): [optional]  # noqa: E501
-            recording (bool): [optional]  # noqa: E501
-            redirect (bool): [optional]  # noqa: E501
-            referrer (str): [optional]  # noqa: E501
-            time_on_page (float): [optional]  # noqa: E501
-            title (str): [optional]  # noqa: E501
-            url (str): [optional]  # noqa: E501
+            distance (int): [optional]  # noqa: E501
+            distance_uom (str): [optional]  # noqa: E501
+            from_address (str): [optional]  # noqa: E501
+            lat (float): [optional]  # noqa: E501
+            lon (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/hit_page_view_meta_data.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/hit_page_view_meta_data.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/hit_session_start.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/hit_session_start.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/hit_session_utm.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/hit_session_utm.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/http_header.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/http_header.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_file.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_file.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_log.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_log.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_query_filter_values.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_query_filter_values.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_query_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_query_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_query_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_query_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_summary.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_summary.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_summary_query_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_summary_query_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/integration_log_summary_query_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/integration_log_summary_query_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_accounting.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_accounting.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_amember.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_amember.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_auto_order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_auto_order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_auto_order_step.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_auto_order_step.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_auto_order_step_arbitrary_unit_cost_schedule.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_auto_order_step_arbitrary_unit_cost_schedule.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_auto_order_step_grandfather_pricing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_auto_order_step_grandfather_pricing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_cc_bill.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_cc_bill.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_channel_partner_mapping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_channel_partner_mapping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_chargeback.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_chargeback.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_chargeback_addendum.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_chargeback_addendum.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_chargeback_adjustment_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_chargeback_adjustment_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_checkout.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_checkout.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content_assignment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content_assignment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content_attribute.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content_attribute.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content_multimedia.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content_multimedia.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_content_multimedia_thumbnail.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_content_multimedia_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_delivery.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_delivery.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_item_pdf_meta.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_item_pdf_meta.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_item_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_item_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_digital_items_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_digital_items_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_ebay.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_ebay.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_ebay_category_specific.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_ebay_category_specific.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_ebay_market_listing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_ebay_market_listing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_ebay_market_place_analysis.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_ebay_market_place_analysis.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_email_notifications.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_email_notifications.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_enrollment123.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_enrollment123.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_fulfillment_addon.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_fulfillment_addon.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_gift_certificate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_gift_certificate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_google_product_search.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_google_product_search.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_identifiers.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_identifiers.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_instant_payment_notification.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_instant_payment_notification.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_instant_payment_notifications.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_instant_payment_notifications.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_internal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_internal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_kit_component.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_kit_component.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_kit_definition.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_kit_definition.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_option.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_option.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_option_value.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_option_value.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_option_value_additional_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_option_value_additional_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_option_value_digital_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_option_value_digital_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_payment_processing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_payment_processing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_physical.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_physical.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_pricing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_pricing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_pricing_tier.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_pricing_tier.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_pricing_tier_discount.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_pricing_tier_discount.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_pricing_tier_limit.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_pricing_tier_limit.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_property.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_property.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_realtime_pricing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_realtime_pricing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_related.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_related.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_related_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_related_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_reporting.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_reporting.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_restriction.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_restriction.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_restriction_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_restriction_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_revguard.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_revguard.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_review.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_review.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_reviews.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_reviews.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_salesforce.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_salesforce.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_case.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_case.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_destination_markup.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_destination_markup.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_destination_restriction.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_destination_restriction.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_distribution_center.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_distribution_center.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_method.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_method.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_shipping_package_requirement.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_shipping_package_requirement.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_tag.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_tag.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_tags.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_tags.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_tax.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_tax.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_tax_exemption.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_tax_exemption.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_third_party_email_marketing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_third_party_email_marketing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_variant_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_variant_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_variation.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_variation.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_variation_option.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_variation_option.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/item_wishlist_member.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/item_wishlist_member.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/items_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/items_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/items_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/items_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/key_value.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/key_value.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_filter_values.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_filter_values.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_filter_values_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_filter_values_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_account.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_account.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_asset.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_asset.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_attribute.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_attribute.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_email.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_email.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_published_meta.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_published_meta.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_purchased_meta.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_purchased_meta.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_item_screenshot.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_item_screenshot.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/library_items_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/library_items_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/linked_account.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/linked_account.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/list_segment_membership.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/list_segment_membership.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/lookup_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/lookup_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/lookup_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/lookup_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/mailgun.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/mailgun.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/metric.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/metric.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/model_property.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/model_property.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/notification.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/notification.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/oauth_revoke_success_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/oauth_revoke_success_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/oauth_token_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/oauth_token_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_affiliate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_affiliate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_affiliate_ledger.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_affiliate_ledger.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_auto_order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_auto_order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_billing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_billing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_buysafe.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_buysafe.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_by_token_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_by_token_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_channel_partner.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_channel_partner.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_checkout.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_checkout.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_coupon.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_coupon.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_digital_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_digital_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_digital_order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_digital_order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_edi.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_edi.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_format.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_format.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_format_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_format_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_fraud_score.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_fraud_score.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_gift.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_gift.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_gift_certificate.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_gift_certificate.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_internal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_internal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_edi.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_edi.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_edi_identification.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_edi_identification.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_edi_lot.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_edi_lot.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_option.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_option.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_option_file_attachment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_option_file_attachment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_property.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_property.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_item_tag.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_item_tag.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_linked_shipment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_linked_shipment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_marketing.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_marketing.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_packing_slip_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_packing_slip_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_check.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_check.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_credit_card.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_credit_card.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_e_check.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_e_check.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_insurance.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_insurance.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_purchase_order.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_purchase_order.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_transaction.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_transaction.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_payment_transaction_detail.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_payment_transaction_detail.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_process_payment_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_process_payment_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_process_payment_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_process_payment_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_property.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_property.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_query.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_query.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_query_batch.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_query_batch.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_quote.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_quote.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_refundable_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_refundable_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_replacement.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_replacement.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_replacement_item.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_replacement_item.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_replacement_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_replacement_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_salesforce.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_salesforce.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_shipping.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_shipping.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_summary.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_summary.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_tag.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_tag.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_taxes.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_taxes.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_token_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_token_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_tracking_number_detail.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_tracking_number_detail.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/order_tracking_number_details.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/order_tracking_number_details.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/orders_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/orders_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/permission.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/permission.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/pricing_tier.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/pricing_tier.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/pricing_tier_notification.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/pricing_tier_notification.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/pricing_tiers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/pricing_tiers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/publish_library_item_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/publish_library_item_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/register_affiliate_click_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/register_affiliate_click_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/register_affiliate_click_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/register_affiliate_click_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/response_metadata.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/response_metadata.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/result_set.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/result_set.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/ruler_validation_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/ruler_validation_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/ruler_validation_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/ruler_validation_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_ad_platform.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_ad_platform.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_geo_distance.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_string_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 
-class ScreenRecordingFilterGeoDistance(ModelNormal):
+class ScreenRecordingFilterStringSearch(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,43 +78,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'distance': (int,),  # noqa: E501
-            'distance_uom': (str,),  # noqa: E501
-            'from_address': (str,),  # noqa: E501
-            'lat': (float,),  # noqa: E501
-            'lon': (float,),  # noqa: E501
+            'does_not_exist': (bool,),  # noqa: E501
+            'exists': (bool,),  # noqa: E501
+            '_is': (str,),  # noqa: E501
+            'is_not': (str,),  # noqa: E501
+            'starts_with': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'distance': 'distance',  # noqa: E501
-        'distance_uom': 'distance_uom',  # noqa: E501
-        'from_address': 'from_address',  # noqa: E501
-        'lat': 'lat',  # noqa: E501
-        'lon': 'lon',  # noqa: E501
+        'does_not_exist': 'does_not_exist',  # noqa: E501
+        'exists': 'exists',  # noqa: E501
+        '_is': 'is',  # noqa: E501
+        'is_not': 'is_not',  # noqa: E501
+        'starts_with': 'starts_with',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ScreenRecordingFilterGeoDistance - a model defined in OpenAPI
+        """ScreenRecordingFilterStringSearch - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,19 +139,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            distance (int): [optional]  # noqa: E501
-            distance_uom (str): [optional]  # noqa: E501
-            from_address (str): [optional]  # noqa: E501
-            lat (float): [optional]  # noqa: E501
-            lon (float): [optional]  # noqa: E501
+            does_not_exist (bool): [optional]  # noqa: E501
+            exists (bool): [optional]  # noqa: E501
+            _is (str): [optional]  # noqa: E501
+            is_not (str): [optional]  # noqa: E501
+            starts_with (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -196,15 +196,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ScreenRecordingFilterGeoDistance - a model defined in OpenAPI
+        """ScreenRecordingFilterStringSearch - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,19 +229,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            distance (int): [optional]  # noqa: E501
-            distance_uom (str): [optional]  # noqa: E501
-            from_address (str): [optional]  # noqa: E501
-            lat (float): [optional]  # noqa: E501
-            lon (float): [optional]  # noqa: E501
+            does_not_exist (bool): [optional]  # noqa: E501
+            exists (bool): [optional]  # noqa: E501
+            _is (str): [optional]  # noqa: E501
+            is_not (str): [optional]  # noqa: E501
+            starts_with (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_ip_search.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_ip_search.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view_event.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view_event.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view_event_param.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view_event_param.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view_param.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view_param.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_page_view_referrer_param.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_page_view_referrer_param.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_range_big_decimal.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_range_big_decimal.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_range_date.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_range_date.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_range_integer.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_range_integer.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_string_search.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_tags_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,24 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from ultracart.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from ultracart.model.error import Error
+    from ultracart.model.response_metadata import ResponseMetadata
+    from ultracart.model.warning import Warning
+    globals()['Error'] = Error
+    globals()['ResponseMetadata'] = ResponseMetadata
+    globals()['Warning'] = Warning
 
-class ScreenRecordingFilterStringSearch(ModelNormal):
+
+class ScreenRecordingTagsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,58 +71,60 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'does_not_exist': (bool,),  # noqa: E501
-            'exists': (bool,),  # noqa: E501
-            '_is': (str,),  # noqa: E501
-            'is_not': (str,),  # noqa: E501
-            'starts_with': (str,),  # noqa: E501
+            'error': (Error,),  # noqa: E501
+            'metadata': (ResponseMetadata,),  # noqa: E501
+            'success': (bool,),  # noqa: E501
+            'tags': ([str],),  # noqa: E501
+            'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'does_not_exist': 'does_not_exist',  # noqa: E501
-        'exists': 'exists',  # noqa: E501
-        '_is': 'is',  # noqa: E501
-        'is_not': 'is_not',  # noqa: E501
-        'starts_with': 'starts_with',  # noqa: E501
+        'error': 'error',  # noqa: E501
+        'metadata': 'metadata',  # noqa: E501
+        'success': 'success',  # noqa: E501
+        'tags': 'tags',  # noqa: E501
+        'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ScreenRecordingFilterStringSearch - a model defined in OpenAPI
+        """ScreenRecordingTagsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,19 +149,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            does_not_exist (bool): [optional]  # noqa: E501
-            exists (bool): [optional]  # noqa: E501
-            _is (str): [optional]  # noqa: E501
-            is_not (str): [optional]  # noqa: E501
-            starts_with (str): [optional]  # noqa: E501
+            error (Error): [optional]  # noqa: E501
+            metadata (ResponseMetadata): [optional]  # noqa: E501
+            success (bool): Indicates if API call was successful. [optional]  # noqa: E501
+            tags ([str]): [optional]  # noqa: E501
+            warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -196,15 +206,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ScreenRecordingFilterStringSearch - a model defined in OpenAPI
+        """ScreenRecordingTagsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,19 +239,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            does_not_exist (bool): [optional]  # noqa: E501
-            exists (bool): [optional]  # noqa: E501
-            _is (str): [optional]  # noqa: E501
-            is_not (str): [optional]  # noqa: E501
-            starts_with (str): [optional]  # noqa: E501
+            error (Error): [optional]  # noqa: E501
+            metadata (ResponseMetadata): [optional]  # noqa: E501
+            success (bool): Indicates if API call was successful. [optional]  # noqa: E501
+            tags ([str]): [optional]  # noqa: E501
+            warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values_event.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values_event.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values_event_params.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values_event_params.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values_page_param.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values_page_param.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_filter_values_page_view.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_filter_values_page_view.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_index_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_index_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_index_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_index_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_reset.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_reset.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_heatmap_url.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_heatmap_url.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_merchant_notes_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_merchant_notes_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_multifield.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_multifield.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view_data_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view_data_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view_event.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view_event.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view_event_parameter.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view_event_parameter.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_page_view_parameter.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_page_view_parameter.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_query_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_query_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_query_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_query_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_segment.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_segment.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_segment_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_segment_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_segments_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_segments_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_settings.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_settings.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_settings_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_settings_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_store_front.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_store_front.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_tags_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_tags_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_tags_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/transaction_email_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     from ultracart.model.response_metadata import ResponseMetadata
     from ultracart.model.warning import Warning
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
     globals()['Warning'] = Warning
 
 
-class ScreenRecordingTagsResponse(ModelNormal):
+class TransactionEmailListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,43 +88,43 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'email_names': ([str],),  # noqa: E501
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
-            'tags': ([str],),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'email_names': 'email_names',  # noqa: E501
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
-        'tags': 'tags',  # noqa: E501
         'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ScreenRecordingTagsResponse - a model defined in OpenAPI
+        """TransactionEmailListResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,18 +149,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            email_names ([str]): [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            tags ([str]): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -206,15 +206,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ScreenRecordingTagsResponse - a model defined in OpenAPI
+        """TransactionEmailListResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,18 +239,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            email_names ([str]): [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            tags ([str]): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_user_agent.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_user_agent.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_user_agent_device.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_user_agent_device.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_user_agent_os.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_user_agent_os.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screen_recording_user_property.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screen_recording_user_property.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/screenshots_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/screenshots_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/self_config.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/self_config.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/simple_value.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/simple_value.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/single_sign_on_authorize_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/single_sign_on_authorize_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/single_sign_on_authorize_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/single_sign_on_authorize_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/single_sign_on_token_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/single_sign_on_token_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/single_sign_on_token_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/single_sign_on_token_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/sovos_config.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/sovos_config.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/state_province.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/state_province.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/step_waiting.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/step_waiting.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/store_front.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/store_front.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/store_fronts_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/store_fronts_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_city.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_city.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_country.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_country.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_country_code.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_country_code.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_county.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_county.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_jar_config.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_jar_config.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_postal_code.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_postal_code.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_activate_result.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_activate_result.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_avalara.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_avalara.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_avalara_companies_result.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_avalara_companies_result.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_avalara_company.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_avalara_company.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_self.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_self.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_self_countries_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_self_countries_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_self_regions_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_self_regions_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_sovos.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_sovos.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_tax_jar.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_tax_jar.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_test_result.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_test_result.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_ultra_cart.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_ultra_cart.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_provider_ultra_cart_state.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_provider_ultra_cart_state.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_providers_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_providers_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_state.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_state.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/tax_state_code.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/tax_state_code.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/temp_multimedia.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/temp_multimedia.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/temp_multimedia_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/temp_multimedia_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/thumbnail_parameters_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/thumbnail_parameters_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/thumbnail_parameters_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/thumbnail_parameters_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/transaction_email.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/transaction_email.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/transaction_email_list_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/transaction_email_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,23 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
+    from ultracart.model.transaction_email import TransactionEmail
     from ultracart.model.warning import Warning
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
+    globals()['TransactionEmail'] = TransactionEmail
     globals()['Warning'] = Warning
 
 
-class TransactionEmailListResponse(ModelNormal):
+class TransactionEmailResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,43 +90,43 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'email_names': ([str],),  # noqa: E501
+            'email': (TransactionEmail,),  # noqa: E501
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email_names': 'email_names',  # noqa: E501
+        'email': 'email',  # noqa: E501
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
         'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TransactionEmailListResponse - a model defined in OpenAPI
+        """TransactionEmailResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,15 +151,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email_names ([str]): [optional]  # noqa: E501
+            email (TransactionEmail): [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
@@ -206,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TransactionEmailListResponse - a model defined in OpenAPI
+        """TransactionEmailResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,15 +241,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email_names ([str]): [optional]  # noqa: E501
+            email (TransactionEmail): [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/transaction_email_option.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/transaction_email_option.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/transaction_email_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/twilios_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
-    from ultracart.model.transaction_email import TransactionEmail
+    from ultracart.model.twilio import Twilio
     from ultracart.model.warning import Warning
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
-    globals()['TransactionEmail'] = TransactionEmail
+    globals()['Twilio'] = Twilio
     globals()['Warning'] = Warning
 
 
-class TransactionEmailResponse(ModelNormal):
+class TwiliosResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -90,43 +90,43 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'email': (TransactionEmail,),  # noqa: E501
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
+            'twilios': ([Twilio],),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
+        'twilios': 'twilios',  # noqa: E501
         'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TransactionEmailResponse - a model defined in OpenAPI
+        """TwiliosResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,18 +151,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (TransactionEmail): [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
+            twilios ([Twilio]): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TransactionEmailResponse - a model defined in OpenAPI
+        """TwiliosResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -241,18 +241,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            email (TransactionEmail): [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
+            twilios ([Twilio]): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/twilio.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/twilio.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/twilio_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/upload_coupon_codes_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,23 +29,21 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
-    from ultracart.model.twilio import Twilio
     from ultracart.model.warning import Warning
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
-    globals()['Twilio'] = Twilio
     globals()['Warning'] = Warning
 
 
-class TwilioResponse(ModelNormal):
+class UploadCouponCodesRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -90,45 +88,43 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'diagnostics': (str,),  # noqa: E501
+            'coupon_codes': ([str],),  # noqa: E501
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
-            'twilio': (Twilio,),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'diagnostics': 'diagnostics',  # noqa: E501
+        'coupon_codes': 'coupon_codes',  # noqa: E501
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
-        'twilio': 'twilio',  # noqa: E501
         'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TwilioResponse - a model defined in OpenAPI
+        """UploadCouponCodesRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,19 +149,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            diagnostics (str): [optional]  # noqa: E501
+            coupon_codes ([str]): Coupon codes. [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            twilio (Twilio): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -211,15 +206,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TwilioResponse - a model defined in OpenAPI
+        """UploadCouponCodesRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,19 +239,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            diagnostics (str): [optional]  # noqa: E501
+            coupon_codes ([str]): Coupon codes. [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            twilio (Twilio): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/twilios_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/users_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
-    from ultracart.model.twilio import Twilio
+    from ultracart.model.user import User
     from ultracart.model.warning import Warning
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
-    globals()['Twilio'] = Twilio
+    globals()['User'] = User
     globals()['Warning'] = Warning
 
 
-class TwiliosResponse(ModelNormal):
+class UsersResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -93,40 +93,40 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
-            'twilios': ([Twilio],),  # noqa: E501
+            'users': ([User],),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
-        'twilios': 'twilios',  # noqa: E501
+        'users': 'users',  # noqa: E501
         'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TwiliosResponse - a model defined in OpenAPI
+        """UsersResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,15 +154,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            twilios ([Twilio]): [optional]  # noqa: E501
+            users ([User]): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TwiliosResponse - a model defined in OpenAPI
+        """UsersResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,15 +244,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            twilios ([Twilio]): [optional]  # noqa: E501
+            users ([User]): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/ultra_cart_config.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/ultra_cart_config.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/upload_coupon_codes_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/user_logins_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,23 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
+    from ultracart.model.user_login import UserLogin
     from ultracart.model.warning import Warning
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
+    globals()['UserLogin'] = UserLogin
     globals()['Warning'] = Warning
 
 
-class UploadCouponCodesRequest(ModelNormal):
+class UserLoginsResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,43 +90,43 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'coupon_codes': ([str],),  # noqa: E501
             'error': (Error,),  # noqa: E501
+            'logins': ([UserLogin],),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'coupon_codes': 'coupon_codes',  # noqa: E501
         'error': 'error',  # noqa: E501
+        'logins': 'logins',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
         'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UploadCouponCodesRequest - a model defined in OpenAPI
+        """UserLoginsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,16 +151,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            coupon_codes ([str]): Coupon codes. [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
+            logins ([UserLogin]): Logins. [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -206,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UploadCouponCodesRequest - a model defined in OpenAPI
+        """UserLoginsResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -239,16 +241,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            coupon_codes ([str]): Coupon codes. [optional]  # noqa: E501
             error (Error): [optional]  # noqa: E501
+            logins ([UserLogin]): Logins. [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/upload_coupon_codes_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/upload_coupon_codes_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/user.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/user.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/user_group_membership.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/user_group_membership.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/user_login.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/user_login.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/user_logins_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/user_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
-    from ultracart.model.user_login import UserLogin
+    from ultracart.model.user import User
     from ultracart.model.warning import Warning
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
-    globals()['UserLogin'] = UserLogin
+    globals()['User'] = User
     globals()['Warning'] = Warning
 
 
-class UserLoginsResponse(ModelNormal):
+class UserResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -91,42 +91,42 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'error': (Error,),  # noqa: E501
-            'logins': ([UserLogin],),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
+            'user': (User,),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'error': 'error',  # noqa: E501
-        'logins': 'logins',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
+        'user': 'user',  # noqa: E501
         'warning': 'warning',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserLoginsResponse - a model defined in OpenAPI
+        """UserResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -152,17 +152,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
-            logins ([UserLogin]): Logins. [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
+            user (User): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserLoginsResponse - a model defined in OpenAPI
+        """UserResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -242,17 +242,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
-            logins ([UserLogin]): Logins. [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
+            user (User): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/user_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_log_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
-    from ultracart.model.user import User
     from ultracart.model.warning import Warning
+    from ultracart.model.webhook_log import WebhookLog
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
-    globals()['User'] = User
     globals()['Warning'] = Warning
+    globals()['WebhookLog'] = WebhookLog
 
 
-class UserResponse(ModelNormal):
+class WebhookLogResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -93,40 +93,40 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
-            'user': (User,),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
+            'webhook_log': (WebhookLog,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
-        'user': 'user',  # noqa: E501
         'warning': 'warning',  # noqa: E501
+        'webhook_log': 'webhook_log',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UserResponse - a model defined in OpenAPI
+        """WebhookLogResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,16 +154,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            user (User): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
+            webhook_log (WebhookLog): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UserResponse - a model defined in OpenAPI
+        """WebhookLogResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,16 +244,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            user (User): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
+            webhook_log (WebhookLog): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/users_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_sample_request_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
-    from ultracart.model.user import User
     from ultracart.model.warning import Warning
+    from ultracart.model.webhook_sample_request import WebhookSampleRequest
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
-    globals()['User'] = User
     globals()['Warning'] = Warning
+    globals()['WebhookSampleRequest'] = WebhookSampleRequest
 
 
-class UsersResponse(ModelNormal):
+class WebhookSampleRequestResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -93,40 +93,40 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
-            'users': ([User],),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
+            'webhook_sample_request': (WebhookSampleRequest,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
-        'users': 'users',  # noqa: E501
         'warning': 'warning',  # noqa: E501
+        'webhook_sample_request': 'webhook_sample_request',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UsersResponse - a model defined in OpenAPI
+        """WebhookSampleRequestResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,16 +154,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            users ([User]): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
+            webhook_sample_request (WebhookSampleRequest): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """UsersResponse - a model defined in OpenAPI
+        """WebhookSampleRequestResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,16 +244,16 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            users ([User]): [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
+            webhook_sample_request (WebhookSampleRequest): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/verification_record.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/verification_record.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/warning.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/warning.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_event_category.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_event_category.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_event_subscription.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_event_subscription.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_log.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_log.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_log_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 from ultracart.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ultracart.model.error import Error
     from ultracart.model.response_metadata import ResponseMetadata
     from ultracart.model.warning import Warning
-    from ultracart.model.webhook_log import WebhookLog
+    from ultracart.model.webhook import Webhook
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
     globals()['Warning'] = Warning
-    globals()['WebhookLog'] = WebhookLog
+    globals()['Webhook'] = Webhook
 
 
-class WebhookLogResponse(ModelNormal):
+class WebhookResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -94,39 +94,39 @@
         """
         lazy_import()
         return {
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
-            'webhook_log': (WebhookLog,),  # noqa: E501
+            'webhook': (Webhook,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
         'warning': 'warning',  # noqa: E501
-        'webhook_log': 'webhook_log',  # noqa: E501
+        'webhook': 'webhook',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WebhookLogResponse - a model defined in OpenAPI
+        """WebhookResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -155,15 +155,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
-            webhook_log (WebhookLog): [optional]  # noqa: E501
+            webhook (Webhook): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WebhookLogResponse - a model defined in OpenAPI
+        """WebhookResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,15 +245,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
-            webhook_log (WebhookLog): [optional]  # noqa: E501
+            webhook (Webhook): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_log_summaries_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_log_summaries_response.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_log_summary.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_log_summary.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhooks_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     from ultracart.model.webhook import Webhook
     globals()['Error'] = Error
     globals()['ResponseMetadata'] = ResponseMetadata
     globals()['Warning'] = Warning
     globals()['Webhook'] = Webhook
 
 
-class WebhookResponse(ModelNormal):
+class WebhooksResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -94,39 +94,39 @@
         """
         lazy_import()
         return {
             'error': (Error,),  # noqa: E501
             'metadata': (ResponseMetadata,),  # noqa: E501
             'success': (bool,),  # noqa: E501
             'warning': (Warning,),  # noqa: E501
-            'webhook': (Webhook,),  # noqa: E501
+            'webhooks': ([Webhook],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'error': 'error',  # noqa: E501
         'metadata': 'metadata',  # noqa: E501
         'success': 'success',  # noqa: E501
         'warning': 'warning',  # noqa: E501
-        'webhook': 'webhook',  # noqa: E501
+        'webhooks': 'webhooks',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WebhookResponse - a model defined in OpenAPI
+        """WebhooksResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -155,15 +155,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
-            webhook (Webhook): [optional]  # noqa: E501
+            webhooks ([Webhook]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +208,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WebhookResponse - a model defined in OpenAPI
+        """WebhooksResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,15 +245,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             error (Error): [optional]  # noqa: E501
             metadata (ResponseMetadata): [optional]  # noqa: E501
             success (bool): Indicates if API call was successful. [optional]  # noqa: E501
             warning (Warning): [optional]  # noqa: E501
-            webhook (Webhook): [optional]  # noqa: E501
+            webhooks ([Webhook]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_sample_request.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/webhook_sample_request.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhook_sample_request_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_search_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,26 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from ultracart.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from ultracart.model.error import Error
-    from ultracart.model.response_metadata import ResponseMetadata
-    from ultracart.model.warning import Warning
-    from ultracart.model.webhook_sample_request import WebhookSampleRequest
-    globals()['Error'] = Error
-    globals()['ResponseMetadata'] = ResponseMetadata
-    globals()['Warning'] = Warning
-    globals()['WebhookSampleRequest'] = WebhookSampleRequest
 
-
-class WebhookSampleRequestResponse(ModelNormal):
+class ConversationSearchRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -73,60 +63,72 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'error': (Error,),  # noqa: E501
-            'metadata': (ResponseMetadata,),  # noqa: E501
-            'success': (bool,),  # noqa: E501
-            'warning': (Warning,),  # noqa: E501
-            'webhook_sample_request': (WebhookSampleRequest,),  # noqa: E501
+            'date_end': (str,),  # noqa: E501
+            'date_start': (str,),  # noqa: E501
+            'email_filter': (str,),  # noqa: E501
+            'language_filter': (str,),  # noqa: E501
+            'medium_filter': (str,),  # noqa: E501
+            'order_by_newest': (bool,),  # noqa: E501
+            'order_by_oldest': (bool,),  # noqa: E501
+            'range_begin': (int,),  # noqa: E501
+            'range_end': (int,),  # noqa: E501
+            'sms_phone_number_filter': (str,),  # noqa: E501
+            'text_search': (str,),  # noqa: E501
+            'visible_filter': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'error': 'error',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
-        'success': 'success',  # noqa: E501
-        'warning': 'warning',  # noqa: E501
-        'webhook_sample_request': 'webhook_sample_request',  # noqa: E501
+        'date_end': 'date_end',  # noqa: E501
+        'date_start': 'date_start',  # noqa: E501
+        'email_filter': 'email_filter',  # noqa: E501
+        'language_filter': 'language_filter',  # noqa: E501
+        'medium_filter': 'medium_filter',  # noqa: E501
+        'order_by_newest': 'order_by_newest',  # noqa: E501
+        'order_by_oldest': 'order_by_oldest',  # noqa: E501
+        'range_begin': 'range_begin',  # noqa: E501
+        'range_end': 'range_end',  # noqa: E501
+        'sms_phone_number_filter': 'sms_phone_number_filter',  # noqa: E501
+        'text_search': 'text_search',  # noqa: E501
+        'visible_filter': 'visible_filter',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WebhookSampleRequestResponse - a model defined in OpenAPI
+        """ConversationSearchRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,19 +153,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            error (Error): [optional]  # noqa: E501
-            metadata (ResponseMetadata): [optional]  # noqa: E501
-            success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            warning (Warning): [optional]  # noqa: E501
-            webhook_sample_request (WebhookSampleRequest): [optional]  # noqa: E501
+            date_end (str): End of the range. [optional]  # noqa: E501
+            date_start (str): Start of the range. [optional]  # noqa: E501
+            email_filter (str): [optional]  # noqa: E501
+            language_filter (str): [optional]  # noqa: E501
+            medium_filter (str): [optional]  # noqa: E501
+            order_by_newest (bool): [optional]  # noqa: E501
+            order_by_oldest (bool): [optional]  # noqa: E501
+            range_begin (int): [optional]  # noqa: E501
+            range_end (int): [optional]  # noqa: E501
+            sms_phone_number_filter (str): [optional]  # noqa: E501
+            text_search (str): [optional]  # noqa: E501
+            visible_filter (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +217,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WebhookSampleRequestResponse - a model defined in OpenAPI
+        """ConversationSearchRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -241,19 +250,26 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            error (Error): [optional]  # noqa: E501
-            metadata (ResponseMetadata): [optional]  # noqa: E501
-            success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            warning (Warning): [optional]  # noqa: E501
-            webhook_sample_request (WebhookSampleRequest): [optional]  # noqa: E501
+            date_end (str): End of the range. [optional]  # noqa: E501
+            date_start (str): Start of the range. [optional]  # noqa: E501
+            email_filter (str): [optional]  # noqa: E501
+            language_filter (str): [optional]  # noqa: E501
+            medium_filter (str): [optional]  # noqa: E501
+            order_by_newest (bool): [optional]  # noqa: E501
+            order_by_oldest (bool): [optional]  # noqa: E501
+            range_begin (int): [optional]  # noqa: E501
+            range_end (int): [optional]  # noqa: E501
+            sms_phone_number_filter (str): [optional]  # noqa: E501
+            text_search (str): [optional]  # noqa: E501
+            visible_filter (bool): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/webhooks_response.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/weight.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,26 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from ultracart.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from ultracart.model.error import Error
-    from ultracart.model.response_metadata import ResponseMetadata
-    from ultracart.model.warning import Warning
-    from ultracart.model.webhook import Webhook
-    globals()['Error'] = Error
-    globals()['ResponseMetadata'] = ResponseMetadata
-    globals()['Warning'] = Warning
-    globals()['Webhook'] = Webhook
 
-
-class WebhooksResponse(ModelNormal):
+class Weight(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,71 +52,69 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('uom',): {
+            'KG': "KG",
+            'G': "G",
+            'LB': "LB",
+            'OZ': "OZ",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'error': (Error,),  # noqa: E501
-            'metadata': (ResponseMetadata,),  # noqa: E501
-            'success': (bool,),  # noqa: E501
-            'warning': (Warning,),  # noqa: E501
-            'webhooks': ([Webhook],),  # noqa: E501
+            'uom': (str,),  # noqa: E501
+            'value': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'error': 'error',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
-        'success': 'success',  # noqa: E501
-        'warning': 'warning',  # noqa: E501
-        'webhooks': 'webhooks',  # noqa: E501
+        'uom': 'uom',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WebhooksResponse - a model defined in OpenAPI
+        """Weight - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,19 +139,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            error (Error): [optional]  # noqa: E501
-            metadata (ResponseMetadata): [optional]  # noqa: E501
-            success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            warning (Warning): [optional]  # noqa: E501
-            webhooks ([Webhook]): [optional]  # noqa: E501
+            uom (str): Unit of measure. [optional]  # noqa: E501
+            value (float): Weight. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,15 +193,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WebhooksResponse - a model defined in OpenAPI
+        """Weight - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -241,19 +226,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            error (Error): [optional]  # noqa: E501
-            metadata (ResponseMetadata): [optional]  # noqa: E501
-            success (bool): Indicates if API call was successful. [optional]  # noqa: E501
-            warning (Warning): [optional]  # noqa: E501
-            webhooks ([Webhook]): [optional]  # noqa: E501
+            uom (str): Unit of measure. [optional]  # noqa: E501
+            value (float): Weight. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model/weight.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model/conversation_autocomplete_value.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ultracart.exceptions import ApiAttributeError
 
 
 
-class Weight(ModelNormal):
+class ConversationAutocompleteValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -52,20 +52,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('uom',): {
-            'KG': "KG",
-            'G': "G",
-            'LB': "LB",
-            'OZ': "OZ",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -84,37 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'uom': (str,),  # noqa: E501
-            'value': (float,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'uom': 'uom',  # noqa: E501
+        'description': 'description',  # noqa: E501
         'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Weight - a model defined in OpenAPI
+        """ConversationAutocompleteValue - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,16 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uom (str): Unit of measure. [optional]  # noqa: E501
-            value (float): Weight. [optional]  # noqa: E501
+            description (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -193,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Weight - a model defined in OpenAPI
+        """ConversationAutocompleteValue - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,16 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            uom (str): Unit of measure. [optional]  # noqa: E501
-            value (float): Weight. [optional]  # noqa: E501
+            description (str): [optional]  # noqa: E501
+            value (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/model_utils.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/model_utils.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/models/__init__.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 from ultracart.model.checkout_state_province_response import CheckoutStateProvinceResponse
 from ultracart.model.city_state_zip import CityStateZip
 from ultracart.model.conversation import Conversation
 from ultracart.model.conversation_agent_auth import ConversationAgentAuth
 from ultracart.model.conversation_agent_auth_response import ConversationAgentAuthResponse
 from ultracart.model.conversation_autocomplete_request import ConversationAutocompleteRequest
 from ultracart.model.conversation_autocomplete_response import ConversationAutocompleteResponse
+from ultracart.model.conversation_autocomplete_value import ConversationAutocompleteValue
 from ultracart.model.conversation_canned_message import ConversationCannedMessage
 from ultracart.model.conversation_canned_message_response import ConversationCannedMessageResponse
 from ultracart.model.conversation_canned_messages_response import ConversationCannedMessagesResponse
 from ultracart.model.conversation_canned_messages_search import ConversationCannedMessagesSearch
 from ultracart.model.conversation_department import ConversationDepartment
 from ultracart.model.conversation_department_response import ConversationDepartmentResponse
 from ultracart.model.conversation_departments_response import ConversationDepartmentsResponse
```

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart/rest.py` & `ultracart_rest_sdk-4.0.99rc0/ultracart/rest.py`

 * *Files identical despite different names*

### Comparing `ultracart_rest_sdk-4.0.98rc0/ultracart_rest_sdk.egg-info/SOURCES.txt` & `ultracart_rest_sdk-4.0.99rc0/ultracart_rest_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 ultracart/model/checkout_state_province_response.py
 ultracart/model/city_state_zip.py
 ultracart/model/conversation.py
 ultracart/model/conversation_agent_auth.py
 ultracart/model/conversation_agent_auth_response.py
 ultracart/model/conversation_autocomplete_request.py
 ultracart/model/conversation_autocomplete_response.py
+ultracart/model/conversation_autocomplete_value.py
 ultracart/model/conversation_canned_message.py
 ultracart/model/conversation_canned_message_response.py
 ultracart/model/conversation_canned_messages_response.py
 ultracart/model/conversation_canned_messages_search.py
 ultracart/model/conversation_department.py
 ultracart/model/conversation_department_response.py
 ultracart/model/conversation_departments_response.py
```

