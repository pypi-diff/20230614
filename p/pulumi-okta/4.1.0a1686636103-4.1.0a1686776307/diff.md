# Comparing `tmp/pulumi_okta-4.1.0a1686636103.tar.gz` & `tmp/pulumi_okta-4.1.0a1686776307.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.1.0a1686636103.tar", last modified: Tue Jun 13 06:13:22 2023, max compression
+gzip compressed data, was "pulumi_okta-4.1.0a1686776307.tar", last modified: Wed Jun 14 21:03:33 2023, max compression
```

## Comparing `pulumi_okta-4.1.0a1686636103.tar` & `pulumi_okta-4.1.0a1686776307.tar`

### file list

```diff
@@ -1,189 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.228051 pulumi_okta-4.1.0a1686636103/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-13 06:13:22.228051 pulumi_okta-4.1.0a1686636103/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.208051 pulumi_okta-4.1.0a1686636103/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.216051 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    31761 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)   137739 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   137444 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.216051 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.220051 pulumi_okta-4.1.0a1686636103/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    37986 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.220051 pulumi_okta-4.1.0a1686636103/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.220051 pulumi_okta-4.1.0a1686636103/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.220051 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.220051 pulumi_okta-4.1.0a1686636103/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/index/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.224051 pulumi_okta-4.1.0a1686636103/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.224051 pulumi_okta-4.1.0a1686636103/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24327 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    32891 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.224051 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.228051 pulumi_okta-4.1.0a1686636103/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.228051 pulumi_okta-4.1.0a1686636103/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.228051 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98382 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:13:22.212051 pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-13 06:13:22.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-13 06:13:22.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:13:22.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:13:22.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:13:22.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 06:13:22.000000 pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:13:22.228051 pulumi_okta-4.1.0a1686636103/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-13 06:13:21.000000 pulumi_okta-4.1.0a1686636103/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.330087 pulumi_okta-4.1.0a1686776307/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-14 21:03:33.330087 pulumi_okta-4.1.0a1686776307/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.322087 pulumi_okta-4.1.0a1686776307/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.322087 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31761 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137739 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137444 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.326087 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.326087 pulumi_okta-4.1.0a1686776307/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37986 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.326087 pulumi_okta-4.1.0a1686776307/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.326087 pulumi_okta-4.1.0a1686776307/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.326087 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.326087 pulumi_okta-4.1.0a1686776307/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/index/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/index/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/index/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/index/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.326087 pulumi_okta-4.1.0a1686776307/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.326087 pulumi_okta-4.1.0a1686776307/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24327 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32891 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.330087 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.330087 pulumi_okta-4.1.0a1686776307/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.330087 pulumi_okta-4.1.0a1686776307/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.330087 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98382 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 21:03:33.322087 pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-14 21:03:33.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-14 21:03:33.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:03:33.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 21:03:33.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 21:03:33.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 21:03:33.000000 pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 21:03:33.330087 pulumi_okta-4.1.0a1686776307/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-14 21:03:32.000000 pulumi_okta-4.1.0a1686776307/setup.py
```

### Comparing `pulumi_okta-4.1.0a1686636103/PKG-INFO` & `pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_okta
-Version: 4.1.0a1686636103
+Name: pulumi-okta
+Version: 4.1.0a1686776307
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.1.0a1686636103/README.md` & `pulumi_okta-4.1.0a1686776307/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/__init__.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,30 @@
     user = _utilities.lazy_import('pulumi_okta.user')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "okta",
+  "mod": "Index/emailDomain",
+  "fqn": "pulumi_okta.index",
+  "classes": {
+   "okta:Index/emailDomain:EmailDomain": "EmailDomain"
+  }
+ },
+ {
+  "pkg": "okta",
+  "mod": "Index/emailDomainVerification",
+  "fqn": "pulumi_okta.index",
+  "classes": {
+   "okta:Index/emailDomainVerification:EmailDomainVerification": "EmailDomainVerification"
+  }
+ },
+ {
+  "pkg": "okta",
   "mod": "app/autoLogin",
   "fqn": "pulumi_okta.app",
   "classes": {
    "okta:app/autoLogin:AutoLogin": "AutoLogin"
   }
  },
  {
```

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/_inputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/_utilities.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/__init__.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/get_app.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/get_oauth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/o_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/outputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/saml.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/swa.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/three_field.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app/user.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/authenticator.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/behaviour.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/brand.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/captcha.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/config/vars.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/domain.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/domain_verification.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/email_customization.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/email_sender.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/email_sender.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/email_sender_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/event_hook.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/factor/factor.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/factor_totp.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_app_group_assignments.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.get_app_group_assignments(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    test = okta.get_app_group_assignments(id=okta_app_oauth["test"]["id"])
     ```
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -91,14 +91,14 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.get_app_group_assignments(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    test = okta.get_app_group_assignments(id=okta_app_oauth["test"]["id"])
     ```
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     ...
```

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_app_user_assignments.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.get_app_user_assignments(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    test = okta.get_app_user_assignments(id=okta_app_oauth["test"]["id"])
     ```
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     __args__ = dict()
     __args__['id'] = id
@@ -91,14 +91,14 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_okta as okta
 
-    test = okta.get_app_user_assignments(id=%!v(PANIC=Format method: runtime error: invalid memory address or nil pointer dereference))
+    test = okta.get_app_user_assignments(id=okta_app_oauth["test"]["id"])
     ```
 
 
     :param str id: The ID of the Okta application you want to retrieve the groups for.
     """
     ...
```

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_brand.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_brands.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_groups.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_template.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_templates.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_theme.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_themes.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/group/get_group.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/group/group.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/group/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/group/role.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/group/rule.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/group_memberships.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/saml.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/idp/social.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/index/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/index/outputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/index/_inputs.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,61 +6,73 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
-    'GetDomainDnsRecordResult',
+    'EmailDomainDnsValidationRecordArgs',
 ]
 
-@pulumi.output_type
-class GetDomainDnsRecordResult(dict):
+@pulumi.input_type
+class EmailDomainDnsValidationRecordArgs:
     def __init__(__self__, *,
-                 expiration: str,
-                 fqdn: str,
-                 record_type: str,
-                 values: Sequence[str]):
-        """
-        :param str expiration: TXT record expiration.
-        :param str fqdn: DNS record name.
-        :param str record_type: Record type can be TXT or CNAME.
-        :param Sequence[str] values: DNS verification value
-        """
-        pulumi.set(__self__, "expiration", expiration)
-        pulumi.set(__self__, "fqdn", fqdn)
-        pulumi.set(__self__, "record_type", record_type)
-        pulumi.set(__self__, "values", values)
+                 expiration: Optional[pulumi.Input[str]] = None,
+                 fqdn: Optional[pulumi.Input[str]] = None,
+                 record_type: Optional[pulumi.Input[str]] = None,
+                 values: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] fqdn: DNS record name.
+        :param pulumi.Input[str] record_type: Record type can be TXT or cname.
+        """
+        if expiration is not None:
+            pulumi.set(__self__, "expiration", expiration)
+        if fqdn is not None:
+            pulumi.set(__self__, "fqdn", fqdn)
+        if record_type is not None:
+            pulumi.set(__self__, "record_type", record_type)
+        if values is not None:
+            pulumi.set(__self__, "values", values)
 
     @property
     @pulumi.getter
-    def expiration(self) -> str:
-        """
-        TXT record expiration.
-        """
+    def expiration(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "expiration")
 
+    @expiration.setter
+    def expiration(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "expiration", value)
+
     @property
     @pulumi.getter
-    def fqdn(self) -> str:
+    def fqdn(self) -> Optional[pulumi.Input[str]]:
         """
         DNS record name.
         """
         return pulumi.get(self, "fqdn")
 
+    @fqdn.setter
+    def fqdn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "fqdn", value)
+
     @property
     @pulumi.getter(name="recordType")
-    def record_type(self) -> str:
+    def record_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Record type can be TXT or CNAME.
+        Record type can be TXT or cname.
         """
         return pulumi.get(self, "record_type")
 
+    @record_type.setter
+    def record_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "record_type", value)
+
     @property
     @pulumi.getter
-    def values(self) -> Sequence[str]:
-        """
-        DNS verification value
-        """
+    def values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         return pulumi.get(self, "values")
 
+    @values.setter
+    def values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "values", value)
+
```

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/inline/hook.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/link_definition.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/link_value.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/network/zone.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/org_configuration.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/org_support.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/outputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/password.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/rule_mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy/signon.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy/signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/provider.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/resource_set.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/role_subscription.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/template_sms.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/theme.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user/get_user.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user/get_users.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user/outputs.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user/user.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user/user_type.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user_admin_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.1.0a1686776307/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.1.0a1686776307/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-okta
-Version: 4.1.0a1686636103
+Name: pulumi_okta
+Version: 4.1.0a1686776307
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.1.0a1686636103/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.1.0a1686776307/pulumi_okta.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -130,14 +130,17 @@
 pulumi_okta/idp/get_saml.py
 pulumi_okta/idp/get_social.py
 pulumi_okta/idp/oidc.py
 pulumi_okta/idp/saml.py
 pulumi_okta/idp/saml_key.py
 pulumi_okta/idp/social.py
 pulumi_okta/index/__init__.py
+pulumi_okta/index/_inputs.py
+pulumi_okta/index/email_domain.py
+pulumi_okta/index/email_domain_verification.py
 pulumi_okta/index/get_domain.py
 pulumi_okta/index/outputs.py
 pulumi_okta/inline/__init__.py
 pulumi_okta/inline/_inputs.py
 pulumi_okta/inline/hook.py
 pulumi_okta/inline/outputs.py
 pulumi_okta/network/__init__.py
```

### Comparing `pulumi_okta-4.1.0a1686636103/setup.py` & `pulumi_okta-4.1.0a1686776307/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.1.0a1686636103"
-PLUGIN_VERSION = "4.1.0-alpha.1686636103+b807a934"
+VERSION = "4.1.0a1686776307"
+PLUGIN_VERSION = "4.1.0-alpha.1686776307+fbaafdf3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'okta', PLUGIN_VERSION])
         except OSError as error:
```

