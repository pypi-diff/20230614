# Comparing `tmp/pulumi_vault-5.9.0a1678129627.tar.gz` & `tmp/pulumi_vault-5.9.0a1678382334.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_vault-5.9.0a1678129627.tar", last modified: Mon Mar  6 19:22:18 2023, max compression
+gzip compressed data, was "pulumi_vault-5.9.0a1678382334.tar", last modified: Thu Mar  9 17:24:16 2023, max compression
```

## Comparing `pulumi_vault-5.9.0a1678129627.tar` & `pulumi_vault-5.9.0a1678382334.tar`

### file list

```diff
@@ -1,242 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.838823 pulumi_vault-5.9.0a1678129627/pulumi_vault/
--rw-r--r--   0 runner    (1001) docker     (123)    25631 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49451 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.838823 pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    98828 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/secret_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/secret_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.838823 pulumi_vault-5.9.0a1678129627/pulumi_vault/alicloud/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/alicloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44594 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/alicloud/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.842823 pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23056 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/auth_backend_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    56415 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    31707 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/auth_backend_role_secret_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/get_auth_backend_role_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/auth_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.842823 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    27972 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_identity_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (123)    42966 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_login.py
--rw-r--r--   0 runner    (1001) docker     (123)   110492 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    26515 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_roletag_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_sts_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    36592 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48029 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.842823 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23531 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    64647 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    30826 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/get_access_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68873 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/cert_auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.842823 pulumi_vault-5.9.0a1678129627/pulumi_vault/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.842823 pulumi_vault-5.9.0a1678129627/pulumi_vault/consul/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/consul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39535 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/consul/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    45427 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/consul/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.846823 pulumi_vault-5.9.0a1678129627/pulumi_vault/database/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   269717 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/database/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   236712 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/database/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72442 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/database/secret_backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30038 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/database/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/database/secret_backend_static_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    97405 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/database/secrets_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/egp_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.846823 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33633 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    72012 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/get_auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24689 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    25844 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/secret_roleset.py
--rw-r--r--   0 runner    (1001) docker     (123)    27192 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/secret_static_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.846823 pulumi_vault-5.9.0a1678129627/pulumi_vault/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/generic/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/generic/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    22772 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/generic/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/get_auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/get_nomad_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/get_policy_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.846823 pulumi_vault-5.9.0a1678129627/pulumi_vault/github/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/github/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55832 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/github/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/github/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/github/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/github/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.850823 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    18410 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/entity_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/entity_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_oidc_client_creds.py
--rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_oidc_openid_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_oidc_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    37231 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    19361 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group_member_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group_member_group_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_duo.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_login_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_okta.py
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_pingid.py
--rw-r--r--   0 runner    (1001) docker     (123)    28626 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    29238 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_key_allowed_client_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.850823 pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64778 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    97264 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.850823 pulumi_vault-5.9.0a1678129627/pulumi_vault/kmip/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kmip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37700 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kmip/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    54330 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kmip/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kmip/secret_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.850823 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30931 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    54921 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/get_auth_backend_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/get_auth_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/get_service_account_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.854823 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secret_subkeys_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secrets_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secrets_list_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18886 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/secret_backend_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    35700 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/secret_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.854823 pulumi_vault-5.9.0a1678129627/pulumi_vault/ldap/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ldap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    90164 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ldap/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ldap/auth_backend_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ldap/auth_backend_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.854823 pulumi_vault-5.9.0a1678129627/pulumi_vault/managed/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/managed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29907 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/managed/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/managed/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    25837 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/managed/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28106 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/mfa_duo.py
--rw-r--r--   0 runner    (1001) docker     (123)    29370 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/mfa_okta.py
--rw-r--r--   0 runner    (1001) docker     (123)    30407 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/mfa_pingid.py
--rw-r--r--   0 runner    (1001) docker     (123)    25211 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/mfa_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    41943 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/nomad_secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/nomad_secret_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.854823 pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/auth_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/auth_backend_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16862 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/auth_backend_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/password_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.854823 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45649 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    18889 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_config_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_config_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    29039 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_crl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    55637 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py
--rw-r--r--   0 runner    (1001) docker     (123)    96745 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    60223 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_root_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    56213 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)    46179 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    38964 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/quota_lease_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    22738 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/quota_rate_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34547 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    21729 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/secret_backend_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    29528 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/raft_autopilot.py
--rw-r--r--   0 runner    (1001) docker     (123)    78444 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/raft_snapshot_agent_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/rgp_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/secret_backend_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)    68242 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/secret_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/pulumi_vault/terraformcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/terraformcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26295 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/terraformcloud/secret_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/terraformcloud/secret_creds.py
--rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/terraformcloud/secret_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    41608 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/pulumi_vault/tokenauth/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/tokenauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60284 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/tokenauth/auth_backend_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/alphabet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/get_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/get_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    22773 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/get_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/get_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    54305 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/secret_backend_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/secret_cache_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:22:18.838823 pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 19:22:18.858823 pulumi_vault-5.9.0a1678129627/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-06 19:22:18.000000 pulumi_vault-5.9.0a1678129627/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.457305 pulumi_vault-5.9.0a1678382334/
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-03-09 17:24:16.457305 pulumi_vault-5.9.0a1678382334/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.429305 pulumi_vault-5.9.0a1678382334/pulumi_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)    25842 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49451 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.429305 pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98828 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/secret_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/secret_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.429305 pulumi_vault-5.9.0a1678382334/pulumi_vault/alicloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/alicloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44594 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/alicloud/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.433305 pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23056 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/auth_backend_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56415 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31707 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/auth_backend_role_secret_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/get_auth_backend_role_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/auth_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.433305 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18242 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27972 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_config_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_identity_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42966 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110492 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26515 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_roletag_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_sts_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36592 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48029 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.433305 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23531 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64647 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30826 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29575 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/get_access_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68873 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/cert_auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.437305 pulumi_vault-5.9.0a1678382334/pulumi_vault/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.437305 pulumi_vault-5.9.0a1678382334/pulumi_vault/consul/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/consul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39535 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/consul/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45427 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/consul/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.437305 pulumi_vault-5.9.0a1678382334/pulumi_vault/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   269717 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/database/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   236712 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/database/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72442 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/database/secret_backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30038 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/database/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22627 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/database/secret_backend_static_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97405 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/database/secrets_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/egp_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.437305 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33633 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72012 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/get_auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24689 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25844 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/secret_roleset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27192 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/secret_static_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.441305 pulumi_vault-5.9.0a1678382334/pulumi_vault/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/generic/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/generic/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22772 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/generic/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/get_auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/get_nomad_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/get_policy_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.441305 pulumi_vault-5.9.0a1678382334/pulumi_vault/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/github/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55832 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/github/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/github/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/github/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/github/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.445305 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19701 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18410 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/entity_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/entity_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_oidc_client_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_oidc_openid_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_oidc_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37231 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19361 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group_member_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group_member_group_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_duo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_login_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_pingid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28626 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29238 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_key_allowed_client_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.445305 pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64778 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97264 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.445305 pulumi_vault-5.9.0a1678382334/pulumi_vault/kmip/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kmip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37700 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kmip/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54330 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kmip/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kmip/secret_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.449305 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30931 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54921 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/get_auth_backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/get_auth_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/get_service_account_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49063 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.449305 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secret_subkeys_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secrets_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secrets_list_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18886 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/secret_backend_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35700 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/secret_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.449305 pulumi_vault-5.9.0a1678382334/pulumi_vault/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ldap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90164 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ldap/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ldap/auth_backend_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ldap/auth_backend_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.449305 pulumi_vault-5.9.0a1678382334/pulumi_vault/managed/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/managed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29907 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/managed/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/managed/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25837 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/managed/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28106 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/mfa_duo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29370 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/mfa_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30407 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/mfa_pingid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25211 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/mfa_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14162 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41943 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/nomad_secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/nomad_secret_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.449305 pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38263 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/auth_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/auth_backend_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16862 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/auth_backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/password_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.453305 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45649 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18889 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_config_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_config_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29039 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_crl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55637 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96745 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60223 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_root_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56213 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46179 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38964 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/quota_lease_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22738 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/quota_rate_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.453305 pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34547 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21729 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/secret_backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29984 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/raft_autopilot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78444 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/raft_snapshot_agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/rgp_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.453305 pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/secret_backend_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71044 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/secret_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.453305 pulumi_vault-5.9.0a1678382334/pulumi_vault/terraformcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/terraformcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26295 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/terraformcloud/secret_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/terraformcloud/secret_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22721 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/terraformcloud/secret_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41608 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.453305 pulumi_vault-5.9.0a1678382334/pulumi_vault/tokenauth/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/tokenauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60284 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/tokenauth/auth_backend_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.457305 pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/alphabet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/get_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/get_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18648 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22773 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.457305 pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/get_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/get_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54305 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/secret_backend_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/secret_cache_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 17:24:16.429305 pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 17:24:16.457305 pulumi_vault-5.9.0a1678382334/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-09 17:24:16.000000 pulumi_vault-5.9.0a1678382334/setup.py
```

### Comparing `pulumi_vault-5.9.0a1678129627/PKG-INFO` & `pulumi_vault-5.9.0a1678382334/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_vault
-Version: 5.9.0a1678129627
+Version: 5.9.0a1678382334
 Summary: A Pulumi package for creating and managing HashiCorp Vault cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-vault
 Keywords: pulumi vault
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_vault-5.9.0a1678129627/README.md` & `pulumi_vault-5.9.0a1678382334/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/__init__.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,22 @@
   "fqn": "pulumi_vault.aws",
   "classes": {
    "vault:aws/authBackendClient:AuthBackendClient": "AuthBackendClient"
   }
  },
  {
   "pkg": "vault",
+  "mod": "aws/authBackendConfigIdentity",
+  "fqn": "pulumi_vault.aws",
+  "classes": {
+   "vault:aws/authBackendConfigIdentity:AuthBackendConfigIdentity": "AuthBackendConfigIdentity"
+  }
+ },
+ {
+  "pkg": "vault",
   "mod": "aws/authBackendIdentityWhitelist",
   "fqn": "pulumi_vault.aws",
   "classes": {
    "vault:aws/authBackendIdentityWhitelist:AuthBackendIdentityWhitelist": "AuthBackendIdentityWhitelist"
   }
  },
  {
```

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/_utilities.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/get_access_credentials.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/secret_library.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/secret_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ad/secret_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ad/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/alicloud/auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/alicloud/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/auth_backend_login.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/auth_backend_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/auth_backend_role_secret_id.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/auth_backend_role_secret_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/approle/get_auth_backend_role_id.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/approle/get_auth_backend_role_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/audit.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/audit.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/auth_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/__init__.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from .. import _utilities
 import typing
 # Export this package's modules as members:
 from .auth_backend_cert import *
 from .auth_backend_client import *
+from .auth_backend_config_identity import *
 from .auth_backend_identity_whitelist import *
 from .auth_backend_login import *
 from .auth_backend_role import *
 from .auth_backend_role_tag import *
 from .auth_backend_roletag_blacklist import *
 from .auth_backend_sts_role import *
 from .get_access_credentials import *
```

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_cert.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_client.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_identity_whitelist.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_identity_whitelist.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_login.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_role_tag.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_role_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_roletag_blacklist.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_roletag_blacklist.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/auth_backend_sts_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/auth_backend_sts_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/get_access_credentials.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/aws/secret_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/aws/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/auth_backend_config.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/get_access_credentials.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/get_access_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/azure/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/cert_auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/cert_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/config/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/config/vars.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/consul/secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/consul/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/consul/secret_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/consul/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/database/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/database/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/database/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/database/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/database/secret_backend_connection.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/database/secret_backend_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/database/secret_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/database/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/database/secret_backend_static_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/database/secret_backend_static_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/database/secrets_mount.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/database/secrets_mount.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/egp_policy.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/egp_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/auth_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/get_auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/get_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/secret_roleset.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/secret_roleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/gcp/secret_static_account.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/gcp/secret_static_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/generic/endpoint.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/generic/endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/generic/get_secret.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/generic/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/generic/secret.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/generic/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/get_auth_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/get_auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/get_nomad_access_token.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/get_nomad_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/get_policy_document.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/get_policy_document.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/github/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/github/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/github/auth_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/github/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/github/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/github/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/github/team.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/github/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/github/user.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/github/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/__init__.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/entity.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/entity_alias.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/entity_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/entity_policies.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/entity_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_entity.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_group.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_oidc_client_creds.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_oidc_client_creds.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_oidc_openid_config.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_oidc_openid_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/get_oidc_public_keys.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/get_oidc_public_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group_alias.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group_member_entity_ids.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group_member_entity_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group_member_group_ids.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group_member_group_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/group_policies.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/group_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_duo.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_duo.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_login_enforcement.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_login_enforcement.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_okta.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_pingid.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_pingid.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/mfa_totp.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/mfa_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_assignment.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_client.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_key.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_key_allowed_client_id.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_key_allowed_client_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_provider.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/oidc_scope.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/oidc_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/identity/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/identity/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/auth_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/jwt/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/jwt/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kmip/secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kmip/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kmip/secret_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kmip/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kmip/secret_scope.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kmip/secret_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/__init__.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/auth_backend_config.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/get_auth_backend_config.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/get_auth_backend_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/get_auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/get_auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/get_service_account_token.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/get_service_account_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kubernetes/secret_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kubernetes/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/__init__.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secret.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secret_subkeys_v2.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secret_subkeys_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secret_v2.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secrets_list.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secrets_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/get_secrets_list_v2.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/get_secrets_list_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/secret.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/secret_backend_v2.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/secret_backend_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/kv/secret_v2.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/kv/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ldap/auth_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ldap/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ldap/auth_backend_group.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ldap/auth_backend_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ldap/auth_backend_user.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ldap/auth_backend_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/managed/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/managed/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/managed/keys.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/managed/keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/managed/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/managed/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/mfa_duo.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/mfa_duo.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/mfa_okta.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/mfa_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/mfa_pingid.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/mfa_pingid.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/mfa_totp.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/mfa_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/mount.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/mount.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/namespace.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/nomad_secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/nomad_secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/nomad_secret_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/nomad_secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/auth_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/auth_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/auth_backend_group.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/auth_backend_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/auth_backend_user.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/auth_backend_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/okta/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/password_policy.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/password_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/__init__.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_cert.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_config_ca.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_config_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_config_urls.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_config_urls.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_crl_config.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_crl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_intermediate_cert_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_intermediate_set_signed.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_root_cert.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_root_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_root_sign_intermediate.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/pkisecret/secret_backend_sign.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/pkisecret/secret_backend_sign.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/policy.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/provider.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/quota_lease_count.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/quota_lease_count.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/quota_rate_limit.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/quota_rate_limit.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/rabbitmq/secret_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/rabbitmq/secret_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/raft_autopilot.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/raft_autopilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,14 +358,22 @@
             dead_server_last_contact_threshold="24h0m0s",
             last_contact_threshold="10s",
             max_trailing_logs=1000,
             min_quorum=3,
             server_stabilization_time="10s")
         ```
 
+        ## Import
+
+        Raft Autopilot config can be imported using the ID, e.g.
+
+        ```sh
+         $ pulumi import vault:index/raftAutopilot:RaftAutopilot autopilot sys/storage/raft/autopilot/configuration
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] cleanup_dead_servers: Specifies whether to remove dead server nodes
                periodically or when a new server joins. This requires that `min-quorum` is also set.
         :param pulumi.Input[str] dead_server_last_contact_threshold: Limit the amount of time a 
                server can go without leader contact before being considered failed. This only takes
                effect when `cleanup_dead_servers` is set.
@@ -407,14 +415,22 @@
             dead_server_last_contact_threshold="24h0m0s",
             last_contact_threshold="10s",
             max_trailing_logs=1000,
             min_quorum=3,
             server_stabilization_time="10s")
         ```
 
+        ## Import
+
+        Raft Autopilot config can be imported using the ID, e.g.
+
+        ```sh
+         $ pulumi import vault:index/raftAutopilot:RaftAutopilot autopilot sys/storage/raft/autopilot/configuration
+        ```
+
         :param str resource_name: The name of the resource.
         :param RaftAutopilotArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(RaftAutopilotArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/raft_snapshot_agent_config.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/raft_snapshot_agent_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/rgp_policy.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/rgp_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/_inputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/outputs.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/secret_backend_ca.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/secret_backend_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/ssh/secret_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/ssh/secret_backend_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                  allowed_user_key_lengths: Optional[pulumi.Input[Mapping[str, pulumi.Input[int]]]] = None,
                  allowed_users: Optional[pulumi.Input[str]] = None,
                  allowed_users_template: Optional[pulumi.Input[bool]] = None,
                  cidr_list: Optional[pulumi.Input[str]] = None,
                  default_critical_options: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  default_extensions: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  default_user: Optional[pulumi.Input[str]] = None,
+                 default_user_template: Optional[pulumi.Input[bool]] = None,
                  key_id_format: Optional[pulumi.Input[str]] = None,
                  max_ttl: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a SecretBackendRole resource.
@@ -61,14 +62,15 @@
                *Deprecated: use* allowed_user_key_config *instead*
         :param pulumi.Input[str] allowed_users: Specifies a comma-separated list of usernames that are to be allowed, only if certain usernames are to be allowed.
         :param pulumi.Input[bool] allowed_users_template: Specifies if `allowed_users` can be declared using identity template policies. Non-templated users are also permitted.
         :param pulumi.Input[str] cidr_list: The comma-separated string of CIDR blocks for which this role is applicable.
         :param pulumi.Input[Mapping[str, Any]] default_critical_options: Specifies a map of critical options that certificates have when signed.
         :param pulumi.Input[Mapping[str, Any]] default_extensions: Specifies a map of extensions that certificates have when signed.
         :param pulumi.Input[str] default_user: Specifies the default username for which a credential will be generated.
+        :param pulumi.Input[bool] default_user_template: If set, `default_users` can be specified using identity template values. A non-templated user is also permitted.
         :param pulumi.Input[str] key_id_format: Specifies a custom format for the key id of a signed certificate.
         :param pulumi.Input[str] max_ttl: Specifies the maximum Time To Live value.
         :param pulumi.Input[str] name: Specifies the name of the role to create.
         :param pulumi.Input[str] namespace: The namespace to provision the resource in.
                The value should not contain leading or trailing forward slashes.
                The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault#namespace).
                *Available only for Vault Enterprise*.
@@ -109,14 +111,16 @@
             pulumi.set(__self__, "cidr_list", cidr_list)
         if default_critical_options is not None:
             pulumi.set(__self__, "default_critical_options", default_critical_options)
         if default_extensions is not None:
             pulumi.set(__self__, "default_extensions", default_extensions)
         if default_user is not None:
             pulumi.set(__self__, "default_user", default_user)
+        if default_user_template is not None:
+            pulumi.set(__self__, "default_user_template", default_user_template)
         if key_id_format is not None:
             pulumi.set(__self__, "key_id_format", key_id_format)
         if max_ttl is not None:
             pulumi.set(__self__, "max_ttl", max_ttl)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace is not None:
@@ -353,14 +357,26 @@
         return pulumi.get(self, "default_user")
 
     @default_user.setter
     def default_user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_user", value)
 
     @property
+    @pulumi.getter(name="defaultUserTemplate")
+    def default_user_template(self) -> Optional[pulumi.Input[bool]]:
+        """
+        If set, `default_users` can be specified using identity template values. A non-templated user is also permitted.
+        """
+        return pulumi.get(self, "default_user_template")
+
+    @default_user_template.setter
+    def default_user_template(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "default_user_template", value)
+
+    @property
     @pulumi.getter(name="keyIdFormat")
     def key_id_format(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies a custom format for the key id of a signed certificate.
         """
         return pulumi.get(self, "key_id_format")
 
@@ -437,14 +453,15 @@
                  allowed_users: Optional[pulumi.Input[str]] = None,
                  allowed_users_template: Optional[pulumi.Input[bool]] = None,
                  backend: Optional[pulumi.Input[str]] = None,
                  cidr_list: Optional[pulumi.Input[str]] = None,
                  default_critical_options: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  default_extensions: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  default_user: Optional[pulumi.Input[str]] = None,
+                 default_user_template: Optional[pulumi.Input[bool]] = None,
                  key_id_format: Optional[pulumi.Input[str]] = None,
                  key_type: Optional[pulumi.Input[str]] = None,
                  max_ttl: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[str]] = None):
         """
@@ -467,14 +484,15 @@
         :param pulumi.Input[str] allowed_users: Specifies a comma-separated list of usernames that are to be allowed, only if certain usernames are to be allowed.
         :param pulumi.Input[bool] allowed_users_template: Specifies if `allowed_users` can be declared using identity template policies. Non-templated users are also permitted.
         :param pulumi.Input[str] backend: The path where the SSH secret backend is mounted.
         :param pulumi.Input[str] cidr_list: The comma-separated string of CIDR blocks for which this role is applicable.
         :param pulumi.Input[Mapping[str, Any]] default_critical_options: Specifies a map of critical options that certificates have when signed.
         :param pulumi.Input[Mapping[str, Any]] default_extensions: Specifies a map of extensions that certificates have when signed.
         :param pulumi.Input[str] default_user: Specifies the default username for which a credential will be generated.
+        :param pulumi.Input[bool] default_user_template: If set, `default_users` can be specified using identity template values. A non-templated user is also permitted.
         :param pulumi.Input[str] key_id_format: Specifies a custom format for the key id of a signed certificate.
         :param pulumi.Input[str] key_type: Specifies the type of credentials generated by this role. This can be either `otp`, `dynamic` or `ca`.
         :param pulumi.Input[str] max_ttl: Specifies the maximum Time To Live value.
         :param pulumi.Input[str] name: Specifies the name of the role to create.
         :param pulumi.Input[str] namespace: The namespace to provision the resource in.
                The value should not contain leading or trailing forward slashes.
                The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault#namespace).
@@ -516,14 +534,16 @@
             pulumi.set(__self__, "cidr_list", cidr_list)
         if default_critical_options is not None:
             pulumi.set(__self__, "default_critical_options", default_critical_options)
         if default_extensions is not None:
             pulumi.set(__self__, "default_extensions", default_extensions)
         if default_user is not None:
             pulumi.set(__self__, "default_user", default_user)
+        if default_user_template is not None:
+            pulumi.set(__self__, "default_user_template", default_user_template)
         if key_id_format is not None:
             pulumi.set(__self__, "key_id_format", key_id_format)
         if key_type is not None:
             pulumi.set(__self__, "key_type", key_type)
         if max_ttl is not None:
             pulumi.set(__self__, "max_ttl", max_ttl)
         if name is not None:
@@ -750,14 +770,26 @@
         return pulumi.get(self, "default_user")
 
     @default_user.setter
     def default_user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_user", value)
 
     @property
+    @pulumi.getter(name="defaultUserTemplate")
+    def default_user_template(self) -> Optional[pulumi.Input[bool]]:
+        """
+        If set, `default_users` can be specified using identity template values. A non-templated user is also permitted.
+        """
+        return pulumi.get(self, "default_user_template")
+
+    @default_user_template.setter
+    def default_user_template(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "default_user_template", value)
+
+    @property
     @pulumi.getter(name="keyIdFormat")
     def key_id_format(self) -> Optional[pulumi.Input[str]]:
         """
         Specifies a custom format for the key id of a signed certificate.
         """
         return pulumi.get(self, "key_id_format")
 
@@ -848,14 +880,15 @@
                  allowed_users: Optional[pulumi.Input[str]] = None,
                  allowed_users_template: Optional[pulumi.Input[bool]] = None,
                  backend: Optional[pulumi.Input[str]] = None,
                  cidr_list: Optional[pulumi.Input[str]] = None,
                  default_critical_options: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  default_extensions: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  default_user: Optional[pulumi.Input[str]] = None,
+                 default_user_template: Optional[pulumi.Input[bool]] = None,
                  key_id_format: Optional[pulumi.Input[str]] = None,
                  key_type: Optional[pulumi.Input[str]] = None,
                  max_ttl: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -910,14 +943,15 @@
         :param pulumi.Input[str] allowed_users: Specifies a comma-separated list of usernames that are to be allowed, only if certain usernames are to be allowed.
         :param pulumi.Input[bool] allowed_users_template: Specifies if `allowed_users` can be declared using identity template policies. Non-templated users are also permitted.
         :param pulumi.Input[str] backend: The path where the SSH secret backend is mounted.
         :param pulumi.Input[str] cidr_list: The comma-separated string of CIDR blocks for which this role is applicable.
         :param pulumi.Input[Mapping[str, Any]] default_critical_options: Specifies a map of critical options that certificates have when signed.
         :param pulumi.Input[Mapping[str, Any]] default_extensions: Specifies a map of extensions that certificates have when signed.
         :param pulumi.Input[str] default_user: Specifies the default username for which a credential will be generated.
+        :param pulumi.Input[bool] default_user_template: If set, `default_users` can be specified using identity template values. A non-templated user is also permitted.
         :param pulumi.Input[str] key_id_format: Specifies a custom format for the key id of a signed certificate.
         :param pulumi.Input[str] key_type: Specifies the type of credentials generated by this role. This can be either `otp`, `dynamic` or `ca`.
         :param pulumi.Input[str] max_ttl: Specifies the maximum Time To Live value.
         :param pulumi.Input[str] name: Specifies the name of the role to create.
         :param pulumi.Input[str] namespace: The namespace to provision the resource in.
                The value should not contain leading or trailing forward slashes.
                The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault#namespace).
@@ -990,14 +1024,15 @@
                  allowed_users: Optional[pulumi.Input[str]] = None,
                  allowed_users_template: Optional[pulumi.Input[bool]] = None,
                  backend: Optional[pulumi.Input[str]] = None,
                  cidr_list: Optional[pulumi.Input[str]] = None,
                  default_critical_options: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  default_extensions: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  default_user: Optional[pulumi.Input[str]] = None,
+                 default_user_template: Optional[pulumi.Input[bool]] = None,
                  key_id_format: Optional[pulumi.Input[str]] = None,
                  key_type: Optional[pulumi.Input[str]] = None,
                  max_ttl: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  ttl: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -1028,14 +1063,15 @@
             if backend is None and not opts.urn:
                 raise TypeError("Missing required property 'backend'")
             __props__.__dict__["backend"] = backend
             __props__.__dict__["cidr_list"] = cidr_list
             __props__.__dict__["default_critical_options"] = default_critical_options
             __props__.__dict__["default_extensions"] = default_extensions
             __props__.__dict__["default_user"] = default_user
+            __props__.__dict__["default_user_template"] = default_user_template
             __props__.__dict__["key_id_format"] = key_id_format
             if key_type is None and not opts.urn:
                 raise TypeError("Missing required property 'key_type'")
             __props__.__dict__["key_type"] = key_type
             __props__.__dict__["max_ttl"] = max_ttl
             __props__.__dict__["name"] = name
             __props__.__dict__["namespace"] = namespace
@@ -1064,14 +1100,15 @@
             allowed_users: Optional[pulumi.Input[str]] = None,
             allowed_users_template: Optional[pulumi.Input[bool]] = None,
             backend: Optional[pulumi.Input[str]] = None,
             cidr_list: Optional[pulumi.Input[str]] = None,
             default_critical_options: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             default_extensions: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             default_user: Optional[pulumi.Input[str]] = None,
+            default_user_template: Optional[pulumi.Input[bool]] = None,
             key_id_format: Optional[pulumi.Input[str]] = None,
             key_type: Optional[pulumi.Input[str]] = None,
             max_ttl: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             namespace: Optional[pulumi.Input[str]] = None,
             ttl: Optional[pulumi.Input[str]] = None) -> 'SecretBackendRole':
         """
@@ -1099,14 +1136,15 @@
         :param pulumi.Input[str] allowed_users: Specifies a comma-separated list of usernames that are to be allowed, only if certain usernames are to be allowed.
         :param pulumi.Input[bool] allowed_users_template: Specifies if `allowed_users` can be declared using identity template policies. Non-templated users are also permitted.
         :param pulumi.Input[str] backend: The path where the SSH secret backend is mounted.
         :param pulumi.Input[str] cidr_list: The comma-separated string of CIDR blocks for which this role is applicable.
         :param pulumi.Input[Mapping[str, Any]] default_critical_options: Specifies a map of critical options that certificates have when signed.
         :param pulumi.Input[Mapping[str, Any]] default_extensions: Specifies a map of extensions that certificates have when signed.
         :param pulumi.Input[str] default_user: Specifies the default username for which a credential will be generated.
+        :param pulumi.Input[bool] default_user_template: If set, `default_users` can be specified using identity template values. A non-templated user is also permitted.
         :param pulumi.Input[str] key_id_format: Specifies a custom format for the key id of a signed certificate.
         :param pulumi.Input[str] key_type: Specifies the type of credentials generated by this role. This can be either `otp`, `dynamic` or `ca`.
         :param pulumi.Input[str] max_ttl: Specifies the maximum Time To Live value.
         :param pulumi.Input[str] name: Specifies the name of the role to create.
         :param pulumi.Input[str] namespace: The namespace to provision the resource in.
                The value should not contain leading or trailing forward slashes.
                The `namespace` is always relative to the provider's configured [namespace](https://www.terraform.io/docs/providers/vault#namespace).
@@ -1131,14 +1169,15 @@
         __props__.__dict__["allowed_users"] = allowed_users
         __props__.__dict__["allowed_users_template"] = allowed_users_template
         __props__.__dict__["backend"] = backend
         __props__.__dict__["cidr_list"] = cidr_list
         __props__.__dict__["default_critical_options"] = default_critical_options
         __props__.__dict__["default_extensions"] = default_extensions
         __props__.__dict__["default_user"] = default_user
+        __props__.__dict__["default_user_template"] = default_user_template
         __props__.__dict__["key_id_format"] = key_id_format
         __props__.__dict__["key_type"] = key_type
         __props__.__dict__["max_ttl"] = max_ttl
         __props__.__dict__["name"] = name
         __props__.__dict__["namespace"] = namespace
         __props__.__dict__["ttl"] = ttl
         return SecretBackendRole(resource_name, opts=opts, __props__=__props__)
@@ -1288,14 +1327,22 @@
     def default_user(self) -> pulumi.Output[Optional[str]]:
         """
         Specifies the default username for which a credential will be generated.
         """
         return pulumi.get(self, "default_user")
 
     @property
+    @pulumi.getter(name="defaultUserTemplate")
+    def default_user_template(self) -> pulumi.Output[Optional[bool]]:
+        """
+        If set, `default_users` can be specified using identity template values. A non-templated user is also permitted.
+        """
+        return pulumi.get(self, "default_user_template")
+
+    @property
     @pulumi.getter(name="keyIdFormat")
     def key_id_format(self) -> pulumi.Output[Optional[str]]:
         """
         Specifies a custom format for the key id of a signed certificate.
         """
         return pulumi.get(self, "key_id_format")
```

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/terraformcloud/secret_backend.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/terraformcloud/secret_backend.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/terraformcloud/secret_creds.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/terraformcloud/secret_creds.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/terraformcloud/secret_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/terraformcloud/secret_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/token.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/tokenauth/auth_backend_role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/tokenauth/auth_backend_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/alphabet.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/alphabet.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/get_decode.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/get_decode.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/get_encode.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/get_encode.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/role.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/template.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/template.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transform/transformation.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transform/transformation.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/get_decrypt.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/get_decrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/get_encrypt.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/get_encrypt.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/secret_backend_key.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/secret_backend_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault/transit/secret_cache_config.py` & `pulumi_vault-5.9.0a1678382334/pulumi_vault/transit/secret_cache_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/PKG-INFO` & `pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-vault
-Version: 5.9.0a1678129627
+Version: 5.9.0a1678382334
 Summary: A Pulumi package for creating and managing HashiCorp Vault cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-vault
 Keywords: pulumi vault
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_vault-5.9.0a1678129627/pulumi_vault.egg-info/SOURCES.txt` & `pulumi_vault-5.9.0a1678382334/pulumi_vault.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 pulumi_vault/approle/auth_backend_login.py
 pulumi_vault/approle/auth_backend_role.py
 pulumi_vault/approle/auth_backend_role_secret_id.py
 pulumi_vault/approle/get_auth_backend_role_id.py
 pulumi_vault/aws/__init__.py
 pulumi_vault/aws/auth_backend_cert.py
 pulumi_vault/aws/auth_backend_client.py
+pulumi_vault/aws/auth_backend_config_identity.py
 pulumi_vault/aws/auth_backend_identity_whitelist.py
 pulumi_vault/aws/auth_backend_login.py
 pulumi_vault/aws/auth_backend_role.py
 pulumi_vault/aws/auth_backend_role_tag.py
 pulumi_vault/aws/auth_backend_roletag_blacklist.py
 pulumi_vault/aws/auth_backend_sts_role.py
 pulumi_vault/aws/get_access_credentials.py
```

### Comparing `pulumi_vault-5.9.0a1678129627/setup.py` & `pulumi_vault-5.9.0a1678382334/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.9.0a1678129627"
-PLUGIN_VERSION = "5.9.0-alpha.1678129627+80ccc529"
+VERSION = "5.9.0a1678382334"
+PLUGIN_VERSION = "5.9.0-alpha.1678382334+8435e08f"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'vault', PLUGIN_VERSION])
         except OSError as error:
```

